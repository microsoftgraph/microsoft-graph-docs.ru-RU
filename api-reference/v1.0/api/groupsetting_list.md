# <a name="list-group-settings"></a><span data-ttu-id="636e9-101">Перечисление параметров группы</span><span class="sxs-lookup"><span data-stu-id="636e9-101">List group settings</span></span>

<span data-ttu-id="636e9-102">Получение списка, включающего объекты параметров группы.</span><span class="sxs-lookup"><span data-stu-id="636e9-102">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="636e9-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="636e9-103">Permissions</span></span>

<span data-ttu-id="636e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="636e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="636e9-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="636e9-106">Permission type</span></span>      | <span data-ttu-id="636e9-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="636e9-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="636e9-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="636e9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="636e9-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="636e9-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="636e9-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="636e9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="636e9-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="636e9-111">Not supported.</span></span>    |
|<span data-ttu-id="636e9-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="636e9-112">Application</span></span> | <span data-ttu-id="636e9-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="636e9-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="636e9-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="636e9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="636e9-115">Перечисление параметров на уровне клиента или отдельной группы.</span><span class="sxs-lookup"><span data-stu-id="636e9-115">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="636e9-116">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="636e9-116">Optional query parameters</span></span>
<span data-ttu-id="636e9-117">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="636e9-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="636e9-118">Примечание. $filter не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="636e9-118">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="636e9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="636e9-119">Request headers</span></span>
| <span data-ttu-id="636e9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="636e9-120">Name</span></span> | <span data-ttu-id="636e9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="636e9-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="636e9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="636e9-122">Authorization</span></span>  | <span data-ttu-id="636e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="636e9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="636e9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="636e9-125">Request body</span></span>
<span data-ttu-id="636e9-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="636e9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="636e9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="636e9-127">Response</span></span>

<span data-ttu-id="636e9-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [groupSetting](../resources/groupsetting.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="636e9-128">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="636e9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="636e9-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="636e9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="636e9-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a><span data-ttu-id="636e9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="636e9-131">Response</span></span>

<span data-ttu-id="636e9-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="636e9-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "displayName": "displayName-value",
      "templateId": "templateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ],
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->