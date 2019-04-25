---
title: 'Синчронизатионсчема: Парсикспрессион'
description: '(.. Объект/ресаурцес/синчронизатион_аттрибутемаппингсаурце.МД). '
localization_priority: Normal
ms.openlocfilehash: 27545333c6ff7b3c9ffde3e1c59abd09465db1c2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545369"
---
# <a name="synchronizationschema-parseexpression"></a><span data-ttu-id="93f1e-103">Синчронизатионсчема: Парсикспрессион</span><span class="sxs-lookup"><span data-stu-id="93f1e-103">synchronizationSchema: parseExpression</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93f1e-104">ПроАнализируйте заданное строковое выражение в объект [Аттрибутемаппингсаурце | (.. Объект/ресаурцес/синчронизатион_аттрибутемаппингсаурце.МД).</span><span class="sxs-lookup"><span data-stu-id="93f1e-104">Parse a given string expression into an [attributeMappingSource|(../resources/synchronization_attributemappingsource.md) object.</span></span> 

<span data-ttu-id="93f1e-105">Более подробную информацию о выражениях можно узнать [в статье Создание выражений для СопоставленИй атрибутов в Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="93f1e-105">For more information about expressions, see [Writing Expressions for Attribute Mappings in Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-writing-expressions-for-attribute-mappings).</span></span>

## <a name="permissions"></a><span data-ttu-id="93f1e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93f1e-106">Permissions</span></span>
<span data-ttu-id="93f1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93f1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93f1e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93f1e-109">Permission type</span></span>                        | <span data-ttu-id="93f1e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93f1e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="93f1e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93f1e-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="93f1e-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93f1e-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="93f1e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93f1e-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="93f1e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93f1e-114">Not supported.</span></span>|
|<span data-ttu-id="93f1e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93f1e-115">Application</span></span>                            |<span data-ttu-id="93f1e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93f1e-116">Not supported.</span></span>| 

## <a name="http-request"></a><span data-ttu-id="93f1e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93f1e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/synchronization/jobs/{id}/schema/parseExpression
POST /servicePrincipals/{id}/synchronization/templates/{id}/schema/parseExpression

```
## <a name="request-headers"></a><span data-ttu-id="93f1e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93f1e-118">Request headers</span></span>
| <span data-ttu-id="93f1e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="93f1e-119">Name</span></span>       | <span data-ttu-id="93f1e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="93f1e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="93f1e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93f1e-121">Authorization</span></span>  | <span data-ttu-id="93f1e-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="93f1e-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="93f1e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="93f1e-123">Request body</span></span>
<span data-ttu-id="93f1e-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="93f1e-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="93f1e-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="93f1e-125">Parameter</span></span>    | <span data-ttu-id="93f1e-126">Тип</span><span class="sxs-lookup"><span data-stu-id="93f1e-126">Type</span></span>   |<span data-ttu-id="93f1e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="93f1e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93f1e-128">выражение</span><span class="sxs-lookup"><span data-stu-id="93f1e-128">expression</span></span>               |<span data-ttu-id="93f1e-129">String</span><span class="sxs-lookup"><span data-stu-id="93f1e-129">String</span></span>               |<span data-ttu-id="93f1e-130">Выражение для синтаксического анализа.</span><span class="sxs-lookup"><span data-stu-id="93f1e-130">Expression to parse.</span></span>|
|<span data-ttu-id="93f1e-131">Тестинпутобжект</span><span class="sxs-lookup"><span data-stu-id="93f1e-131">testInputObject</span></span>          |[<span data-ttu-id="93f1e-132">Експрессионинпутобжект</span><span class="sxs-lookup"><span data-stu-id="93f1e-132">expressionInputObject</span></span>](../resources/synchronization-expressioninputobject.md)|<span data-ttu-id="93f1e-133">Тестовый объект данных, с которым вычисляется выражение.</span><span class="sxs-lookup"><span data-stu-id="93f1e-133">Test data object to evaluate expression against.</span></span> <span data-ttu-id="93f1e-134">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="93f1e-134">Optional.</span></span>|
|<span data-ttu-id="93f1e-135">Таржетаттрибутедефинитион</span><span class="sxs-lookup"><span data-stu-id="93f1e-135">targetAttributeDefinition</span></span>|[<span data-ttu-id="93f1e-136">Аттрибутедефинитион</span><span class="sxs-lookup"><span data-stu-id="93f1e-136">attributeDefinition</span></span>](../resources/synchronization-attributedefinition.md) |<span data-ttu-id="93f1e-137">Определение атрибута, который будет сопоставлен с этим выражением.</span><span class="sxs-lookup"><span data-stu-id="93f1e-137">Definition of the attribute that will be mapped to this expression.</span></span> <span data-ttu-id="93f1e-138">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="93f1e-138">Optional.</span></span>|

## <a name="response"></a><span data-ttu-id="93f1e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="93f1e-139">Response</span></span>
<span data-ttu-id="93f1e-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [парсикспрессионреспонсе](../resources/synchronization-parseexpressionresponse.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93f1e-140">If successful, this method returns a `200 OK` response code and a [parseExpressionResponse](../resources/synchronization-parseexpressionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93f1e-141">Пример</span><span class="sxs-lookup"><span data-stu-id="93f1e-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="93f1e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="93f1e-142">Request</span></span>
<span data-ttu-id="93f1e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93f1e-143">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="93f1e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="93f1e-144">Response</span></span>
<span data-ttu-id="93f1e-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="93f1e-145">The following is an example of the response.</span></span> 

><span data-ttu-id="93f1e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93f1e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-parseexpression.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
