---
title: Получить синхронизациюSchema
description: Извлечение схемы для данного задания синхронизации или шаблона.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: bd321f3375623914afa6cc9c803b18e2a22d1ed4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952954"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="e8af8-103">Получить синхронизациюSchema</span><span class="sxs-lookup"><span data-stu-id="e8af8-103">Get synchronizationSchema</span></span>

<span data-ttu-id="e8af8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8af8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8af8-105">Извлечение схемы для данного задания синхронизации или шаблона.</span><span class="sxs-lookup"><span data-stu-id="e8af8-105">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8af8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8af8-106">Permissions</span></span>
<span data-ttu-id="e8af8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8af8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8af8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8af8-109">Permission type</span></span>                        | <span data-ttu-id="e8af8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8af8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8af8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8af8-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="e8af8-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8af8-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="e8af8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8af8-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e8af8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8af8-114">Not supported.</span></span> |
|<span data-ttu-id="e8af8-115">Application</span><span class="sxs-lookup"><span data-stu-id="e8af8-115">Application</span></span>                            |<span data-ttu-id="e8af8-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8af8-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e8af8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8af8-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="e8af8-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e8af8-118">Request headers</span></span>

| <span data-ttu-id="e8af8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e8af8-119">Name</span></span>           | <span data-ttu-id="e8af8-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e8af8-120">Type</span></span>    | <span data-ttu-id="e8af8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e8af8-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e8af8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8af8-122">Authorization</span></span>  | <span data-ttu-id="e8af8-123">string</span><span class="sxs-lookup"><span data-stu-id="e8af8-123">string</span></span>  | <span data-ttu-id="e8af8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8af8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8af8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8af8-126">Request body</span></span>

<span data-ttu-id="e8af8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8af8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8af8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8af8-128">Response</span></span>

<span data-ttu-id="e8af8-129">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [синхронизацииSchema](../resources/synchronization-synchronizationschema.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e8af8-129">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8af8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e8af8-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e8af8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8af8-131">Request</span></span>
<span data-ttu-id="e8af8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8af8-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8af8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8af8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="c"></a>[<span data-ttu-id="e8af8-134">C#</span><span class="sxs-lookup"><span data-stu-id="e8af8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8af8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8af8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8af8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8af8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8af8-137">Java</span><span class="sxs-lookup"><span data-stu-id="e8af8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e8af8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8af8-138">Response</span></span>
<span data-ttu-id="e8af8-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e8af8-139">The following is an example of a response.</span></span>

><span data-ttu-id="e8af8-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e8af8-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e8af8-141">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e8af8-141">All the properties will be returned in an actual call.</span></span>
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


