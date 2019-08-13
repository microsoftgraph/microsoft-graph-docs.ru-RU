---
title: 'Директоридефинитион: обнаружение'
description: 'Ознакомьтесь с последним определением схемы для подготовки к работе с приложением. '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 55063d676697a5c0f5acad88290fd831910db2a4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321332"
---
# <a name="directorydefinition-discover"></a><span data-ttu-id="d6a03-103">Директоридефинитион: обнаружение</span><span class="sxs-lookup"><span data-stu-id="d6a03-103">directoryDefinition: discover</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6a03-104">Ознакомьтесь с последним определением схемы для подготовки к работе с приложением.</span><span class="sxs-lookup"><span data-stu-id="d6a03-104">Discover the latest schema definition for provisioning to an application.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d6a03-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6a03-105">Permissions</span></span>

<span data-ttu-id="d6a03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6a03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6a03-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6a03-108">Permission type</span></span>                        | <span data-ttu-id="d6a03-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6a03-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d6a03-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6a03-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6a03-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6a03-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="d6a03-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6a03-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6a03-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6a03-113">Not supported.</span></span> |
| <span data-ttu-id="d6a03-114">Только для приложений</span><span class="sxs-lookup"><span data-stu-id="d6a03-114">Application-only</span></span>                            | <span data-ttu-id="d6a03-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="d6a03-115">None.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6a03-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6a03-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

## <a name="request-headers"></a><span data-ttu-id="d6a03-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6a03-117">Request headers</span></span>

| <span data-ttu-id="d6a03-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6a03-118">Header</span></span>        | <span data-ttu-id="d6a03-119">Значение</span><span class="sxs-lookup"><span data-stu-id="d6a03-119">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="d6a03-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6a03-120">Authorization</span></span> | <span data-ttu-id="d6a03-121">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="d6a03-121">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d6a03-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6a03-122">Request body</span></span>

<span data-ttu-id="d6a03-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d6a03-123">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="d6a03-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6a03-124">Response</span></span>

<span data-ttu-id="d6a03-125">В случае успешного выполнения этот метод возвращает `200 OK` ответ с объектом [директоридефинитион](../resources/synchronization-directorydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="d6a03-125">If successful, this method returns a `200 OK` response with a [directoryDefinition](../resources/synchronization-directorydefinition.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="d6a03-126">Пример</span><span class="sxs-lookup"><span data-stu-id="d6a03-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6a03-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6a03-127">Request</span></span>
<span data-ttu-id="d6a03-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6a03-128">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d6a03-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6a03-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "discover_directorydefinition"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d6a03-130">C#</span><span class="sxs-lookup"><span data-stu-id="d6a03-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/discover-directorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d6a03-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6a03-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/discover-directorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d6a03-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d6a03-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/discover-directorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d6a03-133">Java</span><span class="sxs-lookup"><span data-stu-id="d6a03-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/discover-directorydefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d6a03-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6a03-134">Response</span></span>

<span data-ttu-id="d6a03-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d6a03-135">The following is an example of a response.</span></span>

><span data-ttu-id="d6a03-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6a03-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
