---
title: 'directoryDefinition: обнаружение'
description: 'Обнаружение последнего определения схемы для предоставления приложения. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8b277d35e1cc83d5a52457cb07ddfe7129eb4cc8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130951"
---
# <a name="directorydefinition-discover"></a><span data-ttu-id="264ee-103">directoryDefinition: обнаружение</span><span class="sxs-lookup"><span data-stu-id="264ee-103">directoryDefinition: discover</span></span>

<span data-ttu-id="264ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="264ee-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="264ee-105">Обнаружение последнего определения схемы для предоставления приложения.</span><span class="sxs-lookup"><span data-stu-id="264ee-105">Discover the latest schema definition for provisioning to an application.</span></span> 

## <a name="permissions"></a><span data-ttu-id="264ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="264ee-106">Permissions</span></span>

<span data-ttu-id="264ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="264ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="264ee-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="264ee-109">Permission type</span></span>                        | <span data-ttu-id="264ee-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="264ee-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="264ee-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="264ee-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="264ee-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="264ee-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="264ee-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="264ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="264ee-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="264ee-114">Not supported.</span></span> |
| <span data-ttu-id="264ee-115">Только для приложений</span><span class="sxs-lookup"><span data-stu-id="264ee-115">Application-only</span></span>                            | <span data-ttu-id="264ee-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="264ee-116">None.</span></span> |

## <a name="http-request"></a><span data-ttu-id="264ee-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="264ee-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

## <a name="request-headers"></a><span data-ttu-id="264ee-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="264ee-118">Request headers</span></span>

| <span data-ttu-id="264ee-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="264ee-119">Header</span></span>        | <span data-ttu-id="264ee-120">Значение</span><span class="sxs-lookup"><span data-stu-id="264ee-120">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="264ee-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="264ee-121">Authorization</span></span> | <span data-ttu-id="264ee-122">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="264ee-122">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="264ee-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="264ee-123">Request body</span></span>

<span data-ttu-id="264ee-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="264ee-124">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="264ee-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="264ee-125">Response</span></span>

<span data-ttu-id="264ee-126">В случае успеха этот метод возвращает ответ `200 OK` с [объектом directoryDefinition.](../resources/synchronization-directorydefinition.md)</span><span class="sxs-lookup"><span data-stu-id="264ee-126">If successful, this method returns a `200 OK` response with a [directoryDefinition](../resources/synchronization-directorydefinition.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="264ee-127">Пример</span><span class="sxs-lookup"><span data-stu-id="264ee-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="264ee-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="264ee-128">Request</span></span>
<span data-ttu-id="264ee-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="264ee-129">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="264ee-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="264ee-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "discover_directorydefinition"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```
# <a name="c"></a>[<span data-ttu-id="264ee-131">C#</span><span class="sxs-lookup"><span data-stu-id="264ee-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/discover-directorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="264ee-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="264ee-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/discover-directorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="264ee-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="264ee-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/discover-directorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="264ee-134">Java</span><span class="sxs-lookup"><span data-stu-id="264ee-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/discover-directorydefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="264ee-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="264ee-135">Response</span></span>

<span data-ttu-id="264ee-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="264ee-136">The following is an example of a response.</span></span>

><span data-ttu-id="264ee-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="264ee-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


