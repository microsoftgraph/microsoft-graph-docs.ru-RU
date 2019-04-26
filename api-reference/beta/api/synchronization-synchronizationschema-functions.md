---
title: 'Синчронизатионсчема: функции'
description: ПереЧисление всех функций, которые в настоящее время поддерживаются в Аттрибутемаппингсаурце.
localization_priority: Normal
ms.openlocfilehash: d5b24f77e61011d6c5a8bc7652c3c4ff168d2e1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33330588"
---
# <a name="synchronizationschema-functions"></a><span data-ttu-id="83fa9-103">Синчронизатионсчема: функции</span><span class="sxs-lookup"><span data-stu-id="83fa9-103">synchronizationSchema: functions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83fa9-104">ПереЧисление всех функций, которые в настоящее время поддерживаются в [аттрибутемаппингсаурце](../resources/synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="83fa9-104">List all the functions currently supported in the [attributeMappingSource](../resources/synchronization-attributemappingsource.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83fa9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83fa9-105">Permissions</span></span>
<span data-ttu-id="83fa9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83fa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83fa9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83fa9-108">Permission type</span></span>                        | <span data-ttu-id="83fa9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="83fa9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="83fa9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83fa9-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="83fa9-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83fa9-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="83fa9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83fa9-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="83fa9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83fa9-113">Not supported.</span></span>|
|<span data-ttu-id="83fa9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83fa9-114">Application</span></span>                            |<span data-ttu-id="83fa9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83fa9-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="83fa9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83fa9-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema/functions
GET /applications/{id}/synchronization/templates/{templateId}/schema/functions
```

## <a name="request-headers"></a><span data-ttu-id="83fa9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83fa9-117">Request headers</span></span>

| <span data-ttu-id="83fa9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="83fa9-118">Name</span></span>           | <span data-ttu-id="83fa9-119">Тип</span><span class="sxs-lookup"><span data-stu-id="83fa9-119">Type</span></span>    | <span data-ttu-id="83fa9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="83fa9-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="83fa9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83fa9-121">Authorization</span></span>  | <span data-ttu-id="83fa9-122">string</span><span class="sxs-lookup"><span data-stu-id="83fa9-122">string</span></span>  | <span data-ttu-id="83fa9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83fa9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="83fa9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83fa9-125">Request body</span></span>

<span data-ttu-id="83fa9-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="83fa9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83fa9-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="83fa9-127">Response</span></span>

<span data-ttu-id="83fa9-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [аттрибутемаппингфунктионсчема](../resources/synchronization-attributemappingfunctionschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83fa9-128">If successful, this method returns a `200 OK` response code and a collection of [attributemappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83fa9-129">Пример</span><span class="sxs-lookup"><span data-stu-id="83fa9-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="83fa9-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="83fa9-130">Request</span></span>
<span data-ttu-id="83fa9-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83fa9-131">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_functions"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions
```

##### <a name="response"></a><span data-ttu-id="83fa9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="83fa9-132">Response</span></span>
<span data-ttu-id="83fa9-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="83fa9-133">The following is an example of a response.</span></span>

><span data-ttu-id="83fa9-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="83fa9-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="83fa9-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83fa9-135">All the properties will be returned in an actual call.</span></span>

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
  "suppressions": []
}
-->
