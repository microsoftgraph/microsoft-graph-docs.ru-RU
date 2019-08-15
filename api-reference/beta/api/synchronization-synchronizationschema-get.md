---
title: Получение Синчронизатионсчема
description: Получение схемы для данного задания или шаблона синхронизации.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7f61f9dc96a68c8901ed6909126250a49e292c39
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409690"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="02191-103">Получение Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="02191-103">Get synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02191-104">Получение схемы для данного задания или шаблона синхронизации.</span><span class="sxs-lookup"><span data-stu-id="02191-104">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="02191-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02191-105">Permissions</span></span>
<span data-ttu-id="02191-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02191-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02191-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02191-108">Permission type</span></span>                        | <span data-ttu-id="02191-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02191-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="02191-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02191-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="02191-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02191-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="02191-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02191-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="02191-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02191-113">Not supported.</span></span> |
|<span data-ttu-id="02191-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02191-114">Application</span></span>                            |<span data-ttu-id="02191-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02191-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="02191-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02191-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="02191-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02191-117">Request headers</span></span>

| <span data-ttu-id="02191-118">Имя</span><span class="sxs-lookup"><span data-stu-id="02191-118">Name</span></span>           | <span data-ttu-id="02191-119">Тип</span><span class="sxs-lookup"><span data-stu-id="02191-119">Type</span></span>    | <span data-ttu-id="02191-120">Описание</span><span class="sxs-lookup"><span data-stu-id="02191-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="02191-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="02191-121">Authorization</span></span>  | <span data-ttu-id="02191-122">string</span><span class="sxs-lookup"><span data-stu-id="02191-122">string</span></span>  | <span data-ttu-id="02191-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02191-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02191-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="02191-125">Request body</span></span>

<span data-ttu-id="02191-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02191-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02191-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="02191-127">Response</span></span>

<span data-ttu-id="02191-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [синчронизатионсчема](../resources/synchronization-synchronizationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="02191-128">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02191-129">Пример</span><span class="sxs-lookup"><span data-stu-id="02191-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="02191-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="02191-130">Request</span></span>
<span data-ttu-id="02191-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02191-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="02191-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="02191-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="02191-133">C#</span><span class="sxs-lookup"><span data-stu-id="02191-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02191-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02191-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="02191-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="02191-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="02191-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="02191-136">Response</span></span>
<span data-ttu-id="02191-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="02191-137">The following is an example of a response.</span></span>

><span data-ttu-id="02191-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="02191-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="02191-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="02191-139">All the properties will be returned in an actual call.</span></span>
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
