---
title: Получение schemaExtension
description: Получите свойства указанного определения схемыExtension.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: bb1cd6e7869faaf67e378a2e24709226c0afc14f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051993"
---
# <a name="get-schemaextension"></a><span data-ttu-id="c0f33-103">Получение schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c0f33-103">Get schemaExtension</span></span>

<span data-ttu-id="c0f33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0f33-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0f33-105">Получите свойства указанного определения [схемыExtension.](../resources/schemaextension.md)</span><span class="sxs-lookup"><span data-stu-id="c0f33-105">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0f33-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0f33-106">Permissions</span></span>
<span data-ttu-id="c0f33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0f33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c0f33-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0f33-109">Permission type</span></span>      | <span data-ttu-id="c0f33-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0f33-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0f33-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0f33-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0f33-112">User.Read, Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f33-112">User.Read, Application.Read.All</span></span>  |
|<span data-ttu-id="c0f33-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0f33-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0f33-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0f33-114">Not supported.</span></span>    |
|<span data-ttu-id="c0f33-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c0f33-115">Application</span></span> | <span data-ttu-id="c0f33-116">Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0f33-116">Application.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0f33-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0f33-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0f33-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0f33-118">Optional query parameters</span></span>
<span data-ttu-id="c0f33-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c0f33-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0f33-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0f33-120">Request headers</span></span>
| <span data-ttu-id="c0f33-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c0f33-121">Name</span></span>      |<span data-ttu-id="c0f33-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c0f33-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c0f33-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0f33-123">Authorization</span></span>  | <span data-ttu-id="c0f33-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0f33-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c0f33-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0f33-126">Content-Type</span></span>   | <span data-ttu-id="c0f33-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c0f33-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0f33-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0f33-128">Request body</span></span>
<span data-ttu-id="c0f33-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0f33-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0f33-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0f33-130">Response</span></span>

<span data-ttu-id="c0f33-131">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект schemaExtension](../resources/schemaextension.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c0f33-131">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0f33-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c0f33-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0f33-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0f33-133">Request</span></span>
<span data-ttu-id="c0f33-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c0f33-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c0f33-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0f33-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/schemaExtensions/graphlearn_test
```
# <a name="c"></a>[<span data-ttu-id="c0f33-136">C#</span><span class="sxs-lookup"><span data-stu-id="c0f33-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0f33-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0f33-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0f33-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0f33-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0f33-139">Java</span><span class="sxs-lookup"><span data-stu-id="c0f33-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c0f33-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0f33-140">Response</span></span>
<span data-ttu-id="c0f33-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c0f33-141">Here is an example of the response.</span></span> <span data-ttu-id="c0f33-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c0f33-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

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
```

## <a name="see-also"></a><span data-ttu-id="c0f33-143">См. также</span><span class="sxs-lookup"><span data-stu-id="c0f33-143">See also</span></span>

- [<span data-ttu-id="c0f33-144">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="c0f33-144">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c0f33-145">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="c0f33-145">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
