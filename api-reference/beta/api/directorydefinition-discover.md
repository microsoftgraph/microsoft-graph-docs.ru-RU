---
title: 'directoryDefinition: откройте для себя'
description: 'Откройте для себя последнее определение схемы для предварительной разработки приложения. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 0f4d5a26128c78dca1245f5b8c15f6a446e4296a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046890"
---
# <a name="directorydefinition-discover"></a><span data-ttu-id="0acfe-103">directoryDefinition: откройте для себя</span><span class="sxs-lookup"><span data-stu-id="0acfe-103">directoryDefinition: discover</span></span>

<span data-ttu-id="0acfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0acfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0acfe-105">Откройте для себя последнее определение схемы для предварительной разработки приложения.</span><span class="sxs-lookup"><span data-stu-id="0acfe-105">Discover the latest schema definition for provisioning to an application.</span></span> 

## <a name="permissions"></a><span data-ttu-id="0acfe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0acfe-106">Permissions</span></span>

<span data-ttu-id="0acfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0acfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0acfe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0acfe-109">Permission type</span></span>                        | <span data-ttu-id="0acfe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0acfe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="0acfe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0acfe-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="0acfe-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0acfe-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="0acfe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0acfe-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="0acfe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0acfe-114">Not supported.</span></span>|
|<span data-ttu-id="0acfe-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0acfe-115">Application</span></span>                            |<span data-ttu-id="0acfe-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0acfe-116">Application.ReadWrite.OwnedBy, Directory.ReadWrite.All</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="0acfe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0acfe-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

## <a name="request-headers"></a><span data-ttu-id="0acfe-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0acfe-118">Request headers</span></span>

| <span data-ttu-id="0acfe-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0acfe-119">Header</span></span>        | <span data-ttu-id="0acfe-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0acfe-120">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="0acfe-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0acfe-121">Authorization</span></span> | <span data-ttu-id="0acfe-122">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="0acfe-122">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0acfe-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0acfe-123">Request body</span></span>

<span data-ttu-id="0acfe-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0acfe-124">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="0acfe-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="0acfe-125">Response</span></span>

<span data-ttu-id="0acfe-126">В случае успешной работы этот метод возвращает ответ `200 OK` с объектом [directoryDefinition.](../resources/synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0acfe-126">If successful, this method returns a `200 OK` response with a [directoryDefinition](../resources/synchronization-directorydefinition.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="0acfe-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0acfe-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="0acfe-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0acfe-128">Request</span></span>
<span data-ttu-id="0acfe-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0acfe-129">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0acfe-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0acfe-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "discover_directorydefinition"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```
# <a name="c"></a>[<span data-ttu-id="0acfe-131">C#</span><span class="sxs-lookup"><span data-stu-id="0acfe-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/discover-directorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0acfe-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0acfe-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/discover-directorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0acfe-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0acfe-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/discover-directorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0acfe-134">Java</span><span class="sxs-lookup"><span data-stu-id="0acfe-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/discover-directorydefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0acfe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0acfe-135">Response</span></span>

<span data-ttu-id="0acfe-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0acfe-136">The following is an example of a response.</span></span>

><span data-ttu-id="0acfe-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0acfe-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "discoverabilities": "AttributeNames, AttributeDataTypes",
  "discoveryDateTime": "2019-03-20T15:47:50.4707552Z",
  "id": "directoryDefinitionId",
  "objects": [{
        "name": "User",
        "attributes": [{
                "name": "Id",
                "type": "String"
            }, {
                "name": "FirstName",
                "type": "String"
            },
            {
                "name": "CustomExendedAttribute",
                "type": "String"
            }  
        ]
    }],
  "version": "bf8c03ac-d45e-47fe-b3a1-711a9418b2b1"
}
 ```


