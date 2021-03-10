---
title: 'synchronizationSchema: filterOperators'
description: Список всех операторов, поддерживаемых в фильтрах scoping.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 0f2274490bba86653e6c1423fa832db265394526
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625646"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="d8806-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="d8806-103">synchronizationSchema: filterOperators</span></span>

<span data-ttu-id="d8806-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8806-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8806-105">Список всех операторов, поддерживаемых в [фильтрах scoping.](../resources/synchronization-filter.md)</span><span class="sxs-lookup"><span data-stu-id="d8806-105">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8806-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8806-106">Permissions</span></span>
<span data-ttu-id="d8806-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8806-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8806-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8806-109">Permission type</span></span>                        | <span data-ttu-id="d8806-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8806-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8806-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8806-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="d8806-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8806-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="d8806-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8806-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="d8806-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8806-114">Not supported.</span></span>|
|<span data-ttu-id="d8806-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d8806-115">Application</span></span>                            |<span data-ttu-id="d8806-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8806-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d8806-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8806-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="d8806-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d8806-118">Request headers</span></span>

| <span data-ttu-id="d8806-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d8806-119">Name</span></span>           | <span data-ttu-id="d8806-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d8806-120">Type</span></span>    | <span data-ttu-id="d8806-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d8806-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="d8806-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8806-122">Authorization</span></span>  | <span data-ttu-id="d8806-123">string</span><span class="sxs-lookup"><span data-stu-id="d8806-123">string</span></span>  | <span data-ttu-id="d8806-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8806-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8806-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8806-126">Request body</span></span>

<span data-ttu-id="d8806-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8806-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8806-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8806-128">Response</span></span>

<span data-ttu-id="d8806-129">В случае успешной работы этот метод возвращает код отклика и объект `200, OK` [коллекции filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d8806-129">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8806-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d8806-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d8806-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8806-131">Request</span></span>
<span data-ttu-id="d8806-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8806-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8806-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8806-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```
# <a name="c"></a>[<span data-ttu-id="d8806-134">C#</span><span class="sxs-lookup"><span data-stu-id="d8806-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-filteroperators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8806-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8806-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-filteroperators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8806-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8806-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-filteroperators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8806-137">Java</span><span class="sxs-lookup"><span data-stu-id="d8806-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationschema-filteroperators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8806-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8806-138">Response</span></span>
<span data-ttu-id="d8806-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d8806-139">The following is an example of a response.</span></span>

><span data-ttu-id="d8806-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d8806-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d8806-141">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="d8806-141">All the properties will be returned in an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.filterOperatorSchema",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "name": "EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "String",
                "Integer"
            ]
        }
    ]
}
```
<!--
Below is the full response, which had to be redacted above as Markdown Scanner tool trips over "type" values containing 
non-string type names like "Integer" or "Boolean"

{
    "value": [
        {
            "name": "EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "IS FALSE",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "IS NOT NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String",
                "Binary",
                "Boolean"
            ]
        },
        {
            "name": "IS NULL",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String",
                "Binary",
                "Boolean"
            ]
        },
        {
            "name": "IS TRUE",
            "arity": "Unary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Boolean"
            ]
        },
        {
            "name": "NOT EQUALS",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "NOT REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        },
        {
            "name": "REGEX MATCH",
            "arity": "Binary",
            "multivaluedComparisonType": "All",
            "supportedAttributeTypes": [
                "Integer",
                "String"
            ]
        }
    ]
}
-->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema: filterOperators",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: synchronizationschema_filteroperators/container/arity:\r\n       Expected type String but actual was Binary. Property: arity, actual value: 'Binary'"
  ]
}
-->


