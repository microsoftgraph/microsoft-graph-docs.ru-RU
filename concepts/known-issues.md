---
title: Известные проблемы с Microsoft Graph
description: В этой статье описываются известные проблемы, связанные с Microsoft Graph. Сведения о последних обновлениях см. в журнале изменений Microsoft Graph.
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: 21667092deabf8a0c078da114325c25dbe223045
ms.sourcegitcommit: a4773239d8559899c3f9433b3073e250a56d2e04
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29994400"
---
# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="e7889-104">Известные проблемы с Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e7889-104">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="e7889-p102">В этой статье описываются известные проблемы, связанные с Microsoft Graph. Сведения о последних обновлениях см. в [журнале изменений Microsoft Graph](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="e7889-p102">This article describes known issues with Microsoft Graph. For information about the latest updates, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="users"></a><span data-ttu-id="e7889-107">Пользователи</span><span class="sxs-lookup"><span data-stu-id="e7889-107">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="e7889-108">Нет мгновенного доступа после создания</span><span class="sxs-lookup"><span data-stu-id="e7889-108">No instant access after creation</span></span>

<span data-ttu-id="e7889-p103">Пользователей можно создавать мгновенно с помощью метода POST для объекта user. Для доступа к службам Office 365 пользователю нужна соответствующая лицензия. Из-за распределенного характера службы файлы, сообщения и события этого пользователя станут доступны посредством API Microsoft Graph через 15 минут после назначения лицензии. В течение этого времени приложения будут получать ошибку HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="e7889-p103">Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="e7889-113">Ограничения для фотографий</span><span class="sxs-lookup"><span data-stu-id="e7889-113">Photo restrictions</span></span>

