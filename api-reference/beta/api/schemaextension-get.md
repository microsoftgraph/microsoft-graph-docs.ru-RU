---
title: Получение schemaExtension
description: Получение свойств указанного определения schemaExtension.
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 05ec95db352b72df579437dd8568b2e4d495bc30
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724703"
---
# <a name="get-schemaextension"></a><span data-ttu-id="b98ce-103">Получение schemaExtension</span><span class="sxs-lookup"><span data-stu-id="b98ce-103">Get schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b98ce-104">Получение свойств указанного определения [schemaExtension](../resources/schemaextension.md) .</span><span class="sxs-lookup"><span data-stu-id="b98ce-104">Get the properties of the specified [schemaExtension](../resources/schemaextension.md) definition.</span></span>

## <a name="permissions"></a><span data-ttu-id="b98ce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b98ce-105">Permissions</span></span>
<span data-ttu-id="b98ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b98ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b98ce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b98ce-108">Permission type</span></span>      | <span data-ttu-id="b98ce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b98ce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b98ce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b98ce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b98ce-111">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b98ce-111">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b98ce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b98ce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b98ce-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b98ce-113">Not supported.</span></span>    |
|<span data-ttu-id="b98ce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b98ce-114">Application</span></span> | <span data-ttu-id="b98ce-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b98ce-115">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b98ce-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b98ce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b98ce-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b98ce-117">Optional query parameters</span></span>
<span data-ttu-id="b98ce-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b98ce-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b98ce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b98ce-119">Request headers</span></span>
| <span data-ttu-id="b98ce-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b98ce-120">Name</span></span>      |<span data-ttu-id="b98ce-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b98ce-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b98ce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b98ce-122">Authorization</span></span>  | <span data-ttu-id="b98ce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b98ce-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b98ce-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b98ce-125">Content-Type</span></span>   | <span data-ttu-id="b98ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b98ce-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b98ce-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b98ce-127">Request body</span></span>
<span data-ttu-id="b98ce-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b98ce-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b98ce-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b98ce-129">Response</span></span>

<span data-ttu-id="b98ce-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [schemaExtension](../resources/schemaextension.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b98ce-130">If successful, this method returns a `200 OK` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b98ce-131">Пример</span><span class="sxs-lookup"><span data-stu-id="b98ce-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b98ce-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="b98ce-132">Request</span></span>
<span data-ttu-id="b98ce-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b98ce-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b98ce-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b98ce-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_schemaextension"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/schemaExtensions/graphlearn_test
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b98ce-135">C#</span><span class="sxs-lookup"><span data-stu-id="b98ce-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b98ce-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b98ce-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b98ce-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b98ce-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b98ce-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b98ce-138">Response</span></span>
<span data-ttu-id="b98ce-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b98ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="b98ce-142">См. также</span><span class="sxs-lookup"><span data-stu-id="b98ce-142">See also</span></span>

- [<span data-ttu-id="b98ce-143">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="b98ce-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b98ce-144">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="b98ce-144">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
