---
title: Получить синхронизациюSchema
description: Извлечение схемы для данного задания синхронизации или шаблона.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 84c1dc9112851330be721f425a01228d278d014b
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50625971"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="3eb15-103">Получить синхронизациюSchema</span><span class="sxs-lookup"><span data-stu-id="3eb15-103">Get synchronizationSchema</span></span>

<span data-ttu-id="3eb15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3eb15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3eb15-105">Извлечение схемы для данного задания синхронизации или шаблона.</span><span class="sxs-lookup"><span data-stu-id="3eb15-105">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="3eb15-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3eb15-106">Permissions</span></span>
<span data-ttu-id="3eb15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eb15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eb15-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3eb15-109">Permission type</span></span>                        | <span data-ttu-id="3eb15-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3eb15-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eb15-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3eb15-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="3eb15-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3eb15-112">Directory.Read.All</span></span>  |
|<span data-ttu-id="3eb15-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3eb15-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="3eb15-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3eb15-114">Not supported.</span></span> |
|<span data-ttu-id="3eb15-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3eb15-115">Application</span></span>                            |<span data-ttu-id="3eb15-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb15-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3eb15-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3eb15-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="3eb15-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3eb15-118">Request headers</span></span>

| <span data-ttu-id="3eb15-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3eb15-119">Name</span></span>           | <span data-ttu-id="3eb15-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3eb15-120">Type</span></span>    | <span data-ttu-id="3eb15-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3eb15-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="3eb15-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eb15-122">Authorization</span></span>  | <span data-ttu-id="3eb15-123">string</span><span class="sxs-lookup"><span data-stu-id="3eb15-123">string</span></span>  | <span data-ttu-id="3eb15-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3eb15-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3eb15-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3eb15-126">Request body</span></span>

<span data-ttu-id="3eb15-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3eb15-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3eb15-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eb15-128">Response</span></span>

<span data-ttu-id="3eb15-129">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [синхронизацииSchema](../resources/synchronization-synchronizationschema.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3eb15-129">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eb15-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3eb15-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3eb15-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3eb15-131">Request</span></span>
<span data-ttu-id="3eb15-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3eb15-132">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3eb15-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3eb15-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="c"></a>[<span data-ttu-id="3eb15-134">C#</span><span class="sxs-lookup"><span data-stu-id="3eb15-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3eb15-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3eb15-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3eb15-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3eb15-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3eb15-137">Java</span><span class="sxs-lookup"><span data-stu-id="3eb15-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3eb15-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3eb15-138">Response</span></span>
<span data-ttu-id="3eb15-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3eb15-139">The following is an example of a response.</span></span>

><span data-ttu-id="3eb15-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3eb15-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3eb15-141">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3eb15-141">All the properties will be returned in an actual call.</span></span>
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


