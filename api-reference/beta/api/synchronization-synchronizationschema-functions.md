---
title: 'synchronizationSchema: функции'
description: Список всех функций, в настоящее время поддерживаемых в attributeMappingSource.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 626ab146bf928691d846b4ffab209720be5b8f66
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132759"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="b5984-103">synchronizationSchema: функции</span><span class="sxs-lookup"><span data-stu-id="b5984-103">synchronizationSchema: functions</span></span>

<span data-ttu-id="b5984-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5984-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5984-105">Перечислить все функции, поддерживаемые в [attributeMappingSource.](../resources/synchronization-attributemappingsource.md)</span><span class="sxs-lookup"><span data-stu-id="b5984-105">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b5984-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5984-106">Permissions</span></span>
<span data-ttu-id="b5984-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5984-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5984-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5984-109">Permission type</span></span>                        | <span data-ttu-id="b5984-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5984-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5984-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5984-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="b5984-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5984-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b5984-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5984-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b5984-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5984-114">Not supported.</span></span>|
|<span data-ttu-id="b5984-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5984-115">Application</span></span>                            |<span data-ttu-id="b5984-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5984-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b5984-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5984-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="b5984-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b5984-118">Request headers</span></span>

| <span data-ttu-id="b5984-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b5984-119">Name</span></span>           | <span data-ttu-id="b5984-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b5984-120">Type</span></span>    | <span data-ttu-id="b5984-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b5984-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b5984-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5984-122">Authorization</span></span>  | <span data-ttu-id="b5984-123">string</span><span class="sxs-lookup"><span data-stu-id="b5984-123">string</span></span>  | <span data-ttu-id="b5984-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5984-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5984-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5984-126">Request body</span></span>

<span data-ttu-id="b5984-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5984-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5984-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5984-128">Response</span></span>

<span data-ttu-id="b5984-129">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b5984-129">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5984-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b5984-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b5984-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5984-131">Request</span></span>
<span data-ttu-id="b5984-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5984-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5984-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5984-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```
# <a name="c"></a>[<span data-ttu-id="b5984-134">C#</span><span class="sxs-lookup"><span data-stu-id="b5984-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/synchronizationschema-functions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5984-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5984-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/synchronizationschema-functions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5984-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5984-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/synchronizationschema-functions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5984-137">Java</span><span class="sxs-lookup"><span data-stu-id="b5984-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/synchronizationschema-functions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b5984-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5984-138">Response</span></span>
<span data-ttu-id="b5984-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b5984-139">The following is an example of a response.</span></span>

><span data-ttu-id="b5984-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b5984-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b5984-141">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b5984-141">All the properties will be returned in an actual call.</span></span>

<!--
{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#functions",
    "value": [
        {
            "name": "Append",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "suffix",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "DefaultDomain",
            "parameters": []
        },
        {
            "name": "AppRoleAssignments",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "FormatDateTime",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "inputFormat",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "outputFormat",
                    "required": true,
                    "type": "String"
                }
            ]
        }
    ]
}
```

<!--
Below is the full response, which had to be redacted above as Markdown Scanner tool trips over "type" values containing 
non-string type names like "Integer" or "Boolean"

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#functions",
    "value": [
        {
            "name": "Append",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "suffix",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "DefaultDomain",
            "parameters": []
        },
        {
            "name": "AppRoleAssignments",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "FormatDateTime",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "inputFormat",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "outputFormat",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "IsNothing",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "Boolean"
                }
            ]
        },
        {
            "name": "Join",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "separator",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": true,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Prepend",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "prefix",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Mid",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "start",
                    "required": true,
                    "type": "Integer"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "length",
                    "required": true,
                    "type": "Integer"
                }
            ]
        },
        {
            "name": "Not",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "Boolean"
                }
            ]
        },
        {
            "name": "Replace",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Find",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "RegularExpression",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "RegularExpressionGroupName",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Replacement",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "ReplacementPropertyName",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "Template",
                    "required": false,
                    "type": "String"
                }
            ]
        },
        {
            "name": "SingleAppRoleAssignment",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Split",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "delimiter",
                    "required": false,
                    "type": "String"
                }
            ]
        },
        {
            "name": "StripSpaces",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                }
            ]
        },
        {
            "name": "Switch",
            "parameters": [
                {
                    "allowMultipleOccurrences": false,
                    "name": "source",
                    "required": true,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": false,
                    "name": "defaultValue",
                    "required": false,
                    "type": "String"
                },
                {
                    "allowMultipleOccurrences": true,
                    "name": "switchValue",
                    "required": false,
                    "type": "String"
                }
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
  "description": "synchronizationSchema: functions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


