---
title: Получение Синчронизатионсчема
description: Получение схемы для данного задания или шаблона синхронизации.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c41028059a032479e6cc1b23ffb20b81665792b7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722260"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="b718d-103">Получение Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="b718d-103">Get synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b718d-104">Получение схемы для данного задания или шаблона синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b718d-104">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="b718d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b718d-105">Permissions</span></span>
<span data-ttu-id="b718d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b718d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b718d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b718d-108">Permission type</span></span>                        | <span data-ttu-id="b718d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b718d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="b718d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b718d-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="b718d-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b718d-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="b718d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b718d-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="b718d-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b718d-113">Not supported.</span></span> |
|<span data-ttu-id="b718d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b718d-114">Application</span></span>                            |<span data-ttu-id="b718d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b718d-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b718d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b718d-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="b718d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b718d-117">Request headers</span></span>

| <span data-ttu-id="b718d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b718d-118">Name</span></span>           | <span data-ttu-id="b718d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b718d-119">Type</span></span>    | <span data-ttu-id="b718d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b718d-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="b718d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b718d-121">Authorization</span></span>  | <span data-ttu-id="b718d-122">string</span><span class="sxs-lookup"><span data-stu-id="b718d-122">string</span></span>  | <span data-ttu-id="b718d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b718d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b718d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b718d-125">Request body</span></span>

<span data-ttu-id="b718d-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b718d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b718d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b718d-127">Response</span></span>

<span data-ttu-id="b718d-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [синчронизатионсчема](../resources/synchronization-synchronizationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b718d-128">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b718d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b718d-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b718d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b718d-130">Request</span></span>
<span data-ttu-id="b718d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b718d-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b718d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b718d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b718d-133">C#</span><span class="sxs-lookup"><span data-stu-id="b718d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b718d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b718d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b718d-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b718d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b718d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b718d-136">Response</span></span>
<span data-ttu-id="b718d-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b718d-137">The following is an example of a response.</span></span>

><span data-ttu-id="b718d-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b718d-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b718d-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b718d-139">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

{
    "directories": [
        {
            "name": "Azure Active Directory",
            "objects": [
                {
                    "name": "User",
                    "attributes": [
                        {
                            "name": "userPrincipalName",
                            "type": "string"
                        }
                    ]
                }
            ]
        },
        {
            "name": "Salesforce",
            "objects": [{}]
        }
    ],
    "synchronizationRules":[
        {
            "name": "USER_TO_USER",
            "sourceDirectoryName": "Azure Active Directory",
            "targetDirectoryName": "Salesforce",
            "objectMappings": [
                {
                    "sourceObjectName": "User",
                    "targetObjectName": "User",
                    "attributeMappings": [
                        {
                            "source": {},
                            "targetAttributeName": "userName"
                        },
                        {}
                    ]
                },
                {}
            ]
        },
        {}
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
