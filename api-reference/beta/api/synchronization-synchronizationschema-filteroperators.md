---
title: 'Синчронизатионсчема: Филтероператорс'
description: Перечисление всех операторов, поддерживаемых в фильтрах областей видимости.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e6be1d3512168e01b4a98ffb486f9758a9901583
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621020"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="4b45a-103">Синчронизатионсчема: Филтероператорс</span><span class="sxs-lookup"><span data-stu-id="4b45a-103">synchronizationSchema: filterOperators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b45a-104">Перечисление всех операторов, поддерживаемых в [фильтрах областей видимости](../resources/synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="4b45a-104">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b45a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b45a-105">Permissions</span></span>
<span data-ttu-id="4b45a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b45a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b45a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b45a-108">Permission type</span></span>                        | <span data-ttu-id="4b45a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b45a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b45a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b45a-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="4b45a-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b45a-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4b45a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b45a-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4b45a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b45a-113">Not supported.</span></span>|
|<span data-ttu-id="4b45a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b45a-114">Application</span></span>                            |<span data-ttu-id="4b45a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b45a-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4b45a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b45a-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="4b45a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b45a-117">Request headers</span></span>

| <span data-ttu-id="4b45a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4b45a-118">Name</span></span>           | <span data-ttu-id="4b45a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4b45a-119">Type</span></span>    | <span data-ttu-id="4b45a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4b45a-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4b45a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b45a-121">Authorization</span></span>  | <span data-ttu-id="4b45a-122">string</span><span class="sxs-lookup"><span data-stu-id="4b45a-122">string</span></span>  | <span data-ttu-id="4b45a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b45a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b45a-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b45a-125">Request body</span></span>

<span data-ttu-id="4b45a-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4b45a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b45a-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b45a-127">Response</span></span>

<span data-ttu-id="4b45a-128">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и объект коллекции [филтероператорсчема](../resources/synchronization-filteroperatorschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b45a-128">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b45a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4b45a-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4b45a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b45a-130">Request</span></span>
<span data-ttu-id="4b45a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b45a-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4b45a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b45a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4b45a-133">C#</span><span class="sxs-lookup"><span data-stu-id="4b45a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-filteroperators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4b45a-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="4b45a-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-filteroperators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4b45a-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4b45a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-filteroperators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4b45a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b45a-136">Response</span></span>
<span data-ttu-id="4b45a-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b45a-137">The following is an example of a response.</span></span>

><span data-ttu-id="4b45a-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4b45a-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4b45a-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b45a-139">All the properties will be returned in an actual call.</span></span>

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
