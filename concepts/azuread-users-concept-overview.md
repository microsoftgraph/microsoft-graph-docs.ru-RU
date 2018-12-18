---
title: Обзор пользователей в Microsoft Graph
description: Пользователи — это представления рабочих или учебных учетных записей Azure Active Directory (Azure AD) либо учетных записей Майкрософт в Microsoft Graph. Ресурс **user** в Microsoft Graph — это центр, из которого вы можете получить доступ к связям и ресурсам, релевантным для ваших пользователей.
author: dkershaw10
ms.openlocfilehash: f9e64ecd3f3a46a74b7a6bcd65955419fd102296
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337305"
---
# <a name="overview-of-users-in-microsoft-graph"></a><span data-ttu-id="52538-104">Обзор пользователей в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="52538-104">Overview of users in Microsoft Graph</span></span>

<span data-ttu-id="52538-105">Пользователи — это представления рабочих или учебных учетных записей Azure Active Directory (Azure AD) либо учетных записей Майкрософт в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="52538-105">Users are the representation of an Azure Active Directory (Azure AD) work or school user account or a Microsoft account in Microsoft Graph.</span></span> <span data-ttu-id="52538-106">Ресурс **user** в Microsoft Graph — это центр, из которого вы можете получить доступ к связям и ресурсам, релевантным для ваших пользователей.</span><span class="sxs-lookup"><span data-stu-id="52538-106">The **user** resource in Microsoft Graph is a hub from which you can access the relationships and resources that are relevant to your users.</span></span>

![Схема, на которой показан пользователь, соединенный с календарем, почтой, контактами, собраниями, задачами, сайтами и документами](images/users.png)

## <a name="develop-user-centric-applications"></a><span data-ttu-id="52538-108">Разработка приложений, ориентированных на пользователей</span><span class="sxs-lookup"><span data-stu-id="52538-108">Develop user-centric applications</span></span>

<span data-ttu-id="52538-109">С помощью Microsoft Graph вы можете получить доступ к связям, документам, контактам и настройкам, контекстно-релевантным для пользователя, вошедшего в систему.</span><span class="sxs-lookup"><span data-stu-id="52538-109">You can use Microsoft Graph to access the relationships, documents, contacts, and preferences that are contextually relevant to the signed-in user.</span></span> <span data-ttu-id="52538-110">Ресурс **user** обеспечивает простой способ доступа к ресурсам пользователя и работы с ними без необходимости совершать дополнительные вызовы, искать информацию о проверке подлинности и отправлять запросы непосредственно к другим ресурсам Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="52538-110">The **user** resource provides straightforward way for you to access and manipulate user resources without having to perform additional calls, look up specific authentication information, and directly issue queries against other Microsoft Graph resources.</span></span>

<span data-ttu-id="52538-111">Чтобы получить доступ к информации и данным пользователя, вам потребуется [получить доступ к этим ресурсам от его имени](auth-v2-user.md).</span><span class="sxs-lookup"><span data-stu-id="52538-111">To access a user's information and data, you'll need to [get access on their behalf](auth-v2-user.md).</span></span> <span data-ttu-id="52538-112">Благодаря проверке подлинности приложения с помощью [согласия администратора](permissions-reference.md) вы можете работать с широким спектром объектов, сопоставленных с пользователем, и изменять их.</span><span class="sxs-lookup"><span data-stu-id="52538-112">Authenticating your application with [admin consent](permissions-reference.md) enables you to work with and update a wider range of entities associated with a user.</span></span>

### <a name="manage-your-organization"></a><span data-ttu-id="52538-113">Управление организацией</span><span class="sxs-lookup"><span data-stu-id="52538-113">Manage your organization</span></span>

<span data-ttu-id="52538-114">Вы можете создавать пользователей в своей организации или изменять ресурсы и связи для существующих пользователей.</span><span class="sxs-lookup"><span data-stu-id="52538-114">Create new users in your organization or update the resources and relationships for existing users.</span></span> <span data-ttu-id="52538-115">С помощью Microsoft Graph вы можете выполнять указанные ниже задачи по управлению пользователями.</span><span class="sxs-lookup"><span data-stu-id="52538-115">You can use Microsoft Graph to perform the following user management tasks:</span></span> 

- <span data-ttu-id="52538-116">Создавать и удалять пользователей в вашей организации Azure AD.</span><span class="sxs-lookup"><span data-stu-id="52538-116">Create or delete users in your Azure AD organization.</span></span>
- <span data-ttu-id="52538-117">Составлять список членства пользователя в группах и определять, является ли пользователь участником какой-либо группы.</span><span class="sxs-lookup"><span data-stu-id="52538-117">List a user's group memberships and determine whether a user is a member of a group.</span></span>
- <span data-ttu-id="52538-118">Составлять список пользователей, подчиняющихся определенному пользователю и назначать менеджеров пользователю.</span><span class="sxs-lookup"><span data-stu-id="52538-118">List the users who report to a user and assign managers to a user.</span></span>
- <span data-ttu-id="52538-119">Отправлять или получать фотографию пользователя.</span><span class="sxs-lookup"><span data-stu-id="52538-119">Upload or retrieve a photo for the user.</span></span>

### <a name="work-with-calendars-and-tasks"></a><span data-ttu-id="52538-120">Работа с календарями и задачами</span><span class="sxs-lookup"><span data-stu-id="52538-120">Work with calendars and tasks</span></span>

<span data-ttu-id="52538-121">Вы можете просматривать и изменять календарь и группы календарей, сопоставленные с пользователям, а также отправлять в них запросы. Кроме того, вы можете выполнять указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="52538-121">You can view, query, and update user calendar and calendar groups associated with a user, including:</span></span>

