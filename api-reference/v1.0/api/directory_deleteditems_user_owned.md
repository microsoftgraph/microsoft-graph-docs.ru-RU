# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="6f5cd-101">**Список удаленных элементов, принадлежащих пользователю**</span><span class="sxs-lookup"><span data-stu-id="6f5cd-101">Added **List deleted items owned by a user** action to directory (deleted items) resource</span></span>

<span data-ttu-id="6f5cd-102">Извлечение списка недавно удаленных элементов, принадлежащих указанному пользователю.</span><span class="sxs-lookup"><span data-stu-id="6f5cd-102">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="6f5cd-103">В настоящее время функция получения списка удаленных элементов поддерживается только для ресурсов группы ([group](../resources/group.md)), принадлежащих пользователю.</span><span class="sxs-lookup"><span data-stu-id="6f5cd-103">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="6f5cd-104">Это служебное действие, и, следовательно, оно не поддерживает разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="6f5cd-104">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="6f5cd-105">Этот API возвращает до 1 000 удаленных объектов пользователя, отсортированных по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="6f5cd-105">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f5cd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f5cd-106">Permissions</span></span>

<span data-ttu-id="6f5cd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](https://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="6f5cd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/en-us/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="6f5cd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f5cd-109">Permission type</span></span> | <span data-ttu-id="6f5cd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f5cd-110">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="6f5cd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f5cd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6f5cd-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f5cd-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6f5cd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f5cd-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6f5cd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f5cd-114">Not supported.</span></span> |
| <span data-ttu-id="6f5cd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f5cd-115">Application</span></span> | <span data-ttu-id="6f5cd-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f5cd-116">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6f5cd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f5cd-117">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="6f5cd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f5cd-118">Request headers</span></span>

| <span data-ttu-id="6f5cd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6f5cd-119">Name</span></span>          | <span data-ttu-id="6f5cd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6f5cd-120">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="6f5cd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f5cd-121">Authorization</span></span> | <span data-ttu-id="6f5cd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f5cd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6f5cd-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f5cd-124">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="6f5cd-125">В тексту запроса необходимо указать следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="6f5cd-125">The request body requires the following parameters:</span></span>

| <span data-ttu-id="6f5cd-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="6f5cd-126">Parameter</span></span>    | <span data-ttu-id="6f5cd-127">Тип</span><span class="sxs-lookup"><span data-stu-id="6f5cd-127">Type</span></span> |<span data-ttu-id="6f5cd-128">Описание</span><span class="sxs-lookup"><span data-stu-id="6f5cd-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f5cd-129">userId</span><span class="sxs-lookup"><span data-stu-id="6f5cd-129">userId</span></span>|<span data-ttu-id="6f5cd-130">String (строка)</span><span class="sxs-lookup"><span data-stu-id="6f5cd-130">String</span></span>|<span data-ttu-id="6f5cd-131">Идентификатор владельца.</span><span class="sxs-lookup"><span data-stu-id="6f5cd-131">ID of the owner.</span></span>|
|<span data-ttu-id="6f5cd-132">type</span><span class="sxs-lookup"><span data-stu-id="6f5cd-132">type</span></span>|<span data-ttu-id="6f5cd-133">String (строка)</span><span class="sxs-lookup"><span data-stu-id="6f5cd-133">String</span></span>|<span data-ttu-id="6f5cd-134">Тип объектов, принадлежащих пользователю, которые необходимо вернуть; `Group` — единственное поддерживаемое значение в настоящее время.</span><span class="sxs-lookup"><span data-stu-id="6f5cd-134">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="6f5cd-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f5cd-135">Response</span></span>

<span data-ttu-id="6f5cd-136">В случае успеха возвращаются коды ответа `200 OK`; объект ответа включает свойства [directory (удаленные элементы)](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="6f5cd-136">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="6f5cd-137">Пример</span><span class="sxs-lookup"><span data-stu-id="6f5cd-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6f5cd-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f5cd-138">Request</span></span>

<span data-ttu-id="6f5cd-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f5cd-139">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="6f5cd-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f5cd-140">Response</span></span>

<span data-ttu-id="6f5cd-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6f5cd-141">Here is an example of the response.</span></span> <span data-ttu-id="6f5cd-142">Примечание: этот объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="6f5cd-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6f5cd-143">Все поддерживаемые свойства возвращаются из фактических вызовов.</span><span class="sxs-lookup"><span data-stu-id="6f5cd-143">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


