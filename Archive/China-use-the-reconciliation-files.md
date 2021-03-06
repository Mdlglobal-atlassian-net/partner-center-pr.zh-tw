---
title: 使用的對帳檔案 （由 21Vianet 運作的合作夥伴中心）
ms.topic: article
ms.date: 10/29/2018
description: 如需計費週期中每項費用的詳細明細項目檢視，請從合作夥伴中心儀表板下載對帳檔案。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.openlocfilehash: 30e3b7a7933678c4af079bb86aa1439559387f2b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132078"
---
# <a name="use-the-reconciliation-files"></a>使用對帳檔案

**適用於**

-   由 21Vianet 營運的合作夥伴中心


如需計費週期中每項費用的詳細明細項目檢視，請從合作夥伴中心儀表板下載對帳檔案。 詳細資料包括每個客戶的訂閱費用，以及詳細事件 (例如，期中增加訂閱基座)。

## <a href="" id="itemizebypartner"></a>由合作夥伴條列


間接模型合作夥伴可以在授權型及用量型對帳檔案中使用這些額外欄位，以便依經銷商詳細列舉。

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>MPN 識別碼</th>
<th>描述</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>MPN 識別碼</td>
<td><p>CSP 合作夥伴 (直接或間接) 的 Microsoft 合作夥伴網路 (MPN) 識別碼。</p></td>
</tr>
<tr class="even">
<td>經銷商 MPN 識別碼</td>
<td><p>只會出現在間接模型合作夥伴的對帳檔案上。</p>
<p>訂閱記錄中的經銷商 MPN 識別碼。 這會對應到合作夥伴中心中針對特定訂閱列出的經銷商識別碼。</p>
<p>若要檢視或更新經銷商，請在合作夥伴中心功能表中選取 \[客戶\]，然後從清單中選擇客戶。 在客戶功能表中，選取 \[訂閱\]，從清單中選擇訂閱。 選取 \[更新\] 以變更 \[經銷商 (MPN 識別碼)\]。</p>
<p>如果雲端解決方案提供者合作夥伴直接向客戶銷售訂閱，他們的 MPN 識別碼將會以 MPN 識別碼和經銷商 MPN 識別碼的形式列出兩次。</p>
<p>如果雲端解決方案提供者合作夥伴具有沒有 MPN 識別碼的經銷商，這個值將會改成設為合作夥伴的 MPN 識別碼。</p>
<p>如果雲端解決方案提供者合作夥伴移除經銷商識別碼，這個值將會設為 -1。</p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> 以授權為基礎的檔案欄位


