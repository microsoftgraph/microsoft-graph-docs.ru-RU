# <a name="get-a-special-folder-by-name"></a><span data-ttu-id="bd932-101">Получение доступа к специальной папке по имени</span><span class="sxs-lookup"><span data-stu-id="bd932-101">Get a special folder by name</span></span>

<span data-ttu-id="bd932-102">Используйте специальную коллекцию для доступа к специальной папке по имени.</span><span class="sxs-lookup"><span data-stu-id="bd932-102">Use the special collection to access a special folder by name.</span></span>

<span data-ttu-id="bd932-p101">Применение специальных папок обеспечивает доступ к известным папкам в OneDrive с помощью простых псевдонимов, благодаря чему можно не искать папку по пути (что потребует локализации) и не ссылаться на нее с использованием идентификатора. Если специальная папка будет переименована или перемещена в другое расположение на диске, такой синтаксис по-прежнему позволит найти ее.</span><span class="sxs-lookup"><span data-stu-id="bd932-p101">Special folders provide simple aliases to access well-known folders in OneDrive without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to find that folder.</span></span>

<span data-ttu-id="bd932-p102">Когда приложение впервые пробует записать что-то в специальную папку, она создается автоматически, если не была создана ранее. Если пользователь удалил такую папку, она создается повторно при записи в нее.</span><span class="sxs-lookup"><span data-stu-id="bd932-p102">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

><span data-ttu-id="bd932-107">**Примечание.**  Если у вас есть разрешения только для чтения и вы запрашиваете несуществующую специальную папку, возвратится сообщение об ошибке `403 Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="bd932-107">**Note:**  If you have read-only permissions and request a special folder that doesn't exist, you'll receive a `403 Forbidden` error.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd932-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd932-108">Permissions</span></span>

<span data-ttu-id="bd932-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bd932-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bd932-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd932-111">Permission type</span></span>                        | <span data-ttu-id="bd932-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd932-112">Permissions (from least to most privileged)</span></span>                                                           |
|:--------------------------------------|:------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="bd932-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd932-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd932-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd932-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |
|<span data-ttu-id="bd932-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd932-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd932-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Files.ReadWrite.AppFolder</span><span class="sxs-lookup"><span data-stu-id="bd932-116">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Files.ReadWrite.AppFolder</span></span>           |
|<span data-ttu-id="bd932-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd932-117">Application</span></span>                            | <span data-ttu-id="bd932-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd932-118">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="bd932-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd932-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/special/{name}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bd932-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bd932-120">Optional query parameters</span></span>

<span data-ttu-id="bd932-121">Этот метод поддерживает [параметры запросов OData](../../../concepts/query_parameters.md) `$expand` и `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bd932-121">This method supports the `$expand` and `$select` [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd932-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd932-122">Request headers</span></span>

| <span data-ttu-id="bd932-123">Имя</span><span class="sxs-lookup"><span data-stu-id="bd932-123">Name</span></span>          | <span data-ttu-id="bd932-124">Тип</span><span class="sxs-lookup"><span data-stu-id="bd932-124">Type</span></span>   | <span data-ttu-id="bd932-125">Описание</span><span class="sxs-lookup"><span data-stu-id="bd932-125">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="bd932-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd932-126">Authorization</span></span> | <span data-ttu-id="bd932-127">string</span><span class="sxs-lookup"><span data-stu-id="bd932-127">string</span></span> | <span data-ttu-id="bd932-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd932-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd932-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd932-130">Request body</span></span>

<span data-ttu-id="bd932-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bd932-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd932-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd932-132">Response</span></span>

<span data-ttu-id="bd932-133">В случае успеха этот метод возвратит код отклика `200 OK` и объект [driveItem](../resources/driveitem.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bd932-133">If successful, this method returns a `200 OK` response code and a [driveItem](../resources/driveitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd932-134">Пример</span><span class="sxs-lookup"><span data-stu-id="bd932-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bd932-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd932-135">Request</span></span>

<span data-ttu-id="bd932-136">Ниже приведен пример запроса на получение списка дисков пользователя.</span><span class="sxs-lookup"><span data-stu-id="bd932-136">Here is an example of the request for the user's drives.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive_special"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/special/{name}
```

##### <a name="response"></a><span data-ttu-id="bd932-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd932-137">Response</span></span>
<span data-ttu-id="bd932-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd932-138">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.driveItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "folder": { },
  "id": "s!lkjqwlkj124912049an",
  "name": "Photos",
  "specialFolder": { "name": "photos" },
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents/Photos",
}
```

## <a name="remarks"></a><span data-ttu-id="bd932-139">Заметки</span><span class="sxs-lookup"><span data-stu-id="bd932-139">Remarks</span></span>

<span data-ttu-id="bd932-140">Чтобы получить список дочерних элементов для специальной папки, можно запросить коллекцию `children` или с помощью параметра [$expand](../../../concepts/query_parameters.md) развернуть этот список.</span><span class="sxs-lookup"><span data-stu-id="bd932-140">To request the children of a special folder, you can request the `children` collection or use the [expand](../../../concepts/query_parameters.md) option to expand the children collection.</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "List drives",
  "keywords": "",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get special folder"
}-->
