# <a name="driveitem-preview"></a><span data-ttu-id="68962-101">driveItem: предварительный просмотр</span><span class="sxs-lookup"><span data-stu-id="68962-101">driveItem: preview</span></span>

<span data-ttu-id="68962-102">Это действие позволяет получать кратковременного встраиваемые URL-адреса для элемента для визуализации временные предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="68962-102">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="68962-103">Если вы хотите получить длинные встраиваемые ссылки, используйте [команду createLink][] API.</span><span class="sxs-lookup"><span data-stu-id="68962-103">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="68962-104">**Примечание:** Действие **предварительного просмотра** в данный момент доступна только на сервере SharePoint и OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="68962-104">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[команду createLink]: driveItem_createLink.md
[createLink]: driveItem_createLink.md

## <a name="permissions"></a><span data-ttu-id="68962-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68962-106">Permissions</span></span>

<span data-ttu-id="68962-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="68962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="68962-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68962-109">Permission type</span></span>                        | <span data-ttu-id="68962-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68962-110">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="68962-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68962-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="68962-112">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68962-112">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="68962-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68962-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68962-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68962-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="68962-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68962-115">Application</span></span>                            | <span data-ttu-id="68962-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68962-116">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="68962-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68962-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="68962-118">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68962-118">Request body</span></span>

<span data-ttu-id="68962-119">Текст запроса определяет свойства встраиваемые URL-адреса, запрашивающего приложения.</span><span class="sxs-lookup"><span data-stu-id="68962-119">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="68962-120">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="68962-120">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="68962-121">Имя</span><span class="sxs-lookup"><span data-stu-id="68962-121">Name</span></span>      |  <span data-ttu-id="68962-122">Тип</span><span class="sxs-lookup"><span data-stu-id="68962-122">Type</span></span>         | <span data-ttu-id="68962-123">Описание</span><span class="sxs-lookup"><span data-stu-id="68962-123">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="68962-124">page</span><span class="sxs-lookup"><span data-stu-id="68962-124">page</span></span>        | <span data-ttu-id="68962-125">Строка или номер</span><span class="sxs-lookup"><span data-stu-id="68962-125">string/number</span></span> | <span data-ttu-id="68962-126">Необязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="68962-126">Optional.</span></span> <span data-ttu-id="68962-127">Номер документа для запуска, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="68962-127">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="68962-128">Указан как строка для использования в будущем случаев вокруг типов файлов, например ZIP.</span><span class="sxs-lookup"><span data-stu-id="68962-128">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="68962-129">zoom</span><span class="sxs-lookup"><span data-stu-id="68962-129">zoom</span></span>        | <span data-ttu-id="68962-130">number</span><span class="sxs-lookup"><span data-stu-id="68962-130">number</span></span>        | <span data-ttu-id="68962-131">Необязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="68962-131">Optional.</span></span> <span data-ttu-id="68962-132">Выбор масштаба для запуска, если это возможно.</span><span class="sxs-lookup"><span data-stu-id="68962-132">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="68962-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="68962-133">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="68962-134">Ответ будет объект JSON, который содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="68962-134">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="68962-135">Имя</span><span class="sxs-lookup"><span data-stu-id="68962-135">Name</span></span>           | <span data-ttu-id="68962-136">Тип</span><span class="sxs-lookup"><span data-stu-id="68962-136">Type</span></span>   | <span data-ttu-id="68962-137">Описание</span><span class="sxs-lookup"><span data-stu-id="68962-137">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="68962-138">getUrl</span><span class="sxs-lookup"><span data-stu-id="68962-138">getUrl</span></span>         | <span data-ttu-id="68962-139">string</span><span class="sxs-lookup"><span data-stu-id="68962-139">string</span></span> | <span data-ttu-id="68962-140">URL-адрес для внедрения с помощью HTTP GET (Интернет-кадров, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="68962-140">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="68962-141">postUrl</span><span class="sxs-lookup"><span data-stu-id="68962-141">postUrl</span></span>        | <span data-ttu-id="68962-142">string</span><span class="sxs-lookup"><span data-stu-id="68962-142">string</span></span> | <span data-ttu-id="68962-143">URL-адрес для внедрения с помощью HTTP POST (отправки формы, JS, и т.д.)</span><span class="sxs-lookup"><span data-stu-id="68962-143">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="68962-144">postParameters</span><span class="sxs-lookup"><span data-stu-id="68962-144">postParameters</span></span> | <span data-ttu-id="68962-145">string</span><span class="sxs-lookup"><span data-stu-id="68962-145">string</span></span> | <span data-ttu-id="68962-146">Параметры отправки для включения при использовании postUrl</span><span class="sxs-lookup"><span data-stu-id="68962-146">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="68962-147">В зависимости от текущего состояния внедрить поддержку указанные параметры могут возвращаться getUrl, postUrl или оба.</span><span class="sxs-lookup"><span data-stu-id="68962-147">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="68962-148">postParameters — это строка в формате `application/x-www-form-urlencoded`, и, если для выполнения ОТПРАВКУ postUrl типа контента необходимо задать соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="68962-148">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="68962-149">Пример:</span><span class="sxs-lookup"><span data-stu-id="68962-149">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="68962-150">Масштаб страницы /</span><span class="sxs-lookup"><span data-stu-id="68962-150">Page/zoom</span></span>

<span data-ttu-id="68962-151">«Страница» и «отобразить» параметры могут быть недоступны для всех приложений предварительного просмотра, но будет применяться, если версия приложения поддерживает его.</span><span class="sxs-lookup"><span data-stu-id="68962-151">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
