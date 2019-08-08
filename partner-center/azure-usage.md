---
title: 適用于保留使用量上限的 Microsoft Azure VM 大小 |合作夥伴中心
ms.topic: article
ms.date: 08/05/2019
Description: 代表您的客戶購買 Microsoft Azure Reservations 時，您需要選擇符合客戶運算需求的虛擬機器 (VM) 大小。
author: LauraBrenner
ms.author: labrenne
keywords: azure, 保留區, vm, 管理, 使用率, 調整大小
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 1c1c0170c5efd8abf2e1afb7bb6ef1dfac2b7e5b
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820189"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>調整 Microsoft Azure VM 大小以提供最大保留區使用率

**適用於**

- 合作夥伴中心
- Azure 入口網站
- 雲端解決方案提供者中的合作夥伴

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>判斷客戶 Azure Reservations 的 VM 大小 

代表您的客戶購買 Microsoft Azure Reservations 時，您需要選擇符合客戶運算需求的虛擬機器 (VM) 大小。 您可以使用下列其中一個方法來找到此項資訊：

- Azure 使用量 API
- Azure 入口網站
- Azure PowerShell
- Azure Resource Manager (ARM) API

以下列出使用每種方法的指示。 購買保留區之後，保留區折扣會自動套用到符合保留區屬性和數量的虛擬機器。 您不需要指派保留區給 VM。

>[!NOTE]
>保留區折扣不適用於傳統或促銷 VM。

>[!IMPORTANT]
>若要正確找出代表您客戶購買的 VM 大小和類型，您必須使用以下所述的其中一種方法，因為合作夥伴中心對帳檔案不會正確顯示 VM 系列類型。

**使用 Azure 使用率 API 取得 VM 大小調整資訊**

1. 使用 API 回應中 additionalInfo 的 ServiceType 屬性值，找出要購買的 VM 大小。
2. 如需詳細資訊，請參閱[合作夥伴中心 API](https://docs.microsoft.com/partner-center/develop/) 中的[取得客戶的 Azure 使用率記錄](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) (英文)。

**使用 Microsoft Azure 入口網站取得 VM 大小調整資訊**

1. 在合作夥伴中心, 移至您的 [**客戶**] 頁面。
2. 尋找想要購買 Azure VM 保留區的客戶，然後選取向下箭號來展開客戶資訊。 選取 **\[Microsoft Azure 管理入口網站\]** 以在 Azure 入口網站中開啟客戶記錄。
3. 從入口網站功能表選取 **\[虛擬機器\]** ，然後選取您要購買保留區的 VM。
4. 在 VM 的詳細資料頁面上，尋找大小及地區資訊 (如下所示)，並使用此資訊在合作夥伴中心中購買保留區。  

    ![詳細資料頁面上的大小和區域資訊](images/usage1.png)

**使用 Microsoft Azure PowerShell 取得 VM 大小調整資訊**

使用下列影像中的資訊，取得您要購買保留區的 VM 大小與位置。 

![VM 位置和大小](images/usage2.png)

**使用 Azure Resource Manager (ARM) API 取得 VM 大小調整資訊**

1. 使用 ARMClient 或 ARM API，呼叫您要購買保留區之 VM 的 ARM 用戶端。

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. 呼叫會傳回 **vmSize** 和 **location** 的值，如下所示。

    ![vmSize 值](images/usage3.png) ![位置值](images/usage4.png)

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>確認 Azure VM 使用率與保留區折扣

代表客戶購買 Azure 保留的 VM 執行個體後，預先支付 VM 空間的折扣會自動套用到符合客戶保留區屬性和數量的虛擬機器。

您可以使用下列其中一項方法，確認客戶的保留區使用率，並查看適用於保留區折扣的虛擬機器：

- Azure 入口網站
- Azure 使用量 API

以下列出使用每種方法的指示。

>[!NOTE]
>只有 Azure 使用量 API 會顯示折扣套用的虛擬機器。  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>在 Microsoft Azure 入口網站中確認客戶的保留區使用率

1. 在合作夥伴中心, 移至您的 [**客戶**] 頁面。

2. 尋找您要確認其保留區折扣和使用率的客戶，然後選取向下箭號來展開客戶資訊。 選取 **\[Microsoft Azure 管理入口網站\]** 以在 Azure 入口網站中開啟客戶記錄。
3. 從入口網站功能表選取 **\[保留區\]** ，然後選取您要查看其使用率的保留區。
4. 在 **\[概觀\]** 頁面上檢查保留區的使用率圖形，其中會顯示多少保留區已套用到虛擬機器。

    >[!NOTE]
    >使用率資料可能會延遲最多 8 小時。

    a. 如果保留區使用率是 100%，表示您的客戶已獲得保留區購買可提供的所有可能節省情形。
    b. 如果保留區使用率是 0%，表示折扣不適用於任何虛擬機器。
    c. 如果保留區使用率介於 1% 和 99% 之間，表示有未使用的權益。

5. 若要避免發生這種情形，請在購買之前正確判斷支援客戶運算需求的 VM 大小。

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>使用 Azure 使用量 API 確認客戶的保留區使用率

>[!NOTE]
>只有 Azure 使用量 API 會顯示折扣套用的虛擬機器。  

您可以使用 Azure 使用量 API 取得保留區使用率資料，來確認客戶獲得保留區折扣，並查看折扣套用到那些 VM (虛擬機器)。 比較範例 A 和範例 B，了解如何確認客戶的保留區使用率。

![保留使用範例](images/usage5.png)

- ReservationId 可識別用於套用折扣至 VM 的 Azure 保留區。
- consumptionMeter 是已套用保留區折扣之 VM 的 MeterId。
- 由於已套用保留區折扣，所以 ReservationMeter 會顯示 $0 費用。

如需詳細資訊，請參閱[合作夥伴中心 API](https://docs.microsoft.com/partner-center/develop/) 中的[取得客戶的 Azure 使用率記錄](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) (英文)。

>[!IMPORTANT]
>軟體成本 (例如 Microsoft Windows Server) 目前不包含在 VM 保留區的價格中，並會在訂單記錄和發票中顯示為不同的一行項目。 不過，如果客戶擁有 Azure Hybrid Use Benefit，將不會套用軟體成本。 如需詳細資訊，請參閱 [Windows 軟體的成本不包括在保留執行個體內](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)。  

## <a name="azure-reservations-resources"></a>Azure Reservations 資源

|**如需相關資訊**   |**閱讀此**    |
|:-----------------------------|:-----------------|
|雲端解決方案提供者中的 Azure Reservations 概觀  | [銷售 Microsoft Azure 保留的 VM 實例](azure-reservations.md)
|在合作夥伴中心為您的客戶購買 Azure 保留   |[購買 Azure 保留](azure-reservations-buying.md)
|在合作夥伴中心管理 Azure 保留專案 | [在合作夥伴中心管理 Azure 保留專案](azure-reservations-manage.md)
|在 Azure 入口網站中購買 Azure Reservations | Azure 說明中的[預付具有 Azure 保留的 VM 執行個體的虛擬機器](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) |
|在 Azure 入口網站中管理 Azure Reservations   |Azure 說明中的[管理保留的 VM 執行個體](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)  |
|使用合作夥伴中心 API 購買 Azure Reservations | 合作夥伴中心開發人員文件中的[購買 Azure 保留的 VM 執行個體](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)
