---
title: 'synchronizationSchema: parseExpression'
description: '(.. / resources/synchronization_attributemappingsource.md) объекта. '
localization_priority: Normal
ms.openlocfilehash: dbde03b9ae85377801ad894c8b8ca22c6baebc85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811027"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="e6e04-103">synchronizationSchema: parseExpression</span><span class="sxs-lookup"><span data-stu-id="e6e04-103">synchronizationSchema: parseExpression</span></span>

> <span data-ttu-id="e6e04-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6e04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6e04-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6e04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6e04-106">Синтаксический анализ указанного строковое выражение в [attributeMappingSource | (.. / resources/synchronization_attributemappingsource.md) объекта.</span><span class="sxs-lookup"><span data-stu-id="e6e04-106">Parse a given string expression into an [attributeMappingSource|(../resources/synchronization_attributemappingsource.md) object.</span></span> 

<span data-ttu-id="e6e04-107">Дополнительные сведения о выражениях можно [Написании выражений для сопоставления атрибута в Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="e6e04-107">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="e6e04-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6e04-108">Permissions</span></span>
<span data-ttu-id="e6e04-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6e04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6e04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6e04-111">Permission type</span></span>                        | <span data-ttu-id="e6e04-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6e04-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6e04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6e04-113">Delegated (work or school account)</span></span>     |<span data-ttu-id="e6e04-114">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6e04-114">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e6e04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6e04-115">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e6e04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6e04-116">Not supported.</span></span>|
|<span data-ttu-id="e6e04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6e04-117">Application</span></span>                            |<span data-ttu-id="e6e04-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6e04-118">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="e6e04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6e04-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="e6e04-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6e04-120">Request headers</span></span>
| <span data-ttu-id="e6e04-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e6e04-121">Name</span></span>       | <span data-ttu-id="e6e04-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e6e04-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e6e04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6e04-123">Authorization</span></span>  | <span data-ttu-id="e6e04-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e6e04-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6e04-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6e04-125">Request body</span></span>
<span data-ttu-id="e6e04-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e6e04-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6e04-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="e6e04-127">Parameter</span></span>    | <span data-ttu-id="e6e04-128">Тип</span><span class="sxs-lookup"><span data-stu-id="e6e04-128">Type</span></span>   |<span data-ttu-id="e6e04-129">Описание</span><span class="sxs-lookup"><span data-stu-id="e6e04-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6e04-130">выражение</span><span class="sxs-lookup"><span data-stu-id="e6e04-130">expression</span></span>               |<span data-ttu-id="e6e04-131">Строка</span><span class="sxs-lookup"><span data-stu-id="e6e04-131">String</span></span>               |<span data-ttu-id="e6e04-132">Выражение для синтаксического разбора.</span><span class="sxs-lookup"><span data-stu-id="e6e04-132">Expression to parse.</span></span>|
|<span data-ttu-id="e6e04-133">testInputObject</span><span class="sxs-lookup"><span data-stu-id="e6e04-133">testInputObject</span></span>          |[<span data-ttu-id="e6e04-134">expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="e6e04-134">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="e6e04-135">Объект данных тестирования для оценки выражения.</span><span class="sxs-lookup"><span data-stu-id="e6e04-135">Test data object to evaluate expression against.</span></span> <span data-ttu-id="e6e04-136">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="e6e04-136">Optional.</span></span>|
|<span data-ttu-id="e6e04-137">targetAttributeDefinition</span><span class="sxs-lookup"><span data-stu-id="e6e04-137">targetAttributeDefinition</span></span>|[<span data-ttu-id="e6e04-138">attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="e6e04-138">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="e6e04-139">Определение атрибута, который будет сопоставлен с этого выражения.</span><span class="sxs-lookup"><span data-stu-id="e6e04-139">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="e6e04-140">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e6e04-140">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="e6e04-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6e04-141">Response</span></span>
<span data-ttu-id="e6e04-142">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e6e04-142">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6e04-143">Пример</span><span class="sxs-lookup"><span data-stu-id="e6e04-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e6e04-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6e04-144">Request</span></span>
<span data-ttu-id="e6e04-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6e04-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_parseexpression"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
Content-type: application/json

{
    "expression":"Replace([preferredLanguage], \"-\", , , \"_\", ,  )",
    "targetAttributeDefinition":null,
    "testInputObject": {
        definition: null,
        properties:[
            { key: "objectId", value : "66E4A8CC-1B7B-435E-95F8-F06CEA133828" },
            { key: "IsSoftDeleted", value: "false"},
            { key: "accountEnabled", value: "true"},
            { key: "streetAddress", value: "1 Redmond Way"},
            { key: "city", value: "Redmond"},
            { key: "state", value: "WA"},
            { key: "postalCode", value: "98052"},
            { key: "country", value: "USA"},
            { key: "department", value: "Sales"},
            { key: "displayName", value: "John Smith"},
            { key: "extensionAttribute1", value: "Sample 1"},
            { key: "extensionAttribute2", value: "Sample 2"},
            { key: "extensionAttribute3", value: "Sample 3"},
            { key: "extensionAttribute4", value: "Sample 4"},
            { key: "extensionAttribute5", value: "Sample 5"},
            { key: "extensionAttribute6", value: "Sample 6"},
            { key: "extensionAttribute7", value: "Sample 1"},
            { key: "extensionAttribute8", value: "Sample 1"},
            { key: "extensionAttribute9", value: "Sample 1"},
            { key: "extensionAttribute10", value: "Sample 1"},
            { key: "extensionAttribute11", value: "Sample 1"},
            { key: "extensionAttribute12", value: "Sample 1"},
            { key: "extensionAttribute13", value: "Sample 1"},
            { key: "extensionAttribute14", value: "Sample 1"},
            { key: "extensionAttribute15", value: "Sample 1"},
            { key: "givenName", value: "John"},
            { key: "jobTitle", value: "Finance manager"},
            { key: "mail", value: "johns@contoso.com"},
            { key: "mailNickname", value: "johns"},
            { key: "manager", value: "maxs@contoso.com"},
            { key: "mobile", value: "425-555-0010"},
            { key: "onPremisesSecurityIdentifier", value: "66E4A8CC-1B7B-435E-95F8-F06CEA133828"},
            { key: "passwordProfile.password", value: ""},
            { key: "physicalDeliveryOfficeName", value: "Main Office"},
            { key: "preferredLanguage", value: "EN-US"},
            { key: "proxyAddresses", value: ""},
            { key: "surname", value: "Smith"},
            { key: "telephoneNumber", value: "425-555-0011"},
            { key: "userPrincipalName", value: "johns@contoso.com"},
            { key: "appRoleAssignments", "value@odata.type":"#Collection(String)", value: ["Default Assignment"] }
        ]
    }
}
```

##### <a name="response"></a><span data-ttu-id="e6e04-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6e04-146">Response</span></span>
<span data-ttu-id="e6e04-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e6e04-147">The following is an example of the response.</span></span> 

><span data-ttu-id="e6e04-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6e04-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.parseExpressionResponse"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "error": null,
    "evaluationSucceeded": true,
    "evaluationResult": [
        "EN_US"
    ],
    "parsedExpression": {
        "expression": "Replace([preferredLanguage], \"-\", , , \"_\", , )",
        "name": "Replace",
        "parameters": [
            {
                "key": "source",
                "value": {
                    "expression": "[preferredLanguage]",
                    "name": "preferredLanguage",
                    "parameters": [],
                    "type": "Attribute"
                }
            },
            {
                "key": "Find",
                "value": {
                    "expression": "\"-\"",
                    "name": "-",
                    "parameters": [],
                    "type": "Constant"
                }
            },
            {
                "key": "Replacement",
                "value": {
                    "expression": "\"_\"",
                    "name": "_",
                    "parameters": [],
                    "type": "Constant"
                }
            }
        ],
        "type": "Function"
    },
    "parsingSucceeded": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: parseExpression",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
