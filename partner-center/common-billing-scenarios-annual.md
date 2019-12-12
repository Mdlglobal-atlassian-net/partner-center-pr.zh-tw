---
title: 常見帳單案例 | 合作夥伴中心
ms.topic: article
ms.date: 11/25/2019
description: 請參閱合作夥伴中心年度計費-新增訂閱時，在計費日期之前新增授權、變更授權數量、暫停/重新開機訂閱。
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: 帳單，付款，訂單，使用量，以授權為基礎的帳單，週年日，期，取消，續約，價格公式，對帳檔案，偵察檔案
ms.localizationpriority: medium
ms.openlocfilehash: d29def486243f3a4ee9060d442dc5e4b024cb1f0
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722475"
---
# <a name="annual-billing-scenarios"></a>年度計費案例

**適當的角色**

- 系統管理代理人
- 帳單管理
- 技術服務代理人
- 銷售代理人

這些範例[一般計費案例](common-billing-scenarios.md)適用于您在合作夥伴中心使用年度計費的情況。

## <a name="new-annual-subscription"></a>新增年度訂閱

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取年度計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|購買時按比例計算之費用|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>在訂用帳戶週年日之後、計費日期之前新增授權

您在 2017 年 2 月 11 日購買新訂閱，包含一份費率為 $211.20 美元/年的授權。 您的訂閱週年日已設定為每個月的 11 日。 Microsoft 帳單系統會建立下列帳務明細︰

- 2017/2/11 – 2018/2/10 期間收費 $211.20。

您於 2017 年 2 月 12 日購買第二份授權。 您的帳單日期為 2017 日 2 月 14 日。 產生了發票和對帳檔案。 對帳檔案將會包含下列帳務明細︰

|收費開始日期  |收費結束日期  |收費類型  |單價 |數量 | 金額 |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2017/2/11 |2018/2/10 |購買時按比例計算費用 |211.20 |1 | 211.20 |

在您的週年日 2017 年 3 月 11 日，Microsoft 帳單系統針對您於 2017 年 2 月 12 日增加的授權建立下列帳務明細：

- 期間 2/11/17-2/10/18 的 $211.20 點數。
- 1 份於 2017/2/11 – 2017/2/11 期間使用的授權，按比例計算的每一授權費用為 $0.58。
- 2 份於 2017/2/12 – 2017/3/10 期間使用的授權，按比例計算的每一授權費用為 $15.62。
- 2 份於 2017/3/11 – 2018/2/10 期間使用的授權，按比例計算的每一授權費用為 $195.00。

您於 2017 年 2 月 11 日購買一份授權。 您於 2017 年 2 月 12 日新增一份授權。 您的帳單日期為 2017 日 2 月 14 日。 您的訂閱於 2018 日 2 月 11 日續約。

您的下一個帳單日期為 2017 年 3 月 14 日，系統產生了發票與對帳檔案。 對帳檔案將會包含下列帳務明細︰

|收費開始日期  |收費結束日期  |收費類型  |單價 |數量 | 金額 |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2017/2/11 |2018/2/10 |循環執行個體 (依比例計算) |-211.20 |1 |-211.20 |
|2017/2/11 |2017/2/11 |循環執行個體 (依比例計算) |0.58 |1 |0.58 |
|2017/2/12 |2017/3/10 |循環執行個體 (依比例計算) |15.62 |2 |31.25 |
|2017/3/11 |2018/2/10 |循環執行個體 (依比例計算) |195.00 |2 |390.00 |

訂閱將於 2018 年 2 月 11 日續約 12 個月。

## <a name="change-license-quantity"></a>變更授權數量

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取年度計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|購買時按比例計算之費用|48.00|1|48.00

您在 2 月 1 日將授權數量從一個增加為兩個。 2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|循環執行個體 (依比例計算)|-48.00|1|-48.00
1/13/2018|1/31/2018|循環執行個體 (依比例計算)|2.47|1|2.47
2/1/2018|1/12/2019|循環執行個體 (依比例計算)|44.98|2|89.96

年度價格是 48.00，相當於每日價格 0.13 (48.00/365)。

單價 = 服務期間天數 x 每天價格 x 授權天數。

1/13/2018 – 1/31/2018 的服務期間有 19 天。

因此，單價 = 2.47 (19x0.13x1)

2/1/2018 – 1/12/2019 的服務期間有 346 天。

因此，單價 = 44.98 (346x0.13x2)

## <a name="suspend-before-30-days"></a>30天前暫停

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取年度計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|購買時按比例計算之費用|48.00|1|48.00

您在 2 月 1 日暫停訂閱。 2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|取消費用|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>30天后暫停

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取年度計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|購買時按比例計算之費用|48.00|1|48.00

2 月 15 日的授權型對帳檔案不會包含此訂閱的任何帳務明細：
您在 3 月 1 日暫停訂閱。 3 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|取消費用|-41.34|1|-41.34

年度價格是 48.00，相當於每日價格 0.13 (48.00/365)。

單價 = 服務期間天數 x 每天價格 x 授權天數。

3/1/2018 – 1/12/2019 的服務期間有 318 天。

因此，單價 = 41.34 (318x0.13x1)。 因為這是貸記金額，所以單價是 -41.34。

## <a name="suspend-and-reactivate"></a>暫停並重新啟動

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取年度計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|購買時按比例計算之費用|48.00|1|48.00

您在 2 月 1 日暫停訂閱。 2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|取消費用|-48.00|1|-48.00

您在 3 月 1 日重新啟用訂閱。 3 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|購買時按比例計算之費用|41.34|1|41.34

年度價格是 48.00，相當於每日價格 0.13 (48.00/365)。

單價 = 服務期間天數 x 每天價格 x 授權天數。

3/1/2018 – 1/12/2019 的服務期間有 318 天。

因此，單價 = 41.34 (318x0.13x1)。