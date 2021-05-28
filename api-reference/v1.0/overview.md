---
title: Справочные материалы по REST API Microsoft Graph v1.0
description: Добро пожаловать в справочник REST API Microsoft Graph для конечной точки версии 1.0.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: non-product-specific
doc_type: conceptualPageType
ms.openlocfilehash: 26ed5f571aae84ce553dc95b04a385f7f9dd8474
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682476"
---
# <a name="microsoft-graph-rest-api-v10-reference"></a><span data-ttu-id="b7255-103">Справочные материалы по REST API Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="b7255-103">Microsoft Graph REST API v1.0 reference</span></span>

<span data-ttu-id="b7255-104">Добро пожаловать в справочник REST API Microsoft Graph для конечной точки версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="b7255-104">Welcome to Microsoft Graph REST API reference for the v1.0 endpoint.</span></span>

<span data-ttu-id="b7255-105">Наборы API в конечной точке версии 1.0 (`https://graph.microsoft.com/v1.0`) находятся в общедоступном состоянии и подверглись строгому процессу проверки и отзывов при участии клиентов, чтобы удовлетворить практические и производственные требования.</span><span class="sxs-lookup"><span data-stu-id="b7255-105">API sets on the v1.0 endpoint (`https://graph.microsoft.com/v1.0`) are in general availability (GA) status, and have gone through a rigorous review-and-feedback process with customers to meet practical, production needs.</span></span> <span data-ttu-id="b7255-106">Обновления для API в этой конечной точке являются добавочными и не прерывают существующие сценарии приложения.</span><span class="sxs-lookup"><span data-stu-id="b7255-106">Updates to APIs on this endpoint are additive in nature and do not break existing app scenarios.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="b7255-107">Основные сценарии выполнения</span><span class="sxs-lookup"><span data-stu-id="b7255-107">Common use cases</span></span>

<span data-ttu-id="b7255-108">Главное достоинство Microsoft Graph заключается в удобной навигации объектов и связей в разных службах, предоставляемой в единой конечной точке REST Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b7255-108">The power of Microsoft Graph lies in easy navigation of entities and relationships across different services exposed on a single Microsoft Graph REST endpoint.</span></span>

