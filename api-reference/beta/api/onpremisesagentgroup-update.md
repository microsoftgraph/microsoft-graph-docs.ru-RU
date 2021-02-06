---
title: Обновление onPremisesAgentGroup
description: Обновление свойств объекта **onPremisesAgentGroup.**
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 1b04124a5e0cb39d59a95f2278b8ea24f9dc2366
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136379"
---
# <a name="update-onpremisesagentgroup"></a><span data-ttu-id="5b2d0-103">Обновление onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="5b2d0-103">Update onPremisesAgentGroup</span></span>

<span data-ttu-id="5b2d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b2d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b2d0-105">Обновление свойств объекта [onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="5b2d0-105">Update the properties of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b2d0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5b2d0-106">Permissions</span></span>

<span data-ttu-id="5b2d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b2d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b2d0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b2d0-109">Permission type</span></span>                        | <span data-ttu-id="5b2d0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b2d0-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b2d0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b2d0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b2d0-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b2d0-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="5b2d0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b2d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b2d0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b2d0-114">Not supported.</span></span> |
| <span data-ttu-id="5b2d0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b2d0-115">Application</span></span>                            | <span data-ttu-id="5b2d0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b2d0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b2d0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b2d0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="request-headers"></a><span data-ttu-id="5b2d0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b2d0-118">Request headers</span></span>

| <span data-ttu-id="5b2d0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5b2d0-119">Name</span></span>       | <span data-ttu-id="5b2d0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5b2d0-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5b2d0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b2d0-121">Authorization</span></span> | <span data-ttu-id="5b2d0-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="5b2d0-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b2d0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b2d0-123">Request body</span></span>

<span data-ttu-id="5b2d0-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="5b2d0-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5b2d0-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="5b2d0-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5b2d0-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5b2d0-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="5b2d0-127">Ниже приводится список свойств, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="5b2d0-127">The following is the list of properties that you can update.</span></span>

| <span data-ttu-id="5b2d0-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b2d0-128">Property</span></span>     | <span data-ttu-id="5b2d0-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5b2d0-129">Type</span></span>        | <span data-ttu-id="5b2d0-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5b2d0-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5b2d0-131">displayName</span><span class="sxs-lookup"><span data-stu-id="5b2d0-131">displayName</span></span>|<span data-ttu-id="5b2d0-132">Строка</span><span class="sxs-lookup"><span data-stu-id="5b2d0-132">String</span></span>| <span data-ttu-id="5b2d0-133">Представляет имя локальной группы агентов.</span><span class="sxs-lookup"><span data-stu-id="5b2d0-133">Represents the on-premises agents group name.</span></span>|

## <a name="response"></a><span data-ttu-id="5b2d0-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b2d0-134">Response</span></span>

<span data-ttu-id="5b2d0-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5b2d0-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5b2d0-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="5b2d0-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b2d0-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b2d0-137">Request</span></span>

<span data-ttu-id="5b2d0-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b2d0-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b2d0-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b2d0-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5b2d0-140">C#</span><span class="sxs-lookup"><span data-stu-id="5b2d0-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b2d0-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b2d0-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b2d0-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b2d0-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5b2d0-143">Java</span><span class="sxs-lookup"><span data-stu-id="5b2d0-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisesagentgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5b2d0-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b2d0-144">Response</span></span>

<span data-ttu-id="5b2d0-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5b2d0-145">The following is an example of the response.</span></span>

> <span data-ttu-id="5b2d0-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b2d0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



