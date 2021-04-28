---
title: Обзор API обзоров доступа
description: API обзоров доступа позволяет программным образом просмотреть доступ к ресурсам Azure AD.
author: FaithOmbongi
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: 92ea2d49fae37c5b4d5ae82e390f897af9ff4cde
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067063"
---
# <a name="overview-of-the-access-reviews-api"></a><span data-ttu-id="4538b-103">Обзор API проверок доступа</span><span class="sxs-lookup"><span data-stu-id="4538b-103">Overview of the access reviews API</span></span>

<span data-ttu-id="4538b-104">API [обзоров](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) доступа в Microsoft Graph позволяет программным образом просмотреть доступ к ресурсам Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4538b-104">The [access reviews API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) in Microsoft Graph allows you to programmatically review access to Azure AD resources.</span></span> <span data-ttu-id="4538b-105">К ним относятся:</span><span class="sxs-lookup"><span data-stu-id="4538b-105">This includes:</span></span>
+ <span data-ttu-id="4538b-106">Создание, чтение, обновление и удаление обзоров доступа, параметров обзора доступа и расписания.</span><span class="sxs-lookup"><span data-stu-id="4538b-106">Creating, reading, updating, and deleting access reviews, access review settings, and schedules.</span></span>
+ <span data-ttu-id="4538b-107">Изучение прошлых обзоров доступа и решений, принятых рецензентами, в том числе действий Azure AD, принятых автоматически.</span><span class="sxs-lookup"><span data-stu-id="4538b-107">Investigating past access reviews and the decisions taken by reviewers, including the steps Azure AD took automatically.</span></span>

## <a name="scope-of-use"></a><span data-ttu-id="4538b-108">Область использования</span><span class="sxs-lookup"><span data-stu-id="4538b-108">Scope of use</span></span>

<span data-ttu-id="4538b-109">API обзоров доступа поддерживают как делегированную, так и контексты приложений.</span><span class="sxs-lookup"><span data-stu-id="4538b-109">The access reviews APIs support both delegated and application contexts.</span></span> <span data-ttu-id="4538b-110">В пользовательском (делегированного) контексте приложение вызывает API отзывов доступа от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="4538b-110">In a user (delegated) context, an application calls the access reviews API on behalf of a user.</span></span> <span data-ttu-id="4538b-111">Типичные сценарии:</span><span class="sxs-lookup"><span data-stu-id="4538b-111">Typical scenarios include:</span></span>
+ <span data-ttu-id="4538b-112">Администратор, использующий сценарий для создания, чтения или обновления обзора доступа.</span><span class="sxs-lookup"><span data-stu-id="4538b-112">An administrator using a script to create, read, or update an access review.</span></span>
+ <span data-ttu-id="4538b-113">Владелец ресурса, использующий приложение или скрипт для создания обзора доступа к своему ресурсу.</span><span class="sxs-lookup"><span data-stu-id="4538b-113">A resource owner using an app or a script to create an access review for a resource they own.</span></span>
+ <span data-ttu-id="4538b-114">Администратор автоматически собирает все решения для одного или более обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="4538b-114">An administrator automatically collecting all decisions for one or more access reviews.</span></span>
  
<span data-ttu-id="4538b-115">Чтобы авторизировать приложение в пользовательском (делегированных) контексте, см. статью получить доступ [от имени пользователя.](/graph/auth-v2-user)</span><span class="sxs-lookup"><span data-stu-id="4538b-115">To authorize your app in a user (delegated) context, see [get access on behalf of a user](/graph/auth-v2-user).</span></span>

<span data-ttu-id="4538b-116">В контексте приложения приложение вызывает API отзывов доступа без входного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4538b-116">In an application context, an application calls the access reviews API without a signed-in user present.</span></span> <span data-ttu-id="4538b-117">Типичный сценарий — это запланированный фоновый сценарий, регулярно собирающий решения для всех обзоров доступа.</span><span class="sxs-lookup"><span data-stu-id="4538b-117">A typical scenario is a scheduled background script regularly collecting decisions for all access reviews.</span></span> <span data-ttu-id="4538b-118">Чтобы разрешить ваше приложение в этом контексте, см. в приложении [get access without a user.](/graph/auth-v2-service)</span><span class="sxs-lookup"><span data-stu-id="4538b-118">To authorize your app in this context, see [get access without a user](/graph/auth-v2-service).</span></span>

## <a name="building-blocks-of-an-access-review"></a><span data-ttu-id="4538b-119">Создание блоков обзора доступа</span><span class="sxs-lookup"><span data-stu-id="4538b-119">Building blocks of an access review</span></span>

