---
title: Get synchronizationSchema
description: Извлекает схему для заданного задания или шаблона синхронизации.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 9e91c0697c39c031f149477d7dbcac5a35679040
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132715"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="7889f-103">Get synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="7889f-103">Get synchronizationSchema</span></span>

<span data-ttu-id="7889f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7889f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7889f-105">Извлекает схему для заданного задания или шаблона синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7889f-105">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="7889f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7889f-106">Permissions</span></span>
<span data-ttu-id="7889f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7889f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7889f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7889f-109">Permission type</span></span>                        | <span data-ttu-id="7889f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7889f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7889f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7889f-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="7889f-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7889f-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="7889f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7889f-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="7889f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7889f-114">Not supported.</span></span> |
|<span data-ttu-id="7889f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7889f-115">Application</span></span>                            |<span data-ttu-id="7889f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7889f-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7889f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7889f-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="7889f-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7889f-118">Request headers</span></span>

| <span data-ttu-id="7889f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7889f-119">Name</span></span>           | <span data-ttu-id="7889f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7889f-120">Type</span></span>    | <span data-ttu-id="7889f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7889f-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="7889f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7889f-122">Authorization</span></span>  | <span data-ttu-id="7889f-123">string</span><span class="sxs-lookup"><span data-stu-id="7889f-123">string</span></span>  | <span data-ttu-id="7889f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7889f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7889f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7889f-126">Request body</span></span>

<span data-ttu-id="7889f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7889f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7889f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="7889f-128">Response</span></span>

<span data-ttu-id="7889f-129">В случае успеха этот метод возвращает код отклика и объект `200 OK` [synchronizationSchema](../resources/synchronization-synchronizationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7889f-129">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7889f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="7889f-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7889f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7889f-131">Request</span></span>
<span data-ttu-id="7889f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7889f-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7889f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7889f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="c"></a>[<span data-ttu-id="7889f-134">C#</span><span class="sxs-lookup"><span data-stu-id="7889f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7889f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7889f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7889f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7889f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7889f-137">Java</span><span class="sxs-lookup"><span data-stu-id="7889f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7889f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7889f-138">Response</span></span>
<span data-ttu-id="7889f-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7889f-139">The following is an example of a response.</span></span>

><span data-ttu-id="7889f-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7889f-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7889f-141">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7889f-141">All the properties will be returned in an actual call.</span></span>
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


