---
title: Работа с интерфейсами API для образования в Microsoft Graph
description: API для образования в Microsoft Graph дополняют ресурсы и данные Microsoft 365 сведениями, актуальными для учебных заведений, учащихся, преподавателей, классов и списков. Это упрощает создание решений, интегрируемых с образовательными ресурсами.
localization_priority: Priority
author: mmast-msft
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 4d36403aef6212831e186fffd401df7155be43fd
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582361"
---
# <a name="working-with-education-apis-in-microsoft-graph"></a><span data-ttu-id="f21f4-104">Работа с интерфейсами API для образования в Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f21f4-104">Working with education APIs in Microsoft Graph</span></span>

<span data-ttu-id="f21f4-105">API для образования в Microsoft Graph дополняют ресурсы и данные Microsoft 365 сведениями, актуальными для учебных заведений, учащихся, преподавателей, классов и списков.</span><span class="sxs-lookup"><span data-stu-id="f21f4-105">The education APIs in Microsoft Graph enhance Microsoft 365 resources and data with information that is relevant for education scenarios, including schools, students, teachers, classes, and enrollments.</span></span> <span data-ttu-id="f21f4-106">Это упрощает создание решений, интегрируемых с образовательными ресурсами.</span><span class="sxs-lookup"><span data-stu-id="f21f4-106">This makes it easy for you to build solutions that integrate with educational resources.</span></span>

<span data-ttu-id="f21f4-107">API для образования включают ресурсы для управления списком и автоматизации заданий, с помощью которых можно взаимодействовать с соответствующими службами в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f21f4-107">The education APIs include rostering resources and assignments resources that you can use to interact with the rostering services in Microsoft Teams.</span></span> <span data-ttu-id="f21f4-108">С помощью этих ресурсов можно управлять списком учащихся и сотрудников учебного учреждения.</span><span class="sxs-lookup"><span data-stu-id="f21f4-108">You can use these resources to manage a school roster.</span></span>

## <a name="authorization"></a><span data-ttu-id="f21f4-109">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f21f4-109">Authorization</span></span>

