---
title: 合作夥伴安全性需求常見問題集 | 合作夥伴中心
ms.topic: article
ms.date: 08/23/2019
description: 關於合作夥伴安全性需求的常見問題集
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 雲端解決方案提供者, 雲端解決方案提供者計畫, CSP, 控制台廠商, CPV, 多重要素驗證, MFA, 安全應用程式模型, 安全應用程式模型, 安全性
ms.localizationpriority: medium
ms.openlocfilehash: 54ac919aeadec85b941e0dce9b1556df843e5fcb
ms.sourcegitcommit: 435634c55c3d20a42083c0a58d96c7f6b8ec0a6d
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/26/2019
ms.locfileid: "70020538"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>關於合作夥伴安全性需求的常見問題集

此文章包含[合作夥伴安全性需求](partner-security-requirements.md)的常見問題集。

## <a name="partner-security-requirements"></a>合作夥伴安全性需求

### <a name="what-are-the-new-partner-security-requirements"></a>新的合作夥伴安全性需求為何？

為了保護合作夥伴和您的客戶，我們要求合作夥伴立即採取下列動作：  

1. **針對合作夥伴租用戶中的所有使用者啟用 Multi-Factor Authentication (MFA)** 。 合作夥伴租用戶中的所有使用者在登入 Microsoft 商業雲端服務，或是透過合作夥伴中心或 API 在雲端解決方案提供者中進行交易時，都必須使用 Multi-Factor Authentication (MFA)。 透過啟用基準保護原則，便可免費將 MFA 提供給合作夥伴租用戶的所有使用者使用。

2. **採用安全應用程式模型架構**。 與 Microsoft API (例如 Azure Resource Manager、Microsoft Graph 及合作夥伴中心 API) 整合的所有合作夥伴都必須採用安全應用程式模型架構，以在啟用基準保護原則時避免對其整合產生任何中斷。

啟用 Multi-Factor Authentication (MFA) 並採用安全應用程式模型架構將可協助保護您的基礎結構，並保護您客戶的資料免於潛在的安全性風險 (例如身分盜用或其他詐騙事件)。  

### <a name="which-partners-need-to-meet-the-requirements"></a>有哪些合作夥伴必須符合需求？

這些需求適用於下列合作夥伴群組：

- 所有參與雲端解決方案提供者 (CSP) 方案且使用 Microsoft 商業雲端服務進行交易的合作夥伴組織
  - 直接帳單合作夥伴
  - 間接提供者
  - 間接轉銷商
- 所有控制台廠商
- 所有顧問方案合作夥伴  

透過主權雲端 (21Vianet、US Government 和 Germany) 進行交易的所有合作夥伴並不需要符合於 8 月 1 日生效的新安全性需求。 不過，我們強烈建議使用主權雲端的所有合作夥伴立即行動並採用這些新的安全性需求。 Microsoft 未來將針對主權雲端的這些安全性需求強制執行，提供額外的詳細資料。

### <a name="what-are-the-key-timelines-and-milestones"></a>有哪些關鍵時程表和里程碑？

