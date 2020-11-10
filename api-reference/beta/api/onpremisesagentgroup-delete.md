---
title: Удаление Онпремисесажентграуп
description: Удаление объекта **онпремисесажентграуп** .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ba173597540597314ca832d0904f2ee34eb517a3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977023"
---
# <a name="delete-onpremisesagentgroup"></a><span data-ttu-id="8d740-103">Удаление Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="8d740-103">Delete onPremisesAgentGroup</span></span>

<span data-ttu-id="8d740-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d740-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d740-105">Удаление объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="8d740-105">Delete an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d740-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d740-106">Permissions</span></span>

<span data-ttu-id="8d740-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d740-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8d740-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d740-109">Permission type</span></span>                        | <span data-ttu-id="8d740-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d740-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d740-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d740-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8d740-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d740-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="8d740-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d740-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d740-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d740-114">Not supported.</span></span> |
| <span data-ttu-id="8d740-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d740-115">Application</span></span>                            | <span data-ttu-id="8d740-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d740-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d740-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d740-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="8d740-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d740-118">Request headers</span></span>

| <span data-ttu-id="8d740-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8d740-119">Name</span></span>          | <span data-ttu-id="8d740-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8d740-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8d740-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d740-121">Authorization</span></span> | <span data-ttu-id="8d740-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="8d740-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d740-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d740-123">Request body</span></span>

<span data-ttu-id="8d740-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d740-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d740-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d740-125">Response</span></span>

<span data-ttu-id="8d740-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8d740-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8d740-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8d740-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8d740-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d740-129">Request</span></span>

<span data-ttu-id="8d740-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d740-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d740-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d740-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesagentgroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
```
# <a name="c"></a>[<span data-ttu-id="8d740-132">C#</span><span class="sxs-lookup"><span data-stu-id="8d740-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d740-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d740-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d740-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d740-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d740-135">Java</span><span class="sxs-lookup"><span data-stu-id="8d740-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-onpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8d740-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d740-136">Response</span></span>

<span data-ttu-id="8d740-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8d740-137">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


