# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="5ba97-101">Удаление приложения из каталога приложений организации</span><span class="sxs-lookup"><span data-stu-id="5ba97-101">Remove an app from your organization's app catalog</span></span>



<span data-ttu-id="5ba97-102">Удаление [приложения](../resources/teamsapp.md) из каталога приложений организации (каталог приложений клиента).</span><span class="sxs-lookup"><span data-stu-id="5ba97-102">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="5ba97-103">Чтобы удалить приложение из каталога приложений вашей организации, укажите `organization` как **distributionMethod** в [teamsCatalogApp](../resources/teamsapp.md) ресурсов.</span><span class="sxs-lookup"><span data-stu-id="5ba97-103">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ba97-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ba97-104">Permissions</span></span>

<span data-ttu-id="5ba97-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="5ba97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="5ba97-107">**Примечание:** Только глобальный администратор может вызывать этот интерфейс API.</span><span class="sxs-lookup"><span data-stu-id="5ba97-107">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="5ba97-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ba97-108">Permission Type</span></span>                        | <span data-ttu-id="5ba97-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ba97-109">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="5ba97-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ba97-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ba97-111">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ba97-111">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="5ba97-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ba97-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ba97-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5ba97-113">Not supported</span></span>|
| <span data-ttu-id="5ba97-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5ba97-114">Application</span></span>                            | <span data-ttu-id="5ba97-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5ba97-115">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ba97-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ba97-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5ba97-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ba97-117">Request headers</span></span>

| <span data-ttu-id="5ba97-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5ba97-118">Header</span></span>        | <span data-ttu-id="5ba97-119">Значение</span><span class="sxs-lookup"><span data-stu-id="5ba97-119">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="5ba97-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ba97-120">Authorization</span></span> | <span data-ttu-id="5ba97-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5ba97-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ba97-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ba97-123">Request body</span></span>

<span data-ttu-id="5ba97-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5ba97-124">None.</span></span>

><span data-ttu-id="5ba97-125">**Примечание:** Используйте код, возвращенный вызова [списка публикации приложений](./teamsapp_list.md) для ссылок на приложением, которое вы хотите обновить.</span><span class="sxs-lookup"><span data-stu-id="5ba97-125">**Note:** Use the ID returned from the [List published apps](./teamsapp_list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="5ba97-126">Не используйте код из манифеста приложения ZIP-архив.</span><span class="sxs-lookup"><span data-stu-id="5ba97-126">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="5ba97-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ba97-127">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="5ba97-128">Пример</span><span class="sxs-lookup"><span data-stu-id="5ba97-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ba97-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ba97-129">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="5ba97-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5ba97-130">Response</span></span>

```http
HTTP/1.1 204 No Content
```