<span data-ttu-id="e7889-p104">Просмотреть и обновить фотографию профиля пользователя можно, только если у пользователя есть почтовый ящик. Кроме того, все фотографии, которые *могли* быть сохранены ранее с помощью свойства **thumbnailPhoto** (с помощью предварительной версии единого API Office 365, Azure AD Graph или службы синхронизации AD Connect), больше не доступны через свойство **photo** Microsoft Graph ресурса [user](/graph/api/resources/user?view=graph-rest-1.0). В этом случае, если фотографию не удастся просмотреть или обновить, возникнет следующая ошибка:</span><span class="sxs-lookup"><span data-stu-id="e7889-p104">Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource. Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```

### <a name="using-delta-query"></a><span data-ttu-id="e7889-117">Запрос изменений</span><span class="sxs-lookup"><span data-stu-id="e7889-117">Using delta query</span></span>

<span data-ttu-id="e7889-118">Об известных проблемах, связанных с запросом изменений, можно узнать в [соответствующем разделе](#delta-query) этой статьи.</span><span class="sxs-lookup"><span data-stu-id="e7889-118">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="microsoft-teams"></a><span data-ttu-id="e7889-119">Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e7889-119">Microsoft Teams</span></span>

### <a name="graph-explorer-and-global-admins"></a><span data-ttu-id="e7889-120">Песочница Graph и глобальные администраторы</span><span class="sxs-lookup"><span data-stu-id="e7889-120">Graph Explorer and global admins</span></span>

<span data-ttu-id="e7889-121">В настоящее время песочница Graph позволяет глобальным администраторам управлять командами, если они не являются ее владельцами или участниками. Но когда другие приложения попытаются выполнить аналогичные действия, вызовы API завершатся сбоем, если текущий пользователь не является участником или владельцем группы.</span><span class="sxs-lookup"><span data-stu-id="e7889-121">Currently, Graph Explorer allows global admins to manipulate teams they are not an owner or member of, but other apps attempting to make the same API calls will fail if the current user is not a member or owner of the team.</span></span>

### <a name="get-teams-and-post-teams-are-not-supported"></a><span data-ttu-id="e7889-122">Методы GET /teams и POST /teams не поддерживаются</span><span class="sxs-lookup"><span data-stu-id="e7889-122">GET /teams and POST /teams are not supported</span></span>

<span data-ttu-id="e7889-123">Сведения о получении списка команд см. в статьях [Перечисление всех команд](teams-list-all-teams.md) и [Перечисление ваших команд](/graph/api/user-list-joinedteams?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="e7889-123">See [list all teams](teams-list-all-teams.md) and [list your teams](/graph/api/user-list-joinedteams?view=graph-rest-1.0) to get a list of teams.</span></span>
<span data-ttu-id="e7889-124">Сведения о создании команд см. в статье [Создание команды](/graph/api/team-put-teams?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="e7889-124">See [create team](/graph/api/team-put-teams?view=graph-rest-1.0) for creating teams.</span></span>

### <a name="missing-teams-in-list-all-teams"></a><span data-ttu-id="e7889-125">Отсутствующие команды в списке всех команд</span><span class="sxs-lookup"><span data-stu-id="e7889-125">Missing teams in list all teams</span></span>

<span data-ttu-id="e7889-126">Некоторые команды, созданные в прошлом, но не использовавшиеся в последнее время пользователем Microsoft Teams, не указываются при использовании метода [перечисления всех команд](teams-list-all-teams.md).</span><span class="sxs-lookup"><span data-stu-id="e7889-126">Some teams that were created in the past but haven't been used recently by a Microsoft Teams user aren't listed by [list all teams](teams-list-all-teams.md).</span></span>
<span data-ttu-id="e7889-127">Новые команды будут перечислены.</span><span class="sxs-lookup"><span data-stu-id="e7889-127">New teams will be listed.</span></span>
<span data-ttu-id="e7889-128">У некоторых старых команд нет свойства **resourceProvisioningOptions**, содержащего значение "Team", которое присваивается недавно созданным командам и командам, посещаемым в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e7889-128">Certain old teams don't have a **resourceProvisioningOptions** property that contains "Team", which is set on newly created teams and teams that are visited in Microsoft Teams.</span></span>
<span data-ttu-id="e7889-129">В будущем свойство **resourceProvisioningOptions** будет присваиваться существующим командам, не открывавшимся в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e7889-129">In the future, we will set **resourceProvisioningOptions** on existing teams that have not been opened in Microsoft Teams.</span></span>

## <a name="groups"></a><span data-ttu-id="e7889-130">Группы</span><span class="sxs-lookup"><span data-stu-id="e7889-130">Groups</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="e7889-131">Разрешения для групп и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e7889-131">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="e7889-132">Microsoft Graph предоставляет два разрешения ([*Group.Read.All*](permissions-reference.md#group-permissions) и [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) для доступа к API для групп и Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e7889-132">Microsoft Graph exposes two permissions ([*Group.Read.All*](permissions-reference.md#group-permissions) and [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) for access to the APIs for groups and Microsoft Teams.</span></span>
<span data-ttu-id="e7889-133">Эти разрешения должен предоставить администратор.</span><span class="sxs-lookup"><span data-stu-id="e7889-133">These permissions must be consented to by an administrator.</span></span>
<span data-ttu-id="e7889-134">В будущем мы планируем добавить новые разрешения для групп и команд, которые смогут предоставлять пользователи.</span><span class="sxs-lookup"><span data-stu-id="e7889-134">In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="e7889-p108">Кроме того, только API для базового администрирования групп и управления ими поддерживает доступ с помощью разрешений только для приложений или делегированных разрешений. Все остальные функции API групп поддерживают только делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="e7889-p108">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="e7889-137">Примеры функций групп, поддерживающих разрешения только для приложений и делегированные разрешения:</span><span class="sxs-lookup"><span data-stu-id="e7889-137">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="e7889-138">создание и удаление групп;</span><span class="sxs-lookup"><span data-stu-id="e7889-138">Creating and deleting groups</span></span>
* <span data-ttu-id="e7889-139">получение и обновление свойств групп, связанных с администрированием групп и управлением ими;</span><span class="sxs-lookup"><span data-stu-id="e7889-139">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="e7889-140">синхронизация, типы и [параметры каталогов](/graph/api/resources/directoryobject?view=graph-rest-1.0) групп;</span><span class="sxs-lookup"><span data-stu-id="e7889-140">Group [directory settings](/graph/api/resources/directoryobject?view=graph-rest-1.0), type, and synchronization</span></span>
* <span data-ttu-id="e7889-141">владельцы и члены групп.</span><span class="sxs-lookup"><span data-stu-id="e7889-141">Group owners and membership</span></span>

<span data-ttu-id="e7889-142">Примеры функций групп, поддерживающих только делегированные разрешения:</span><span class="sxs-lookup"><span data-stu-id="e7889-142">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="e7889-143">групповые беседы, события, фотографии;</span><span class="sxs-lookup"><span data-stu-id="e7889-143">Group conversations, events, photo</span></span>
* <span data-ttu-id="e7889-144">внешние отправители, разрешенные или запрещенные отправители, подписка на группы;</span><span class="sxs-lookup"><span data-stu-id="e7889-144">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="e7889-145">избранное пользователей и счетчик непросмотренных элементов.</span><span class="sxs-lookup"><span data-stu-id="e7889-145">User favorites and unseen count</span></span>

### <a name="policy"></a><span data-ttu-id="e7889-146">Политика</span><span class="sxs-lookup"><span data-stu-id="e7889-146">Policy</span></span>

<span data-ttu-id="e7889-147">С помощью Microsoft Graph можно создать группу Office 365 и присвоить ей название в обход всех групповых политик Office 365, настроенных через Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="e7889-147">Using Microsoft Graph to create and name an Office 365 group bypasses any Office 365 group policies that are configured through Outlook Web App.</span></span>

### <a name="adding-and-getting-attachments-of-group-posts"></a><span data-ttu-id="e7889-148">Добавление и получение вложений в записях групп</span><span class="sxs-lookup"><span data-stu-id="e7889-148">Adding and getting attachments of group posts</span></span>

<span data-ttu-id="e7889-p109">В настоящее время при [добавлении](/graph/api/post-post-attachments?view=graph-rest-1.0) вложений в записи группы, [отображении](/graph/api/post-list-attachments?view=graph-rest-1.0) и получении вложений возвращается сообщение об ошибке "Запрос OData не поддерживается". Для версий `/v1.0` и `/beta` подготовлено исправление. Оно станет доступно всем пользователям в конце января 2016 года.</span><span class="sxs-lookup"><span data-stu-id="e7889-p109">[Adding](/graph/api/post-post-attachments?view=graph-rest-1.0) attachments to group posts, [listing](/graph/api/post-list-attachments?view=graph-rest-1.0) and getting attachments of group posts currently return the error message "The OData request is not supported." A fix has been rolled out for both the `/v1.0` and `/beta` versions, and is expected to be widely available by the end of January 2016.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="e7889-151">Установка свойства allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="e7889-151">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="e7889-152">В настоящее время существует проблема, из-за которой невозможно установить свойство **allowExternalSenders** группы в операции POST или PATCH как в `/v1.0`, так и в `/beta`.</span><span class="sxs-lookup"><span data-stu-id="e7889-152">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="e7889-153">Работа с запросами изменений</span><span class="sxs-lookup"><span data-stu-id="e7889-153">Using delta query</span></span>

<span data-ttu-id="e7889-154">Об известных проблемах, связанных с запросом изменений, можно узнать в [соответствующем разделе](#delta-query) этой статьи.</span><span class="sxs-lookup"><span data-stu-id="e7889-154">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="bookings"></a><span data-ttu-id="e7889-155">Bookings</span><span class="sxs-lookup"><span data-stu-id="e7889-155">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="e7889-156">Ошибка ErrorExceededFindCountLimit при запросе bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="e7889-156">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="e7889-157">При получении списка по запросу `bookingBusinesses` возвращается ошибка с указанным ниже кодом, если у организации есть несколько компаний в Bookings, а учетная запись, с использованием которой отправлен запрос, не принадлежит администратору.</span><span class="sxs-lookup"><span data-stu-id="e7889-157">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several Bookings businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="e7889-158">В качестве обходного решения можно ограничить группу компаний, возвращаемых по запросу, указав параметр `query`. Пример:</span><span class="sxs-lookup"><span data-stu-id="e7889-158">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```


