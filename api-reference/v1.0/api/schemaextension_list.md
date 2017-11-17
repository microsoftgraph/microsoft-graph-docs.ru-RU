# <a name="list-schemaextensions"></a><span data-ttu-id="7309e-101">Перечисление schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="7309e-101">List schemaExtensions</span></span>

<span data-ttu-id="7309e-102">Получение списка объектов [schemaExtension](../resources/schemaextension.md), созданных любыми приложениями, которыми вы владеете в текущем клиенте (они могут иметь состояние **InDevelopment**, **Available** или **Deprecated**), и всех других расширений схемы, принадлежащих другим приложениям и отмеченных как **Available**.</span><span class="sxs-lookup"><span data-stu-id="7309e-102">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7309e-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7309e-103">Permissions</span></span>
<span data-ttu-id="7309e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7309e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="7309e-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7309e-106">Permission type</span></span>      | <span data-ttu-id="7309e-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7309e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7309e-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7309e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7309e-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7309e-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7309e-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7309e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7309e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7309e-111">Not supported.</span></span>    |
|<span data-ttu-id="7309e-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7309e-112">Application</span></span> | <span data-ttu-id="7309e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7309e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7309e-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7309e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7309e-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7309e-115">Optional query parameters</span></span>
<span data-ttu-id="7309e-116">Этот метод поддерживает [параметры запросов OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7309e-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7309e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7309e-117">Request headers</span></span>
| <span data-ttu-id="7309e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="7309e-118">Name</span></span>      |<span data-ttu-id="7309e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="7309e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7309e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7309e-120">Authorization</span></span>  | <span data-ttu-id="7309e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7309e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7309e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7309e-123">Content-Type</span></span>   | <span data-ttu-id="7309e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7309e-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7309e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7309e-125">Request body</span></span>
<span data-ttu-id="7309e-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7309e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7309e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7309e-127">Response</span></span>

<span data-ttu-id="7309e-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [schemaExtension](../resources/schemaextension.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7309e-128">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7309e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7309e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7309e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7309e-130">Request</span></span>
<span data-ttu-id="7309e-131">В приведенном ниже примере показано, как искать определенное расширение среди всех доступных расширений путем фильтрации по уникальному **идентификатору** расширения.</span><span class="sxs-lookup"><span data-stu-id="7309e-131">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="7309e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7309e-132">Response</span></span>
<span data-ttu-id="7309e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7309e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 274

{
  "value": [
    {
      "id":"graphlearn_test",
      "description": "Yet another test schema",
      "targetTypes": [
          "User", "Group"
      ],
      "status": "InDevelopment",
      "owner": "24d3b144-21ae-4080-943f-7067b395b913",
      "properties": [
          {
              "name": "testName",
              "type": "String"
          }
      ]
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="7309e-136">См. также</span><span class="sxs-lookup"><span data-stu-id="7309e-136">See also</span></span>

- [<span data-ttu-id="7309e-137">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="7309e-137">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="7309e-138">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="7309e-138">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->