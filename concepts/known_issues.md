# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="eade9-101">Известные проблемы с Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="eade9-101">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="eade9-p101">В этой статье описываются известные проблемы, связанные с Microsoft Graph. Сведения о последних обновлениях см. в [журнале изменений Microsoft Graph](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="eade9-p101">This article describes known issues with Microsoft Graph. For information about the latest updates, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="users"></a><span data-ttu-id="eade9-104">Пользователи</span><span class="sxs-lookup"><span data-stu-id="eade9-104">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="eade9-105">Нет мгновенного доступа после создания</span><span class="sxs-lookup"><span data-stu-id="eade9-105">No instant access after creation</span></span>

<span data-ttu-id="eade9-p102">Пользователей можно создавать мгновенно с помощью метода POST для объекта user. Для доступа к службам Office 365 пользователю нужна соответствующая лицензия. Из-за распределенного характера службы файлы, сообщения и события этого пользователя станут доступны посредством API Microsoft Graph через 15 минут после назначения лицензии. В течение этого времени приложения будут получать ошибку HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="eade9-p102">Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="eade9-110">Ограничения для фотографий</span><span class="sxs-lookup"><span data-stu-id="eade9-110">Photo restrictions</span></span>

<span data-ttu-id="eade9-p103">Просмотреть и обновить фотографию профиля пользователя можно, только если у пользователя есть почтовый ящик. Кроме того, все фотографии, которые *могли* быть сохранены ранее с помощью свойства **thumbnailPhoto** (с помощью предварительной версии единого API Office 365, Azure AD Graph или службы синхронизации AD Connect), больше не доступны через свойство **photo** Microsoft Graph ресурса [user](../api-reference/v1.0/resources/user.md). В этом случае, если фотографию не удастся просмотреть или обновить, возникнет следующая ошибка:</span><span class="sxs-lookup"><span data-stu-id="eade9-p103">Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](../api-reference/v1.0/resources/user.md) resource. Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```


### <a name="using-delta-query"></a><span data-ttu-id="eade9-114">Запрос изменений</span><span class="sxs-lookup"><span data-stu-id="eade9-114">Using delta query</span></span>

<span data-ttu-id="eade9-115">Об известных проблемах, связанных с использованием запросов изменений, можно узнать в [соответствующем разделе](#delta-query) этой статьи.</span><span class="sxs-lookup"><span data-stu-id="eade9-115">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="groups-and-microsoft-teams"></a><span data-ttu-id="eade9-116">Группы и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="eade9-116">Groups and Microsoft Teams</span></span>

><span data-ttu-id="eade9-117">**Примечание.** В настоящее время служба Microsoft Teams доступна только в конечной точке бета-версии Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="eade9-117">**Note** Microsoft Teams is currently in preview and is available only in the Microsoft Graph beta endpoint.</span></span>

### <a name="policy"></a><span data-ttu-id="eade9-118">Политика</span><span class="sxs-lookup"><span data-stu-id="eade9-118">Policy</span></span>

<span data-ttu-id="eade9-119">С помощью Microsoft Graph можно создать группу Office 365 и присвоить ей название в обход всех групповых политик Office 365, настроенных через Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="eade9-119">Using Microsoft Graph to create and name an Office 365 group bypasses any Office 365 group policies that are configured through Outlook Web App.</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="eade9-120">Разрешения для групп и Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="eade9-120">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="eade9-p104">В Microsoft Graph доступны два разрешения (*Group.Read.All* и *Group.ReadWrite.All*) для доступа к API для групп и Microsoft Teams. На предоставление этих разрешений должен согласиться администратор (в предварительной версии было иначе). В будущем мы планируем добавить новые разрешения для групп и команд, на предоставление которых смогут соглашаться пользователи.</span><span class="sxs-lookup"><span data-stu-id="eade9-p104">Microsoft Graph exposes two permissions (*Group.Read.All* and *Group.ReadWrite.All*) for access to the APIs for groups and Microsoft Teams. These permissions must be consented to by an administrator (which is a change from preview).  In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="eade9-p105">Кроме того, только API для базового администрирования групп и управления ими поддерживает доступ с помощью разрешений только для приложений или делегированных разрешений. Все остальные функции API групп поддерживают только делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="eade9-p105">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="eade9-126">Примеры функций групп, поддерживающих разрешения только для приложений и делегированные разрешения:</span><span class="sxs-lookup"><span data-stu-id="eade9-126">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="eade9-127">создание и удаление групп;</span><span class="sxs-lookup"><span data-stu-id="eade9-127">Creating and deleting groups</span></span>
* <span data-ttu-id="eade9-128">получение и обновление свойств групп, связанных с администрированием групп и управлением ими;</span><span class="sxs-lookup"><span data-stu-id="eade9-128">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="eade9-129">синхронизация, типы и [параметры каталогов](../api-reference/v1.0/resources/directoryobject.md) групп;</span><span class="sxs-lookup"><span data-stu-id="eade9-129">Group [directory settings](../api-reference/v1.0/resources/directoryobject.md), type, and synchronization</span></span>
* <span data-ttu-id="eade9-130">владельцы и члены групп.</span><span class="sxs-lookup"><span data-stu-id="eade9-130">Group owners and membership</span></span>

<span data-ttu-id="eade9-131">Примеры функций групп, поддерживающих только делегированные разрешения:</span><span class="sxs-lookup"><span data-stu-id="eade9-131">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="eade9-132">групповые беседы, события, фотографии;</span><span class="sxs-lookup"><span data-stu-id="eade9-132">Group conversations, events, photo</span></span>
* <span data-ttu-id="eade9-133">внешние отправители, разрешенные или запрещенные отправители, подписка на группы;</span><span class="sxs-lookup"><span data-stu-id="eade9-133">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="eade9-134">избранное пользователей и счетчик непросмотренных элементов;</span><span class="sxs-lookup"><span data-stu-id="eade9-134">User favorites and unseen count</span></span>
* <span data-ttu-id="eade9-135">Чаты и каналы Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="eade9-135">Microsoft Teams channels and chats</span></span>

### <a name="teams-in-microsoft-teams-preview"></a><span data-ttu-id="eade9-136">Рабочие группы в Microsoft Teams (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="eade9-136">Teams in Microsoft Teams (preview)</span></span>

<span data-ttu-id="eade9-p106">Группы Office 365 и Microsoft Teams [имеют схожие функции](../api-reference/beta/resources/teams_api_overview.md). Все API групп можно использовать с рабочими группами за исключением того, что в настоящее время нельзя создать рабочую группу с помощью API создания групп.  Эта возможность появится в будущих выпусках API.</span><span class="sxs-lookup"><span data-stu-id="eade9-p106">Microsoft Teams and Office 365 groups [share similar functionality](../api-reference/beta/resources/teams_api_overview.md). All group APIs can be used with teams, with the exception that the Create group API does not currently allow you to create a team.  Future API releases will support this.</span></span>

### <a name="microsoft-teams-chat-threads-and-chat-messages-preview"></a><span data-ttu-id="eade9-140">Цепочки и сообщения чата Microsoft Teams (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="eade9-140">Microsoft Teams chat threads and chat messages (preview)</span></span>

<span data-ttu-id="eade9-p107">В настоящее время в каналах можно создавать цепочки чата, но нельзя читать существующие цепочки и добавлять в них ответы. Кроме того, нельзя читать или записывать прямые чаты между пользователями, которые выходят за рамки команды или канала.  В будущих выпусках API появятся дополнительные возможности в этой области.</span><span class="sxs-lookup"><span data-stu-id="eade9-p107">Currently, you can create chat threads in channels, but you cannot read existing chat threads or add replies to them. Also, you cannot read or write direct chats between users that are outside the scope of a team or channel.  Future API releases will add additional capabilities in this area.</span></span>

### <a name="microsoft-teams-users-list-of-joined-teams-preview"></a><span data-ttu-id="eade9-144">Список рабочих групп, в которых состоит пользователь Microsoft Teams (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="eade9-144">Microsoft Teams user's list of joined teams (preview)</span></span>

<span data-ttu-id="eade9-p108">На данный момент [перечисление рабочих групп, к которым присоединился пользователь,](../api-reference/beta/api/user_list_joinedteams.md) возможно только в случае вошедшего пользователя, для которого у вызывающего есть [делегированные разрешения](permissions_reference.md).  Будущие выпуски будут поддерживать эту операцию для любого указанного ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="eade9-p108">Currrently, [listing the teams a user has joined](../api-reference/beta/api/user_list_joinedteams.md) only works for the 'me' user for which the caller has [delegated permissions](permissions_reference.md).  Future releases will support this operation for any specified user ID.</span></span>

### <a name="adding-and-getting-attachments-of-group-posts"></a><span data-ttu-id="eade9-147">Добавление и получение вложений в записях групп</span><span class="sxs-lookup"><span data-stu-id="eade9-147">Adding and getting attachments of group posts</span></span>

<span data-ttu-id="eade9-p109">В настоящее время при [добавлении](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/post_post_attachments) вложений в записи группы, [отображении](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/post_list_attachments) и получении вложений возвращается сообщение об ошибке "Запрос OData не поддерживается". Для версий `/v1.0` и `/beta` подготовлено исправление. Оно станет доступно всем пользователям в конце января 2016 года.</span><span class="sxs-lookup"><span data-stu-id="eade9-p109">[Adding](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/post_post_attachments) attachments to group posts, [listing](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/post_list_attachments) and getting attachments of group posts currently return the error message "The OData request is not supported." A fix has been rolled out for both the `/v1.0` and `/beta` versions, and is expected to be widely available by the end of January 2016.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="eade9-150">Установка свойства allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="eade9-150">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="eade9-151">В настоящее время существует проблема, из-за которой невозможно установить свойство **allowExternalSenders** группы в операции POST или PATCH как в `/v1.0`, так и в `/beta`.</span><span class="sxs-lookup"><span data-stu-id="eade9-151">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="eade9-152">Работа с запросами изменений</span><span class="sxs-lookup"><span data-stu-id="eade9-152">Using delta query</span></span>

<span data-ttu-id="eade9-153">Об известных проблемах, связанных с запросом изменений, можно узнать в [соответствующем разделе](#delta-query) этой статьи.</span><span class="sxs-lookup"><span data-stu-id="eade9-153">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>


## <a name="bookings"></a><span data-ttu-id="eade9-154">Bookings</span><span class="sxs-lookup"><span data-stu-id="eade9-154">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="eade9-155">Ошибка ErrorExceededFindCountLimit при запросе bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="eade9-155">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="eade9-156">При получении списка по запросу `bookingBusinesses` возвращается ошибка с указанным ниже кодом, если у организации есть несколько компаний в Bookings, а учетная запись, с использованием которой отправлен запрос, не принадлежит администратору.</span><span class="sxs-lookup"><span data-stu-id="eade9-156">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several Bookings businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="eade9-157">В качестве обходного решения можно ограничить группу компаний, возвращаемых по запросу, указав параметр `query`. Пример:</span><span class="sxs-lookup"><span data-stu-id="eade9-157">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```


