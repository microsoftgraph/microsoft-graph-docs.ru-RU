---
title: 'synchronizationSchema: filterOperators'
description: Список всех операторы, поддерживаемые в области видимости фильтров.
ms.openlocfilehash: 968abf6584868b2b0b5e664c59f14eebc780f151
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077997"
---
# <a name="synchronizationschema-filteroperators"></a><span data-ttu-id="3d312-103">synchronizationSchema: filterOperators</span><span class="sxs-lookup"><span data-stu-id="3d312-103">synchronizationSchema: filterOperators</span></span>

> <span data-ttu-id="3d312-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3d312-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3d312-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d312-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3d312-106">Список всех операторы, поддерживаемые в [области видимости фильтров](../resources/synchronization-filter.md).</span><span class="sxs-lookup"><span data-stu-id="3d312-106">List all operators supported in the [scoping filters](../resources/synchronization-filter.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3d312-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d312-107">Permissions</span></span>
<span data-ttu-id="3d312-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d312-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d312-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d312-110">Permission type</span></span>                        | <span data-ttu-id="3d312-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d312-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d312-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d312-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="3d312-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d312-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3d312-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d312-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3d312-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d312-115">Not supported.</span></span>|
|<span data-ttu-id="3d312-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d312-116">Application</span></span>                            |<span data-ttu-id="3d312-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d312-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3d312-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d312-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/filterOperators
GET /applications/{id}/synchronization/templates/{templateId}/schema/filterOperators
```

## <a name="request-headers"></a><span data-ttu-id="3d312-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d312-119">Request headers</span></span>

| <span data-ttu-id="3d312-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3d312-120">Name</span></span>           | <span data-ttu-id="3d312-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3d312-121">Type</span></span>    | <span data-ttu-id="3d312-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3d312-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3d312-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d312-123">Authorization</span></span>  | <span data-ttu-id="3d312-124">string</span><span class="sxs-lookup"><span data-stu-id="3d312-124">string</span></span>  | <span data-ttu-id="3d312-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d312-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d312-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d312-127">Request body</span></span>

<span data-ttu-id="3d312-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d312-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d312-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d312-129">Response</span></span>

<span data-ttu-id="3d312-130">Успешно завершена, этот метод возвращает `200, OK` код ответа и объект коллекции [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3d312-130">If successful, this method returns a `200, OK` response code and a [filterOperatorSchema](../resources/synchronization-filteroperatorschema.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d312-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3d312-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3d312-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d312-132">Request</span></span>
<span data-ttu-id="3d312-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d312-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators
```

##### <a name="response"></a><span data-ttu-id="3d312-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="3d312-134">Response</span></span>
<span data-ttu-id="3d312-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3d312-135">The following is an example of a response.</span></span>

><span data-ttu-id="3d312-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3d312-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3d312-137">Будут возвращены все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="3d312-137">All the properties will be returned in an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: filterOperators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->