<span data-ttu-id="4538b-120">Обзоры доступа структурированы логически и состоят из этих блоков:</span><span class="sxs-lookup"><span data-stu-id="4538b-120">Access reviews are structured logically and are comprised of these building blocks:</span></span>
+ <span data-ttu-id="4538b-121">**Определения расписания обзоров** доступа — логический план, содержащий параметры обзора доступа и его экземпляры.</span><span class="sxs-lookup"><span data-stu-id="4538b-121">**Access reviews schedule definitions** -  The logical blueprint that contains the settings of an access review and its instances.</span></span>
+ <span data-ttu-id="4538b-122">**Экземпляр проверки доступа** . Представляет действие проверки, которое имеет область, рецензенты и состояние.</span><span class="sxs-lookup"><span data-stu-id="4538b-122">**Access review instance** - Represents a review activity that has a scope, reviewers, and a status.</span></span> <span data-ttu-id="4538b-123">Определение проверки доступа может иметь несколько экземпляров, как это имеется в повторяющихся отзывах.</span><span class="sxs-lookup"><span data-stu-id="4538b-123">An access review definition may have multiple instances as is the case in recurring reviews.</span></span> <span data-ttu-id="4538b-124">Разовая рецензия имеет ровно один экземпляр.</span><span class="sxs-lookup"><span data-stu-id="4538b-124">One-off reviews have exactly one instance.</span></span>
+ <span data-ttu-id="4538b-125">**Элементы решений,** записанные для проверки. Представляете решение рецензента, принятое в экземпляре, включая штамп времени и обоснование решения.</span><span class="sxs-lookup"><span data-stu-id="4538b-125">**Decision items recorded for a review** - Represent a decision a reviewer made on an instance, including the time stamp and justification for the decision.</span></span> <span data-ttu-id="4538b-126">В каждом экземпляре отзывов принимается столько же решений, сколько и количество пользователей, которые рассматриваются.</span><span class="sxs-lookup"><span data-stu-id="4538b-126">Each review instance has as many decisions as the number of users under review.</span></span> <span data-ttu-id="4538b-127">Если решения не приняты, то есть рецензенты не ответили на отзыв, объекты решения для экземпляра не будут.</span><span class="sxs-lookup"><span data-stu-id="4538b-127">If there are no decisions taken, that is, reviewers haven’t responded to the review, there will be no decision objects for the instance.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4538b-128">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="4538b-128">Next steps</span></span>

<span data-ttu-id="4538b-129">Попробуйте следующие учебники для управления отзывами о доступе:</span><span class="sxs-lookup"><span data-stu-id="4538b-129">Try out the following tutorials to manage access reviews:</span></span>

+ [<span data-ttu-id="4538b-130">Используйте API отзывов доступа для групп, чтобы просмотреть доступ к группам безопасности</span><span class="sxs-lookup"><span data-stu-id="4538b-130">Use access reviews API for groups to review access to your security groups</span></span>](tutorial-accessreviews-securitygroup.md)
+ [<span data-ttu-id="4538b-131">Используйте API обзоров доступа для групп, чтобы просмотреть доступ ко всем группам Microsoft 365 с гостевых пользователей</span><span class="sxs-lookup"><span data-stu-id="4538b-131">Use access reviews API for groups to review access to all your Microsoft 365 groups with guest users</span></span>](tutorial-accessreviews-M365group.md)

## <a name="see-also"></a><span data-ttu-id="4538b-132">См. также</span><span class="sxs-lookup"><span data-stu-id="4538b-132">See also</span></span>

+ [<span data-ttu-id="4538b-133">Планирование Azure Active Directory проверки доступа</span><span class="sxs-lookup"><span data-stu-id="4538b-133">Planning Azure Active Directory Access Reviews deployment</span></span>](/azure/active-directory/governance/deploy-access-reviews)
+ [<span data-ttu-id="4538b-134">Создание обзора доступа групп & приложений</span><span class="sxs-lookup"><span data-stu-id="4538b-134">Create an access review of groups & applications</span></span>](/azure/active-directory/governance/create-access-review)
+ [<span data-ttu-id="4538b-135">Получение доступа от имени пользователя</span><span class="sxs-lookup"><span data-stu-id="4538b-135">Get access on behalf of a user</span></span>](/graph/auth-v2-user)
+ [<span data-ttu-id="4538b-136">Получение доступа без пользователя</span><span class="sxs-lookup"><span data-stu-id="4538b-136">Get access without a user</span></span>](/graph/auth-v2-service)
