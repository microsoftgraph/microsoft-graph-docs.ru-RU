---
title: Обновление Онпремисесажентграуп
description: Обновление свойств объекта **онпремисесажентграуп** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 61ed8eade5f69de89e5550e5692201a3935cf2d8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414488"
---
# <a name="update-onpremisesagentgroup"></a><span data-ttu-id="a9ef3-103">Обновление Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="a9ef3-103">Update onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9ef3-104">Обновление свойств объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="a9ef3-104">Update the properties of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9ef3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9ef3-105">Permissions</span></span>

<span data-ttu-id="a9ef3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9ef3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9ef3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9ef3-108">Permission type</span></span>                        | <span data-ttu-id="a9ef3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9ef3-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9ef3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9ef3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9ef3-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a9ef3-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="a9ef3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9ef3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9ef3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9ef3-113">Not supported.</span></span> |
| <span data-ttu-id="a9ef3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9ef3-114">Application</span></span>                            | <span data-ttu-id="a9ef3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9ef3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9ef3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9ef3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/agentGroups
```

## <a name="request-headers"></a><span data-ttu-id="a9ef3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9ef3-117">Request headers</span></span>

| <span data-ttu-id="a9ef3-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a9ef3-118">Name</span></span>       | <span data-ttu-id="a9ef3-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a9ef3-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a9ef3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9ef3-120">Authorization</span></span> | <span data-ttu-id="a9ef3-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a9ef3-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9ef3-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9ef3-122">Request body</span></span>

<span data-ttu-id="a9ef3-123">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a9ef3-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a9ef3-124">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a9ef3-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a9ef3-125">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a9ef3-125">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="a9ef3-126">Ниже приведен список свойств, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="a9ef3-126">The following is the list of properties that you can update.</span></span>

| <span data-ttu-id="a9ef3-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9ef3-127">Property</span></span>     | <span data-ttu-id="a9ef3-128">Тип</span><span class="sxs-lookup"><span data-stu-id="a9ef3-128">Type</span></span>        | <span data-ttu-id="a9ef3-129">Описание</span><span class="sxs-lookup"><span data-stu-id="a9ef3-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a9ef3-130">displayName</span><span class="sxs-lookup"><span data-stu-id="a9ef3-130">displayName</span></span>|<span data-ttu-id="a9ef3-131">String</span><span class="sxs-lookup"><span data-stu-id="a9ef3-131">String</span></span>| <span data-ttu-id="a9ef3-132">Представляет имя группы локальных агентов.</span><span class="sxs-lookup"><span data-stu-id="a9ef3-132">Represents the on-premises agents group name.</span></span>|

## <a name="response"></a><span data-ttu-id="a9ef3-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9ef3-133">Response</span></span>

<span data-ttu-id="a9ef3-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a9ef3-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a9ef3-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="a9ef3-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9ef3-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9ef3-136">Request</span></span>

<span data-ttu-id="a9ef3-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9ef3-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a9ef3-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9ef3-138">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="a9ef3-139">C#</span><span class="sxs-lookup"><span data-stu-id="a9ef3-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9ef3-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9ef3-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a9ef3-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a9ef3-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a9ef3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9ef3-142">Response</span></span>

<span data-ttu-id="a9ef3-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a9ef3-143">The following is an example of the response.</span></span>

> <span data-ttu-id="a9ef3-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a9ef3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
