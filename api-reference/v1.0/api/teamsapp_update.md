# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="5a217-101">Обновление приложений, опубликованной в каталоге приложений организации</span><span class="sxs-lookup"><span data-stu-id="5a217-101">Update apps published to your organization's app catalog</span></span>



<span data-ttu-id="5a217-102">Обновление [приложения](../resources/teamsapp.md) ранее опубликованы в каталоге приложений группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="5a217-102">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="5a217-103">Этот интерфейс API специально обновляет приложение, опубликованной в каталоге приложений организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="5a217-103">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="5a217-104">Чтобы опубликовать в каталоге приложений организации, укажите `organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5a217-104">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a217-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a217-105">Permissions</span></span>

<span data-ttu-id="5a217-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="5a217-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="5a217-108">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="5a217-108">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="5a217-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a217-109">Permission Type</span></span>                        | <span data-ttu-id="5a217-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a217-110">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="5a217-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a217-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a217-112">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a217-112">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="5a217-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a217-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a217-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5a217-114">Not supported</span></span>|
| <span data-ttu-id="5a217-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a217-115">Application</span></span>                            | <span data-ttu-id="5a217-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5a217-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a217-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a217-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5a217-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a217-118">Request headers</span></span>

| <span data-ttu-id="5a217-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5a217-119">Header</span></span>        | <span data-ttu-id="5a217-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5a217-120">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="5a217-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a217-121">Authorization</span></span> | <span data-ttu-id="5a217-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a217-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5a217-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a217-124">Content-Type</span></span>  | <span data-ttu-id="5a217-125">приложение/zip</span><span class="sxs-lookup"><span data-stu-id="5a217-125">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a217-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a217-126">Request body</span></span>

<span data-ttu-id="5a217-127">Zip полезных команд манифеста: Для приложения группы ZIP-файл, [перейдите в раздел Create пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="5a217-127">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="5a217-128">**Примечание:** Используйте код, возвращенный вызова [списка публикации приложений](./teamsapp_list.md) для ссылок на приложением, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="5a217-128">**Note:** Use the ID returned from the [List published apps](./teamsapp_list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="5a217-129">Не используйте код из манифеста приложения ZIP-архив.</span><span class="sxs-lookup"><span data-stu-id="5a217-129">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="5a217-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a217-130">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="5a217-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5a217-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a217-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a217-132">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="5a217-133">Для приложения группы ZIP-файл [видеть создать пакет приложения](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="5a217-133">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="5a217-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a217-134">Response</span></span>

```
HTTP/1.1 204 No Content
```
