---
title: Перечисление schemaExtensions
description: 'Получите список объектов схемыExtension, созданных любыми приложениями, которые принадлежат вам в текущем клиенте (это может быть '
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 8e1d8e1810f579b7c1e5d31a6e0a221a1df1d7c6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053505"
---
# <a name="list-schemaextensions"></a><span data-ttu-id="d3233-103">Перечисление schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="d3233-103">List schemaExtensions</span></span>

<span data-ttu-id="d3233-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3233-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3233-105">Получите список объектов [схемыExtension,](../resources/schemaextension.md) созданных любыми приложениями, которыми вы владеете в текущем клиенте (которые могут быть **InDevelopment,** **Available** или **Deprecated),** и все другие расширения схемы, которые принадлежат другим приложениям, которые помечены как **Доступные**.</span><span class="sxs-lookup"><span data-stu-id="d3233-105">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

> <span data-ttu-id="d3233-106">**Примечание:** В списке также будут содержаться определения расширения схемы (помеченные как ) созданные другими разработчиками `Available` из других клиентов.</span><span class="sxs-lookup"><span data-stu-id="d3233-106">**Note:** The list will also contain schema extension definitions (marked as `Available`) created by other developers from other tenants.</span></span> <span data-ttu-id="d3233-107">Это отличается от других API-интерфейсов, возвращающих только данные определенного клиента.</span><span class="sxs-lookup"><span data-stu-id="d3233-107">This is different from other APIs that only return tenant-specific data.</span></span> <span data-ttu-id="d3233-108">Данные расширения, созданные на основе определений расширения схемы, являются конкретными для клиента и могут быть доступны только приложениям, явно предоставленным разрешениям.</span><span class="sxs-lookup"><span data-stu-id="d3233-108">Extension data created based on schema extension definitions is tenant-specific and can only be accessed by apps explicitly granted permission.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d3233-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3233-109">Permissions</span></span>
<span data-ttu-id="d3233-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3233-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d3233-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3233-112">Permission type</span></span>      | <span data-ttu-id="d3233-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3233-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3233-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3233-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d3233-115">User.Read, Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3233-115">User.Read, Application.Read.All</span></span>   |
|<span data-ttu-id="d3233-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3233-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3233-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3233-117">Not supported.</span></span>    |
|<span data-ttu-id="d3233-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="d3233-118">Application</span></span> | <span data-ttu-id="d3233-119">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3233-119">Application.Read.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d3233-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3233-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d3233-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d3233-121">Optional query parameters</span></span>
<span data-ttu-id="d3233-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d3233-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3233-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3233-123">Request headers</span></span>
| <span data-ttu-id="d3233-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d3233-124">Name</span></span>      |<span data-ttu-id="d3233-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d3233-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3233-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3233-126">Authorization</span></span>  | <span data-ttu-id="d3233-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3233-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d3233-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3233-129">Content-Type</span></span>   | <span data-ttu-id="d3233-130">application/json</span><span class="sxs-lookup"><span data-stu-id="d3233-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3233-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3233-131">Request body</span></span>
<span data-ttu-id="d3233-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3233-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3233-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3233-133">Response</span></span>

<span data-ttu-id="d3233-134">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [схемыExtension](../resources/schemaextension.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d3233-134">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d3233-135">Пример</span><span class="sxs-lookup"><span data-stu-id="d3233-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3233-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3233-136">Request</span></span>
<span data-ttu-id="d3233-137">В следующем примере показано, как искать среди всех доступных расширений для определенного, фильтруя уникальный **id.**</span><span class="sxs-lookup"><span data-stu-id="d3233-137">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="d3233-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3233-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
# <a name="c"></a>[<span data-ttu-id="d3233-139">C#</span><span class="sxs-lookup"><span data-stu-id="d3233-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextensions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3233-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3233-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextensions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3233-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3233-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextensions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3233-142">Java</span><span class="sxs-lookup"><span data-stu-id="d3233-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schemaextensions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d3233-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3233-143">Response</span></span>
<span data-ttu-id="d3233-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d3233-144">Here is an example of the response.</span></span> <span data-ttu-id="d3233-145">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d3233-145">Note: The response object shown here might be shortened for readability.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d3233-146">См. также</span><span class="sxs-lookup"><span data-stu-id="d3233-146">See also</span></span>

- [<span data-ttu-id="d3233-147">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="d3233-147">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d3233-148">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="d3233-148">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
