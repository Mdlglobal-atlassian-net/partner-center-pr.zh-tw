---
title: 雲端解決方案提供者地區授權租用戶彙總
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 請依照下列指示合併不同國家/地區的租用戶。 這包括遷移客戶帳戶和客戶訂閱的步驟。
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: LauraBrenner
ms.author: labrenne
keywords: 移轉客戶, 佈建, 租用戶帳戶, 合併租用戶
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 813d24c12501edc7b633d3e10b5174d02ed881d1
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/07/2020
ms.locfileid: "82907993"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>CSP 區域授權租使用者匯總的指示

**適用於**

-  合作夥伴中心
-  Microsoft Cloud for US Government 適用的合作夥伴中心

**適當的角色**

- 全域系統管理員
- 系統管理代理人

\[某些資訊與預先發行的產品有關，在正式發行之前，可能會大幅修改。 Microsoft 對本文提供之資訊，不作任何明示或暗示之保證。\]

請依照下列指示合併不同國家/地區的租用戶。

**注意**：您必須知道您從轉換帳戶佈建之客戶的所有訂閱和基座數目。 您將在移轉程序中，於新的中央雲端解決方案提供者帳戶底下被精確地重新佈建那些相同的訂閱與相同的基座數目。 請使用匯出清單功能來協助建立要移到集中式租用戶之客戶的清單。 合作夥伴選擇合併他們的租用戶。 合併完成之後，合作夥伴就無法回復到先前的狀態。 請注意，也需要執行客戶動作。



## <a name="prepare-for-migration"></a>為移轉做準備


-   使用**轉換**（現有）帳戶（您將轉換的帳戶）登入**合作夥伴中心**，並記下所有客戶和為這些客戶布建的所有服務。

