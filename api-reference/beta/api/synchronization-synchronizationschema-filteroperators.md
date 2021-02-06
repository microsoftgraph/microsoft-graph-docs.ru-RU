---
title: 'synchronizationSchema: filterOperators'
description: Список всех операторов, поддерживаемых фильтрами области.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 9d790707aa11642499924dd93f75e2cec3945bb3
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133835"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="bbbc3-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="bbbc3-103">synchronizationSchema: filterOperators</span></span>

<span data-ttu-id="bbbc3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbbc3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbbc3-105">Список всех операторов, поддерживаемых [фильтрами области.](../resources/synchronization-filter.md)</span><span class="sxs-lookup"><span data-stu-id="bbbc3-105">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bbbc3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bbbc3-106">Permissions</span></span>
<span data-ttu-id="bbbc3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbbc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbbc3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bbbc3-109">Permission type</span></span>                        | <span data-ttu-id="bbbc3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bbbc3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbbc3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bbbc3-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="bbbc3-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbbc3-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="bbbc3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bbbc3-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="bbbc3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbbc3-114">Not supported.</span></span>|
|<span data-ttu-id="bbbc3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bbbc3-115">Application</span></span>                            |<span data-ttu-id="bbbc3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bbbc3-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bbbc3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bbbc3-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="bbbc3-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bbbc3-118">Request headers</span></span>

| <span data-ttu-id="bbbc3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bbbc3-119">Name</span></span>           | <span data-ttu-id="bbbc3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="bbbc3-120">Type</span></span>    | <span data-ttu-id="bbbc3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="bbbc3-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="bbbc3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbbc3-122">Authorization</span></span>  | <span data-ttu-id="bbbc3-123">string</span><span class="sxs-lookup"><span data-stu-id="bbbc3-123">string</span></span>  | <span data-ttu-id="bbbc3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bbbc3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbbc3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bbbc3-126">Request body</span></span>

<span data-ttu-id="bbbc3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bbbc3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbbc3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbbc3-128">Response</span></span>

<span data-ttu-id="bbbc3-129">В случае успеха этот метод возвращает код отклика и объект коллекции `200, OK` [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bbbc3-129">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbbc3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bbbc3-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bbbc3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bbbc3-131">Request</span></span>
<span data-ttu-id="bbbc3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bbbc3-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bbbc3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbbc3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```
# <a name="c"></a>[<span data-ttu-id="bbbc3-134">C#</span><span class="sxs-lookup"><span data-stu-id="bbbc3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-filteroperators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbbc3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbbc3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-filteroperators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbbc3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbbc3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-filteroperators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bbbc3-137">Java</span><span class="sxs-lookup"><span data-stu-id="bbbc3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationschema-filteroperators-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="bbbc3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bbbc3-138">Response</span></span>
<span data-ttu-id="bbbc3-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bbbc3-139">The following is an example of a response.</span></span>

><span data-ttu-id="bbbc3-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bbbc3-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bbbc3-141">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bbbc3-141">All the properties will be returned in an actual call.</span></span>

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


