---
title: 'synchronizationSchema: filterOperators'
description: Список всех операторы, поддерживаемые в области видимости фильтров.
localization_priority: Normal
ms.openlocfilehash: 68e0c9f583e92989213d1442aee1610b1495bae0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641710"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="98451-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="98451-103">synchronizationSchema: filterOperators</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98451-104">Список всех операторы, поддерживаемые в [области видимости фильтров](../resources/synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="98451-104">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="98451-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98451-105">Permissions</span></span>
<span data-ttu-id="98451-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98451-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98451-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98451-108">Permission type</span></span>                        | <span data-ttu-id="98451-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98451-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="98451-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98451-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="98451-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98451-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="98451-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98451-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="98451-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98451-113">Not supported.</span></span>|
|<span data-ttu-id="98451-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98451-114">Application</span></span>                            |<span data-ttu-id="98451-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98451-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="98451-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98451-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="98451-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98451-117">Request headers</span></span>

| <span data-ttu-id="98451-118">Имя</span><span class="sxs-lookup"><span data-stu-id="98451-118">Name</span></span>           | <span data-ttu-id="98451-119">Тип</span><span class="sxs-lookup"><span data-stu-id="98451-119">Type</span></span>    | <span data-ttu-id="98451-120">Описание</span><span class="sxs-lookup"><span data-stu-id="98451-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="98451-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="98451-121">Authorization</span></span>  | <span data-ttu-id="98451-122">строка</span><span class="sxs-lookup"><span data-stu-id="98451-122">string</span></span>  | <span data-ttu-id="98451-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98451-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98451-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98451-125">Request body</span></span>

<span data-ttu-id="98451-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98451-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98451-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="98451-127">Response</span></span>

<span data-ttu-id="98451-128">Успешно завершена, этот метод возвращает `200, OK` код ответа и объект коллекции [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="98451-128">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98451-129">Пример</span><span class="sxs-lookup"><span data-stu-id="98451-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="98451-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="98451-130">Request</span></span>
<span data-ttu-id="98451-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98451-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```

##### <a name="response"></a><span data-ttu-id="98451-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="98451-132">Response</span></span>
<span data-ttu-id="98451-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="98451-133">The following is an example of a response.</span></span>

><span data-ttu-id="98451-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="98451-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="98451-135">Будут возвращены все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="98451-135">All the properties will be returned in an actual call.</span></span>

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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-filteroperators.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