若要針對您對客戶訂單的費用來對帳，請比較對帳檔案中的 Syndication\_Partner\_Subscription\_Number 與合作夥伴中心的訂閱識別碼。

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>資料行</strong></td>
<td><strong>描述</strong></td>
<td><strong>範例值</strong></td>
</tr>
<tr class="even">
<td>PartnerId</td>
<td><p>特定帳單實體的唯一識別碼 (GUID 格式)。 對帳時不需要，但可能是很有用的資訊。 在所有資料列中都是如此。</p></td>
<td>8ddd03642-test-test-test-46b58d356b4e</td>
</tr>
<tr class="odd">
<td>CustomerID</td>
<td><p>用來識別客戶的唯一 Microsoft ID（GUID 格式）。</p></td>
<td>12ABCD34-001A-BCD2-987C-3210ABCD5678</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>訂單在 Microsoft 帳單平台中的唯一識別碼。 可在連絡支援時方便識別訂單，但不是用於對帳。</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>訂閱在 Microsoft 帳單平台中的唯一識別碼。 可在連絡支援時方便識別訂閱，但不是用於對帳。</p>
<p>這與合作夥伴管理主控台上的訂閱識別碼不一樣。 請參閱 Syndication_Partner_Subscription_Number。</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SyndicationPartnerSubscriptionNumber</td>
<td><p>訂閱的唯一識別碼。 客戶可針對同一方案擁有多項訂閱，因此這對於對帳檔案分析而言很重要。</p>
<p>這個欄位對應到合作夥伴管理主控台中的訂閱識別碼。</p></td>
<td>fb977ab5-test-test-test-24c8d9591708</td>
</tr>
<tr class="odd">
<td>OfferID</td>
<td><p>唯一的優惠識別碼。 根據價目表的標準優惠識別碼。</p>
<p><b>注意</b>：此值不符合優惠識別碼從價格清單。 請參閱下方的 DurableOfferID。</p></td>
<td>FE616D64-E9A8-40EF-843F-152E9BBEF3D1</td>
</tr>
<tr class="even">
<td>DurableOfferID</td>
<td><p>唯一的持續性優惠識別碼，如價目表中所定義。</p>
<p><b>注意</b>：此值符合優惠識別碼從價格清單。</p></td>
<td>1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</td>
</tr>
<tr class="odd">
<td>OfferName</td>
<td><p>客戶購買的服務優惠名稱，如價目表中所定義。</p></td>
<td>Microsoft Office 365 (Plan E3)</td>
</tr>
<tr class="even">
<td>SubscriptionStartDate</td>
<td><p>訂閱開始日期設定為送出訂單之後的隔日。 藉由同時查看訂閱開始日期與結束日期，您就可以判斷客戶是否仍在第一年訂閱期內，或下一年的訂閱已續約。</p>
<p>時間一律是一天的開始時間 (0:00)。</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>SubscriptionEndDate</td>
<td><p>訂用帳戶結束日期：12 個月 + x 天後 （以配合計費日期的夥伴） 的開始日期或續約日期起的 12 個月。</p>
<p>續約時，價格會更新至目前的價目表。 自動續約之前，可能需要與客戶連絡。</p>
<p>時間一律是一天的開始時間 (0:00)。</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="even">
<td>ChargeStartDate</td>
<td><p>開始計算費用的日期。</p>
<p>當客戶變更基座數目時，此數字用於計算每日 (按比例) 的費用。</p>
<p>時間一律是一天的開始時間 (0:00)。</p></td>
<td>2/1/2015 0:00</td>
</tr>
<tr class="odd">
<td>ChargeEndDate</td>
<td><p>結束計算費用的日期。</p>
<p>當客戶變更基座數目時，此數字用於計算每日 (按比例) 的費用。</p>
<p>時間一律是一天的結束時間 (23:59)。</p></td>
<td>2/28/2015 23:59</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>費用或調整的類型。 請參閱<a href="#charge_types">對應發票和對帳檔案之間的費用</a></p></td>
<td><p>請參閱<a href="#charge_types">對應發票和對帳檔案之間的費用</a></p></td>
</tr>
<tr class="odd">
<td>UnitPrice</td>
<td><p>每一基座價格。 請確定這與對帳期間儲存在您帳單系統中的資訊相符。</p></td>
<td>6.82</td>
</tr>
<tr class="even">
<td>數量</td>
<td><p>基座數目。 請確定這與對帳期間儲存在您帳單系統中的資訊相符。</p></td>
<td>2</td>
</tr>
<tr class="odd">
<td>數量</td>
<td><p>數量總價。 檢查計算金額與您用來為客戶計算此項目的方式是否相符時很有用。</p></td>
<td>13.32</td>
</tr>
<tr class="even">
<td>TotalOtherDiscount</td>
<td><p>套用至這些費用的折扣金額。 符合獎勵資格之 IUR 或新訂閱的訂單，也將於此欄中包含折扣金額。</p></td>
<td>2.32</td>
</tr>
<tr class="odd">
<td>小計</td>
<td><p>稅前總計。 如果有折扣，可檢查小計是否和預期的總金額相符。</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>稅</td>
<td><p>稅金費用 (根據您所在市場的稅金規則與特定情況)。</p></td>
<td>0</td>
</tr>
<tr class="odd">
<td>TotalForCustomer</td>
<td><p>稅後總計。 檢查發票中是否向您收取稅金。</p></td>
<td>11</td>
</tr>
<tr class="even">
<td>貨幣</td>
<td><p>貨幣類型。 每一帳單實體都只有一種貨幣。 檢查是否與您的第一張發票相符，然後在進行任何重大帳單平台更新之後檢查。</p></td>
<td>CNY</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>合作夥伴中心中回報的客戶組織名稱。 這在使用您的系統資訊對帳發票時非常重要。</p></td>
<td>測試客戶 A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>雲端解決方案提供者合作夥伴的 MPN 識別碼</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>訂閱記錄中的經銷商 MPN 識別碼。 請參閱[依合作夥伴詳細列舉](#itemizebypartner)。</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>DomainName</td>
<td><p>用來協助識別客戶的客戶網域名稱。</p></td>
<td>example.onmicrosoft.com</td>
</tr>
<tr class="odd">
<td>SubscriptionName</td>
<td><p>訂閱暱稱。 如果未指定任何暱稱，合作夥伴中心會使用 OfferName。</p></td>
<td>PROJECT ONLINE</td>
</tr>
<tr class="even">
<td>SubscriptionDescription</td>
<td><p>客戶購買的服務優惠名稱，如價目表中所定義。 （這是優惠名稱的相同欄位）。</p></td>
<td>PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a>基於使用方式檔案欄位


若要針對您客戶使用量的費用來對帳，請比較對帳檔案中的 ResellerID/ResellerName/ResellerBillableAccount、客戶名稱，與合作夥伴中心的訂閱識別碼。

下列欄位說明使用哪些服務及費率。

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>資料行</strong></td>
<td><strong>描述</strong></td>
<td><strong>範例值</strong></td>
</tr>
<tr class="even">
<td>PartnerID</td>
<td><p>合作夥伴識別碼 (GUID 格式)。</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="odd">
<td>PartnerName</td>
<td><p>合作夥伴名稱。</p></td>
<td>Acme Incorporated</td>
</tr>
<tr class="even">
<td>PartnerBillableAccountID</td>
<td><p>合作夥伴帳戶識別碼。</p></td>
<td>1010578050</td>
</tr>
<tr class="odd">
<td>CustomerName</td>
<td><p>合作夥伴中心中回報的客戶組織名稱。 這在使用您的系統資訊對帳發票時非常重要。</p></td>
<td>測試客戶 A</td>
</tr>
<tr class="even">
<td>MPNID</td>
<td><p>雲端解決方案提供者合作夥伴的 MPN 識別碼。</p></td>
<td>4390934</td>
</tr>
<tr class="odd">
<td>ResellerMPNID</td>
<td><p>訂閱記錄中的經銷商 MPN 識別碼。 請參閱[依合作夥伴詳細列舉](#itemizebypartner)。</p></td>
<td>4390934</td>
</tr>
<tr class="even">
<td>InvoiceNumber</td>
<td><p>交易的指定位置顯示的發票號碼。</p></td>
<td>D020001IVK</td>
</tr>
<tr class="odd">
<td>ChargeStartDate</td>
<td><p>計費週期的開始日期，當顯示之前未收取潛在使用量資料費用的日期時除外 (從前一個計費週期開始)。</p>
<p>時間一律是一天的開始時間 (0:00)。</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="even">
<td>ChargeEndDate</td>
<td><p>計費週期的結束日期，當顯示之前未收取潛在使用量資料費用的日期時除外 (從前一個計費週期開始)。</p>
<p>時間一律是一天的結束時間 (23:59)。</p></td>
<td>2/28/2014 23:59</td>
</tr>
<tr class="odd">
<td>SubscriptionID</td>
<td><p>訂閱在 Microsoft 帳單平台中的唯一識別碼。 可在連絡支援時方便識別訂閱，但不是用於對帳。</p>
<p>這與合作夥伴管理主控台上的訂閱識別碼不一樣。</p></td>
<td>usCBMgAAAAAAAAIA</td>
</tr>
<tr class="even">
<td>SubscriptionName</td>
<td><p>服務優惠的暱稱。</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="odd">
<td>SubscriptionDescription</td>
<td><p>服務優惠的企業營運</p></td>
<td>Microsoft Azure</td>
</tr>
<tr class="even">
<td>OrderID</td>
<td><p>訂單在 Microsoft 帳單平台中的唯一識別碼。 可在連絡支援時方便識別訂閱，但不是用於對帳。</p></td>
<td>566890604832738111</td>
</tr>
<tr class="odd">
<td>ServiceName</td>
<td><p>要求的 Azure 服務名稱。</p></td>
<td>虛擬機器</td>
</tr>
<tr class="even">
<td>ServiceType</td>
<td><p>Microsoft Azure 服務的特定類型。</p></td>
<td><ul>
<li>服務匯流排 – 個人或套件</li>
<li>SQL Azure 資料庫 – Business 或 Web Edition</li>
</ul></td>
</tr>
<tr class="odd">
<td>ResourceGUID</td>
<td><p>所有服務資料與定價結構的特定唯一識別碼。</p></td>
<td>DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</td>
</tr>
<tr class="even">
<td>Resource Name</td>
<td><p>Azure 資源的名稱。</p></td>
<td><ul>
<li>資料轉入 (GB)</li>
<li>資料轉出 (GB)</li>
</ul></td>
</tr>
<tr class="odd">
<td>地區</td>
<td><p>使用量適用的地區。 主要用來指定資料傳輸速率，費率因地區而異。</p></td>
<td>亞太地區、歐洲、拉丁美洲、北美洲</td>
</tr>
<tr class="even">
<td>SKU</td>
<td><p>優惠的 MSFT 唯一識別碼</p></td>
<td>7UD 00001</td>
</tr>
<tr class="odd">
<td><p>DetailLineItemId</p></td>
<td><p>用於詳細列出指定計費期間中，服務或資源不同費率的識別碼和數量。 對於 Azure 分層評分，到某個數量的計費單位會有一個評分，之後則有不同評分。</p></td>
<td>1</td>
</tr>
<tr class="even">
<td>ConsumedQuantity</td>
<td><p>報表期間耗用的服務量 (小時、GB 等等)</p>
<p>同時包括先前報表期間任何未計費的使用量。</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>IncludedQuantity</td>
<td><p>包含在優惠中的單位。 通常不會出現在雲端解決方案提供者中。</p></td>
<td>0</td>
</tr>
<tr class="even">
<td><p>OverageQuantity</p></td>
<td><p>不包含在優惠中的單位，必須由合作夥伴支付。</p>
<p>等同於 ConsumedQuantity - IncludedQuantity。</p></td>
<td>11</td>
</tr>
<tr class="odd">
<td>ListPrice</td>
<td><p>訂閱開始日期的生效優惠價格。</p></td>
<td>$0.0808</td>
</tr>
<tr class="even">
<td>PretaxCharges</td>
<td><p>ListPrist 乘以 OverageQuantity，四捨五入至美分。</p></td>
<td>$0.085</td>
</tr>
<tr class="odd">
<td>TaxAmount</td>
<td><p>稅金費用 (根據您所在市場的稅金規則與特定情況)。</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>PostTaxTotal</td>
<td><p>稅後總計 (當適用稅金時)。</p></td>
<td>$0.93</td>
</tr>
<tr class="odd">
<td>貨幣</td>
<td><p>貨幣類型。 每一帳單實體都只有一種貨幣。 檢查是否與您的第一張發票相符，然後在進行任何重大帳單平台更新之後檢查。</p></td>
<td>CNY</td>
</tr>
<tr class="even">
<td>PretaxEffectiveRate</td>
<td><p>每個單位的稅前價格。 等於 PretaxCharges / OverageQuantity, 四捨五入至美分。</p></td>
<td>$0.08</td>
</tr>
<tr class="odd">
<td>PostTaxEffectiveRate</td>
<td><p>每個單位的稅後價格。 等於 PostTaxTotal / OverageQuantity，或 PretaxEffectiveRate + 每單位數量稅率，四捨五入至美分。</p></td>
<td>$0.08</td>
</tr>
<tr class="even">
<td>ChargeType</td>
<td><p>費用或調整的類型。 請參閱<a href="#charge_types">對應發票和對帳檔案之間的費用</a></p></td>
<td><p>請參閱<a href="#charge_types">對應發票和對帳檔案之間的費用</a></p></td>
</tr>
<tr class="odd">
<td>CustomerBillableAccount</td>
<td><p>MSFT 帳單平台的唯一帳戶識別碼。</p></td>
<td>1280018095</td>
</tr>
<tr class="even">
<td>UsageDate</td>
<td><p>服務部署的日期。</p></td>
<td>2/1/2014 0:00</td>
</tr>
<tr class="odd">
<td>MeteredRegion</td>
<td><p>此欄可識別適用及填入此項目之服務地區內的資料中心的位置。</p></td>
<td>東亞、東南亞、北歐、西歐、美國中北部、美國中南部</td>
</tr>
<tr class="even">
<td>MeteredService</td>
<td><p>此欄是用來追蹤可能未在 \[服務名稱\] 欄中特別指出的個別 Microsoft Azure 服務。 例如，在 \[服務名稱\] 欄中，資料傳輸是回報為 &quot;Microsoft Azure - 所有服務&quot;。 此 MeteredService 欄會指出使用量與哪個特定服務有關。</p></td>
<td>AccessControl、CDN、Compute、Database、ServiceBus、Storage</td>
</tr>
<tr class="odd">
<td>MeteredServiceType</td>
<td><p>進一步釐清超出 MeteredService 欄位提供之層級的個別 Microsoft Azure 服務副標題。</p></td>
<td>外部</td>
</tr>
<tr class="even">
<td>Project</td>
<td><p>客戶為其服務執行個體定義的名稱</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>ServiceInfo</td>
<td><p>於某一天佈建及使用的 ServiceBus 連線數目。</p></td>
<td>例如：如果您在有 30 天的月份中有個別佈建的連線時，「服務資訊 1」的讀數會是「1.000000 連線 / 30 天」。 如果您有 25 的組件的佈建的服務匯流排連線，而且您必須在那一天使用 1，表示您那一天的每日使用量聲明 」 25 的連線 / 已使用的 30 天：1.000000”.</td>
</tr>
<tr class="even">
<td>CustomerID</td>
<td><p>用來識別客戶的唯一 Microsoft ID（GUID 格式）。</p></td>
<td>ORDDC52E52FDEF405786F0642DD0108BE4</td>
</tr>
<tr class="odd">
<td>DomainName</td>
<td><p>用來協助識別客戶的客戶網域名稱。</p></td>
<td>example.onmicrosoft.com</td></tr>
</tbody>
</table>



## <a href="" id="charge_types"></a>發票和對帳檔案之間的對應費用

您的發票提供費用摘要，而對帳檔案則提供包括費用類型等明細項目交易的詳細細項。

若要交互參照發票和對帳檔案之間的費用金額，您可以使用 Microsoft Excel 篩選選項，在對帳檔案上依費用類型篩選，以便將發票費用對應到對帳檔案上的一組費用細項。

下表顯示發票區段和對帳檔案上可能會顯示之相關費用類型之間的對應。 

<table>
<tbody>
<tr>
<td>
<p><strong>發票費用的描述</strong></p>
</td>
<td>
<p><strong>對帳檔案費用描述 （ChargeType 資料行）</strong></p>
</td>
<td>
<p><strong>此費用是什麼？</strong></p>
</td>
<td>
<p><strong>如何將這些 ChargeTypes 對應到發票？</strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong>週期性費用</strong></p>
</td>
<td>
<p>取消執行個體按比例計算</p>
</td>
<td>
<p>當關聯的基座變更時，按比例計算退款給客戶的費用</p>
</td>
<td rowspan="8">
<p>從授權型檔案，加總 <strong>Amount</strong> 欄</p>
</td>
</tr>
<tr>
<td>
<p>循環費用</p>
</td>
<td>
<p>訂閱的定期費用</p>
</td>
</tr>
<tr>
<td>
<p>循環執行個體 (依比例計算)</p>
</td>
<td>
<p>當關聯的基座變更時，按比例計算向客戶收取的費用</p>
</td>
</tr>
<tr>
<td>
<p>取消時按比例計算費用</p>
</td>
<td>
<p>取消時服務未使用部分之按比例計算的退款</p>
</td>
</tr>
<tr>
<td>
<p>購買時按比例計算費用</p>
</td>
<td>
<p>在購買時按比例計算的費用</p>
</td>
</tr>
<tr>
<td>
<p>購買費用</p>
</td>
<td>
<p>訂閱的初始費用</p>
</td>
</tr>
<tr>
<td>
<p>續約時按比例計算費用</p>
</td>
<td>
<p>訂閱續約時按比例計算的費用</p>
</td>
</tr>
<tr>
<td>
<p>續約費用</p>
</td>
<td>
<p>訂閱續約時的費用</p>
</td>
</tr>
<tr>
<td>
<p><strong>其他產品和服務</strong></p>
</td>
<td>
<p>啟用時按比例計算費用</p>
</td>
<td>
<p>從啟用到計費期間結束時按比例計算的費用</p>
</td>
<td>
<p>從授權型檔案，加總 <strong>Amount</strong> 欄</p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong>使用量費用</strong></p>
</td>
<td>
<p>取消時的存取用量費用</p>
</td>
<td>
<p>在目前計費期間中取消時，未支付之使用量的存取用量費用</p>
</td>
<td rowspan="2">
<p>從用量型檔案，加總 <strong>PretaxCharges</strong> 欄</p>
</td>
</tr>
<tr>
<td>
<p>目前週期的存取用量費用</p>
</td>
<td>
<p>目前計費期間的存取用量費用</p>
</td>
</tr>
<tr>
<td>
<p><strong>信用額度&amp;調整</strong></p>
</td>
<td>
<p>明細項目位移</p>
</td>
<td>
<p>明細項目的部分或完整退款 (含稅)</p>
</td>
<td>
<p>從授權型檔案，加總 <strong>TotalForCustomer</strong> 欄</p>
<p>從用量型檔案，加總 <strong>PostTaxTotal</strong> 欄</p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong>其他折扣</strong></br>
<em>(usage-based)</em></p>
</td>
<td>
<p>啟用折扣</p>
</td>
<td>
<p>啟用訂閱時套用的折扣</p>
</td>
<td rowspan="4">
<p>從用量型檔案，加總 <strong>PretaxCharges</strong> 欄</p>
</td>
</tr>
<tr>
<td>
<p>循環折扣</p>
</td>
<td>
<p>套用至定期費用的折扣</p>
</td>
</tr><tr>
<td>
<p>續約折扣</p>
</td>
<td>
<p>訂閱續約時套用的折扣</p>
</td>
</tr><tr>
<td>
<p>取消折扣</p>
</td>
<td>
<p>折扣取消時收取的費用</p>
</td>
</tr>
<tr>
<td>
<p><strong>其他折扣</strong></br>
<em>（以授權為基礎）</em></p>
</td>
<td>
<p><em>可套用至多個收費類型</em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p>從授權型檔案，加總 <strong>TotalOtherDiscount</strong> 欄</p>
</td>
</tr>
<tr>
<td>
<p><strong>稅金</strong>&nbsp;或&nbsp;<strong>加值稅</strong></p>
</td>
<td>
<p><em>可套用至多個收費類型</em></p>
<p><em>例外狀況：「 位移明細項目 」 已經包含稅金。請參閱信用額度&amp;調整上面。</em></p>
</td>
<td>
<p>稅金或加值稅 (VAT)</p>
</td>
<td>
<p>從授權型檔案，加總 <strong>Tax</strong> 欄</p>
<p>從用量型檔案，加總 <strong>TaxAmount</strong> 欄</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
