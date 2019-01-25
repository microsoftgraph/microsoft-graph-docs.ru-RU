---
title: 'synchronizationSchema: функций'
description: Список всех функций, поддерживаемые в настоящее время в attributeMappingSource.
localization_priority: Normal
ms.openlocfilehash: edfdb169f9945759e062cf2c57d5f6f3b4c22f2e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523416"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="16cb4-103">synchronizationSchema: функций</span><span class="sxs-lookup"><span data-stu-id="16cb4-103">synchronizationSchema: functions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16cb4-104">Список всех функций, поддерживаемые в настоящее время в [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="16cb4-104">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="16cb4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16cb4-105">Permissions</span></span>
<span data-ttu-id="16cb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16cb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16cb4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16cb4-108">Permission type</span></span>                        | <span data-ttu-id="16cb4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16cb4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="16cb4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16cb4-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="16cb4-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16cb4-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="16cb4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16cb4-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="16cb4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16cb4-113">Not supported.</span></span>|
|<span data-ttu-id="16cb4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="16cb4-114">Application</span></span>                            |<span data-ttu-id="16cb4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16cb4-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="16cb4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16cb4-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="16cb4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16cb4-117">Request headers</span></span>

| <span data-ttu-id="16cb4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="16cb4-118">Name</span></span>           | <span data-ttu-id="16cb4-119">Тип</span><span class="sxs-lookup"><span data-stu-id="16cb4-119">Type</span></span>    | <span data-ttu-id="16cb4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="16cb4-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="16cb4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="16cb4-121">Authorization</span></span>  | <span data-ttu-id="16cb4-122">string</span><span class="sxs-lookup"><span data-stu-id="16cb4-122">string</span></span>  | <span data-ttu-id="16cb4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16cb4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16cb4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16cb4-125">Request body</span></span>

<span data-ttu-id="16cb4-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16cb4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16cb4-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="16cb4-127">Response</span></span>

<span data-ttu-id="16cb4-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="16cb4-128">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16cb4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="16cb4-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="16cb4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="16cb4-130">Request</span></span>
<span data-ttu-id="16cb4-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16cb4-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```

##### <a name="response"></a><span data-ttu-id="16cb4-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="16cb4-132">Response</span></span>
<span data-ttu-id="16cb4-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="16cb4-133">The following is an example of a response.</span></span>

><span data-ttu-id="16cb4-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="16cb4-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="16cb4-135">Будут возвращены все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="16cb4-135">All the properties will be returned in an actual call.</span></span>

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
    "Error: /api-reference/beta/api/synchronization-synchronizationschema-functions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