與這些安全性需求相關聯的條款將會立即新增至[適用於雲端解決方案提供者計畫的計畫指南](https://go.microsoft.com/fwlink/p/?LinkId=617100)。 從 2019 年 8 月 1 日開始，您必須實作這些安全性需求以符合參與雲端解決方案提供者計畫的規範。

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>如果我不採取任何動作，會發生什麼事情？

在強制執行這些合作夥伴安全性需求之後，未遵守這些安全性作法及義務的合作夥伴，將無法在雲端解決方案提供者計畫中進行交易，或利用委派系統管理員權限來管理客戶租用戶。 我們正在為需求建立強制執行日期，並且將通知合作夥伴相關的日期與詳細資訊。

### <a name="what-will-happen-if-i-dont-implement-mfa-as-per-this-new-security-requirement-by-august-1-2019"></a>如果我在 2019 年 8 月 1 日之前都沒有根據這個新的安全性需求實作 MFA，會發生什麼事？

從 2019 年 8 月 1 日開始，在[適用於雲端解決方案提供者計畫的計畫指南](https://go.microsoft.com/fwlink/p/?LinkId=617100)中與這些安全性需求相關聯的條款將會生效。 參與雲端解決方案提供者計畫的所有合作夥伴都應該符合這些需求，以符合條款規範並保護其業務。 在我們於不久的未來開始針對合作夥伴安全性需求進行技術強制執行之後，未遵守這些安全性作法的合作夥伴可能會失去在雲端解決方案提供者計畫中進行交易，或利用委派系統管理員權限來管理客戶租用戶的能力。 我們正在建立強制執行日期，並且很快便會將該日期通知合作夥伴。

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>Microsoft 為何要強制執行這些新的需求？

確保客戶及合作夥伴的安全性和隱私權是 Microsoft 最為優先的工作。 我們持續看到更為複雜且更加頻繁發生的安全性攻擊，這些攻擊主要都與身分識別入侵事件有關。 由於預防性控制項在對抗安全性攻擊的整體防禦策略中扮演重要角色，我們將會開始強制執行一組強制的安全性需求，以協助保護合作夥伴與其客戶。

### <a name="does-this-apply-to-all-geographies"></a>這是否適用於所有地理位置？

是。這適用於所有地理位置。 我們強烈建議所有合作夥伴透過主權雲端 (21Vianet、US Government 和 Germany) 進行交易，並立即採取這些新的安全性需求。 不過，這些合作夥伴不需要符合 2019 年 8 月 1 日生效的新安全性需求。 Microsoft 未來將針對主權雲端的這些安全性需求強制執行，提供額外的詳細資料。

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>是否可以要求特別排除某個帳戶？

否。您無法針對強制執行 MFA 的需求排除任何帳戶。 基於合作夥伴所擁有的高度權限，[適用於雲端解決方案提供者計畫的計畫指南](https://go.microsoft.com/fwlink/p/?LinkId=617100)要求針對您合作夥伴租用戶中的每個帳戶強制執行 MFA。

## <a name="required-actions"></a>必要動作

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>我需要採取哪些關鍵動作來符合需求？

雲端解決方案提供者計畫 (直接帳單、間接提供者及間接轉銷商)、顧問及控制台廠商中的所有合作夥伴都必須符合需求。

1. **為所有使用者強制執行 MFA**

    雲端解決方案提供者計畫、顧問及控制台廠商中的所有合作夥伴都必須針對其合作夥伴租用戶中的所有使用者強制執行 MFA。 這可以透過啟用[要求系統管理員使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) \(部分機器翻譯\)、[使用者保護基準](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) \(部分機器翻譯\)，以及任何未來的基準原則來達成。 基準原則所提供的功能將會持續演進，以保護合作夥伴和客戶不受持續變動之安全性威脅的危害。 因此，請務必檢閱[基準原則文件](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) \(部分機器翻譯\) 以深入了解。

    - 參閱[基準原則：要求系統管理員使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) \(部分機器翻譯\)，以取得如何啟用「要求系統管理員使用 MFA」基準原則的詳細資料。
    - 參閱[基準原則：使用者保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) \(部分機器翻譯\)，以取得如何啟用「使用者保護」基準原則的詳細資料。
    - 了解[基準保護原則](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) \(部分機器翻譯\) 的概念。

    其他考量：

    - 間接提供者必須與間接轉銷商合作以上線至合作夥伴中心 (如果他們尚未這麼做)，並鼓勵其轉銷商符合需求。
    - Azure MFA 現已透過基準原則免費提供給合作夥伴租用戶中的所有使用者使用，其唯一驗證的方法是使用 [Microsoft Authenticator 應用程式](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)。
    - 如果需要其他方法 (例如 SMS 或電子郵件)，[Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU 能提供額外的驗證方法。
    - 合作夥伴也可以在存取 Microsoft 商業雲端服務時，針對每個使用者運用協力廠商 MFA 解決方案。

2. **採用安全應用程式模型架構**

    已使用任何 API (例如 Azure Resource Manager、Microsoft Graph、合作夥伴中心 API 等) 開發自訂整合，或是使用 PowerShell 等工具實作自訂自動化的所有合作夥伴，都必須採用[安全應用程式模型架構](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) \(英文\) 來與 Microsoft 雲端服務整合。 如果未這麼做，則可能會因部署 MFA 而導致中斷。 下列資源能提供採用此模型之方法的相關概觀和指引。

    - [安全應用程式模型概觀](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) \(英文\)
    - [合作夥伴中心：安全應用程式模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [雲端解決方案提供者計畫中的合作夥伴：用於啟用安全應用程式模型的 .NET 範例程式碼](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) \(英文\)
    - [雲端解決方案提供者計畫中的合作夥伴：用於啟用安全應用程式模型的 Java 範例程式碼](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model) \(英文\)
    - [合作夥伴中心驗證文件](https://docs.microsoft.com/partner-center/develop/partner-center-authentication) \(英文\)
    - [合作夥伴中心 PowerShell Multi-Factor Authentication (MFA) 文件](https://docs.microsoft.com/partner-center/develop/multi-factor-auth) \(英文\)

    如果您使用的是控制台，則必須洽詢廠商有關採用安全應用程式模型架構的事宜。

    控制台廠商必須以控制台廠商的身分針對合作夥伴中心進行[上線](https://docs.microsoft.com/partner-center/enroll-as-cpv)，並立即開始實作此需求。 請參閱[合作夥伴中心：安全應用程式模型架構](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 控制台廠商必須接受並管理雲端解決方案提供者合作夥伴的同意 (而非認證)，並清除所有現有雲端解決方案提供者合作夥伴的認證。

## <a name="multi-factor-authentication"></a>多重要素驗證

### <a name="what-is-multi-factor-authentication-mfa"></a>什麼是 Multi-Factor Authentication (MFA)？

MFA 是一種安全性機制，可以透過一個以上的必要安全性和驗證程序來驗證個人。 它是透過要求進行下列兩種或更多驗證方法來運作：

- 您知道的資訊 (通常是密碼)
- 您擁有的事物 (不易複製的受信任裝置，例如電話)
- 代表您身分的事物 (生物識別技術)

### <a name="what-are-baseline-protection-policies"></a>什麼是基準保護原則？

[Microsoft 基準保護原則](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) \(部分機器翻譯\) (目前處於預覽狀態) 是一組預先定義的原則，可協助組織抵禦許多常見的攻擊。 這些常見的攻擊可能包括密碼噴灑、重播和網路釣魚。 基準保護原則適用於所有版本的 Azure Active Directory。 Microsoft 將這些基準保護原則提供給所有人使用的原因，是因為以身分識別為基礎的攻擊在過去幾年一直持續攀升。 這些原則的目標是為了確保所有組織都能在不需額外成本的情況下，具備基準層級的安全性。

> [!NOTE]
> Microsoft 基準原則與相關功能將會持續演進，以更有效地保護合作夥伴和客戶不受持續變動之安全性威脅的危害。 我們可能很快就會對基準原則的命名和分類做出變更。 我們強烈建議您直接造訪基準原則頁面以查看最新資訊。

### <a name="what-baseline-policies-must-i-enable"></a>我必須啟用哪些基準原則？

如果您計畫運用目前的基準保護原則來為合作夥伴租用戶中的每個使用者提供 MFA，便必須啟用[要求系統管理員使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) \(部分機器翻譯\) 和[使用者保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) \(部分機器翻譯\) 基準原則。 這些基準保護原則將能免費滿足為合作夥伴租用戶中的每個使用者提供 MFA 的需求，前提是合作夥伴必須透過行動裝置使用 Microsoft Authenticator 應用程式。

[要求系統管理員使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) \(部分機器翻譯\) 基準原則會運用在合作夥伴目錄中的系統管理使用者身上，而[使用者保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) \(部分機器翻譯\) 基準原則會運用來保護合作夥伴租用戶中的非系統管理使用者。 使用者必須註冊 MFA 才能啟用這些原則。 在使用者成功註冊之後，系統會在他們嘗試登入時，根據原則的條件提示他們進行 MFA。 基準原則所提供的功能將會持續演進，以保護合作夥伴和客戶不受持續變動之安全性威脅的危害。 因此，請務必檢閱[基準原則文件](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) \(部分機器翻譯\) 以深入了解。

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>如何啟用「要求系統管理員使用 MFA」原則？

「要求系統管理員使用 MFA」基準原則可透過 Azure 管理入口網站啟用。 請參閱[基準原則：要求系統管理員使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) \(部分機器翻譯\)，以取得如何啟用此基準原則的詳細資料。

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>如何啟用「使用者保護」原則？

「使用者保護」基準原則可透過 Azure 管理入口網站啟用。 請參閱[基準原則：使用者保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) \(部分機器翻譯\)，以取得如何啟用此基準原則的詳細資料。

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>系統是否會自動啟用基準原則？

否。若要啟用這些原則，身為全域系統管理員、安全性系統管理員，或條件式存取系統管理員角色之成員的使用者必須設定原則以立即使用原則。

### <a name="what-is-the-cost-of-enabling-mfa"></a>啟用 MFA 的成本為何？

您可透過實作[要求系統管理員使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) \(部分機器翻譯\) 和[使用者保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) \(部分機器翻譯\) 基準保護原則，來使用 Microsoft 免費提供的 MFA。 此版本 MFA 唯一的驗證選項是 [Microsoft Authenticator 應用程式](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)。 如果需要撥打電話或 SMS 訊息，便必須購買 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) 授權。 或者，您可以運用協力廠商解決方案來為合作夥伴租用戶中的每個使用者提供MFA；在此情況下，您必須負責確保 MFA 解決方案已強制執行，且您已符合規範。

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>如果我已經有 MFA 解決方案，需要採取哪些動作？

透過這些安全性需求，合作夥伴租用戶中的使用者在存取 Microsoft 商業雲端服務時，必須使用 MFA 進行驗證。 您可以使用協力廠商解決方案來滿足這些需求。 Microsoft 已不再針對獨立身分識別提供者提供驗證測試，以確認與 Azure Active Directory 之間的相容性。 如果您想要測試您產品的互通性，請參閱這些[指導方針](https://www.microsoft.com/download/details.aspx?id=56843) \(英文\)。

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>我可以使用哪些驗證方法來驗證 MFA？

您可透過實作[要求系統管理員使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) \(部分機器翻譯\) 和[使用者保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) \(部分機器翻譯\) 基準保護原則，來使用 Microsoft 免費提供的 MFA。 此版本 MFA 唯一的驗證選項是 [Microsoft Authenticator 應用程式](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)。 如果需要撥打電話或 SMS 訊息，便必須購買 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) 授權。 或者，您可以運用協力廠商解決方案來為合作夥伴租用戶中的每個使用者提供MFA；在此情況下，您必須負責確保 MFA 解決方案已強制執行，且您已符合規範。

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>我使用多個合作夥伴租用戶來進行交易。 我是否需要對它們全部實作 MFA？

是。您必須針對與雲端解決方案提供者計畫或顧問計畫相關聯的每個 Azure Active Directory 租用戶強制執行 MFA。 如果您計畫購買 Azure Active Directory Premium 授權，則您必須為每個 Azure Active Directory 租用戶中的使用者購買授權。

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>我合作夥伴租用戶中的每個使用者是否都必須強制執行 MFA？*

[要求系統管理員使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) \(部分機器翻譯\) 和[使用者保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) \(部分機器翻譯\) 基準保護原則將會針對您合作夥伴租用戶中的每個使用者強制執行 MFA。 如果您正在運用這些原則來提供 MFA，且正在使用 [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview) 應用程式，便不需要購買任何額外的授權。 否則，您將必須購買適當的解決方案來為合作夥伴租用戶中的每個使用者提供 MFA。

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>我是 Microsoft 的直接帳單合作夥伴。 我需要做些什麼？

直接帳單雲端解決方案提供者合作夥伴必須針對其合作夥伴租用戶中的每個使用者強制執行 MFA。

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>我是間接轉銷商，且僅透過經銷商進行交易。 我仍然需要這麼做嗎？

所有間接轉銷商都必須針對其合作夥伴租用戶中的每個使用者強制執行 MFA。 這是間接轉銷商必須執行的動作。

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>我不使用合作夥伴中心 API。 我是否仍然需要實作 MFA？

是。此安全性需求適用於所有使用者，包括合作夥伴租用戶中的合作夥伴系統管理使用者及使用者。

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>哪些協力廠商提供與 Azure Active Directory 相容的 MFA 解決方案？

線上有許多 MFA 解決方案的獨立評論，例如 [Gartner](https://www.gartner.com/en/webinars/3881781) \(英文\)。 檢閱 MFA 廠商及解決方案時，合作夥伴必須確保他們所選擇的解決方案能與 Azure Active Directory 相容。

Microsoft 已不再針對獨立身分識別提供者提供驗證測試，以確認與 Azure Active Directory 之間的相容性。 如果您想要測試您產品的互通性，請參閱這些[指導方針](https://www.microsoft.com/download/details.aspx?id=56843) \(英文\)。

如需詳細資訊，請參閱 [Azure AD 同盟相容性清單](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility) \(部分機器翻譯\)。

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>我要如何在我們的整合沙箱中測試 MFA？

您應該針對您的整合沙箱租用戶啟用[要求系統管理員使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) \(部分機器翻譯\) 和[使用者保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) \(部分機器翻譯\) 基準原則。 透過此原則，租用戶中的每個使用者都必須使用 MFA 進行驗證。

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>啟用 MFA 是否會影響我與客戶租用戶之間的互動方式？

不。 履行這些安全性需求將不會影響您管理客戶的方式。 您執行委派系統管理作業的能力將不會中斷。

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>我的客戶是否需要遵守合作夥伴安全性需求？

否。您不需要針對您客戶 Azure AD 租用戶中的每個使用者強制執行 MFA。 不過，建議您與每個客戶合作，以判斷保護其使用者的最佳方式。

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>是否可以搭配基準保護原則使用應用程式密碼？

是。可以使用[應用程式密碼](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) \(部分機器翻譯\)。 您應該檢閱[這裡](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) \(部分機器翻譯\) 所記載的應用程式密碼使用考量，以判斷它們是否支援您的需求。

### <a name="can-any-user-be-excluded-from-this-requirement"></a>是否可以將任何使用者排除於此需求之外？

否。您合作夥伴租用戶中的每個使用者 (包括服務帳戶) 都必須使用 MFA 進行驗證。

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>合作夥伴安全性需求是否適用於整合沙箱？

是。合作夥伴安全性需求適用於整合沙箱。 這代表您必須為整合沙箱租用戶中的使用者實作適當的 MFA 解決方案。 建議您實作基準保護原則來提供 MFA。

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>我如何設定緊急存取 (緊急開關) 帳戶？

一般認為的最佳做法，是建立一或兩個緊急存取帳戶，以因應不小心被封鎖在自己的 Azure AD 租用戶之外的情況。 基於合作夥伴安全性需求，每個使用者都必須使用 MFA 進行驗證。 這代表您必須修改緊急存取帳戶的定義。 它可以是運用協力廠商解決方案來進行 MFA 的帳戶。

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>合作夥伴安全性需求會如何影響來賓使用者？

來賓使用者在存取合作夥伴租用戶中的資源時，將必須使用 MFA 進行驗證。 合作夥伴安全性需求對於存取其自己租用戶中資源的來賓使用者將不會有任何影響。

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>如果我是使用協力廠商解決方案，是否需要 Active Directory 同盟服務 (ADFS)？

否。如果您使用協力廠商解決方案，則並不需要 Active Directory 同盟服務 (ADFS)。 建議您與解決方案的廠商合作，以判斷其解決方案的需求為何。

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>是否一定要啟用基準保護原則？

否。您不一定需要啟用基準保護原則。 唯一的需求是針對合作夥伴租用戶中的每個使用者 (包括服務帳戶) 強制執行 MFA。

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>是否可以使用條件式存取來符合 MFA 需求？

是。您可以使用條件式存取來針對合作夥伴租用戶中的每個使用者 (包括服務帳戶) 強制執行 MFA。 不過，基於合作夥伴所擁有的高度權限，我們必須確保每個使用者的每個驗證都有 MFA 挑戰。 這代表您將無法運用條件式存取能避開 MFA 需求的功能。

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>實作基準保護原則能提供哪些驗證選項？

針對透過實作基準保護原則所提供的 MFA 版本，唯一可用的驗證選項是驗證器應用程式。 使用撥打電話和簡訊的方式被視為較不安全。 因此，這些選項並無法透過此版本的 MFA 使用。

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>合作夥伴安全性需求是否會影響到 Azure AD Connect 所使用的服務帳戶？

否。合作夥伴安全性需求並不會影響到 Azure AD Connect 所使用的服務帳戶。 如果您因強制執行 MFA 而遇到與 Azure AD Connect 相關的問題，請向 Microsoft 支援服務開啟技術性支援要求。

## <a name="secure-application-model"></a>安全應用程式模型

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>誰應該採用安全應用程式模型來符合需求？

Microsoft 正在引進一個能運用 Multi-Factor Authentication 的安全可擴充架構，來驗證雲端解決方案提供者 (CSP) 合作夥伴和控制台廠商 (CPV)。 如需詳細資訊，請參閱[安全應用程式模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 已使用任何 API (例如 Azure Resource Manager、Microsoft Graph、合作夥伴中心 API 等) 開發自訂整合，或是使用 PowerShell 等工具實作自訂自動化的所有合作夥伴，都必須採用[安全應用程式模型架構](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) \(英文\) 來與 Microsoft 雲端服務整合。

### <a name="what-is-the-secure-application-model"></a>什麼是安全應用程式模型？

Microsoft 正在引進一個能運用 Multi-Factor Authentication 的安全可擴充架構，來驗證雲端解決方案提供者 (CSP) 合作夥伴和控制台廠商 (CPV)。 如需詳細資訊，請參閱[安全應用程式模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。  

### <a name="how-do-i-implement-the-secure-application-model"></a>我要如何實作安全應用程式模型？

已使用任何 API (例如 Azure Resource Manager、Microsoft Graph、合作夥伴中心 API 等) 開發自訂整合，或是使用 PowerShell 等工具實作自訂自動化的所有合作夥伴，都必須採用[安全應用程式模型架構](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) \(英文\) 來與 Microsoft 雲端服務整合。 如果未這麼做，則可能會因部署 MFA 而導致中斷。 下列資源能提供採用此模型之方法的相關概觀和指引。

- [安全應用程式模型概觀](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) \(英文\)
- [合作夥伴中心：安全應用程式模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [雲端解決方案提供者計畫中的合作夥伴：用於啟用安全應用程式模型的 .NET 範例程式碼](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) \(英文\)
- [雲端解決方案提供者計畫中的合作夥伴：用於啟用安全應用程式模型的 Java 範例程式碼](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model) \(英文\)
- [合作夥伴中心驗證文件](https://docs.microsoft.com/partner-center/develop/partner-center-authentication) \(英文\)
- [合作夥伴中心 PowerShell Multi-Factor Authentication (MFA) 文件](https://docs.microsoft.com/partner-center/develop/multi-factor-auth) \(英文\)

如果您使用的是控制台，則必須洽詢廠商有關採用安全應用程式模型架構的事宜。

控制台廠商必須以控制台廠商的身分針對合作夥伴中心進行[上線](https://docs.microsoft.com/partner-center/enroll-as-cpv)，並立即開始實作此需求。 請參閱[合作夥伴中心：安全應用程式模型架構](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 控制台廠商必須接受並管理雲端解決方案提供者合作夥伴的同意 (而非認證)，並清除所有現有雲端解決方案提供者合作夥伴的認證。

### <a name="who-is-a-control-panel-vendor-cpv"></a>誰是控制台廠商 (CPV)？

控制台廠商是開發應用程式以供雲端解決方案提供者合作夥伴用來與合作夥伴中心 API 整合的獨立軟體廠商。 控制台廠商不是能直接存取合作夥伴中心儀表板或 API 的雲端解決方案提供者合作夥伴。 如需詳細描述，請參閱[合作夥伴中心：安全應用程式模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)。

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>安全應用程式模型是否僅需針對合作夥伴中心 API/SDK 實作？

在啟用*要求系統管理員使用 MFA* 和*使用者保護*基準原則之後，每個使用者都必須使用 Multi-Factor Authentication 進行驗證。 這代表您必須針對要以非互動方式執行，且仰賴使用使用者認證進行驗證的每個 API、CLI 及 PowerShell 模組 (例如 Azure、Azure AD、MS Online、合作夥伴中心等) 實作安全應用程式模型。

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>我正在使用 PowerShell 之類的自動化工具。 我要如何實作安全應用程式模型？

如果您的自動化是要以非互動方式執行，且仰賴使用使用者認證進行驗證，則您必須實作安全應用程式模型。 請參閱[安全應用程式模型 | 合作夥伴中心 PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) \(英文\) 以取得如何實作此架構的指引。  請記住，並非所有自動化工具都會提供使用存取權杖進行驗證的能力。 如果您需要協助以了解應該進行哪些變更，請在[合作夥伴中心安全性指引](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) \(英文\) 群組上張貼訊息。

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>應用程式系統管理員在執行同意程序時，應該提供哪些使用者認證？

建議您使用已指派最低權限的服務帳戶。 就合作夥伴中心 API 而言，這表示您應該使用已指派「銷售代理人」或「系統管理代理人」角色的帳戶。

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>應用程式系統管理員在執行同意程序時，為何不應該提供全域系統管理使用者認證？

使用最低權限的身分識別是最佳做法，因為那可降低風險。 不建議使用具有全域系統管理權限之帳戶的原因，是因為那會提供比起所需範圍還要多的權限

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>我是雲端解決方案提供者合作夥伴。 我要如何知道自己的控制台廠商 (CPV) 是否正在實作該解決方案？

針對使用控制台廠商 (CPV) 解決方案來在雲端解決方案提供者 (CSP) 計畫中進行交易的合作夥伴，您必須負責洽詢自己的 CPV。

### <a name="i-am-a-cpv-how-do-i-enroll"></a>我是 CPV。 我要如何註冊？

若要註冊為控制台廠商 (CPV)，請遵循[這裡](https://docs.microsoft.com/partner-center/enroll-as-cpv)所提供的指導方針。

若要接收註冊連結，CPV 必須連絡 [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com)，並提供與該 CPV 具有商務關係或了解其業務的 Microsoft 員工贊助者。 例如合作夥伴開發經理 (PDM)。

在您註冊至合作夥伴中心並註冊您的應用程式之後，您將能存取合作夥伴中心 API。 如果您是新的 CPV，您將能透過合作夥伴中心通知接收到您的沙箱資訊。 在您完成 Microsoft CPV 的註冊，並接受 CPV 合約之後，您便可以：

1. 管理多租用戶應用程式 (將應用程式加入 Azure 入口網站、在合作夥伴中心中將應用程式註冊及解除註冊)。 注意：CPV 必須在合作夥伴中心註冊其應用程式，以取得合作夥伴中心 API 的授權。 單純將應用程式加入 Azure 入口網站，並無法授權 CPV 應用程式使用合作夥伴中心 API。
2. 檢視及管理您的 CPV 設定檔。
3. 檢視及管理您需要存取 CPV 功能的使用者。 CPV 唯一可以擁有的角色是全域管理員。

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>我正在使用合作夥伴中心 SDK。 該 SDK 是否會自動採用安全應用程式模型？

否。您必須遵循[安全應用程式模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)中所提供的指導方針。

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>我是否可以搭配未啟用 MFA 的帳戶針對安全應用程式模型產生重新整理權杖？

是。可以使用未強制執行 MFA 的帳戶產生重新整理權杖。 不過您不應該這麼做，因為基於 MFA 需求的因素，使用未啟用 MFA 的帳戶產生的所有權杖都會無法存取資源。

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>在啟用 MFA 的情況下，我的應用程式要如何取得存取權杖？

您必須遵循[安全應用程式模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)，其中會提供如何在遵守新安全性需求的情況下執行此操作的詳細資料。 您可以在[這裡](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) \(英文\) 找到 .NET 範例程式碼，並在[這裡](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model) \(英文\) 找到 Java 範例程式碼。

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>身為 CPV，我要如何在我們的 CPV 租用戶，或是 CSP 合作夥伴的租用戶中建立 Azure AD 應用程式？

CPV 必須在與其註冊為 CPV 時所關聯的租用戶中建立 Azure Active Directory 應用程式。

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>我是使用僅限應用程式驗證的 CSP。 我是否需要進行任何變更？

僅限應用程式驗證並不會受到影響，因為使用者認證不會用來要求存取權杖。 如果會共用使用者認證，控制台廠商 (CPV) 必須採用[安全應用程式模型架構](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)，並清除其所擁有的任何現有合作夥伴認證。

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>身為 CPV，我是否可以運用僅限應用程式驗證樣式來取得存取權杖？

否。控制台廠商合作夥伴並無法運用僅限應用程式驗證樣式來代表合作夥伴要求存取權杖。 他們應該實作安全應用程式模型，這能運用應用程式 + 使用者驗證樣式。

## <a name="key-resources"></a>主要資源

### <a name="how-to-get-started"></a>如何開始使用

- [合作夥伴安全性需求：逐步指南](https://docs.microsoft.com/partner-center/partner-security-requirements)。
- 將您的問題和意見反應移至此[合作夥伴中心安全性指引群組](https://aka.ms/MPCSecurityGuidance) \(英文\)。
- 參與近期的合作夥伴辦公時間和網路研討會。 請查看[這裡的詳細排程和資源](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) \(英文\)。

### <a name="resources-for-enabling-mfa"></a>啟用 MFA 的資源

- 了解[基準保護原則](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) \(部分機器翻譯\) 的概念。
- 參閱[基準原則：要求系統管理員使用 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) \(部分機器翻譯\)，以取得如何啟用「要求系統管理員使用 MFA」基準原則的詳細資料。
- 參閱[基準原則：使用者保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) \(部分機器翻譯\)，以取得如何啟用「使用者保護」基準原則的詳細資料。

### <a name="resources-for-adopting-secure-application-model"></a>採用安全應用程式模型的資源

- [安全應用程式模型概觀](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) \(英文\)
- [合作夥伴中心：安全應用程式模型指南](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [雲端解決方案提供者計畫中的合作夥伴：用於啟用安全應用程式模型的 .NET 範例程式碼](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) \(英文\)
- [雲端解決方案提供者計畫中的合作夥伴：用於啟用安全應用程式模型的 Java 範例程式碼](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model) \(英文\)
- [合作夥伴中心驗證文件](https://docs.microsoft.com/partner-center/develop/partner-center-authentication) \(英文\)
- [合作夥伴中心 PowerShell Multi-Factor Authentication (MFA) 文件](https://docs.microsoft.com/partner-center/develop/multi-factor-auth) \(英文\)

## <a name="support"></a>支援

### <a name="where-can-i-get-support"></a>我可以在哪裡取得支援？

如需符合安全性需求的支援資源，如果您具有進階合作夥伴支援 (ASfP)，請連絡您的服務帳戶經理；如果您具有頂級合作夥伴支援合約 (PSfP)，請連絡您的服務帳戶經理及技術帳戶經理。

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>我如何取得啟用基準原則的協助？

- 合作夥伴可以運用 MPN 權益的諮詢時數，以取得如何實作安全性需求的詳細指引。
- 您可透過 MPN 權益使用適用於 Azure Active Directory 的技術產品支援選項。 能存取有效 ASfP 或 PSfP 合約的合作夥伴可以與其相關聯的帳戶經理 (SAM/TAM) 合作，以了解最適合他們的選項。
- 搭配合作夥伴中心實作基準原則的支援，可透過[合作夥伴中心服務要求](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)來存取。 請選取 [MFA & Secure Application Model]  \(MFA 與安全應用程式模型\) 作為主題。

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>我如何取得技術資訊和支援以協助採用安全應用程式模型架構？

您可透過 MPN 權益使用適用於 Azure Active Directory 的技術產品支援選項。 能存取有效 ASfP 或 PSfP 訂用帳戶的合作夥伴可以與其相關聯的帳戶經理 (SAM/TAM) 合作，以了解最適合他們的選項。

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>我可以在哪裡找到技術性常見問題的詳細資訊？

關於技術性常見問題的相關資訊可在[這裡](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues)找到。