## <a name="calendars"></a><span data-ttu-id="eade9-158">Календари</span><span class="sxs-lookup"><span data-stu-id="eade9-158">Calendars</span></span>

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="eade9-159">Добавление календарей ICS в почтовый ящик пользователя и доступ к ним</span><span class="sxs-lookup"><span data-stu-id="eade9-159">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="eade9-160">В настоящее время календари ICS поддерживаются частично:</span><span class="sxs-lookup"><span data-stu-id="eade9-160">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="eade9-161">Вы можете добавить календарь ICS в почтовый ящик пользователя через интерфейс пользователя, но не через API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="eade9-161">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="eade9-p110">[Перечисление календарей пользователя](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/user_list_calendars) позволяет получить свойства **name**, **color** и **id** всех [календарей](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/calendar) в группе календарей пользователя по умолчанию или указанной группе календарей, в том числе календарей ICS. URL-адрес ICS невозможно хранить и открывать в ресурсе calendar.</span><span class="sxs-lookup"><span data-stu-id="eade9-p110">[Listing the user's calendars](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/user_list_calendars) lets you get the **name**, **color** and **id** properties of each [calendar](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/calendar) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="eade9-164">Вы также можете [отобразить события](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/calendar_list_events) календаря ICS.</span><span class="sxs-lookup"><span data-stu-id="eade9-164">You can also [list the events](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/calendar_list_events) of an ICS-based calendar.</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="eade9-165">Доступ к общему календарю</span><span class="sxs-lookup"><span data-stu-id="eade9-165">Accessing a shared calendar</span></span>

<span data-ttu-id="eade9-166">При использовании следующей операции для доступа к событиям в календаре другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="eade9-166">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET \users('{id}')\calendars('{id}')\events
```

<span data-ttu-id="eade9-p111">Может возникнуть ошибка HTTP 500 `ErrorInternalServerTransientError`. Ошибка возникает, потому что:</span><span class="sxs-lookup"><span data-stu-id="eade9-p111">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="eade9-169">Существуют два способа реализации общего доступа к календарю, которые для ясности мы будем называть "старый" способ и "новый" способ.</span><span class="sxs-lookup"><span data-stu-id="eade9-169">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="eade9-170">Новый способ в настоящее время доступен для предоставления доступа к календарям с разрешениями на просмотр или редактирование, но не с делегированными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="eade9-170">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="eade9-171">С помощью REST API календаря можно просматривать и редактировать общие календари, только если доступ к ним предоставлен **новым** способом.</span><span class="sxs-lookup"><span data-stu-id="eade9-171">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="eade9-172">С помощью REST API календаря нельзя просматривать или редактировать общие календари (или их события), если доступ к ним предоставлен **старым** способом.</span><span class="sxs-lookup"><span data-stu-id="eade9-172">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="eade9-173">Если доступ к календарю был предоставлен с разрешениями на просмотр или редактирование, но старым способом, вы можете вручную обновить календарь, чтобы использовать новый способ.</span><span class="sxs-lookup"><span data-stu-id="eade9-173">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="eade9-174">Чтобы можно было использовать новый способ, со временем Outlook автоматически обновит все общие календари, в том числе те, доступ к которым предоставлен с делегированными разрешениями.</span><span class="sxs-lookup"><span data-stu-id="eade9-174">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="eade9-175">Чтобы с этой целью вручную обновить общий календарь, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="eade9-175">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="eade9-176">Получатель удаляет календарь, доступ к которому был ранее ему предоставлен.</span><span class="sxs-lookup"><span data-stu-id="eade9-176">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="eade9-177">Владелец повторно предоставляет доступ к календарю в Outlook в Интернете, Outlook на iOS или Outlook на Android.</span><span class="sxs-lookup"><span data-stu-id="eade9-177">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="eade9-p113">Получатель повторно принимает календарь, используя Outlook в Интернете. (Скоро можно будет использовать другие клиенты Outlook.)</span><span class="sxs-lookup"><span data-stu-id="eade9-p113">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="eade9-180">Доступ к календарю успешно предоставлен новым способом, если получатель может просмотреть его в Outlook на iOS или Outlook на Android.</span><span class="sxs-lookup"><span data-stu-id="eade9-180">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="eade9-p114">Календарь, доступ к которому предоставлен новым способом, выглядит как один из стандартных календарей в вашем почтовом ящике. С помощью REST API календаря можно просматривать и редактировать события в общем календаре, как в своем собственном. Например:</span><span class="sxs-lookup"><span data-stu-id="eade9-p114">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET \me\calendars('{id}')\events
```


## <a name="contacts"></a><span data-ttu-id="eade9-184">Контакты</span><span class="sxs-lookup"><span data-stu-id="eade9-184">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="eade9-185">Контакты организации доступны только в бета-версии</span><span class="sxs-lookup"><span data-stu-id="eade9-185">Organization contacts available in only beta</span></span>

<span data-ttu-id="eade9-p115">В настоящее время поддерживаются только личные контакты. В настоящее время контакты организации не поддерживаются в версии `/v1.0`, но их можно найти в версии `/beta`.</span><span class="sxs-lookup"><span data-stu-id="eade9-p115">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="eade9-188">Папка контактов по умолчанию</span><span class="sxs-lookup"><span data-stu-id="eade9-188">Default contacts folder</span></span>

<span data-ttu-id="eade9-189">В версии `/v1.0` запрос `GET /me/contactFolders` не включает папку контактов пользователя по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="eade9-189">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="eade9-p116">Эта ошибка будет исправлена. Чтобы получить идентификатор папки контактов по умолчанию, вы можете использовать следующий запрос на [отображение контактов](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/user_list_contacts) и свойство **parentFolderId**:</span><span class="sxs-lookup"><span data-stu-id="eade9-p116">A fix will be made available. Meanwhile, you can use the following [list contacts](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/api/user_list_contacts) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="eade9-192">В указанном выше запросе:</span><span class="sxs-lookup"><span data-stu-id="eade9-192">In the above query:</span></span>

1. <span data-ttu-id="eade9-193">`/me/contacts?$top=1` возвращает свойства [контакта](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/contact) в папке контактов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="eade9-193">`/me/contacts?$top=1` gets the properties of a [contact](http://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/contact) in the default contacts folder.</span></span>
2. <span data-ttu-id="eade9-194">При добавлении `&$select=parentFolderId` возвращается только свойство контакта **parentFolderId** — идентификатор папки контактов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="eade9-194">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="eade9-195">Доступ к контактам через папку контактов в бета-версии</span><span class="sxs-lookup"><span data-stu-id="eade9-195">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="eade9-196">В настоящее время в версии `/beta` существует проблема, из-за которой нельзя получить доступ к ресурсу [contact](../api-reference/beta/resources/contact.md), указав его родительскую папку в URL-адресе запроса REST, как показано в 2 приведенных ниже сценариях.</span><span class="sxs-lookup"><span data-stu-id="eade9-196">In the `/beta` version, there is currently an issue that prevents accessing a [contact](../api-reference/beta/resources/contact.md) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="eade9-197">Доступ к контакту из папки верхнего уровня [contactFolder](../api-reference/beta/resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="eade9-197">Accessing a contact from a top level [contactFolder](../api-reference/beta/resources/contactfolder.md) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="eade9-p117">Доступ к контакту в дочерней папке папки **contactFolder**.  В приведенном ниже примере показан один уровень вложения, но для хранения контакта допускается несколько.</span><span class="sxs-lookup"><span data-stu-id="eade9-p117">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="eade9-200">Кроме того, вы можете просто [получить](../api-reference/beta/api/contact_get.md) контакт по его идентификатору, как показано ниже, так как конечная точка /contacts для запроса GET в версии `/beta` применяется ко всем контактам в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="eade9-200">As an alternative, you can simply [get](../api-reference/beta/api/contact_get.md) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a><span data-ttu-id="eade9-201">Сообщения</span><span class="sxs-lookup"><span data-stu-id="eade9-201">Messages</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="eade9-202">Параметр comment для создания черновика</span><span class="sxs-lookup"><span data-stu-id="eade9-202">The comment parameter for creating a draft</span></span>

<span data-ttu-id="eade9-203">Параметр **comment** для создания ответа или черновика ([createReply](../api-reference/v1.0/api/message_createreply.md), [createReplyAll](../api-reference/v1.0/api/message_createreplyall.md), [createForward](../api-reference/v1.0/api/message_createforward.md)) не включается в текст полученного черновика сообщения.</span><span class="sxs-lookup"><span data-stu-id="eade9-203">The **comment** parameter for creating a reply or forward draft ([createReply](../api-reference/v1.0/api/message_createreply.md), [createReplyAll](../api-reference/v1.0/api/message_createreplyall.md), [createForward](../api-reference/v1.0/api/message_createforward.md)) does not become part of the body of the resultant message draft.</span></span>


## <a name="drives-files-and-content-streaming"></a><span data-ttu-id="eade9-204">Диски, файлы и потоковая передача контента</span><span class="sxs-lookup"><span data-stu-id="eade9-204">Drives, files and content streaming</span></span>

* <span data-ttu-id="eade9-205">При первом доступе к личному диску пользователя с помощью Microsoft Graph до открытия им своего личного сайта в браузере возвращается ответ 401.</span><span class="sxs-lookup"><span data-stu-id="eade9-205">First time access to a user's personal drive through the Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="eade9-206">Ограничения параметров запроса</span><span class="sxs-lookup"><span data-stu-id="eade9-206">Query parameter limitations</span></span>

* <span data-ttu-id="eade9-207">Не поддерживается несколько пространств имен.</span><span class="sxs-lookup"><span data-stu-id="eade9-207">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="eade9-208">Не поддерживаются запросы GET для `$ref` и приведение для пользователей, групп, устройств, субъектов-служб и приложений.</span><span class="sxs-lookup"><span data-stu-id="eade9-208">GETs on `$ref` and casting is not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="eade9-p118">Не поддерживается `@odata.bind`. Это значит, что разработчики не смогут правильно задавать параметры `Accepted` и `RejectedSenders` для группы.</span><span class="sxs-lookup"><span data-stu-id="eade9-p118">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the `Accepted` or `RejectedSenders` on a group.</span></span>
* <span data-ttu-id="eade9-211">Отсутствует `@odata.id` для навигации по объектам без вложений (например, сообщениям) при использовании минимальных метаданных.</span><span class="sxs-lookup"><span data-stu-id="eade9-211">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="eade9-212">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="eade9-212"></span></span>
  * <span data-ttu-id="eade9-213">Отсутствует поддержка `nextLink`.</span><span class="sxs-lookup"><span data-stu-id="eade9-213">No support for `nextLink`</span></span>
  * <span data-ttu-id="eade9-214">Поддерживается не более одного уровня развертывания.</span><span class="sxs-lookup"><span data-stu-id="eade9-214">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="eade9-215">Не поддерживаются дополнительные параметры (`$filter`, `$select`).</span><span class="sxs-lookup"><span data-stu-id="eade9-215">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="eade9-216">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="eade9-216"></span></span>
  * <span data-ttu-id="eade9-217">Конечная точка `/attachments` не поддерживает фильтры.</span><span class="sxs-lookup"><span data-stu-id="eade9-217">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="eade9-218">При ее наличии параметр `$filter` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="eade9-218">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="eade9-219">Фильтрация нескольких рабочих нагрузок не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eade9-219">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="eade9-220">`$search`:</span><span class="sxs-lookup"><span data-stu-id="eade9-220"></span></span>
  * <span data-ttu-id="eade9-221">Полнотекстовый поиск доступен только для некоторых объектов, например сообщений.</span><span class="sxs-lookup"><span data-stu-id="eade9-221">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="eade9-222">Поиск по нескольким рабочим нагрузкам не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eade9-222">Cross-workload searching is not supported.</span></span>

## <a name="delta-query"></a><span data-ttu-id="eade9-223">Разностный запрос</span><span class="sxs-lookup"><span data-stu-id="eade9-223">Delta query</span></span>

* <span data-ttu-id="eade9-224">При отслеживании изменений в отношениях иногда неправильно возвращается контекст OData.</span><span class="sxs-lookup"><span data-stu-id="eade9-224">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="eade9-225">Расширения схемы (устаревшие) не возвращаются с оператором $select и возвращаются без него.</span><span class="sxs-lookup"><span data-stu-id="eade9-225">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="eade9-226">Клиенты не могут отслеживать изменения в открытых расширениях и зарегистрированных расширениях схемы.</span><span class="sxs-lookup"><span data-stu-id="eade9-226">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="application-and-serviceprincipal-api-changes"></a><span data-ttu-id="eade9-227">Изменения в API application и servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="eade9-227">Application and servicePrincipal API changes</span></span>

<span data-ttu-id="eade9-p120">Скоро в объекты [application](../api-reference/beta/resources/application.md) и [servicePrincipal](../api-reference/beta/resources/serviceprincipal.md) будут внесены изменения. Ниже приведено краткое описание текущих ограничений и возможностей API, находящихся в разработке.</span><span class="sxs-lookup"><span data-stu-id="eade9-p120">There are changes to the [application](../api-reference/beta/resources/application.md) and [servicePrincipal](../api-reference/beta/resources/serviceprincipal.md) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="eade9-230">Текущие ограничения:</span><span class="sxs-lookup"><span data-stu-id="eade9-230">Current limitations:</span></span>

* <span data-ttu-id="eade9-231">Некоторые свойства application (такие как appRoles и addIns) будут доступны только после внесения всех изменений.</span><span class="sxs-lookup"><span data-stu-id="eade9-231">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="eade9-232">Регистрировать можно только мультитенантные приложения.</span><span class="sxs-lookup"><span data-stu-id="eade9-232">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="eade9-233">Обновлять можно только приложения, зарегистрированные после первоначального обновления бета-версии.</span><span class="sxs-lookup"><span data-stu-id="eade9-233">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="eade9-234">Пользователи Azure Active Directory могут регистрировать приложения и добавлять владельцев.</span><span class="sxs-lookup"><span data-stu-id="eade9-234">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="eade9-235">Поддержка протоколов OpenID Connect и OAuth.</span><span class="sxs-lookup"><span data-stu-id="eade9-235">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="eade9-236">Невозможно назначение политик приложению.</span><span class="sxs-lookup"><span data-stu-id="eade9-236">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="eade9-237">Не выполняются операции с ownedObjects, для которых требуется код appId (например, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span><span class="sxs-lookup"><span data-stu-id="eade9-237">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="eade9-238">В разработке:</span><span class="sxs-lookup"><span data-stu-id="eade9-238">In development:</span></span>

* <span data-ttu-id="eade9-239">Возможность регистрировать однотенантные приложения.</span><span class="sxs-lookup"><span data-stu-id="eade9-239">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="eade9-240">Обновления объекта servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="eade9-240">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="eade9-241">Перевод существующих приложений Azure AD на обновленную модель.</span><span class="sxs-lookup"><span data-stu-id="eade9-241">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="eade9-242">Поддержка appRoles, предварительно авторизованные клиенты, необязательные утверждения, утверждения членства в группе и брендинг.</span><span class="sxs-lookup"><span data-stu-id="eade9-242">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="eade9-243">Пользователи учетной записи Майкрософт (MSA) могут регистрировать приложения.</span><span class="sxs-lookup"><span data-stu-id="eade9-243">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="eade9-244">Поддержка протоколов SAML и WsFed.</span><span class="sxs-lookup"><span data-stu-id="eade9-244">Support for SAML and WsFed protocols.</span></span>

## <a name="extensions"></a><span data-ttu-id="eade9-245">Расширения</span><span class="sxs-lookup"><span data-stu-id="eade9-245">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="eade9-246">Отслеживание изменений не поддерживается</span><span class="sxs-lookup"><span data-stu-id="eade9-246">Change tracking is not supported</span></span>

<span data-ttu-id="eade9-247">Отслеживание изменений не поддерживается для свойств открытых расширений и расширений схемы.</span><span class="sxs-lookup"><span data-stu-id="eade9-247">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="eade9-248">Одновременное создание ресурса и открытого расширения</span><span class="sxs-lookup"><span data-stu-id="eade9-248">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="eade9-p121">Невозможно указать открытое расширение при создании экземпляра **administrativeUnit**, **device**, **group**, **organization** или **user**. Сначала необходимо создать экземпляр, а затем указать данные открытого расширения в последующем запросе ``POST`` к этому экземпляру.</span><span class="sxs-lookup"><span data-stu-id="eade9-p121">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="eade9-251">Создание экземпляра ресурса с одновременным добавлением данных расширения схемы</span><span class="sxs-lookup"><span data-stu-id="eade9-251">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="eade9-252">Вы не можете указать расширение схемы в той же операции, которая создает экземпляр **contact**, **event**, **message** или **post**.</span><span class="sxs-lookup"><span data-stu-id="eade9-252">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="eade9-253">Сперва нужно создать экземпляр ресурса, а затем выполнить операцию `PATCH` для этого экземпляра, чтобы добавить расширение схемы и пользовательские данные.</span><span class="sxs-lookup"><span data-stu-id="eade9-253">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="eade9-254">Для каждого экземпляра ресурса разрешено не более 100 значений свойства расширения схемы</span><span class="sxs-lookup"><span data-stu-id="eade9-254">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="eade9-255">В настоящее время для каждого экземпляра таких ресурсов каталога, как **device**, **group** и **user**, можно установить не более 100 значений свойства расширения схемы.</span><span class="sxs-lookup"><span data-stu-id="eade9-255">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="eade9-256">Фильтрация по свойствам расширения схемы поддерживается не для всех типов объектов</span><span class="sxs-lookup"><span data-stu-id="eade9-256">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="eade9-257">Фильтрация по свойствам расширения схемы (с помощью выражения `$filter`) не поддерживается для типов сущностей Outlook **contact**, **event**, **message** или **post**.</span><span class="sxs-lookup"><span data-stu-id="eade9-257">Filtering on schema extension properties (using the `$filter` expresssion) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="json-batching"></a><span data-ttu-id="eade9-258">Пакетная обработка JSON</span><span class="sxs-lookup"><span data-stu-id="eade9-258">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="eade9-259">Не поддерживаются вложенные пакеты</span><span class="sxs-lookup"><span data-stu-id="eade9-259">No nested batch</span></span>

<span data-ttu-id="eade9-260">Пакетные запросы JSON не должны содержать вложенных пакетных запросов.</span><span class="sxs-lookup"><span data-stu-id="eade9-260">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="eade9-261">Все отдельные запросы должны быть синхронными</span><span class="sxs-lookup"><span data-stu-id="eade9-261">All individual requests must be synchronous</span></span>

<span data-ttu-id="eade9-p123">Все запросы, содержащиеся в пакетном запросе, должны выполняться синхронно. Параметр `respond-async`, если он имеется, будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="eade9-p123">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="eade9-264">Не поддерживается диалоговая обработка</span><span class="sxs-lookup"><span data-stu-id="eade9-264">No transactions</span></span>

<span data-ttu-id="eade9-p124">В настоящее время Microsoft Graph не поддерживает диалоговую обработку отдельных запросов. Свойство `atomicityGroup` отдельных запросов будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="eade9-p124">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="eade9-267">URI должны быть относительными</span><span class="sxs-lookup"><span data-stu-id="eade9-267">URIs must be relative</span></span>

<span data-ttu-id="eade9-p125">Всегда указывайте относительные URI в пакетных запросах. Microsoft Graph сделает эти URL-адреса абсолютными с помощью конечной точки версии, включенной в URL-адрес пакета.</span><span class="sxs-lookup"><span data-stu-id="eade9-p125">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="eade9-270">Ограничение на размер пакета</span><span class="sxs-lookup"><span data-stu-id="eade9-270">Limit on batch size</span></span>

<span data-ttu-id="eade9-271">В настоящее время в пакетный запрос JSON можно включить не более 20 отдельных запросов.</span><span class="sxs-lookup"><span data-stu-id="eade9-271">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="eade9-272">Упрощенные зависимости</span><span class="sxs-lookup"><span data-stu-id="eade9-272">Simplified dependencies</span></span>

<span data-ttu-id="eade9-p126">Отдельные запросы могут зависеть от других отдельных запросов. В настоящее время запросы могут зависеть только от одного другого запроса и должны соответствовать одному из этих шаблонов:</span><span class="sxs-lookup"><span data-stu-id="eade9-p126">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="eade9-275">Параллельный — для отдельных запросов не указаны зависимости в свойстве `dependsOn`.</span><span class="sxs-lookup"><span data-stu-id="eade9-275">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="eade9-276">Последовательный — все отдельные запросы зависят от предыдущего отдельного запроса.</span><span class="sxs-lookup"><span data-stu-id="eade9-276">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="eade9-277">Идентичный — для всех отдельных запросов в свойстве `dependsOn` указана одна и та же зависимость.</span><span class="sxs-lookup"><span data-stu-id="eade9-277">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="eade9-278">После усовершенствования пакетной обработки JSON эти ограничения будут удалены.</span><span class="sxs-lookup"><span data-stu-id="eade9-278">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="eade9-279">Приложения Cloud Solution Provider</span><span class="sxs-lookup"><span data-stu-id="eade9-279">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="eade9-280">Приложения CSP должны использовать конечную точку Azure AD</span><span class="sxs-lookup"><span data-stu-id="eade9-280">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="eade9-p127">Приложения CSP должны получать маркеры из конечных точек Azure AD (версии 1) для успешного вызова Microsoft Graph в своих клиентах, управляемых партнерами. В настоящее время получение маркера через конечную точку Azure AD версии 2.0 не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eade9-p127">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="eade9-283">В некоторых клиентах предоставленные приложениям CSP разрешения не работают</span><span class="sxs-lookup"><span data-stu-id="eade9-283">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="eade9-284">Предоставленные приложениям CSP разрешения могут не работать в некоторых клиентах.</span><span class="sxs-lookup"><span data-stu-id="eade9-284">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="eade9-285">После первого входа в приложение, использующее делегированные разрешения, в новом клиенте может возникнуть эта ошибка: `AADSTS50000: There was an error issuing a token`.</span><span class="sxs-lookup"><span data-stu-id="eade9-285">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="eade9-286">Приложение, использующее разрешения для приложений, может получить маркер, но ему может быть неожиданно отказано в доступе при вызове Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="eade9-286">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="eade9-287">Мы делаем все возможное, чтобы как можно быстрее исправить эту ошибку.</span><span class="sxs-lookup"><span data-stu-id="eade9-287">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="eade9-288">Для целей разработки и тестирования можно использовать следующее временное решение.</span><span class="sxs-lookup"><span data-stu-id="eade9-288">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="eade9-p128">**ПРИМЕЧАНИЕ.** Это не окончательное решение и предназначено только для целей разработки.  Оно станет ненужным после исправления упомянутой выше ошибки.  Удалять указанный ниже субъект-службу не нужно.</span><span class="sxs-lookup"><span data-stu-id="eade9-p128">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="eade9-p129">Откройте сеанс Azure AD PowerShell 2 и подключитесь к клиенту `customer`, введя учетные данные администратора в окне входа. Скачать и установить Azure AD PowerShell 2 можно [здесь](https://www.powershellgallery.com/packages/AzureAD).</span><span class="sxs-lookup"><span data-stu-id="eade9-p129">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="eade9-294">Создайте субъект-службу Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="eade9-294">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="eade9-295">Функции, доступные только в REST API Office 365 или API Graph Azure AD</span><span class="sxs-lookup"><span data-stu-id="eade9-295">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="eade9-p130">Некоторые функции еще не доступны в Microsoft Graph. Если вы не нашли нужную функцию, можете использовать специальные [REST API Office 365](https://msdn.microsoft.com/ru-RU/office/office365/api/api-catalog). Сведения о функциях, доступных только через API Azure AD Graph, читайте в записи [Microsoft Graph или Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) в блоге.</span><span class="sxs-lookup"><span data-stu-id="eade9-p130">Some functionality is not yet available in Microsoft Graph. If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](https://msdn.microsoft.com/ru-RU/office/office365/api/api-catalog). For Azure Active Directory, please refer to the [Microsoft Graph or Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) blog post on the features that are only available through Azure AD Graph API.</span></span>

## <a name="feedback"></a><span data-ttu-id="eade9-299">Отзывы</span><span class="sxs-lookup"><span data-stu-id="eade9-299">Feedback</span></span>

> <span data-ttu-id="eade9-p131">Ваш отзыв важен для нас. Для связи с нами используйте сайт [Stack Overflow](http://stackoverflow.com/questions/tagged/microsoftgraph).</span><span class="sxs-lookup"><span data-stu-id="eade9-p131">Your feedback is important to us. Connect with us on [Stack Overflow](http://stackoverflow.com/questions/tagged/microsoftgraph).</span></span>
