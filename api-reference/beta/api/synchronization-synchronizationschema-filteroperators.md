---
title: 'Синчронизатионсчема: Филтероператорс'
description: Перечисление всех операторов, поддерживаемых в фильтрах областей видимости.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b80c14879cb04f615d4feafaece48166f56b1a7f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443016"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="7e72e-103">Синчронизатионсчема: Филтероператорс</span><span class="sxs-lookup"><span data-stu-id="7e72e-103">synchronizationSchema: filterOperators</span></span>

<span data-ttu-id="7e72e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e72e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e72e-105">Перечисление всех операторов, поддерживаемых в [фильтрах областей видимости](../resources/synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="7e72e-105">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e72e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7e72e-106">Permissions</span></span>
<span data-ttu-id="7e72e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e72e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e72e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7e72e-109">Permission type</span></span>                        | <span data-ttu-id="7e72e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7e72e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e72e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7e72e-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="7e72e-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e72e-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7e72e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7e72e-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7e72e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e72e-114">Not supported.</span></span>|
|<span data-ttu-id="7e72e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7e72e-115">Application</span></span>                            |<span data-ttu-id="7e72e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7e72e-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7e72e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7e72e-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="7e72e-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7e72e-118">Request headers</span></span>

| <span data-ttu-id="7e72e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7e72e-119">Name</span></span>           | <span data-ttu-id="7e72e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7e72e-120">Type</span></span>    | <span data-ttu-id="7e72e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7e72e-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7e72e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e72e-122">Authorization</span></span>  | <span data-ttu-id="7e72e-123">string</span><span class="sxs-lookup"><span data-stu-id="7e72e-123">string</span></span>  | <span data-ttu-id="7e72e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7e72e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e72e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7e72e-126">Request body</span></span>

<span data-ttu-id="7e72e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7e72e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e72e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="7e72e-128">Response</span></span>

<span data-ttu-id="7e72e-129">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и объект коллекции [филтероператорсчема](../resources/synchronization-filteroperatorschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7e72e-129">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e72e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7e72e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7e72e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7e72e-131">Request</span></span>
<span data-ttu-id="7e72e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7e72e-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e72e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e72e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```
# <a name="c"></a>[<span data-ttu-id="7e72e-134">C#</span><span class="sxs-lookup"><span data-stu-id="7e72e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-filteroperators-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e72e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e72e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-filteroperators-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e72e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e72e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-filteroperators-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7e72e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7e72e-137">Response</span></span>
<span data-ttu-id="7e72e-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7e72e-138">The following is an example of a response.</span></span>

><span data-ttu-id="7e72e-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7e72e-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7e72e-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7e72e-140">All the properties will be returned in an actual call.</span></span>

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
