---
title: Перечисление schemaExtensions
description: 'Получение списка объектов schemaExtension, созданных любыми приложениями, которыми владеет текущий клиент (которые можно '
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 1c43bd8227b80661c7194e8269dfce3ee76d0f96
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863483"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="588ec-103">Перечисление schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="588ec-103">List schemaExtensions</span></span>

<span data-ttu-id="588ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="588ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="588ec-105">Получение списка объектов [schemaExtension](../resources/schemaextension.md) , созданных всеми приложениями, которыми вы владеете в текущем клиенте (которая может быть **разработкой**, **доступной**или **устаревшей**), а также всеми другими расширениями схемы, принадлежащими другим приложениям, которые помечены как **Доступные**.</span><span class="sxs-lookup"><span data-stu-id="588ec-105">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

> <span data-ttu-id="588ec-106">**Примечание:** Список также будет содержать определения расширений схемы (помеченные как `Available` ), созданные другими разработчиками из других клиентов.</span><span class="sxs-lookup"><span data-stu-id="588ec-106">**Note:** The list will also contain schema extension definitions (marked as `Available`) created by other developers from other tenants.</span></span> <span data-ttu-id="588ec-107">Это отличается от других интерфейсов API, которые возвращают только данные, зависящие от клиента.</span><span class="sxs-lookup"><span data-stu-id="588ec-107">This is different from other APIs that only return tenant-specific data.</span></span> <span data-ttu-id="588ec-108">Данные расширения, созданные на основе определений расширений схемы, зависят от клиента и доступны только для приложений, которым явно предоставлено разрешение.</span><span class="sxs-lookup"><span data-stu-id="588ec-108">Extension data created based on schema extension definitions is tenant-specific and can only be accessed by apps explicitly granted permission.</span></span> 

## <a name="permissions"></a><span data-ttu-id="588ec-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="588ec-109">Permissions</span></span>
<span data-ttu-id="588ec-110">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="588ec-110">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="588ec-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="588ec-111">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="588ec-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="588ec-112">Permission type</span></span>      | <span data-ttu-id="588ec-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="588ec-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="588ec-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="588ec-114">Delegated (work or school account)</span></span> | <span data-ttu-id="588ec-115">User. Read, Application. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="588ec-115">User.Read, Application.Read.All</span></span>   |
|<span data-ttu-id="588ec-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="588ec-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="588ec-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="588ec-117">Not supported.</span></span>    |
|<span data-ttu-id="588ec-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="588ec-118">Application</span></span> | <span data-ttu-id="588ec-119">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="588ec-119">Application.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="588ec-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="588ec-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="588ec-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="588ec-121">Optional query parameters</span></span>
<span data-ttu-id="588ec-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="588ec-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="588ec-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="588ec-123">Request headers</span></span>
| <span data-ttu-id="588ec-124">Имя</span><span class="sxs-lookup"><span data-stu-id="588ec-124">Name</span></span>      |<span data-ttu-id="588ec-125">Описание</span><span class="sxs-lookup"><span data-stu-id="588ec-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="588ec-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="588ec-126">Authorization</span></span>  | <span data-ttu-id="588ec-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="588ec-127">Bearer {token}.</span></span> <span data-ttu-id="588ec-128">Required.</span><span class="sxs-lookup"><span data-stu-id="588ec-128">Required.</span></span> |
| <span data-ttu-id="588ec-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="588ec-129">Content-Type</span></span>   | <span data-ttu-id="588ec-130">application/json</span><span class="sxs-lookup"><span data-stu-id="588ec-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="588ec-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="588ec-131">Request body</span></span>
<span data-ttu-id="588ec-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="588ec-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="588ec-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="588ec-133">Response</span></span>

<span data-ttu-id="588ec-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [schemaExtension](../resources/schemaextension.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="588ec-134">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="588ec-135">Пример</span><span class="sxs-lookup"><span data-stu-id="588ec-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="588ec-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="588ec-136">Request</span></span>
<span data-ttu-id="588ec-137">В приведенном ниже примере показано, как просмотреть все доступные расширения для конкретного объекта, выполнив фильтрацию по его уникальному **идентификатору**.</span><span class="sxs-lookup"><span data-stu-id="588ec-137">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="588ec-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="588ec-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
# <a name="c"></a>[<span data-ttu-id="588ec-139">C#</span><span class="sxs-lookup"><span data-stu-id="588ec-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextensions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="588ec-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="588ec-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextensions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="588ec-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="588ec-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextensions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="588ec-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="588ec-142">Response</span></span>
<span data-ttu-id="588ec-143">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="588ec-143">Here is an example of the response.</span></span> <span data-ttu-id="588ec-144">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="588ec-144">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="588ec-145">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="588ec-145">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="588ec-146">См. также</span><span class="sxs-lookup"><span data-stu-id="588ec-146">See also</span></span>

- [<span data-ttu-id="588ec-147">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="588ec-147">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="588ec-148">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="588ec-148">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
