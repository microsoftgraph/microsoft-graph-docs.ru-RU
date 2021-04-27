---
title: Обновление наPremisesAgentGroup
description: Обновление свойств объекта **onPremisesAgentGroup.**
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 892acaa068347ca6a555d163d01ec71b118c0285
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049235"
---
# <a name="update-onpremisesagentgroup"></a><span data-ttu-id="5634d-103">Обновление наPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="5634d-103">Update onPremisesAgentGroup</span></span>

<span data-ttu-id="5634d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5634d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5634d-105">Обновление свойств объекта [onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5634d-105">Update the properties of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5634d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5634d-106">Permissions</span></span>

<span data-ttu-id="5634d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5634d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5634d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5634d-109">Permission type</span></span>                        | <span data-ttu-id="5634d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5634d-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5634d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5634d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5634d-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5634d-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="5634d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5634d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5634d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5634d-114">Not supported.</span></span> |
| <span data-ttu-id="5634d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5634d-115">Application</span></span>                            | <span data-ttu-id="5634d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5634d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5634d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5634d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="request-headers"></a><span data-ttu-id="5634d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5634d-118">Request headers</span></span>

| <span data-ttu-id="5634d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5634d-119">Name</span></span>       | <span data-ttu-id="5634d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5634d-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5634d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5634d-121">Authorization</span></span> | <span data-ttu-id="5634d-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="5634d-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5634d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5634d-123">Request body</span></span>

<span data-ttu-id="5634d-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="5634d-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5634d-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="5634d-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5634d-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5634d-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="5634d-127">Ниже приводится список свойств, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="5634d-127">The following is the list of properties that you can update.</span></span>

| <span data-ttu-id="5634d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5634d-128">Property</span></span>     | <span data-ttu-id="5634d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5634d-129">Type</span></span>        | <span data-ttu-id="5634d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5634d-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5634d-131">displayName</span><span class="sxs-lookup"><span data-stu-id="5634d-131">displayName</span></span>|<span data-ttu-id="5634d-132">String</span><span class="sxs-lookup"><span data-stu-id="5634d-132">String</span></span>| <span data-ttu-id="5634d-133">Представляет локальное имя группы агентов.</span><span class="sxs-lookup"><span data-stu-id="5634d-133">Represents the on-premises agents group name.</span></span>|

## <a name="response"></a><span data-ttu-id="5634d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5634d-134">Response</span></span>

<span data-ttu-id="5634d-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5634d-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5634d-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="5634d-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5634d-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5634d-137">Request</span></span>

<span data-ttu-id="5634d-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5634d-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5634d-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5634d-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_onpremisesagentgroup"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
Content-type: application/json

{
    "displayName": "Group New Name"
}
```
# <a name="c"></a>[<span data-ttu-id="5634d-140">C#</span><span class="sxs-lookup"><span data-stu-id="5634d-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5634d-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5634d-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5634d-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5634d-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5634d-143">Java</span><span class="sxs-lookup"><span data-stu-id="5634d-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5634d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="5634d-144">Response</span></span>

<span data-ttu-id="5634d-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5634d-145">The following is an example of the response.</span></span>

> <span data-ttu-id="5634d-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5634d-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update onpremisesagentgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



