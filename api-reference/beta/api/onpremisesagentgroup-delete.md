---
title: Удаление наPremisesAgentGroup
description: Удаление **объекта onPremisesAgentGroup.**
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 853d270edfdfe5f35c5bc0bc6ee16b784333977f
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781144"
---
# <a name="delete-onpremisesagentgroup"></a><span data-ttu-id="347dc-103">Удаление наPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="347dc-103">Delete onPremisesAgentGroup</span></span>

<span data-ttu-id="347dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="347dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="347dc-105">Удаление [объекта onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="347dc-105">Delete an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="347dc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="347dc-106">Permissions</span></span>

<span data-ttu-id="347dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="347dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="347dc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="347dc-109">Permission type</span></span>                        | <span data-ttu-id="347dc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="347dc-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="347dc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="347dc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="347dc-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="347dc-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="347dc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="347dc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="347dc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="347dc-114">Not supported.</span></span> |
| <span data-ttu-id="347dc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="347dc-115">Application</span></span>                            | <span data-ttu-id="347dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="347dc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="347dc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="347dc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="347dc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="347dc-118">Request headers</span></span>

| <span data-ttu-id="347dc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="347dc-119">Name</span></span>          | <span data-ttu-id="347dc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="347dc-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="347dc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="347dc-121">Authorization</span></span> | <span data-ttu-id="347dc-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="347dc-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="347dc-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="347dc-123">Request body</span></span>

<span data-ttu-id="347dc-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="347dc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="347dc-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="347dc-125">Response</span></span>

<span data-ttu-id="347dc-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="347dc-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="347dc-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="347dc-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="347dc-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="347dc-129">Request</span></span>

<span data-ttu-id="347dc-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="347dc-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="347dc-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="347dc-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesagentgroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
```
# <a name="c"></a>[<span data-ttu-id="347dc-132">C#</span><span class="sxs-lookup"><span data-stu-id="347dc-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="347dc-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="347dc-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="347dc-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="347dc-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="347dc-135">Java</span><span class="sxs-lookup"><span data-stu-id="347dc-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-onpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="347dc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="347dc-136">Response</span></span>

<span data-ttu-id="347dc-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="347dc-137">The following is an example of the response.</span></span>

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