- <span data-ttu-id="52538-122">Отображать списки событий и создавать события в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="52538-122">List and create events on a users calendar.</span></span>
- <span data-ttu-id="52538-123">Просматривать задачи, назначенные пользователю.</span><span class="sxs-lookup"><span data-stu-id="52538-123">View tasks assigned to a user.</span></span>
- <span data-ttu-id="52538-124">Находить свободное время для собраний с участием нескольких пользователей.</span><span class="sxs-lookup"><span data-stu-id="52538-124">Find free meeting times for a set of users.</span></span>
- <span data-ttu-id="52538-125">Получать список напоминаний, установленных в календаре пользователя.</span><span class="sxs-lookup"><span data-stu-id="52538-125">Get a list of reminders set on a user's calendar.</span></span>

### <a name="administer-mail-and-handle-contacts"></a><span data-ttu-id="52538-126">Администрирование почты и обработка контактов</span><span class="sxs-lookup"><span data-stu-id="52538-126">Administer mail and handle contacts</span></span>

<span data-ttu-id="52538-127">Вы можете настраивать параметры почты и списки контактов пользователя, а также отправлять почту от имени пользователя. Кроме того, вы можете выполнять указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="52538-127">You can configure user mail settings and contact lists and send mail on a user's behalf, including:</span></span>

- <span data-ttu-id="52538-128">Отображать почтовые сообщения и отправлять новые сообщения.</span><span class="sxs-lookup"><span data-stu-id="52538-128">List mail messages and send new mail.</span></span>
- <span data-ttu-id="52538-129">Создавать и отображать контакты пользователя и упорядочивать их в папках.</span><span class="sxs-lookup"><span data-stu-id="52538-129">Create and list user contacts and organize contacts in folders.</span></span>
- <span data-ttu-id="52538-130">Получать и изменять папки и параметры почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="52538-130">Retrieve and update mailbox folders and settings.</span></span>

### <a name="enrich-your-app-with-user-insights"></a><span data-ttu-id="52538-131">Дополнять возможности приложения аналитикой пользователя</span><span class="sxs-lookup"><span data-stu-id="52538-131">Enrich your app with user insights</span></span>

<span data-ttu-id="52538-132">Добиться максимальной релевантности в приложении, показывая недавно использованные или популярные документы и контакты, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="52538-132">Maximize relevance in your application by promoting recently used or trending documents and contacts associated with a user.</span></span> <span data-ttu-id="52538-133">С помощью Microsoft Graph вы можете выполнять указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="52538-133">You can use Microsoft Graph to:</span></span>

- <span data-ttu-id="52538-134">Возвращать документы, недавно просмотренные и измененные каким-либо пользователем.</span><span class="sxs-lookup"><span data-stu-id="52538-134">Return documents recently viewed and modified by a user.</span></span>
- <span data-ttu-id="52538-135">Возвращать популярные документы и сайты, связанные с активностью пользователя.</span><span class="sxs-lookup"><span data-stu-id="52538-135">Return documents and sites trending around a user's activity.</span></span>
- <span data-ttu-id="52538-136">Отображать документы, доступ к которым предоставлен пользователю в электронных письмах или в OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="52538-136">List documents shared with a user through email or OneDrive for Business.</span></span>

## <a name="api-reference"></a><span data-ttu-id="52538-137">Справочные материалы по API</span><span class="sxs-lookup"><span data-stu-id="52538-137">API reference</span></span>
<span data-ttu-id="52538-138">Ищете справочные материалы по API для этой службы?</span><span class="sxs-lookup"><span data-stu-id="52538-138">Looking for the API reference for this service?</span></span>

- [<span data-ttu-id="52538-139">API пользователей в Microsoft Graph 1.0</span><span class="sxs-lookup"><span data-stu-id="52538-139">Users API in Microsoft Graph v1.0</span></span>](/graph/api/resources/users?view=graph-rest-1.0)
- [<span data-ttu-id="52538-140">API пользователей в бета-версии Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="52538-140">Users API in Microsoft Graph beta</span></span>](/graph/api/resources/users?view=graph-rest-beta)

## <a name="next-steps"></a><span data-ttu-id="52538-141">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="52538-141">Next steps</span></span>

- <span data-ttu-id="52538-142">Узнайте больше о том, как [работать с пользователями](/graph/api/resources/users?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="52538-142">Learn more about how to [work with users](/graph/api/resources/users?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="52538-143">Проанализируйте собственные данные из ресурса **user** в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="52538-143">Explore your own data from the **user** resource in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="52538-144">Выполняйте аутентификацию с помощью Microsoft Graph [от имени пользователя](auth-v2-user.md) или [с использованием управляющей программы или службы с согласия администратора](auth-v2-service.md).</span><span class="sxs-lookup"><span data-stu-id="52538-144">Authenticate with Microsoft Graph [on behalf of a user](auth-v2-user.md) or [as a daemon or service by consent of an administator](auth-v2-service.md).</span></span>
- <span data-ttu-id="52538-145">Настройте управление доступом и политики доступа для пользователей с помощью [API Azure AD](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="52538-145">Set access control and policies for users with the [Azure AD API](/graph/api/resources/azure-ad-overview?view=graph-rest-1.0).</span></span>
- <span data-ttu-id="52538-146">Просмотрите [разрешения](permissions-reference.md), которые потребуются вашему приложению для доступа к данным пользователей.</span><span class="sxs-lookup"><span data-stu-id="52538-146">Review the [permissions](permissions-reference.md) your app will need to access user data.</span></span> 
<!-- This isn't really a next step; let's remove to keep the list of links concise.>
- Stay up to date with Microsoft Graph [changelog](changelog.md).
-->
