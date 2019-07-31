---
title: Получение Синчронизатионсчема
description: Получение схемы для данного задания или шаблона синхронизации.
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 55f6b6935808cd96bf9eebf8e2662d0649bbb66c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977673"
---
# <a name="get-synchronizationschema"></a><span data-ttu-id="e2672-103">Получение Синчронизатионсчема</span><span class="sxs-lookup"><span data-stu-id="e2672-103">Get synchronizationSchema</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2672-104">Получение схемы для данного задания или шаблона синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e2672-104">Retrieve the schema for a given synchronization job or template.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2672-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e2672-105">Permissions</span></span>
<span data-ttu-id="e2672-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2672-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2672-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2672-108">Permission type</span></span>                        | <span data-ttu-id="e2672-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2672-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2672-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2672-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="e2672-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2672-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="e2672-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2672-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="e2672-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2672-113">Not supported.</span></span> |
|<span data-ttu-id="e2672-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2672-114">Application</span></span>                            |<span data-ttu-id="e2672-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2672-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e2672-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2672-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
GET /servicePrincipals/{id}/synchronization/templates/{templateId}/schema
GET /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a><span data-ttu-id="e2672-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e2672-117">Request headers</span></span>

| <span data-ttu-id="e2672-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e2672-118">Name</span></span>           | <span data-ttu-id="e2672-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e2672-119">Type</span></span>    | <span data-ttu-id="e2672-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e2672-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="e2672-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2672-121">Authorization</span></span>  | <span data-ttu-id="e2672-122">string</span><span class="sxs-lookup"><span data-stu-id="e2672-122">string</span></span>  | <span data-ttu-id="e2672-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2672-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2672-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e2672-125">Request body</span></span>

<span data-ttu-id="e2672-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e2672-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2672-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2672-127">Response</span></span>

<span data-ttu-id="e2672-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [синчронизатионсчема](../resources/synchronization-synchronizationschema.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e2672-128">If successful, this method returns a `200 OK` response code and a [synchronizationSchema](../resources/synchronization-synchronizationschema.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2672-129">Пример</span><span class="sxs-lookup"><span data-stu-id="e2672-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e2672-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2672-130">Request</span></span>
<span data-ttu-id="e2672-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2672-131">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e2672-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2672-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e2672-133">C#</span><span class="sxs-lookup"><span data-stu-id="e2672-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-synchronizationschema-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e2672-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="e2672-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-synchronizationschema-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e2672-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e2672-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-synchronizationschema-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e2672-136">Java</span><span class="sxs-lookup"><span data-stu-id="e2672-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-synchronizationschema-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e2672-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2672-137">Response</span></span>
<span data-ttu-id="e2672-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e2672-138">The following is an example of a response.</span></span>

><span data-ttu-id="e2672-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e2672-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e2672-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2672-140">All the properties will be returned in an actual call.</span></span>
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