![地區客戶清單](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a>移轉客戶帳戶


1.  使用**轉換**（新）帳戶（您要轉換的使用者）登入您的**合作夥伴中心**，然後流覽至**客戶**的客戶清單。

2.  選取客戶。

3.  按一下 [**要求轉銷商關聯**性]。 系統就會提供您一則預設的電子郵件訊息以供您提供給您的客戶。 此訊息包含一個 URL，其中包含您新的合作夥伴中心帳戶唯一的組織識別碼。

4.  **客戶動作：** 確保您要移轉的每個作用中客戶都會造訪此 URL。 開啟 URL 時，會提示客戶登入 Office 365 入口網站。 客戶使用和用來存取 Azure 及 Office 365 管理入口網站時相同的組織識別碼登入。

5.  登入之後，就會提示客戶帳戶的全域系統管理員送出合約，以提供委派的系統管理員權限給新的雲端解決方案提供者帳戶。 如果他們同意，客戶就能選取核取方塊並同意授權關係。

當客戶提交合約之後，就會出現在合作夥伴的客戶清單中。

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>移轉 Office 365 和非 Azure 用量型訂閱


1.  在您的客戶簽署合約之後，您就可以在您的集中式合作夥伴租用戶底下重新建立他們的訂閱。

2.  從**合作夥伴中心**選取 [**客戶**]。

3.  開啟您要移轉之客戶的公司名稱。

4.  按一下 [**新增訂**用帳戶]。

5.  從目錄新增正確的訂閱與基座數目。 請使用從合作夥伴帳戶**轉換**中提供的資訊進行驗證。

![客戶清單](images/regionalcustomer2.png)

6.  按一下 [**提交]。**

服務現在會從**轉換到**合作夥伴帳戶提供給客戶。

請重複這些步驟來移轉所有其他客戶的訂閱。

在繼續到下一節之前，請確定存在於 **\[轉換來源\]** 合作夥伴帳戶底下的所有客戶訂閱，都已經在 **\[轉換至\]** 合作夥伴帳戶底下重新佈建。

**注意** 合作夥伴必須在合作夥伴中心的 [從合作夥伴] 租使用者帳戶**轉換**時暫停訂閱，並在合作夥伴中心的 [**轉換至**合作夥伴租使用者帳戶] 下設定這些訂用帳戶，以確保不會發生雙重計費。 如果因為未正確設定要停用的 **\[轉換來源\]** 訂閱而發生任何重疊帳單，點數的支援要求將會被拒絕。



## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>停用 \[轉換來源\] 合作夥伴帳戶底下的 Office 365 訂閱


在從合作夥伴帳戶**轉換**下停用 CSP 訂用帳戶，會停止任何未來的帳單。 您不需要手動停用 Azrue 訂閱，因為 Azure 訂閱會在移轉過程中自動停用。

1.  使用 [**從 CSP 轉換**] 帳戶登入**合作夥伴中心**，並流覽至 [客戶] 清單。

2.  開啟含有要停用之訂閱的客戶，然後選取第一項要停用的服務。
3.  將 [訂用帳戶] 設定為 [已**暫停**]，然後按一下 [**提交**]。

 >[!**注意**]暫停訂閱可確保不會進行雙重計費。

~~~
The Subscription shows **suspended** on the subscriptions list.
~~~

4.  請針對客戶底下的所有訂閱重複這些步驟。 確認全部顯示 **\[暫停\]**。

5.  選取清單中的下一個客戶，並重複停用所有訂閱的程序。

## <a name="migrating-azure-usage-based-subscriptions"></a>移轉 Azure 用量型訂閱

Azure，基於使用方式的 CSP 訂用帳戶不需要手動遷移，如同 Office 365 CSP 訂用帳戶的情況。 Microsoft Azure 支援可以將 Azure 訂閱和所有部署的服務或資源從 **\[轉換來源\]** 雲端解決方案提供者經銷商帳戶移轉至 **\[轉換至\]** 雲端解決方案提供者經銷商帳戶。 轉換期間對客戶的服務不會中斷。

1.  請確定需要移轉 Azure 訂閱的客戶帳戶已經接受要與新的 **\[轉換至\]** 雲端解決方案提供者帳戶關聯的合約。
2.  合作夥伴會通知 Microsoft 具有 Azure 訂用帳戶的客戶帳戶已準備好進行遷移，並提供這些客戶的公司名稱。
3.  Microsoft 移轉 Azure 用量型訂閱並在移轉完成時通知合作夥伴。
4.  合作夥伴在合作夥伴中心的 [客戶訂用帳戶] 區段下，確認 [從 CSP 轉銷商帳戶**轉換**] 下的 Azure 訂用帳戶現在顯示為 [已暫停]。
5.  合作夥伴確認在 [正在**轉換至**CSP 轉銷商帳戶] 下的 Azure 訂用帳戶現在會在合作夥伴中心的 [客戶訂閱] 區段底下顯示 [**作用中]** 狀態。

>[!**注意**]停用客戶下的訂用帳戶並不會變更客戶在 Customers 清單中的外觀。 目前沒有將客戶從清單移除的選項。 合作夥伴應避免將訂用帳戶從他們在未來的**轉換中**，新增回給這些客戶。



6.  針對所有客戶下的所有訂用帳戶，重複這些步驟，以停止未來**從帳戶轉換**的費用。 合作夥伴將會收到一份最終發票，其中包含取消日期到計費期間最後一天之間未使用天數的點數。 未來在該最終計費期間之後將不會再產生發票。

### <a name="notes"></a>備忘錄

-   只要服務是在停用訂用帳戶之前，從**轉換為**csp 帳戶布建，則從 csp 帳戶的**轉換**中停用訂閱並不會影響終端客戶的服務。

-   訂用帳戶無法供客戶使用，且在暫停或取消時不會產生費用。

-   目前沒有任何方式可以將客戶完全從客戶清單中移除。

-   **注意** 合作夥伴必須在合作夥伴中心的 [從合作夥伴租使用者帳戶**轉換**時] 暫停訂閱，這當天是那些訂用帳戶轉換成的相同日期，並設定在合作夥伴中心的 [**轉換為**合作夥伴租使用者帳戶] 下，以確保不會發生雙重計費。 由於未正確設定從訂用帳戶**轉換**為暫停的計費，Microsoft 不會支援信用額度的要求。



### <a name="simplify-migration-using-export"></a>使用匯出功能簡化移轉

使用 **\[匯出功能\]**，您就可以擷取您需要在新的合併結構中使用的訂閱：

1.  按一下 [合作夥伴中心] 上的 [**客戶**]，以查看現有結構中的客戶清單。

2.  開啟想查看之客戶的名稱。

3.  在 [**訂閱**] 頁面上，按一下 [**匯出訂閱**]，將訂閱的詳細資料匯出至 Excel 檔案。

4.  請使用此清單在您新的合併租用戶中重新建立訂閱。

### <a name="api-registration"></a>API 註冊

如需 API 註冊的詳細資訊，請[參閱此頁面](https://go.microsoft.com/fwlink/?linkid=847990)。