## <a name="calendars"></a><span data-ttu-id="e7889-159">Календари</span><span class="sxs-lookup"><span data-stu-id="e7889-159">Calendars</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="e7889-160">Доступ к общему календарю</span><span class="sxs-lookup"><span data-stu-id="e7889-160">Accessing a shared calendar</span></span>

<span data-ttu-id="e7889-161">При использовании следующей операции для доступа к событиям в календаре другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="e7889-161">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET \users('{id}')\calendars('{id}')\events
```

<span data-ttu-id="e7889-p110">Может возникнуть ошибка HTTP 500 `ErrorInternalServerTransientError`. Ошибка возникает, потому что:</span><span class="sxs-lookup"><span data-stu-id="e7889-p110">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="e7889-164">Существуют два способа реализации общего доступа к календарю, которые для ясности мы будем называть "старый" способ и "новый" способ.</span><span class="sxs-lookup"><span data-stu-id="e7889-164">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="e7889-165">Новый способ в настоящее время доступен для предоставления доступа к календарям с разрешениями на просмотр или редактирование, но не с делегированными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="e7889-165">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="e7889-166">С помощью REST API календаря можно просматривать и редактировать общие календари, только если доступ к ним предоставлен **новым** способом.</span><span class="sxs-lookup"><span data-stu-id="e7889-166">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="e7889-167">С помощью REST API календаря нельзя просматривать или редактировать общие календари (или их события), если доступ к ним предоставлен **старым** способом.</span><span class="sxs-lookup"><span data-stu-id="e7889-167">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="e7889-168">Если доступ к календарю был предоставлен с разрешениями на просмотр или редактирование, но старым способом, вы можете вручную обновить календарь, чтобы использовать новый способ.</span><span class="sxs-lookup"><span data-stu-id="e7889-168">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="e7889-169">Чтобы можно было использовать новый способ, со временем Outlook автоматически обновит все общие календари, в том числе те, доступ к которым предоставлен с делегированными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="e7889-169">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="e7889-170">Чтобы с этой целью вручную обновить общий календарь, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="e7889-170">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="e7889-171">Получатель удаляет календарь, доступ к которому был ранее ему предоставлен.</span><span class="sxs-lookup"><span data-stu-id="e7889-171">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="e7889-172">Владелец повторно предоставляет доступ к календарю в Outlook в Интернете, Outlook на iOS или Outlook на Android.</span><span class="sxs-lookup"><span data-stu-id="e7889-172">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="e7889-p112">Получатель повторно принимает календарь, используя Outlook в Интернете. (Скоро можно будет использовать другие клиенты Outlook.)</span><span class="sxs-lookup"><span data-stu-id="e7889-p112">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="e7889-175">Доступ к календарю успешно предоставлен новым способом, если получатель может просмотреть его в Outlook на iOS или Outlook на Android.</span><span class="sxs-lookup"><span data-stu-id="e7889-175">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="e7889-p113">Календарь, доступ к которому предоставлен новым способом, выглядит как один из стандартных календарей в вашем почтовом ящике. С помощью REST API календаря можно просматривать и редактировать события в общем календаре, как в своем собственном. Например:</span><span class="sxs-lookup"><span data-stu-id="e7889-p113">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET \me\calendars('{id}')\events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="e7889-179">Добавление календарей ICS в почтовый ящик пользователя и доступ к ним</span><span class="sxs-lookup"><span data-stu-id="e7889-179">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="e7889-180">В настоящее время календари ICS поддерживаются частично:</span><span class="sxs-lookup"><span data-stu-id="e7889-180">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="e7889-181">Вы можете добавить календарь ICS в почтовый ящик пользователя через интерфейс пользователя, но не через API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e7889-181">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="e7889-p114">[Перечисление календарей пользователя](/graph/api/user-list-calendars?view=graph-rest-1.0) позволяет получить свойства **name**, **color** и **id** всех [календарей](/graph/api/resources/calendar?view=graph-rest-1.0) в группе календарей пользователя по умолчанию или указанной группе календарей, в том числе календарей ICS. URL-адрес ICS невозможно хранить и открывать в ресурсе calendar.</span><span class="sxs-lookup"><span data-stu-id="e7889-p114">[Listing the user's calendars](/graph/api/user-list-calendars?view=graph-rest-1.0) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="e7889-184">Вы также можете [отобразить события](/graph/api/calendar-list-events?view=graph-rest-1.0) календаря ICS.</span><span class="sxs-lookup"><span data-stu-id="e7889-184">You can also [list the events](/graph/api/calendar-list-events?view=graph-rest-1.0) of an ICS-based calendar.</span></span>

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a><span data-ttu-id="e7889-185">Поддержка свойства onlineMeetingUrl для Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e7889-185">onlineMeetingUrl property support for Microsoft Teams</span></span>

<span data-ttu-id="e7889-186">В настоящее время свойство **onlineMeetingUrl** ресурса [event](/graph/api/resources/event?view=graph-rest-1.0) для собрания Skype означает URL-адрес для собрания по сети.</span><span class="sxs-lookup"><span data-stu-id="e7889-186">Currently, the **onlineMeetingUrl** property of a Skype meeting [event](/graph/api/resources/event?view=graph-rest-1.0) would indicate the online meeting URL.</span></span> <span data-ttu-id="e7889-187">Однако для ресурса event собрания в Microsoft Teams задано значение NULL.</span><span class="sxs-lookup"><span data-stu-id="e7889-187">However, that property for a Microsoft Teams meeting event is set to null.</span></span>

## <a name="calls-and-online-meetings"></a><span data-ttu-id="e7889-188">Звонки и собрания по сети</span><span class="sxs-lookup"><span data-stu-id="e7889-188">Calls and online meetings</span></span>

> <span data-ttu-id="e7889-189">**Примечание.** В настоящее время звонки и собрания по сети находятся в предварительной версии и доступны только в конечной точке бета-версии Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e7889-189">**Note** Calling and online meetings are currently in preview and are available only in the Microsoft Graph beta endpoint.</span></span>

- <span data-ttu-id="e7889-190">Путь навигации `/applications/{id}` не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7889-190">Navigation path `/applications/{id}` is not supported.</span></span> <span data-ttu-id="e7889-191">Навигация к приложению (даже собственному) через глобальный узел приложений не разрешена.</span><span class="sxs-lookup"><span data-stu-id="e7889-191">Navigating through the global applications node to the application, even your own, is not allowed.</span></span> <span data-ttu-id="e7889-192">Используйте только навигацию `/app`.</span><span class="sxs-lookup"><span data-stu-id="e7889-192">Please use the `/app` navigation only.</span></span>

## <a name="contacts"></a><span data-ttu-id="e7889-193">Контакты</span><span class="sxs-lookup"><span data-stu-id="e7889-193">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="e7889-194">Контакты организации доступны только в бета-версии</span><span class="sxs-lookup"><span data-stu-id="e7889-194">Organization contacts available in only beta</span></span>

<span data-ttu-id="e7889-p117">В настоящее время поддерживаются только личные контакты. В настоящее время контакты организации не поддерживаются в версии `/v1.0`, но их можно найти в версии `/beta`.</span><span class="sxs-lookup"><span data-stu-id="e7889-p117">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="e7889-197">Папка контактов по умолчанию</span><span class="sxs-lookup"><span data-stu-id="e7889-197">Default contacts folder</span></span>

<span data-ttu-id="e7889-198">В версии `/v1.0` запрос `GET /me/contactFolders` не включает папку контактов пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e7889-198">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="e7889-p118">Эта ошибка будет исправлена. Чтобы получить идентификатор папки контактов по умолчанию, вы можете использовать следующий запрос на [отображение контактов](/graph/api/user-list-contacts?view=graph-rest-1.0) и свойство **parentFolderId**:</span><span class="sxs-lookup"><span data-stu-id="e7889-p118">A fix will be made available. Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="e7889-201">В указанном выше запросе:</span><span class="sxs-lookup"><span data-stu-id="e7889-201">In the above query:</span></span>

1. <span data-ttu-id="e7889-202">`/me/contacts?$top=1` возвращает свойства [контакта](/graph/api/resources/contact?view=graph-rest-1.0) в папке контактов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e7889-202">`/me/contacts?$top=1` gets the properties of a [contact](/graph/api/resources/contact?view=graph-rest-1.0) in the default contacts folder.</span></span>
2. <span data-ttu-id="e7889-203">При добавлении `&$select=parentFolderId` возвращается только свойство контакта **parentFolderId** — идентификатор папки контактов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e7889-203">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="e7889-204">Доступ к контактам через папку контактов в бета-версии</span><span class="sxs-lookup"><span data-stu-id="e7889-204">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="e7889-205">В настоящее время в версии `/beta` существует проблема, из-за которой нельзя получить доступ к ресурсу [contact](/graph/api/resources/contact?view=graph-rest-beta), указав его родительскую папку в URL-адресе запроса REST, как показано в 2 приведенных ниже сценариях.</span><span class="sxs-lookup"><span data-stu-id="e7889-205">In the `/beta` version, there is currently an issue that prevents accessing a [contact](/graph/api/resources/contact?view=graph-rest-beta) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="e7889-206">Доступ к контакту из папки верхнего уровня [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="e7889-206">Accessing a contact from a top level [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="e7889-p119">Доступ к контакту в дочерней папке папки **contactFolder**.  В приведенном ниже примере показан один уровень вложения, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="e7889-p119">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="e7889-209">Кроме того, вы можете просто [получить](/graph/api/contact-get?view=graph-rest-beta) контакт по его идентификатору, как показано ниже, так как конечная точка /contacts для запроса GET в версии `/beta` применяется ко всем контактам в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="e7889-209">As an alternative, you can simply [get](/graph/api/contact-get?view=graph-rest-beta) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a><span data-ttu-id="e7889-210">Сообщения</span><span class="sxs-lookup"><span data-stu-id="e7889-210">Messages</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="e7889-211">Параметр comment для создания черновика</span><span class="sxs-lookup"><span data-stu-id="e7889-211">The comment parameter for creating a draft</span></span>

<span data-ttu-id="e7889-212">Параметр **comment** для создания ответа или черновика ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) не включается в текст полученного черновика сообщения.</span><span class="sxs-lookup"><span data-stu-id="e7889-212">The **comment** parameter for creating a reply or forward draft ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) does not become part of the body of the resultant message draft.</span></span>

### <a name="get-messages-returns-chats-in-microsoft-teams"></a><span data-ttu-id="e7889-213">При использовании запроса GET для сообщений возвращаются также чаты в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e7889-213">GET messages returns chats in Microsoft Teams</span></span>

<span data-ttu-id="e7889-214">В конечных точках версии 1 и бета-версии данные отклика для `GET /users/id/messages` включают чаты Microsoft Teams, не входящие в область группы или канала.</span><span class="sxs-lookup"><span data-stu-id="e7889-214">In both the v1 and beta endpoints, the response of `GET /users/id/messages` includes the user's Microsoft Teams chats that occurred outside the scope of a team or channel.</span></span> <span data-ttu-id="e7889-215">Тема этих сообщений чата: "IM".</span><span class="sxs-lookup"><span data-stu-id="e7889-215">These chat messages have "IM" as their subject.</span></span>


## <a name="drives-files-and-content-streaming"></a><span data-ttu-id="e7889-216">Диски, файлы и потоковая передача контента</span><span class="sxs-lookup"><span data-stu-id="e7889-216">Drives, files and content streaming</span></span>

* <span data-ttu-id="e7889-217">При первом доступе к личному диску пользователя с помощью Microsoft Graph до открытия им своего личного сайта в браузере возвращается ответ 401.</span><span class="sxs-lookup"><span data-stu-id="e7889-217">First time access to a user's personal drive through the Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="e7889-218">Ограничения параметров запроса</span><span class="sxs-lookup"><span data-stu-id="e7889-218">Query parameter limitations</span></span>

* <span data-ttu-id="e7889-219">Не поддерживается несколько пространств имен.</span><span class="sxs-lookup"><span data-stu-id="e7889-219">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="e7889-220">Не поддерживаются запросы GET для `$ref` и приведение для пользователей, групп, устройств, субъектов-служб и приложений.</span><span class="sxs-lookup"><span data-stu-id="e7889-220">GETs on `$ref` and casting is not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="e7889-p121">Не поддерживается `@odata.bind`. Это значит, что разработчики не смогут правильно задавать параметры `Accepted` и `RejectedSenders` для группы.</span><span class="sxs-lookup"><span data-stu-id="e7889-p121">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the `Accepted` or `RejectedSenders` on a group.</span></span>
* <span data-ttu-id="e7889-223">Отсутствует `@odata.id` для навигации по объектам без вложений (например, сообщениям) при использовании минимальных метаданных.</span><span class="sxs-lookup"><span data-stu-id="e7889-223">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="e7889-224">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="e7889-224"></span></span>
  * <span data-ttu-id="e7889-225">Отсутствует поддержка `nextLink`.</span><span class="sxs-lookup"><span data-stu-id="e7889-225">No support for `nextLink`</span></span>
  * <span data-ttu-id="e7889-226">Поддерживается не более одного уровня развертывания.</span><span class="sxs-lookup"><span data-stu-id="e7889-226">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="e7889-227">Не поддерживаются дополнительные параметры (`$filter`, `$select`).</span><span class="sxs-lookup"><span data-stu-id="e7889-227">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="e7889-228">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="e7889-228"></span></span>
  * <span data-ttu-id="e7889-229">Конечная точка `/attachments` не поддерживает фильтры.</span><span class="sxs-lookup"><span data-stu-id="e7889-229">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="e7889-230">При ее наличии параметр `$filter` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="e7889-230">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="e7889-231">Фильтрация нескольких рабочих нагрузок не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7889-231">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="e7889-232">`$search`:</span><span class="sxs-lookup"><span data-stu-id="e7889-232"></span></span>
  * <span data-ttu-id="e7889-233">Полнотекстовый поиск доступен только для некоторых объектов, например сообщений.</span><span class="sxs-lookup"><span data-stu-id="e7889-233">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="e7889-234">Поиск по нескольким рабочим нагрузкам не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7889-234">Cross-workload searching is not supported.</span></span>

## <a name="delta-query"></a><span data-ttu-id="e7889-235">Разностный запрос</span><span class="sxs-lookup"><span data-stu-id="e7889-235">Delta query</span></span>

* <span data-ttu-id="e7889-236">При отслеживании изменений в отношениях иногда неправильно возвращается контекст OData.</span><span class="sxs-lookup"><span data-stu-id="e7889-236">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="e7889-237">Расширения схемы (устаревшие) не возвращаются с оператором $select и возвращаются без него.</span><span class="sxs-lookup"><span data-stu-id="e7889-237">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="e7889-238">Клиенты не могут отслеживать изменения в открытых расширениях и зарегистрированных расширениях схемы.</span><span class="sxs-lookup"><span data-stu-id="e7889-238">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="application-and-serviceprincipal-api-changes"></a><span data-ttu-id="e7889-239">Изменения в API application и servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="e7889-239">Application and servicePrincipal API changes</span></span>

<span data-ttu-id="e7889-p123">Скоро в объекты [application](/graph/api/resources/application?view=graph-rest-beta) и [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) будут внесены изменения. Ниже приведено краткое описание текущих ограничений и возможностей API, находящихся в разработке.</span><span class="sxs-lookup"><span data-stu-id="e7889-p123">There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="e7889-242">Текущие ограничения:</span><span class="sxs-lookup"><span data-stu-id="e7889-242">Current limitations:</span></span>

* <span data-ttu-id="e7889-243">Некоторые свойства application (такие как appRoles и addIns) будут доступны только после внесения всех изменений.</span><span class="sxs-lookup"><span data-stu-id="e7889-243">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="e7889-244">Регистрировать можно только мультитенантные приложения.</span><span class="sxs-lookup"><span data-stu-id="e7889-244">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="e7889-245">Обновлять можно только приложения, зарегистрированные после первоначального обновления бета-версии.</span><span class="sxs-lookup"><span data-stu-id="e7889-245">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="e7889-246">Пользователи Azure Active Directory могут регистрировать приложения и добавлять владельцев.</span><span class="sxs-lookup"><span data-stu-id="e7889-246">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="e7889-247">Поддержка протоколов OpenID Connect и OAuth.</span><span class="sxs-lookup"><span data-stu-id="e7889-247">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="e7889-248">Невозможно назначение политик приложению.</span><span class="sxs-lookup"><span data-stu-id="e7889-248">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="e7889-249">Не выполняются операции с ownedObjects, для которых требуется код appId (например, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span><span class="sxs-lookup"><span data-stu-id="e7889-249">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="e7889-250">В разработке:</span><span class="sxs-lookup"><span data-stu-id="e7889-250">In development:</span></span>

* <span data-ttu-id="e7889-251">Возможность регистрировать однотенантные приложения.</span><span class="sxs-lookup"><span data-stu-id="e7889-251">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="e7889-252">Обновления объекта servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="e7889-252">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="e7889-253">Перевод существующих приложений Azure AD на обновленную модель.</span><span class="sxs-lookup"><span data-stu-id="e7889-253">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="e7889-254">Поддержка appRoles, предварительно авторизованные клиенты, необязательные утверждения, утверждения членства в группе и брендинг.</span><span class="sxs-lookup"><span data-stu-id="e7889-254">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="e7889-255">Пользователи учетной записи Майкрософт (MSA) могут регистрировать приложения.</span><span class="sxs-lookup"><span data-stu-id="e7889-255">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="e7889-256">Поддержка протоколов SAML и WsFed.</span><span class="sxs-lookup"><span data-stu-id="e7889-256">Support for SAML and WsFed protocols.</span></span>

## <a name="extensions"></a><span data-ttu-id="e7889-257">Расширения</span><span class="sxs-lookup"><span data-stu-id="e7889-257">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="e7889-258">Отслеживание изменений не поддерживается</span><span class="sxs-lookup"><span data-stu-id="e7889-258">Change tracking is not supported</span></span>

<span data-ttu-id="e7889-259">Отслеживание изменений не поддерживается для свойств открытых расширений и расширений схемы.</span><span class="sxs-lookup"><span data-stu-id="e7889-259">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="e7889-260">Одновременное создание ресурса и открытого расширения</span><span class="sxs-lookup"><span data-stu-id="e7889-260">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="e7889-p124">Невозможно указать открытое расширение при создании экземпляра **administrativeUnit**, **device**, **group**, **organization** или **user**. Сначала необходимо создать экземпляр, а затем указать данные открытого расширения в последующем запросе ``POST`` к этому экземпляру.</span><span class="sxs-lookup"><span data-stu-id="e7889-p124">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="e7889-263">Создание экземпляра ресурса с одновременным добавлением данных расширения схемы</span><span class="sxs-lookup"><span data-stu-id="e7889-263">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="e7889-264">Вы не можете указать расширение схемы в той же операции, которая создает экземпляр **contact**, **event**, **message** или **post**.</span><span class="sxs-lookup"><span data-stu-id="e7889-264">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="e7889-265">Сперва нужно создать экземпляр ресурса, а затем выполнить операцию `PATCH` для этого экземпляра, чтобы добавить расширение схемы и пользовательские данные.</span><span class="sxs-lookup"><span data-stu-id="e7889-265">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="e7889-266">Для каждого экземпляра ресурса разрешено не более 100 значений свойства расширения схемы</span><span class="sxs-lookup"><span data-stu-id="e7889-266">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="e7889-267">В настоящее время для каждого экземпляра таких ресурсов каталога, как **device**, **group** и **user**, можно установить не более 100 значений свойства расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="e7889-267">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="e7889-268">Фильтрация по свойствам расширения схемы поддерживается не для всех типов объектов</span><span class="sxs-lookup"><span data-stu-id="e7889-268">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="e7889-269">Фильтрация по свойствам расширения схемы (с помощью выражения `$filter`) не поддерживается для типов сущностей Outlook **contact**, **event**, **message** или **post**.</span><span class="sxs-lookup"><span data-stu-id="e7889-269">Filtering on schema extension properties (using the `$filter` expresssion) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="json-batching"></a><span data-ttu-id="e7889-270">Пакетная обработка JSON</span><span class="sxs-lookup"><span data-stu-id="e7889-270">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="e7889-271">Не поддерживаются вложенные пакеты</span><span class="sxs-lookup"><span data-stu-id="e7889-271">No nested batch</span></span>

<span data-ttu-id="e7889-272">Пакетные запросы JSON не должны содержать вложенных пакетных запросов.</span><span class="sxs-lookup"><span data-stu-id="e7889-272">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="e7889-273">Все отдельные запросы должны быть синхронными</span><span class="sxs-lookup"><span data-stu-id="e7889-273">All individual requests must be synchronous</span></span>

<span data-ttu-id="e7889-p126">Все запросы, содержащиеся в пакетном запросе, должны выполняться синхронно. Параметр `respond-async`, если он имеется, будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="e7889-p126">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="e7889-276">Не поддерживается диалоговая обработка</span><span class="sxs-lookup"><span data-stu-id="e7889-276">No transactions</span></span>

<span data-ttu-id="e7889-p127">В настоящее время Microsoft Graph не поддерживает диалоговую обработку отдельных запросов. Свойство `atomicityGroup` отдельных запросов будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="e7889-p127">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="e7889-279">URI должны быть относительными</span><span class="sxs-lookup"><span data-stu-id="e7889-279">URIs must be relative</span></span>

<span data-ttu-id="e7889-p128">Всегда указывайте относительные URI в пакетных запросах. Microsoft Graph сделает эти URL-адреса абсолютными с помощью конечной точки версии, включенной в URL-адрес пакета.</span><span class="sxs-lookup"><span data-stu-id="e7889-p128">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="e7889-282">Ограничение на размер пакета</span><span class="sxs-lookup"><span data-stu-id="e7889-282">Limit on batch size</span></span>

<span data-ttu-id="e7889-283">В настоящее время в пакетный запрос JSON можно включить не более 20 отдельных запросов.</span><span class="sxs-lookup"><span data-stu-id="e7889-283">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="e7889-284">Упрощенные зависимости</span><span class="sxs-lookup"><span data-stu-id="e7889-284">Simplified dependencies</span></span>

<span data-ttu-id="e7889-p129">Отдельные запросы могут зависеть от других отдельных запросов. В настоящее время запросы могут зависеть только от одного другого запроса и должны соответствовать одному из этих шаблонов:</span><span class="sxs-lookup"><span data-stu-id="e7889-p129">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="e7889-287">Параллельный — для отдельных запросов не указаны зависимости в свойстве `dependsOn`.</span><span class="sxs-lookup"><span data-stu-id="e7889-287">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="e7889-288">Последовательный — все отдельные запросы зависят от предыдущего отдельного запроса.</span><span class="sxs-lookup"><span data-stu-id="e7889-288">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="e7889-289">Идентичный — для всех отдельных запросов в свойстве `dependsOn` указана одна и та же зависимость.</span><span class="sxs-lookup"><span data-stu-id="e7889-289">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="e7889-290">После усовершенствования пакетной обработки JSON эти ограничения будут удалены.</span><span class="sxs-lookup"><span data-stu-id="e7889-290">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="e7889-291">Приложения Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="e7889-291">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="e7889-292">Приложения CSP должны использовать конечную точку Azure AD</span><span class="sxs-lookup"><span data-stu-id="e7889-292">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="e7889-p130">Приложения CSP должны получать маркеры из конечных точек Azure AD (версии 1) для успешного вызова Microsoft Graph в своих клиентах, управляемых партнерами. В настоящее время получение маркера через конечную точку Azure AD версии 2.0 не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7889-p130">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="e7889-295">В некоторых клиентах предоставленные приложениям CSP разрешения не работают</span><span class="sxs-lookup"><span data-stu-id="e7889-295">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="e7889-296">Предоставленные приложениям CSP разрешения могут не работать в некоторых клиентах.</span><span class="sxs-lookup"><span data-stu-id="e7889-296">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="e7889-297">После первого входа в приложение, использующее делегированные разрешения, в новом клиенте может возникнуть эта ошибка: `AADSTS50000: There was an error issuing a token`.</span><span class="sxs-lookup"><span data-stu-id="e7889-297">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="e7889-298">Приложение, использующее разрешения для приложений, может получить маркер, но ему может быть неожиданно отказано в доступе при вызове Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e7889-298">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="e7889-299">Мы делаем все возможное, чтобы как можно быстрее исправить эту ошибку.</span><span class="sxs-lookup"><span data-stu-id="e7889-299">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="e7889-300">Для целей разработки и тестирования можно использовать следующее временное решение.</span><span class="sxs-lookup"><span data-stu-id="e7889-300">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="e7889-p131">**ПРИМЕЧАНИЕ.** Это не окончательное решение и предназначено только для целей разработки.  Оно станет ненужным после исправления упомянутой выше ошибки.  Удалять указанный ниже субъект-службу не нужно.</span><span class="sxs-lookup"><span data-stu-id="e7889-p131">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="e7889-p132">Откройте сеанс Azure AD PowerShell 2 и подключитесь к клиенту `customer`, введя учетные данные администратора в окне входа. Скачать и установить Azure AD PowerShell 2 можно [здесь](https://www.powershellgallery.com/packages/AzureAD).</span><span class="sxs-lookup"><span data-stu-id="e7889-p132">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="e7889-306">Создайте субъект-службу Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e7889-306">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="e7889-307">Функции, доступные только в REST API Office 365 или API Graph Azure AD</span><span class="sxs-lookup"><span data-stu-id="e7889-307">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="e7889-p133">Некоторые функции еще не доступны в Microsoft Graph. Если вы не нашли нужную функцию, можете использовать специальные [REST API Office 365](https://msdn.microsoft.com/office/office365/api/api-catalog). Сведения о функциях, доступных только через API Azure AD Graph, читайте в записи [Microsoft Graph или Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) в блоге.</span><span class="sxs-lookup"><span data-stu-id="e7889-p133">Some functionality is not yet available in Microsoft Graph. If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](https://msdn.microsoft.com/office/office365/api/api-catalog). For Azure Active Directory, please refer to the [Microsoft Graph or Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) blog post on the features that are only available through Azure AD Graph API.</span></span>

