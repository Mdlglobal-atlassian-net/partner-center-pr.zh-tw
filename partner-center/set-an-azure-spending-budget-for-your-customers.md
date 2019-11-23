---
title: 為客戶設定 Azure 消費預算 | 合作夥伴中心
ms.topic: article
ms.date: 11/21/2019
description: Set a monthly budget per customer in Partner Center.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 05212746e1ccbcc5081c68ca97ced6a99e20bb8c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384896"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="f8e63-103">為客戶設定 Azure 消費預算</span><span class="sxs-lookup"><span data-stu-id="f8e63-103">Set an Azure spending budget for your customers</span></span>

<span data-ttu-id="f8e63-104">適用於：</span><span class="sxs-lookup"><span data-stu-id="f8e63-104">Applies to:</span></span>

- <span data-ttu-id="f8e63-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="f8e63-105">Partner Center</span></span>
- <span data-ttu-id="f8e63-106">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="f8e63-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="f8e63-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f8e63-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="f8e63-108">This helps your customers manage their Azure spending.</span><span class="sxs-lookup"><span data-stu-id="f8e63-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="f8e63-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span><span class="sxs-lookup"><span data-stu-id="f8e63-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="f8e63-110">It also helps your customers budget their Azure spending so their monthly bill isn't higher than they anticipate.</span><span class="sxs-lookup"><span data-stu-id="f8e63-110">It also helps your customers budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>


> [!NOTE]  
> <span data-ttu-id="f8e63-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span><span class="sxs-lookup"><span data-stu-id="f8e63-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="f8e63-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span><span class="sxs-lookup"><span data-stu-id="f8e63-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="f8e63-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span><span class="sxs-lookup"><span data-stu-id="f8e63-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="f8e63-114">You can then work with your customer(s) to identify the root cause and manage costs.</span><span class="sxs-lookup"><span data-stu-id="f8e63-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="f8e63-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span><span class="sxs-lookup"><span data-stu-id="f8e63-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="f8e63-116">Check current Azure spending</span><span class="sxs-lookup"><span data-stu-id="f8e63-116">Check current Azure spending</span></span>](#check-current-azure-spending)
- [<span data-ttu-id="f8e63-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span><span class="sxs-lookup"><span data-stu-id="f8e63-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)
- [<span data-ttu-id="f8e63-118">View itemized costs by service for usage-based subscriptions</span><span class="sxs-lookup"><span data-stu-id="f8e63-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="f8e63-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span><span class="sxs-lookup"><span data-stu-id="f8e63-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="f8e63-120">Azure spending data</span><span class="sxs-lookup"><span data-stu-id="f8e63-120">Azure spending data</span></span>

<span data-ttu-id="f8e63-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span><span class="sxs-lookup"><span data-stu-id="f8e63-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="f8e63-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span><span class="sxs-lookup"><span data-stu-id="f8e63-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="f8e63-123">The spending data is *refreshed once per day*.</span><span class="sxs-lookup"><span data-stu-id="f8e63-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="f8e63-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span><span class="sxs-lookup"><span data-stu-id="f8e63-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="f8e63-125">Set Azure spending budget</span><span class="sxs-lookup"><span data-stu-id="f8e63-125">Set Azure spending budget</span></span>

<span data-ttu-id="f8e63-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="f8e63-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="f8e63-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="f8e63-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="f8e63-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="f8e63-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span><span class="sxs-lookup"><span data-stu-id="f8e63-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>
4. <span data-ttu-id="f8e63-130">Enter a value for **Monthly budget**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-130">Enter a value for **Monthly budget**.</span></span>
5. <span data-ttu-id="f8e63-131">Choose **Apply** to save your changes.</span><span class="sxs-lookup"><span data-stu-id="f8e63-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="f8e63-132">You can also *set a budget for an individual customer* in their subscription settings:</span><span class="sxs-lookup"><span data-stu-id="f8e63-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="f8e63-133">Sign in to the Partner Center dashboard.</span><span class="sxs-lookup"><span data-stu-id="f8e63-133">Sign in to the Partner Center dashboard.</span></span>
2. <span data-ttu-id="f8e63-134">In the left-hand menu under **CSP**, choose **Customers**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>
3. <span data-ttu-id="f8e63-135">On the **Customers** page, select the customer's **Company name**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-135">On the **Customers** page, select the customer's **Company name**.</span></span>
4. <span data-ttu-id="f8e63-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>
5. <span data-ttu-id="f8e63-137">Enter a value for the budget.</span><span class="sxs-lookup"><span data-stu-id="f8e63-137">Enter a value for the budget.</span></span>
6. <span data-ttu-id="f8e63-138">Choose **Apply** to save your changes.</span><span class="sxs-lookup"><span data-stu-id="f8e63-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="f8e63-139">Remove Azure spending budget</span><span class="sxs-lookup"><span data-stu-id="f8e63-139">Remove Azure spending budget</span></span>

<span data-ttu-id="f8e63-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="f8e63-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="f8e63-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="f8e63-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="f8e63-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="f8e63-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span><span class="sxs-lookup"><span data-stu-id="f8e63-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>
4. <span data-ttu-id="f8e63-144">Choose **Remove budget**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="f8e63-145">Check current Azure spending</span><span class="sxs-lookup"><span data-stu-id="f8e63-145">Check current Azure spending</span></span>

<span data-ttu-id="f8e63-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span><span class="sxs-lookup"><span data-stu-id="f8e63-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="f8e63-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="f8e63-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="f8e63-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="f8e63-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span><span class="sxs-lookup"><span data-stu-id="f8e63-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="f8e63-150">Notifications for budget limits</span><span class="sxs-lookup"><span data-stu-id="f8e63-150">Notifications for budget limits</span></span>

<span data-ttu-id="f8e63-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span><span class="sxs-lookup"><span data-stu-id="f8e63-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="f8e63-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span><span class="sxs-lookup"><span data-stu-id="f8e63-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="f8e63-153">This option helps you can keep an eye on your Azure bill.</span><span class="sxs-lookup"><span data-stu-id="f8e63-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="f8e63-154">To configure email notifications:</span><span class="sxs-lookup"><span data-stu-id="f8e63-154">To configure email notifications:</span></span>

1. <span data-ttu-id="f8e63-155">登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="f8e63-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="f8e63-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="f8e63-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span></span>
4. <span data-ttu-id="f8e63-158">Choose **Change email address** to see the email address for notifications.</span><span class="sxs-lookup"><span data-stu-id="f8e63-158">Choose **Change email address** to see the email address for notifications.</span></span>
5. <span data-ttu-id="f8e63-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span></span> <span data-ttu-id="f8e63-160">If the email address *is correct*, choose **Cancel**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-160">If the email address *is correct*, choose **Cancel**.</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="f8e63-161">Itemized costs by service</span><span class="sxs-lookup"><span data-stu-id="f8e63-161">Itemized costs by service</span></span>

<span data-ttu-id="f8e63-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span><span class="sxs-lookup"><span data-stu-id="f8e63-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="f8e63-163">登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="f8e63-163">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="f8e63-164">In the left-hand menu under **CSP**, choose **Customers**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>
3. <span data-ttu-id="f8e63-165">On the **Customers** page, select the customer's **Company name**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-165">On the **Customers** page, select the customer's **Company name**.</span></span>
4. <span data-ttu-id="f8e63-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span><span class="sxs-lookup"><span data-stu-id="f8e63-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>
5. <span data-ttu-id="f8e63-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span><span class="sxs-lookup"><span data-stu-id="f8e63-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
