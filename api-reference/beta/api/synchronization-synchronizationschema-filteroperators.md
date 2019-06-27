---
title: 'Синчронизатионсчема: Филтероператорс'
description: Перечисление всех операторов, поддерживаемых в фильтрах областей видимости.
localization_priority: Normal
ms.openlocfilehash: 526b2de933c113462d9c4b7cc4a5168e16a11010
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271304"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="b58e4-103">Синчронизатионсчема: Филтероператорс</span><span class="sxs-lookup"><span data-stu-id="b58e4-103">synchronizationSchema: filterOperators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b58e4-104">Перечисление всех операторов, поддерживаемых в [фильтрах областей видимости](../resources/synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="b58e4-104">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b58e4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b58e4-105">Permissions</span></span>
<span data-ttu-id="b58e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b58e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b58e4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b58e4-108">Permission type</span></span>                        | <span data-ttu-id="b58e4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b58e4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b58e4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b58e4-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="b58e4-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b58e4-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b58e4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b58e4-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b58e4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b58e4-113">Not supported.</span></span>|
|<span data-ttu-id="b58e4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b58e4-114">Application</span></span>                            |<span data-ttu-id="b58e4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b58e4-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b58e4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b58e4-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="b58e4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b58e4-117">Request headers</span></span>

| <span data-ttu-id="b58e4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b58e4-118">Name</span></span>           | <span data-ttu-id="b58e4-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b58e4-119">Type</span></span>    | <span data-ttu-id="b58e4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b58e4-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b58e4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b58e4-121">Authorization</span></span>  | <span data-ttu-id="b58e4-122">string</span><span class="sxs-lookup"><span data-stu-id="b58e4-122">string</span></span>  | <span data-ttu-id="b58e4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b58e4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b58e4-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b58e4-125">Request body</span></span>

<span data-ttu-id="b58e4-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b58e4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b58e4-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="b58e4-127">Response</span></span>

<span data-ttu-id="b58e4-128">В случае успешного выполнения этот метод возвращает `200, OK` код отклика и объект коллекции [филтероператорсчема](../resources/synchronization-filteroperatorschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b58e4-128">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b58e4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b58e4-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b58e4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b58e4-130">Request</span></span>
<span data-ttu-id="b58e4-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b58e4-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```

##### <a name="response"></a><span data-ttu-id="b58e4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b58e4-132">Response</span></span>
<span data-ttu-id="b58e4-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b58e4-133">The following is an example of a response.</span></span>

><span data-ttu-id="b58e4-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b58e4-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b58e4-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b58e4-135">All the properties will be returned in an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b58e4-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b58e4-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b58e4-137">C#</span><span class="sxs-lookup"><span data-stu-id="b58e4-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/synchronizationschema_filteroperators-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b58e4-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="b58e4-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/synchronizationschema_filteroperators-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b58e4-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b58e4-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/synchronizationschema_filteroperators-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-filteroperators.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-filteroperators.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-filteroperators.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: synchronizationschema_filteroperators/container/arity:\r\n       Expected type String but actual was Binary. Property: arity, actual value: 'Binary'"
  ]
}
-->
