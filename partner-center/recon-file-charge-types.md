---
title: 對帳檔案收費類型 |合作夥伴中心
ms.topic: article
ms.date: 08/26/2019
description: 合作夥伴中心對帳檔案的費用類型（以授權為基礎、使用方式和一次性）、點數和折扣。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389806"
---
# <a name="understand-charge-types"></a>瞭解費用類型

適用於：

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

本主題描述發票區段與您的對帳檔案上可能的相關收費類型之間的對應。 您的發票會提供費用的摘要。 您的對帳檔案提供明細專案交易的詳細細目，包括費用類型。 如需有關對帳檔案的詳細資訊，請參閱[如何使用對帳](use-the-reconciliation-files.md)檔案。

以[使用量為基礎的對](usage-based-recon-files.md)帳檔案和以[授權為基礎的對帳](license-based-recon-files.md)檔案，只會顯示使用量相關的交易和費用（耗用的單位和相關費用）。

> [!NOTE]
> 對帳檔案中不會顯示顯示在發票上做為**調整**的一次性信用額度、折扣或退款。

## <a name="map-charge-types-to-invoice-charges"></a>將費用類型對應到發票費用

若要在您的發票和對帳檔案之間交叉參考費用，請使用 Microsoft Excel 中的篩選選項。 依對帳檔案上的收費類型進行篩選，將發票費用對應至對帳檔案的一組費用明細。

## <a name="license-based-charges"></a>授權型費用

若要將這些以授權為基礎的費用對應到您的發票，請加總以授權為基礎的檔案中的**金額**資料行。

| 費用描述（對帳檔案中的 ChargeType 資料行） | 收費說明 |
| ------------------------------------------------------------- | ------------------ |
| 啟用費用 | 購買後使用訂用帳戶時，向客戶收取的金額。 |
| 取消費用 | 當相關聯的基座變更時，會向客戶收取按比例計算的費用。 |
| 循環費用 | 訂用帳戶的定期費用。 |
| 循環執行個體 (依比例計算) | 當相關聯的基座變更時，從客戶評估的按比例計算費用。 |
| 取消時按比例計算費用 | 取消時未使用的服務部分按比例計算。 |
| 購買時按比例計算費用 | 使用年度計費時，訂用帳戶的費用類型。 |
| 購買費用 | 使用每月計費時，訂用帳戶的費用類型。 |
| 續約時按比例計算費用 | 訂閱更新時按比例計算費用。 |
| 續約費用 | 訂閱續約時的費用 |
| 啟用時按比例計算費用 | 從啟用到計費週期結束之前，> 按比例計算的費用。 |

## <a name="one-time-charges"></a>一次性費用

若要將這些一次性費用對應到您的發票，請加總以授權為基礎的檔案中的**金額**資料行。

| 費用描述（對帳檔案中的 ChargeType 資料行） | 收費說明 |
| ------------------------------------------------------------- | ------------------ |
| 新增 | 在建立新購買時使用。 |
| addQuantity | 用於原始購買的退款和增加後的新數量。 |
| removeQuantity | 用於原始購買的退款和減少後的新數量。 |
| 取消 | 在取消訂用帳戶時使用。 |
| 轉換 | 當授權升級，但基座數目維持不變時使用。 |

## <a name="usage-charges"></a>使用量費用

若要將這些使用量費用對應至您的發票，請將**計算 pretaxcharges**資料行與使用方式檔案加總。

| 費用描述（對帳檔案中的 ChargeType 資料行） | 收費說明 |
| ------------------------------------------------------------- | ------------------ |
| 取消時的存取用量費用 | 在目前計費期間，取消未付款使用量時，存取使用費用。 |
| 目前週期的存取用量費用 | 存取目前計費週期的使用費用。 |

### <a name="credits"></a>點數

若要將這些點數對應至您的發票：

- 加總以授權為基礎的檔案中的**TotalForCustomer** 。
- 加總以使用方式為基礎之檔案中的**PostTaxTotal**資料行。

| 費用描述（對帳檔案中的 ChargeType 資料行） | 收費說明 |
| ------------------------------------------------------------- | ------------------ |
| 明細項目位移 | 明細專案的部分或全部退款，包括稅金。 |

### <a name="usage-based-discounts"></a>用量型折扣

若要將這些以使用量為基礎的折扣對應至您的發票，請將**計算 pretaxcharges**資料行與使用方式檔案加總。

| 費用描述（對帳檔案中的 ChargeType 資料行） | 收費說明 |
| ------------------------------------------------------------- | ------------------ |
| 啟用折扣 | 啟用訂用帳戶時所套用的折扣。 |
| 循環折扣 | 定期費用所套用的折扣。 |
| 續約折扣 | 更新訂閱時所套用的折扣。 |
| 取消折扣 | 取消折扣時所套用的費用。 |

### <a name="license-based-discounts"></a>授權型折扣

若要將以授權為基礎的折扣對應至您的發票，請將**TotalOtherDiscount**資料行與授權檔加總。

*以授權為基礎的折扣可能適用于多種費用類型。*