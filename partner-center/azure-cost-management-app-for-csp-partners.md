---
title: 適用於 CSP 合作夥伴的 Cloudyn 支援的 Azure 成本管理 | 合作夥伴中心
ms.topic: article
ms.date: 03/15/2019
description: Cloudyn 支援的 Azure 成本管理需要對 Partner Center API 佈建存取權。
author: Janet
ms.author: janet
Keywords: Azure 成本管理應用程式, 管理成本, web 應用程式
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 27ff91d9d42f08e44f812663f3d4409e1080d580
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820307"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="dd36f-104">Azure CSP 合作夥伴適用的 Azure 成本管理應用程式</span><span class="sxs-lookup"><span data-stu-id="dd36f-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="dd36f-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="dd36f-105">**Applies to**</span></span>

-  <span data-ttu-id="dd36f-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="dd36f-106">Partner Center</span></span>

[<span data-ttu-id="dd36f-107">取得 Azure 成本管理的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="dd36f-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="dd36f-108">開始之前</span><span class="sxs-lookup"><span data-stu-id="dd36f-108">Before you begin</span></span>
<span data-ttu-id="dd36f-109">在可以使用 Azure 成本管理之前，請先確定您符合下列需求：</span><span class="sxs-lookup"><span data-stu-id="dd36f-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="dd36f-110">您是雲端解決方案提供者計畫的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="dd36f-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="dd36f-111">您有能力建立 Partner Center API Web 應用程式。</span><span class="sxs-lookup"><span data-stu-id="dd36f-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="dd36f-112">總覽</span><span class="sxs-lookup"><span data-stu-id="dd36f-112">Overview</span></span>

<span data-ttu-id="dd36f-113">Cloudyn 是一個 web 應用程式, 可讓您追蹤及管理客戶使用 Azure 的程度, 以及該使用量的成本。</span><span class="sxs-lookup"><span data-stu-id="dd36f-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="dd36f-114">您是透過合作夥伴中心 API 使用此應用程式。</span><span class="sxs-lookup"><span data-stu-id="dd36f-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="dd36f-115">在合作夥伴中心註冊您的 Web 應用程式</span><span class="sxs-lookup"><span data-stu-id="dd36f-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="dd36f-116">當您在合作夥伴中心註冊 Azure Active Directory Web 應用程式，您就啟用對合作夥伴中心 API 的存取權。</span><span class="sxs-lookup"><span data-stu-id="dd36f-116">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="dd36f-117">使用[全域系統管理員或系統管理代理人帳戶](create-user-accounts-and-set-permissions.md)登入[合作夥伴中心](https://partnercenter.microsoft.com/pcv/dashboard/overview)。</span><span class="sxs-lookup"><span data-stu-id="dd36f-117">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="dd36f-118">從**合作夥伴中心**, 選取 [**帳戶設定** &gt; ] [ **[應用程式管理](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** ]。</span><span class="sxs-lookup"><span data-stu-id="dd36f-118">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="dd36f-119">在 **\[Web 應用程式\]** 區段中，按一下 **\[新增 Web 應用程式\]** 。</span><span class="sxs-lookup"><span data-stu-id="dd36f-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="dd36f-120">**注意**：如果您先前已建立 web 應用程式, 可以略過步驟3。</span><span class="sxs-lookup"><span data-stu-id="dd36f-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="dd36f-121">複製並儲存您 Web 應用程式的**商務識別碼** GUID 和**應用程式識別碼** GUID。</span><span class="sxs-lookup"><span data-stu-id="dd36f-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="dd36f-122">您將需要這兩個識別碼，才能使用 30 天免費試用版的 Azure 成本管理應用程式。</span><span class="sxs-lookup"><span data-stu-id="dd36f-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="dd36f-123">將秘密金鑰新增到您的應用程式。</span><span class="sxs-lookup"><span data-stu-id="dd36f-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="dd36f-124">在 **\[新增金鑰\]** 按鈕旁邊的下拉式清單中，選取 1 或 2 年期間。</span><span class="sxs-lookup"><span data-stu-id="dd36f-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="dd36f-125">按一下 **\[新增金鑰\]** 。</span><span class="sxs-lookup"><span data-stu-id="dd36f-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="dd36f-126">複製並儲存秘密金鑰值。</span><span class="sxs-lookup"><span data-stu-id="dd36f-126">Copy and save the secret key value.</span></span> <span data-ttu-id="dd36f-127">您將需要此值，以便使用 30 天免費試用版。</span><span class="sxs-lookup"><span data-stu-id="dd36f-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="dd36f-128">應用程式秘密金鑰就像是具有較長到期日的密碼。</span><span class="sxs-lookup"><span data-stu-id="dd36f-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="dd36f-129">請將金鑰值儲存在安全的位置，以供未來使用。</span><span class="sxs-lookup"><span data-stu-id="dd36f-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="dd36f-130">後續步驟</span><span class="sxs-lookup"><span data-stu-id="dd36f-130">Next steps</span></span>
<span data-ttu-id="dd36f-131">啟動 [30 天免費試用版](https://go.microsoft.com/fwlink/?linkid=857895)。</span><span class="sxs-lookup"><span data-stu-id="dd36f-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="dd36f-132">若要啟動試用版，您需要下列資訊：</span><span class="sxs-lookup"><span data-stu-id="dd36f-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="dd36f-133">合作夥伴中心登入憑證</span><span class="sxs-lookup"><span data-stu-id="dd36f-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="dd36f-134">商務識別碼 GUID</span><span class="sxs-lookup"><span data-stu-id="dd36f-134">Commerce ID GUID</span></span>
- <span data-ttu-id="dd36f-135">應用程式識別碼 GUID</span><span class="sxs-lookup"><span data-stu-id="dd36f-135">App ID GUID</span></span>
- <span data-ttu-id="dd36f-136">應用程式秘密金鑰值</span><span class="sxs-lookup"><span data-stu-id="dd36f-136">Application secret key value</span></span>
