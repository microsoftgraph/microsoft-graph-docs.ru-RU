# <a name="get-group"></a><span data-ttu-id="16892-101">Вывод группы</span><span class="sxs-lookup"><span data-stu-id="16892-101">Get group</span></span>
<span data-ttu-id="16892-102">Получение свойств и связей объекта группы.</span><span class="sxs-lookup"><span data-stu-id="16892-102">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="16892-103">Свойства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="16892-103">Default properties</span></span>

<span data-ttu-id="16892-p101">Ниже показан набор свойств, используемый по умолчанию и возвращаемый при получении групп или выводе списка групп. Это подмножество всех доступных свойств.</span><span class="sxs-lookup"><span data-stu-id="16892-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span>

* <span data-ttu-id="16892-106">description</span><span class="sxs-lookup"><span data-stu-id="16892-106">description</span></span>
* <span data-ttu-id="16892-107">displayName</span><span class="sxs-lookup"><span data-stu-id="16892-107">displayName</span></span>
* <span data-ttu-id="16892-108">groupTypes</span><span class="sxs-lookup"><span data-stu-id="16892-108">groupTypes</span></span>
* <span data-ttu-id="16892-109">id</span><span class="sxs-lookup"><span data-stu-id="16892-109">id</span></span>
* <span data-ttu-id="16892-110">mail</span><span class="sxs-lookup"><span data-stu-id="16892-110">mail</span></span>
* <span data-ttu-id="16892-111">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="16892-111">mailEnabled</span></span>
* <span data-ttu-id="16892-112">mailNickname</span><span class="sxs-lookup"><span data-stu-id="16892-112">mailNickname</span></span>
* <span data-ttu-id="16892-113">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="16892-113">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="16892-114">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="16892-114">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="16892-115">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="16892-115">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="16892-116">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="16892-116">proxyAddresses</span></span>
* <span data-ttu-id="16892-117">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="16892-117">securityEnabled</span></span>
* <span data-ttu-id="16892-118">visibility</span><span class="sxs-lookup"><span data-stu-id="16892-118">visibility</span></span>

<span data-ttu-id="16892-119">По умолчанию следующие свойства групп не возвращаются:</span><span class="sxs-lookup"><span data-stu-id="16892-119">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="16892-120">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="16892-120">allowExternalSenders</span></span>
* <span data-ttu-id="16892-121">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="16892-121">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="16892-122">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="16892-122">isSubscribedByMail</span></span>
* <span data-ttu-id="16892-123">unseenCount</span><span class="sxs-lookup"><span data-stu-id="16892-123">unseenCount</span></span>

<span data-ttu-id="16892-p102">Для их получения используйте параметр запроса **$select**. Примеры.</span><span class="sxs-lookup"><span data-stu-id="16892-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="16892-126">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16892-126">Permissions</span></span>
<span data-ttu-id="16892-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="16892-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16892-129">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16892-129">Permission type</span></span>      | <span data-ttu-id="16892-130">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16892-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16892-131">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16892-131">Delegated (work or school account)</span></span> | <span data-ttu-id="16892-132">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16892-132">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="16892-133">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16892-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16892-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16892-134">Not supported.</span></span>    |
|<span data-ttu-id="16892-135">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16892-135">Application</span></span> | <span data-ttu-id="16892-136">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16892-136">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="16892-137">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16892-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16892-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16892-138">Optional query parameters</span></span>
<span data-ttu-id="16892-139">Этот метод поддерживает [параметры запросов OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="16892-139">This method supports the [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16892-140">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16892-140">Request headers</span></span>
| <span data-ttu-id="16892-141">Имя</span><span class="sxs-lookup"><span data-stu-id="16892-141">Name</span></span>       | <span data-ttu-id="16892-142">Тип</span><span class="sxs-lookup"><span data-stu-id="16892-142">Type</span></span> | <span data-ttu-id="16892-143">Описание</span><span class="sxs-lookup"><span data-stu-id="16892-143">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="16892-144">Authorization</span><span class="sxs-lookup"><span data-stu-id="16892-144">Authorization</span></span>  | <span data-ttu-id="16892-145">string</span><span class="sxs-lookup"><span data-stu-id="16892-145">string</span></span>  | <span data-ttu-id="16892-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16892-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16892-148">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16892-148">Request body</span></span>
<span data-ttu-id="16892-149">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16892-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16892-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="16892-150">Response</span></span>
<span data-ttu-id="16892-151">В случае успеха этот метод возвращает код отклика `200 OK` и объект [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="16892-151">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16892-152">Пример</span><span class="sxs-lookup"><span data-stu-id="16892-152">Example</span></span>
#### <a name="request"></a><span data-ttu-id="16892-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="16892-153">Request</span></span>
<span data-ttu-id="16892-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16892-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="16892-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="16892-155">Response</span></span>
<span data-ttu-id="16892-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16892-156">The following is an example of the response.</span></span>

><span data-ttu-id="16892-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="16892-157">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="16892-158">При фактическом вызове будут возвращены все свойства по умолчанию, как описано ранее.</span><span class="sxs-lookup"><span data-stu-id="16892-158">The default properties will be returned from an actual call, as described before.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
