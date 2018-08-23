# <a name="use-the-onenote-rest-api"></a><span data-ttu-id="5dcce-101">Использование REST API для OneNote</span><span class="sxs-lookup"><span data-stu-id="5dcce-101">Use the OneNote REST API</span></span>

<span data-ttu-id="5dcce-102">Microsoft Graph позволяет вашему приложению получать авторизованный доступ к записным книжкам OneNote, разделам и страницам в личной учетной записи или учетной записи организации.</span><span class="sxs-lookup"><span data-stu-id="5dcce-102">Microsoft Graph lets your app get authorized access to a user's OneNote notebooks, sections, and pages in a personal or organization account.</span></span> <span data-ttu-id="5dcce-103">С [соответствующими или делегированными разрешениями приложения](../../../concepts/permissions_reference.md#notes-permissions)ваше приложение может получать доступ к данным OneNote пользователя, выполнившего вход в систему, или любого пользователя в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5dcce-103">With the [appropriate delegated or application permissions](../../../concepts/permissions_reference.md#notes-permissions), your app can access the OneNote data of the signed-in user or any user in a tenant.</span></span>

## <a name="root-url"></a><span data-ttu-id="5dcce-104">Корневой URL-адрес</span><span class="sxs-lookup"><span data-stu-id="5dcce-104">Root URL</span></span>
<span data-ttu-id="5dcce-105">Для всех вызовов API OneNote используется следующий формат корневого URL-адреса службы OneNote.</span><span class="sxs-lookup"><span data-stu-id="5dcce-105">The OneNote service root URL uses the following format for all calls to the OneNote API.</span></span>
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
<span data-ttu-id="5dcce-106">Сегмент `version` URL-адреса представляет собой версию Microsoft Graph, которую вы хотите использовать:</span><span class="sxs-lookup"><span data-stu-id="5dcce-106">The `version` segment in the URL represents the version of Microsoft Graph that you want to use.</span></span>

- <span data-ttu-id="5dcce-107">`v1.0` предназначено для стабильного производственного кода.</span><span class="sxs-lookup"><span data-stu-id="5dcce-107">`v1.0` is for stable production code.</span></span>
- <span data-ttu-id="5dcce-108">`beta` |||UNTRANSLATED_CONTENT_START|||is to try out a feature that's in development.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="5dcce-108">`beta` is to try out a feature that's in development.</span></span> <span data-ttu-id="5dcce-109">Возможности и функции в конечной точке бета-версии могут изменяться. Мы не рекомендуем использовать её в рабочем коде.</span><span class="sxs-lookup"><span data-stu-id="5dcce-109">Features and functionality in the beta endpoint might change; we don't recommend that you use it in your production code.</span></span>

<span data-ttu-id="5dcce-110">В качестве места расположения могут быть записные книжки пользователя в Office 365 или объекте-получателе OneDrive, групповые записные книжки, или размещенные на сайте SharePoint в Office 365 групповые записные книжки.</span><span class="sxs-lookup"><span data-stu-id="5dcce-110">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

![Стек разработки API-интерфейса OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a><span data-ttu-id="5dcce-112">Записные книжки пользователя</span><span class="sxs-lookup"><span data-stu-id="5dcce-112">User notebooks</span></span>
<span data-ttu-id="5dcce-113">Чтобы получить доступ к персональным записным книжкам объекта-получателя OneDrive или OneDrive для бизнеса, воспользуйтесь одним из следующих URL-адресов:</span><span class="sxs-lookup"><span data-stu-id="5dcce-113">User notebooks To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- <span data-ttu-id="5dcce-114">`me` |||UNTRANSLATED_CONTENT_START|||is for OneNote content that the current user can access (owned and shared).|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="5dcce-114">`me` is for OneNote content that the current user can access (owned and shared).</span></span>
- <span data-ttu-id="5dcce-115">`users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем.</span><span class="sxs-lookup"><span data-stu-id="5dcce-115">`users/{id}` is for OneNote content that the specified user (in the URL) has shared with the current user.</span></span> <span data-ttu-id="5dcce-116">Используйте API[пользователей](users.md).</span><span class="sxs-lookup"><span data-stu-id="5dcce-116">[Use the Planner API](users.md)</span></span>
> <span data-ttu-id="5dcce-117">**Примечание.** Вы можете получить идентификаторы пользователя, отправив запрос GET на `https://graph.microsoft.com/v1.0/users`.</span><span class="sxs-lookup"><span data-stu-id="5dcce-117">**Note:** You can get user ids by making a GET request on `https://graph.microsoft.com/v1.0/users`.</span></span>

### <a name="group-notebooks"></a><span data-ttu-id="5dcce-118">Групповые записные книжки</span><span class="sxs-lookup"><span data-stu-id="5dcce-118">Group notebooks</span></span>
<span data-ttu-id="5dcce-119"> Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="5dcce-119">Group notebooks To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a><span data-ttu-id="5dcce-120">Записные книжки на сайте SharePoint</span><span class="sxs-lookup"><span data-stu-id="5dcce-120">SharePoint site notebooks</span></span>

<span data-ttu-id="5dcce-121">Чтобы получить доступ к записным книжкам на узле группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:</span><span class="sxs-lookup"><span data-stu-id="5dcce-121">SharePoint site notebooks To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

