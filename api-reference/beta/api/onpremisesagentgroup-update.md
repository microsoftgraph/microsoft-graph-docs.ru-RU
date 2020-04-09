---
title: Обновление Онпремисесажентграуп
description: Обновление свойств объекта **онпремисесажентграуп** .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 58d452bea88c58de944cdb4f48bf482025abb2ba
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200239"
---
# <a name="update-onpremisesagentgroup"></a><span data-ttu-id="6b893-103">Обновление Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="6b893-103">Update onPremisesAgentGroup</span></span>

<span data-ttu-id="6b893-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b893-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b893-105">Обновление свойств объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6b893-105">Update the properties of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b893-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b893-106">Permissions</span></span>

<span data-ttu-id="6b893-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b893-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b893-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b893-109">Permission type</span></span>                        | <span data-ttu-id="6b893-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b893-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b893-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b893-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b893-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b893-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="6b893-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b893-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b893-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b893-114">Not supported.</span></span> |
| <span data-ttu-id="6b893-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b893-115">Application</span></span>                            | <span data-ttu-id="6b893-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b893-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b893-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b893-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="request-headers"></a><span data-ttu-id="6b893-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b893-118">Request headers</span></span>

| <span data-ttu-id="6b893-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6b893-119">Name</span></span>       | <span data-ttu-id="6b893-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6b893-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6b893-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b893-121">Authorization</span></span> | <span data-ttu-id="6b893-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6b893-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b893-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b893-123">Request body</span></span>

<span data-ttu-id="6b893-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6b893-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6b893-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="6b893-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6b893-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6b893-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="6b893-127">Ниже приведен список свойств, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="6b893-127">The following is the list of properties that you can update.</span></span>

| <span data-ttu-id="6b893-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b893-128">Property</span></span>     | <span data-ttu-id="6b893-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6b893-129">Type</span></span>        | <span data-ttu-id="6b893-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6b893-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6b893-131">displayName</span><span class="sxs-lookup"><span data-stu-id="6b893-131">displayName</span></span>|<span data-ttu-id="6b893-132">String</span><span class="sxs-lookup"><span data-stu-id="6b893-132">String</span></span>| <span data-ttu-id="6b893-133">Представляет имя группы локальных агентов.</span><span class="sxs-lookup"><span data-stu-id="6b893-133">Represents the on-premises agents group name.</span></span>|

## <a name="response"></a><span data-ttu-id="6b893-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b893-134">Response</span></span>

<span data-ttu-id="6b893-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6b893-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6b893-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="6b893-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6b893-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b893-137">Request</span></span>

<span data-ttu-id="6b893-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b893-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b893-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b893-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6b893-140">C#</span><span class="sxs-lookup"><span data-stu-id="6b893-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b893-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b893-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b893-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b893-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6b893-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b893-143">Response</span></span>

<span data-ttu-id="6b893-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6b893-144">The following is an example of the response.</span></span>

> <span data-ttu-id="6b893-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6b893-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
