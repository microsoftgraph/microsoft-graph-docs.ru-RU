---
title: 'синхронизацияSchema: parseExpression'
description: '(.. /resources/synchronization_attributemappingsource.md) объекта. '
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d7f8ec86ae12f7aa1c6ae9620d7dbfb0f41aeebc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049718"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="4c897-103">синхронизацияSchema: parseExpression</span><span class="sxs-lookup"><span data-stu-id="4c897-103">synchronizationSchema: parseExpression</span></span>

<span data-ttu-id="4c897-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c897-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c897-105">Размыть заданное выражение строки в [объект attributeMappingSource.](../resources/synchronization-attributemappingsource.md)</span><span class="sxs-lookup"><span data-stu-id="4c897-105">Parse a given string expression into an [attributeMappingSource](../resources/synchronization-attributemappingsource.md) object.</span></span>

<span data-ttu-id="4c897-106">Дополнительные сведения о выражениях см. в [статьи Writing Expressions for Attribute Mappings in Azure Active Directory.](/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings)</span><span class="sxs-lookup"><span data-stu-id="4c897-106">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c897-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c897-107">Permissions</span></span>
<span data-ttu-id="4c897-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c897-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c897-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c897-110">Permission type</span></span>                        | <span data-ttu-id="4c897-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c897-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c897-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c897-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="4c897-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c897-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4c897-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c897-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4c897-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c897-115">Not supported.</span></span>|
|<span data-ttu-id="4c897-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4c897-116">Application</span></span>                            |<span data-ttu-id="4c897-117">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c897-117">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c897-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c897-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="4c897-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c897-119">Request headers</span></span>
| <span data-ttu-id="4c897-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4c897-120">Name</span></span>       | <span data-ttu-id="4c897-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4c897-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4c897-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c897-122">Authorization</span></span>  | <span data-ttu-id="4c897-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4c897-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c897-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c897-124">Request body</span></span>
<span data-ttu-id="4c897-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4c897-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4c897-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="4c897-126">Parameter</span></span>    | <span data-ttu-id="4c897-127">Тип</span><span class="sxs-lookup"><span data-stu-id="4c897-127">Type</span></span>   |<span data-ttu-id="4c897-128">Описание</span><span class="sxs-lookup"><span data-stu-id="4c897-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c897-129">выражение</span><span class="sxs-lookup"><span data-stu-id="4c897-129">expression</span></span>               |<span data-ttu-id="4c897-130">String</span><span class="sxs-lookup"><span data-stu-id="4c897-130">String</span></span>               |<span data-ttu-id="4c897-131">Выражение для размыкать.</span><span class="sxs-lookup"><span data-stu-id="4c897-131">Expression to parse.</span></span>|
|<span data-ttu-id="4c897-132">testInputObject</span><span class="sxs-lookup"><span data-stu-id="4c897-132">testInputObject</span></span>          |[<span data-ttu-id="4c897-133">expressionInputObject</span><span class="sxs-lookup"><span data-stu-id="4c897-133">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="4c897-134">Протестировать объект данных для оценки выражений.</span><span class="sxs-lookup"><span data-stu-id="4c897-134">Test data object to evaluate expression against.</span></span> <span data-ttu-id="4c897-135">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4c897-135">Optional.</span></span>|
|<span data-ttu-id="4c897-136">targetAttributeDefinition</span><span class="sxs-lookup"><span data-stu-id="4c897-136">targetAttributeDefinition</span></span>|[<span data-ttu-id="4c897-137">attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="4c897-137">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="4c897-138">Определение атрибута, который будет относяться к этому выражению.</span><span class="sxs-lookup"><span data-stu-id="4c897-138">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="4c897-139">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4c897-139">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="4c897-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c897-140">Response</span></span>
<span data-ttu-id="4c897-141">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4c897-141">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c897-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4c897-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4c897-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c897-143">Request</span></span>
<span data-ttu-id="4c897-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c897-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c897-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c897-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4c897-146">C#</span><span class="sxs-lookup"><span data-stu-id="4c897-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-parseexpression-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c897-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c897-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-parseexpression-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c897-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c897-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-parseexpression-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4c897-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c897-149">Response</span></span>
<span data-ttu-id="4c897-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4c897-150">The following is an example of the response.</span></span>

><span data-ttu-id="4c897-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4c897-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSchema: parseExpression",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


