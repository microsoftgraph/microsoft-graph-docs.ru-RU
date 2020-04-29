---
title: Перечисление schemaExtensions
description: 'Получение списка объектов schemaExtension, созданных любыми приложениями, которыми владеет текущий клиент (которые можно '
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: d959e9f1440f4c83b0f6c8ca3a91a68241010b4d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509957"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="17d76-103">Перечисление schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="17d76-103">List schemaExtensions</span></span>

<span data-ttu-id="17d76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17d76-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="17d76-105">Получение списка объектов [schemaExtension](../resources/schemaextension.md) , созданных всеми приложениями, которыми вы владеете в текущем клиенте (которая может быть **разработкой**, **доступной**или **устаревшей**), а также всеми другими расширениями схемы, принадлежащими другим приложениям, которые помечены как **Доступные**.</span><span class="sxs-lookup"><span data-stu-id="17d76-105">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="permissions"></a><span data-ttu-id="17d76-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17d76-106">Permissions</span></span>
<span data-ttu-id="17d76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17d76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="17d76-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17d76-109">Permission type</span></span>      | <span data-ttu-id="17d76-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17d76-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17d76-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17d76-111">Delegated (work or school account)</span></span> | <span data-ttu-id="17d76-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17d76-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="17d76-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17d76-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17d76-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17d76-114">Not supported.</span></span>    |
|<span data-ttu-id="17d76-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17d76-115">Application</span></span> | <span data-ttu-id="17d76-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17d76-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17d76-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17d76-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="17d76-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="17d76-118">Optional query parameters</span></span>
<span data-ttu-id="17d76-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="17d76-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17d76-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17d76-120">Request headers</span></span>
| <span data-ttu-id="17d76-121">Имя</span><span class="sxs-lookup"><span data-stu-id="17d76-121">Name</span></span>      |<span data-ttu-id="17d76-122">Описание</span><span class="sxs-lookup"><span data-stu-id="17d76-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="17d76-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17d76-123">Authorization</span></span>  | <span data-ttu-id="17d76-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17d76-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17d76-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17d76-126">Content-Type</span></span>   | <span data-ttu-id="17d76-127">application/json</span><span class="sxs-lookup"><span data-stu-id="17d76-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="17d76-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="17d76-128">Request body</span></span>
<span data-ttu-id="17d76-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="17d76-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17d76-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="17d76-130">Response</span></span>

<span data-ttu-id="17d76-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [schemaExtension](../resources/schemaextension.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17d76-131">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17d76-132">Пример</span><span class="sxs-lookup"><span data-stu-id="17d76-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17d76-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="17d76-133">Request</span></span>
<span data-ttu-id="17d76-134">В приведенном ниже примере показано, как просмотреть все доступные расширения для конкретного объекта, выполнив фильтрацию по его уникальному **идентификатору**.</span><span class="sxs-lookup"><span data-stu-id="17d76-134">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="17d76-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="17d76-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
# <a name="c"></a>[<span data-ttu-id="17d76-136">C#</span><span class="sxs-lookup"><span data-stu-id="17d76-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextensions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17d76-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17d76-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextensions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17d76-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17d76-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextensions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17d76-139">Java</span><span class="sxs-lookup"><span data-stu-id="17d76-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schemaextensions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="17d76-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="17d76-140">Response</span></span>
<span data-ttu-id="17d76-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17d76-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="17d76-144">См. также</span><span class="sxs-lookup"><span data-stu-id="17d76-144">See also</span></span>

- [<span data-ttu-id="17d76-145">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="17d76-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="17d76-146">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="17d76-146">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
