---
title: 'Директоридефинитион: обнаружение'
description: 'Ознакомьтесь с последним определением схемы для подготовки к работе с приложением. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b78cfe4eefa17893cf072f15e56837a4e6ee078
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008939"
---
# <a name="directorydefinition-discover"></a><span data-ttu-id="b5d71-103">Директоридефинитион: обнаружение</span><span class="sxs-lookup"><span data-stu-id="b5d71-103">directoryDefinition: discover</span></span>

<span data-ttu-id="b5d71-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5d71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5d71-105">Ознакомьтесь с последним определением схемы для подготовки к работе с приложением.</span><span class="sxs-lookup"><span data-stu-id="b5d71-105">Discover the latest schema definition for provisioning to an application.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b5d71-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5d71-106">Permissions</span></span>

<span data-ttu-id="b5d71-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5d71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5d71-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5d71-109">Permission type</span></span>                        | <span data-ttu-id="b5d71-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5d71-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b5d71-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5d71-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5d71-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5d71-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="b5d71-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5d71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5d71-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5d71-114">Not supported.</span></span> |
| <span data-ttu-id="b5d71-115">Только для приложений</span><span class="sxs-lookup"><span data-stu-id="b5d71-115">Application-only</span></span>                            | <span data-ttu-id="b5d71-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="b5d71-116">None.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5d71-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5d71-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

## <a name="request-headers"></a><span data-ttu-id="b5d71-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5d71-118">Request headers</span></span>

| <span data-ttu-id="b5d71-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b5d71-119">Header</span></span>        | <span data-ttu-id="b5d71-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b5d71-120">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="b5d71-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5d71-121">Authorization</span></span> | <span data-ttu-id="b5d71-122">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="b5d71-122">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b5d71-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5d71-123">Request body</span></span>

<span data-ttu-id="b5d71-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b5d71-124">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="b5d71-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5d71-125">Response</span></span>

<span data-ttu-id="b5d71-126">В случае успешного выполнения этот метод возвращает `200 OK` ответ с объектом [директоридефинитион](../resources/synchronization-directorydefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="b5d71-126">If successful, this method returns a `200 OK` response with a [directoryDefinition](../resources/synchronization-directorydefinition.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="b5d71-127">Пример</span><span class="sxs-lookup"><span data-stu-id="b5d71-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5d71-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5d71-128">Request</span></span>
<span data-ttu-id="b5d71-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5d71-129">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5d71-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5d71-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "discover_directorydefinition"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```
# <a name="c"></a>[<span data-ttu-id="b5d71-131">C#</span><span class="sxs-lookup"><span data-stu-id="b5d71-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/discover-directorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5d71-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5d71-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/discover-directorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5d71-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5d71-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/discover-directorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b5d71-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5d71-134">Response</span></span>

<span data-ttu-id="b5d71-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b5d71-135">The following is an example of a response.</span></span>

><span data-ttu-id="b5d71-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b5d71-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


