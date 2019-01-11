---
title: 'synchronizationSchema: функций'
description: Список всех функций, поддерживаемые в настоящее время в attributeMappingSource.
localization_priority: Normal
ms.openlocfilehash: 5dc7734e9d747ac1e832aebb7d9c7355c2fbb52f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841010"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="3a3cf-103">synchronizationSchema: функций</span><span class="sxs-lookup"><span data-stu-id="3a3cf-103">synchronizationSchema: functions</span></span>

> <span data-ttu-id="3a3cf-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3a3cf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a3cf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a3cf-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a3cf-106">Список всех функций, поддерживаемые в настоящее время в [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="3a3cf-106">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3a3cf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a3cf-107">Permissions</span></span>
<span data-ttu-id="3a3cf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a3cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a3cf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a3cf-110">Permission type</span></span>                        | <span data-ttu-id="3a3cf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a3cf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a3cf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a3cf-112">Delegated (work or school account)</span></span>     |<span data-ttu-id="3a3cf-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a3cf-113">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="3a3cf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a3cf-114">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3a3cf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a3cf-115">Not supported.</span></span>|
|<span data-ttu-id="3a3cf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a3cf-116">Application</span></span>                            |<span data-ttu-id="3a3cf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a3cf-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3a3cf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a3cf-118">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="3a3cf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a3cf-119">Request headers</span></span>

| <span data-ttu-id="3a3cf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="3a3cf-120">Name</span></span>           | <span data-ttu-id="3a3cf-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3a3cf-121">Type</span></span>    | <span data-ttu-id="3a3cf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3a3cf-122">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3a3cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a3cf-123">Authorization</span></span>  | <span data-ttu-id="3a3cf-124">string</span><span class="sxs-lookup"><span data-stu-id="3a3cf-124">string</span></span>  | <span data-ttu-id="3a3cf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a3cf-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a3cf-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3a3cf-127">Request body</span></span>

<span data-ttu-id="3a3cf-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a3cf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a3cf-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a3cf-129">Response</span></span>

<span data-ttu-id="3a3cf-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3a3cf-130">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a3cf-131">Пример</span><span class="sxs-lookup"><span data-stu-id="3a3cf-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3a3cf-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a3cf-132">Request</span></span>
<span data-ttu-id="3a3cf-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a3cf-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```

##### <a name="response"></a><span data-ttu-id="3a3cf-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="3a3cf-134">Response</span></span>
<span data-ttu-id="3a3cf-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3a3cf-135">The following is an example of a response.</span></span>

><span data-ttu-id="3a3cf-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3a3cf-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3a3cf-137">Будут возвращены все свойства в фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="3a3cf-137">All the properties will be returned in an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: functions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