<span data-ttu-id="b7255-109">Некоторые из этих служб предназначены для выполнения сложных сценариев для [пользователей](./resources/user.md) и [групп](./resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="b7255-109">A number of these services are designed to enable rich scenarios around a [user](./resources/user.md) and around a [group](./resources/group.md).</span></span>

### <a name="user-centric-use-cases-in-v10"></a><span data-ttu-id="b7255-110">Сценарии выполнения, ориентированные на пользователя, в версии 1.0</span><span class="sxs-lookup"><span data-stu-id="b7255-110">User-centric use cases in v1.0</span></span>

1. <span data-ttu-id="b7255-111">[Получение профиля](./api/user-get.md) и [фотографии](./resources/profilephoto.md) пользователя Мария.</span><span class="sxs-lookup"><span data-stu-id="b7255-111">[Get the profile](./api/user-get.md) and [photo](./resources/profilephoto.md) of a user, Lisa.</span></span>
2. <span data-ttu-id="b7255-112">[Получение сведений о профиле менеджера Марии](./api/user-list-manager.md) и [идентификаторов ее подчиненных](./api/user-list-directreports.md), хранимых в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b7255-112">[Get the profile information about Lisa's manager](./api/user-list-manager.md) and [IDs of her direct reports](./api/user-list-directreports.md), all stored in Azure Active Directory.</span></span>
3. <span data-ttu-id="b7255-113">[Получение доступа к файлам Марии в OneDrive для бизнеса](./api/driveitem-list-children.md), поиск [удостоверения](./resources/identityset.md) последнего человека, который внес изменения в [файл](./resources/driveitem.md), и переход к профилю этого человека.</span><span class="sxs-lookup"><span data-stu-id="b7255-113">[Access Lisa's files on OneDrive for Business](./api/driveitem-list-children.md), find the [identity](./resources/identityset.md) of the last person who modified a [file](./resources/driveitem.md) there, and navigate to that person's profile.</span></span>
4. <span data-ttu-id="b7255-114">[Получение доступа к календарю Марии](./api/calendar-get.md) в Exchange Online и [определение наиболее подходящего времени для встречи Марии с ее группой](./api/user-findmeetingtimes.md) в следующие две недели.</span><span class="sxs-lookup"><span data-stu-id="b7255-114">[Access Lisa's calendar](./api/calendar-get.md) on Exchange Online and [determine the best time for Lisa to meet with her team](./api/user-findmeetingtimes.md) in the next two weeks.</span></span>
5. <span data-ttu-id="b7255-115">[Подписка](./api/subscription-post-subscriptions.md) и [отслеживание изменений](./api/event-delta.md) в календаре Марии, уведомление Марии, если она проводит более 80% своего времени на собраниях.</span><span class="sxs-lookup"><span data-stu-id="b7255-115">[Subscribe to](./api/subscription-post-subscriptions.md) and [track changes](./api/event-delta.md) in Lisa's calendar, tell Lisa when she is spending more than 80% of her time in meetings.</span></span>
6. <span data-ttu-id="b7255-116">[Настройка автоматических ответов,](./api/user-update-mailboxsettings.md#example-1) когда Мария находится вне офиса.</span><span class="sxs-lookup"><span data-stu-id="b7255-116">[Set automatic replies](./api/user-update-mailboxsettings.md#example-1) when Lisa is away from the office.</span></span>
7. <span data-ttu-id="b7255-117">[Определение людей, которые наиболее важны для Марии,](./api/user-list-people.md) в зависимости от общения, совместной работы и корпоративных связей.</span><span class="sxs-lookup"><span data-stu-id="b7255-117">[Get the people who are most relevant to Lisa](./api/user-list-people.md), based on communication, collaboration, and business relationships.</span></span>
8. <span data-ttu-id="b7255-118">Получение последней проекции продаж из [диаграммы](./resources/chart.md) в файле Excel в инструменте Марии OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="b7255-118">Get the latest sales projection from a [chart](./resources/chart.md) in an Excel file in Lisa's OneDrive for Business.</span></span>
9. <span data-ttu-id="b7255-119">[Поиск задач, назначенных Марии, в планировщике](./api/planneruser-list-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="b7255-119">[Find the tasks assigned to Lisa in Planner](./api/planneruser-list-tasks.md).</span></span>

### <a name="microsoft-365-group-use-cases-in-v10"></a><span data-ttu-id="b7255-120">Варианты использования групп Microsoft 365 в версии 1.0</span><span class="sxs-lookup"><span data-stu-id="b7255-120">Microsoft 365 group use cases in v1.0</span></span>

1. <span data-ttu-id="b7255-121">Запуск отчета о группах Microsoft 365 в организации и определение группы с самыми часто [общающимися участниками группы](./api/reportroot-getoffice365groupsactivitycounts.md).</span><span class="sxs-lookup"><span data-stu-id="b7255-121">Run a report on Microsoft 365 groups in an organization and identify the group with the most [communication among group members](./api/reportroot-getoffice365groupsactivitycounts.md).</span></span>
2. <span data-ttu-id="b7255-122">[Поиск планов группы Microsoft 365](./api/plannergroup-list-plans.md) и [назначение задач](./resources/plannerassignments.md) в плане.</span><span class="sxs-lookup"><span data-stu-id="b7255-122">[Find the plans of this Microsoft 365 group](./api/plannergroup-list-plans.md), and the [assignment of tasks](./resources/plannerassignments.md) in that plan.</span></span>
3. <span data-ttu-id="b7255-123">[Начало новой беседы](./api/group-post-conversations.md) в группе Microsoft 365, чтобы определить, хотят ли участники [создать другую группу](./api/group-post-groups.md) для предоставления общего доступа к рабочей нагрузке.</span><span class="sxs-lookup"><span data-stu-id="b7255-123">[Start a new conversation](./api/group-post-conversations.md) in the Microsoft 365 group to determine if members want to [create another group](./api/group-post-groups.md) to share the workload.</span></span>
4. <span data-ttu-id="b7255-124">[Получение стандартной записной книжки](./api/notebook-get.md) для группы и [создание страницы](./api/section-post-pages.md) для записи результата исследования.</span><span class="sxs-lookup"><span data-stu-id="b7255-124">[Get the default notebook](./api/notebook-get.md) for the group and [create a page](./api/section-post-pages.md) to note the outcome of the investigation.</span></span>

## <a name="other-api-versions"></a><span data-ttu-id="b7255-125">Другие версии API</span><span class="sxs-lookup"><span data-stu-id="b7255-125">Other API versions</span></span>

<span data-ttu-id="b7255-126">В настоящее время существует две версии REST API Microsoft Graph – версия 1.0 и бета-версия.</span><span class="sxs-lookup"><span data-stu-id="b7255-126">There are currently 2 versions of Microsoft Graph REST APIs - v1.0 and beta.</span></span>
<span data-ttu-id="b7255-127">Если вас интересует новые и улучшенные API, которые по-прежнему находятся в предварительной версии, см. статью [Справочник по конечной точке бета-версии Microsoft Graph](/graph/api/overview?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="b7255-127">If you're interested in new or enhanced APIs that are still in preview status, see [Microsoft Graph beta endpoint reference](/graph/api/overview?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="b7255-128">Следует помнить, что API в предварительной версии могут изменяться и могут нарушить работу существующих сценариев без уведомлений.</span><span class="sxs-lookup"><span data-stu-id="b7255-128">Be aware that APIs in preview status are subject to change, and may break existing scenarios without notice.</span></span> <span data-ttu-id="b7255-129">Не создавайте зависимость рабочей среды от API в конечной точке бета-версии.</span><span class="sxs-lookup"><span data-stu-id="b7255-129">Don't take a production dependency on APIs in the beta endpoint.</span></span>

<span data-ttu-id="b7255-130">Дополнительные сведения см. в статье [Управление версиями и поддержка](/graph/versioning-and-support).</span><span class="sxs-lookup"><span data-stu-id="b7255-130">Find more information about [versioning and support](/graph/versioning-and-support).</span></span>

## <a name="call-the-v10-endpoint"></a><span data-ttu-id="b7255-131">Вызов конечной точки версии 1.0</span><span class="sxs-lookup"><span data-stu-id="b7255-131">Call the v1.0 endpoint</span></span>

<span data-ttu-id="b7255-132">В запросах API Microsoft Graph к конечной точке версии 1.0 используется следующий шаблон:</span><span class="sxs-lookup"><span data-stu-id="b7255-132">Microsoft Graph API requests to the v1.0 endpoint use the following pattern:</span></span>

```http
https://graph.microsoft.com/v1.0/{resource}?[query_parameters]
```

<span data-ttu-id="b7255-133">Дополнительные сведения см. в статье [Использование API Microsoft Graph](/graph/use-the-api).</span><span class="sxs-lookup"><span data-stu-id="b7255-133">For details, see [Use the Microsoft Graph API](/graph/use-the-api).</span></span>

## <a name="whats-new"></a><span data-ttu-id="b7255-134">Новые возможности</span><span class="sxs-lookup"><span data-stu-id="b7255-134">What's new</span></span>
<span data-ttu-id="b7255-135">Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) конечной точки версии 1.0.</span><span class="sxs-lookup"><span data-stu-id="b7255-135">Find out about the [latest new features and updates](/graph/whats-new-overview) in the v1.0 endpoint.</span></span>

## <a name="connect-with-us"></a><span data-ttu-id="b7255-136">Обратная связь</span><span class="sxs-lookup"><span data-stu-id="b7255-136">Connect with us</span></span>

<span data-ttu-id="b7255-137">Есть ли дополнительные API или функции, которые вы бы хотели увидеть в Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="b7255-137">Are there additional APIs or features you'd like to see in Microsoft Graph?</span></span> <span data-ttu-id="b7255-138">Опубликуйте новый запрос функции на [форуме идей платформы для разработчиков Microsoft 365](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span><span class="sxs-lookup"><span data-stu-id="b7255-138">Post new feature requests on the [Microsoft 365 Developer Platform ideas forum](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span></span>

<span data-ttu-id="b7255-139">Хотите оставить отзыв по существующим API Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="b7255-139">Have feedback for existing Microsoft Graph APIs?</span></span> <span data-ttu-id="b7255-140">Свяжитесь с нами в [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues).</span><span class="sxs-lookup"><span data-stu-id="b7255-140">Connect with us on [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues).</span></span>