<span data-ttu-id="f21f4-110">Чтобы вызывать API для образования в Microsoft Graph, приложению необходимо получить маркер доступа.</span><span class="sxs-lookup"><span data-stu-id="f21f4-110">To call the education APIs in Microsoft Graph, your app will need to acquire an access token.</span></span> <span data-ttu-id="f21f4-111">Подробные сведения о маркерах доступа см. в статье [Получение маркеров доступа для вызова Microsoft Graph](/graph/auth/).</span><span class="sxs-lookup"><span data-stu-id="f21f4-111">For details about access tokens, see [Get access tokens to call Microsoft Graph](/graph/auth/).</span></span> <span data-ttu-id="f21f4-112">Приложению также потребуются соответствующие разрешения.</span><span class="sxs-lookup"><span data-stu-id="f21f4-112">Your app will also need the appropriate permissions.</span></span> <span data-ttu-id="f21f4-113">Дополнительные сведения см. в разделе [Разрешения для образования](/graph/permissions-reference#education-permissions).</span><span class="sxs-lookup"><span data-stu-id="f21f4-113">For more information, see [Education permissions](/graph/permissions-reference#education-permissions).</span></span>

### <a name="app-permissions-to-enable-school-it-admins-to-consent"></a><span data-ttu-id="f21f4-114">Разрешения, которые должны предоставить приложению ИТ-администраторы учебного заведения</span><span class="sxs-lookup"><span data-stu-id="f21f4-114">App permissions to enable school IT admins to consent</span></span>

<span data-ttu-id="f21f4-115">Для развертывания приложений, интегрированных с API для образования в Microsoft Graph, ИТ-администраторы учебного заведения должны предоставить разрешения, запрашиваемые приложением.</span><span class="sxs-lookup"><span data-stu-id="f21f4-115">To deploy apps that are integrated with the Education APIs in Microsoft Graph, school IT admins must first grant consent to the permissions requested by the app.</span></span> <span data-ttu-id="f21f4-116">Повторный запрос появится, только если разрешения изменятся.</span><span class="sxs-lookup"><span data-stu-id="f21f4-116">This consent has to be granted only once, unless the permissions change.</span></span> <span data-ttu-id="f21f4-117">Когда администратор предоставит разрешения, приложение будет подготовлено к работе для всех пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="f21f4-117">After the admin consents, the app is provisioned for all users in the tenant.</span></span>

<span data-ttu-id="f21f4-118">Чтобы отобразить диалоговое окно для предоставления разрешений, используйте приведенный ниже вызов REST.</span><span class="sxs-lookup"><span data-stu-id="f21f4-118">To show a consent dialog box, use the following REST call.</span></span>

``` http
GET https://login.microsoftonline.com/{tenant}/adminconsent?
client_id={clientId}&state=12345&redirect_uri={redirectUrl}
```

| <span data-ttu-id="f21f4-119">Параметр</span><span class="sxs-lookup"><span data-stu-id="f21f4-119">Parameter</span></span>   | <span data-ttu-id="f21f4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f21f4-120">Description</span></span>                                                               |
| :---------- | :------------------------------------------------------------------------ |
| <span data-ttu-id="f21f4-121">Tenant</span><span class="sxs-lookup"><span data-stu-id="f21f4-121">Tenant</span></span>      | <span data-ttu-id="f21f4-122">ИД клиента учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f21f4-122">Tenant ID of the school.</span></span> <span data-ttu-id="f21f4-123">Используйте полный идентификатор, например onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="f21f4-123">Use the full ID, which includes onmicrosoft.com.</span></span> |
| <span data-ttu-id="f21f4-124">clientId</span><span class="sxs-lookup"><span data-stu-id="f21f4-124">clientId</span></span>    | <span data-ttu-id="f21f4-125">Идентификатор клиента приложения.</span><span class="sxs-lookup"><span data-stu-id="f21f4-125">Client ID of the app.</span></span>                                                     |
| <span data-ttu-id="f21f4-126">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="f21f4-126">redirectUrl</span></span> | <span data-ttu-id="f21f4-127">URL-адрес перенаправления приложения.</span><span class="sxs-lookup"><span data-stu-id="f21f4-127">App redirect URL.</span></span>                                                         |

## <a name="rostering"></a><span data-ttu-id="f21f4-128">Списки</span><span class="sxs-lookup"><span data-stu-id="f21f4-128">Rostering</span></span>

<span data-ttu-id="f21f4-129">API для работы со списком позволяют извлекать данные из клиента Microsoft 365 учебного заведения, подготовленного с помощью [Microsoft School Data Sync](https://sds.microsoft.com/). Эти API предоставляют доступ к сведениям об учебных заведениях, секциях, преподавателях, учащихся и списках.</span><span class="sxs-lookup"><span data-stu-id="f21f4-129">The rostering APIs enable you to extract data from a school's Microsoft 365 tenant provisioned with [Microsoft School Data Sync](https://sds.microsoft.com/). These APIs provide access to information about schools, sections, teachers, students, and rosters.</span></span> <span data-ttu-id="f21f4-130">Эти API поддерживают как сценарии только для приложений (синхронизацию), так и сценарии для приложений и пользователей (интерактивные).</span><span class="sxs-lookup"><span data-stu-id="f21f4-130">The APIs support both app-only (sync) scenarios, and app + user (interactive) scenarios.</span></span> <span data-ttu-id="f21f4-131">API, поддерживающие интерактивные сценарии, применяют политики RBAC на основе роли вызывающего API пользователя.</span><span class="sxs-lookup"><span data-stu-id="f21f4-131">The APIs that support interactive scenarios enforce region-appropriate RBAC policies based on the user role calling the API.</span></span> <span data-ttu-id="f21f4-132">Это обеспечивает согласованность API и минимальную область действия политики независимо от конфигурации администрирования в клиентах.</span><span class="sxs-lookup"><span data-stu-id="f21f4-132">This provides a consistent API and minimal policy surface, regardless of the administrative configuration within tenants.</span></span> <span data-ttu-id="f21f4-133">Кроме того, API также предоставляют разрешения для образования, позволяющие настроить доступ к данным.</span><span class="sxs-lookup"><span data-stu-id="f21f4-133">In addition, the APIs also provide education-specific permissions to ensure that the right user has access to the data.</span></span>

<span data-ttu-id="f21f4-134">С помощью API для работы со списком можно предоставить пользователю приложения следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="f21f4-134">You can use the rostering APIs to enable an app user to know:</span></span>

- <span data-ttu-id="f21f4-135">его роль;</span><span class="sxs-lookup"><span data-stu-id="f21f4-135">Who I am</span></span>
- <span data-ttu-id="f21f4-136">предметы, которые он изучает или преподает;</span><span class="sxs-lookup"><span data-stu-id="f21f4-136">What classes I attend or teach</span></span>
- <span data-ttu-id="f21f4-137">задания и сроки их выполнения.</span><span class="sxs-lookup"><span data-stu-id="f21f4-137">What I need to do and by when</span></span>

<span data-ttu-id="f21f4-138">API для работы со списком предоставляют следующие ключевые ресурсы:</span><span class="sxs-lookup"><span data-stu-id="f21f4-138">The rostering APIs provide the following key resources:</span></span>

- <span data-ttu-id="f21f4-139">[educationSchool](educationschool.md) — учебное заведение;</span><span class="sxs-lookup"><span data-stu-id="f21f4-139">[educationSchool](educationschool.md) - Represents the school.</span></span>
- <span data-ttu-id="f21f4-140">[educationClass](educationclass.md) — класс в учебном заведении;</span><span class="sxs-lookup"><span data-stu-id="f21f4-140">[educationClass](educationclass.md) - Represents a class within a school.</span></span>
- <span data-ttu-id="f21f4-141">[educationTerm](educationterm.md) — определенная часть учебного года;</span><span class="sxs-lookup"><span data-stu-id="f21f4-141">[educationTerm](educationterm.md) - Represents a designated portion of the academic year.</span></span>
- <span data-ttu-id="f21f4-142">[educationTeacher](educationteacher.md) — пользователь с основной ролью "Преподаватель";</span><span class="sxs-lookup"><span data-stu-id="f21f4-142">[educationTeacher](educationteacher.md) - Represents a user with the primary role of 'Teacher'.</span></span>
- <span data-ttu-id="f21f4-143">[educationStudent](educationstudent.md) — пользователь с основной ролью "Учащийся".</span><span class="sxs-lookup"><span data-stu-id="f21f4-143">[educationStudent](educationstudent.md) - Represents a user with the primary role of 'student'.</span></span>

<span data-ttu-id="f21f4-144">API для работы со списком поддерживают следующие сценарии:</span><span class="sxs-lookup"><span data-stu-id="f21f4-144">The rostering APIs support the following scenarios:</span></span>

- <span data-ttu-id="f21f4-145">[перечисление всех учебных заведений](../api/educationroot-list-schools.md);</span><span class="sxs-lookup"><span data-stu-id="f21f4-145">[List all schools](../api/educationroot-list-schools.md)</span></span>
- <span data-ttu-id="f21f4-146">[перечисление учебных заведений, в которых преподается определенный предмет](../api/educationclass-list-schools.md);</span><span class="sxs-lookup"><span data-stu-id="f21f4-146">[List schools in which a class is taught](../api/educationclass-list-schools.md)</span></span>
- <span data-ttu-id="f21f4-147">[перечисление учебных заведений пользователя](../api/educationuser-list-schools.md);</span><span class="sxs-lookup"><span data-stu-id="f21f4-147">[List schools for a user](../api/educationuser-list-schools.md)</span></span>
- <span data-ttu-id="f21f4-148">[получение всех классов](../api/educationroot-list-classes.md);</span><span class="sxs-lookup"><span data-stu-id="f21f4-148">[Get all classes](../api/educationroot-list-classes.md)</span></span>
- <span data-ttu-id="f21f4-149">[получение классов в учебном заведении](../api/educationschool-list-classes.md);</span><span class="sxs-lookup"><span data-stu-id="f21f4-149">[Get classes in a school](../api/educationschool-list-classes.md)</span></span>
- <span data-ttu-id="f21f4-150">[список классов пользователя](../api/educationuser-list-classes.md);</span><span class="sxs-lookup"><span data-stu-id="f21f4-150">[List classes for a user](../api/educationuser-list-classes.md)</span></span>
- <span data-ttu-id="f21f4-151">[добавление классов в учебном заведении](../api/educationschool-post-classes.md);</span><span class="sxs-lookup"><span data-stu-id="f21f4-151">[Add classes to a school](../api/educationschool-post-classes.md)</span></span>
- <span data-ttu-id="f21f4-152">[получение учащихся и преподавателей класса](../api/educationclass-list-members.md);</span><span class="sxs-lookup"><span data-stu-id="f21f4-152">[Get students and teachers for a class](../api/educationclass-list-members.md)</span></span>
- <span data-ttu-id="f21f4-153">[добавление учащихся в класс](../api/educationclass-post-members.md);</span><span class="sxs-lookup"><span data-stu-id="f21f4-153">[Add members to a class](../api/educationclass-post-members.md)</span></span>
- <span data-ttu-id="f21f4-154">[список преподавателей класса](../api/educationclass-list-teachers.md);</span><span class="sxs-lookup"><span data-stu-id="f21f4-154">[List teachers for a class](../api/educationclass-list-teachers.md)</span></span>
- <span data-ttu-id="f21f4-155">[получение пользователей учебного заведения](../api/educationschool-list-users.md).</span><span class="sxs-lookup"><span data-stu-id="f21f4-155">[Get users in a school](../api/educationschool-list-users.md)</span></span>

<!-- Should you list delete scenarios here as well? -->

## <a name="whats-new"></a><span data-ttu-id="f21f4-156">Новые возможности</span><span class="sxs-lookup"><span data-stu-id="f21f4-156">What's new</span></span>

<span data-ttu-id="f21f4-157">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.</span><span class="sxs-lookup"><span data-stu-id="f21f4-157">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f21f4-158">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f21f4-158">Next steps</span></span>

<span data-ttu-id="f21f4-159">С помощью API для образования в Microsoft Graph вы можете создавать решения с доступом к спискам пользователей учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="f21f4-159">Use the Microsoft Graph education APIs to build education solutions that access school rosters.</span></span> <span data-ttu-id="f21f4-160">Чтобы узнать больше:</span><span class="sxs-lookup"><span data-stu-id="f21f4-160">To learn more:</span></span>

- <span data-ttu-id="f21f4-161">Изучите ресурсы и методы, наиболее полезные для вашего сценария.</span><span class="sxs-lookup"><span data-stu-id="f21f4-161">Explore the resources and methods that are most helpful to your scenario.</span></span>
- <span data-ttu-id="f21f4-162">опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="f21f4-162">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>