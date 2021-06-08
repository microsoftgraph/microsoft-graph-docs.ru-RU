---
title: Обновление наPremisesAgentGroup
description: Обновление свойств объекта **onPremisesAgentGroup.**
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: b78c82989f8fc06daed22dd0a80cb1d07be8e77e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785956"
---
# <a name="update-onpremisesagentgroup"></a><span data-ttu-id="25173-103">Обновление наPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="25173-103">Update onPremisesAgentGroup</span></span>

<span data-ttu-id="25173-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25173-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25173-105">Обновление свойств объекта [onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="25173-105">Update the properties of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="25173-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="25173-106">Permissions</span></span>

<span data-ttu-id="25173-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25173-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="25173-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25173-109">Permission type</span></span>                        | <span data-ttu-id="25173-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="25173-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="25173-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25173-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="25173-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25173-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="25173-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25173-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25173-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25173-114">Not supported.</span></span> |
| <span data-ttu-id="25173-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25173-115">Application</span></span>                            | <span data-ttu-id="25173-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25173-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25173-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25173-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="request-headers"></a><span data-ttu-id="25173-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25173-118">Request headers</span></span>

| <span data-ttu-id="25173-119">Имя</span><span class="sxs-lookup"><span data-stu-id="25173-119">Name</span></span>       | <span data-ttu-id="25173-120">Описание</span><span class="sxs-lookup"><span data-stu-id="25173-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="25173-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25173-121">Authorization</span></span> | <span data-ttu-id="25173-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="25173-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="25173-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25173-123">Request body</span></span>

<span data-ttu-id="25173-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="25173-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="25173-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="25173-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="25173-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="25173-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="25173-127">Ниже приводится список свойств, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="25173-127">The following is the list of properties that you can update.</span></span>

| <span data-ttu-id="25173-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="25173-128">Property</span></span>     | <span data-ttu-id="25173-129">Тип</span><span class="sxs-lookup"><span data-stu-id="25173-129">Type</span></span>        | <span data-ttu-id="25173-130">Описание</span><span class="sxs-lookup"><span data-stu-id="25173-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="25173-131">displayName</span><span class="sxs-lookup"><span data-stu-id="25173-131">displayName</span></span>|<span data-ttu-id="25173-132">String</span><span class="sxs-lookup"><span data-stu-id="25173-132">String</span></span>| <span data-ttu-id="25173-133">Представляет локальное имя группы агентов.</span><span class="sxs-lookup"><span data-stu-id="25173-133">Represents the on-premises agents group name.</span></span>|

## <a name="response"></a><span data-ttu-id="25173-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="25173-134">Response</span></span>

<span data-ttu-id="25173-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="25173-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="25173-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="25173-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="25173-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="25173-137">Request</span></span>

<span data-ttu-id="25173-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25173-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="25173-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="25173-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="25173-140">C#</span><span class="sxs-lookup"><span data-stu-id="25173-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25173-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25173-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25173-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25173-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25173-143">Java</span><span class="sxs-lookup"><span data-stu-id="25173-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="25173-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="25173-144">Response</span></span>

<span data-ttu-id="25173-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="25173-145">The following is an example of the response.</span></span>

> <span data-ttu-id="25173-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="25173-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response"
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



