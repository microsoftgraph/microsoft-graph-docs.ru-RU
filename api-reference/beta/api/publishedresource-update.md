---
title: Обновление Публишедресаурце
description: Обновление свойств объекта [публишедресаурце](../resources/publishedresource.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2645e33b4b5a91607ab1f682c8b70e7485163fb4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412329"
---
# <a name="update-publishedresource"></a><span data-ttu-id="26e35-103">Обновление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="26e35-103">Update publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26e35-104">Обновление свойств объекта публишедресаурце [публишедресаурце](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="26e35-104">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="26e35-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26e35-105">Permissions</span></span>

<span data-ttu-id="26e35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26e35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26e35-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26e35-108">Permission type</span></span>                        | <span data-ttu-id="26e35-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26e35-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="26e35-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26e35-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="26e35-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="26e35-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="26e35-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26e35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26e35-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e35-113">Not supported.</span></span> |
| <span data-ttu-id="26e35-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26e35-114">Application</span></span>                            | <span data-ttu-id="26e35-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26e35-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="26e35-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26e35-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="26e35-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26e35-117">Request headers</span></span>

| <span data-ttu-id="26e35-118">Имя</span><span class="sxs-lookup"><span data-stu-id="26e35-118">Name</span></span>       | <span data-ttu-id="26e35-119">Описание</span><span class="sxs-lookup"><span data-stu-id="26e35-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="26e35-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26e35-120">Authorization</span></span> | <span data-ttu-id="26e35-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="26e35-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="26e35-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26e35-122">Request body</span></span>

<span data-ttu-id="26e35-123">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="26e35-123">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="26e35-124">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="26e35-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="26e35-125">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="26e35-125">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="26e35-126">В следующей таблице перечислены свойства, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="26e35-126">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="26e35-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="26e35-127">Property</span></span>     | <span data-ttu-id="26e35-128">Тип</span><span class="sxs-lookup"><span data-stu-id="26e35-128">Type</span></span>        | <span data-ttu-id="26e35-129">Описание</span><span class="sxs-lookup"><span data-stu-id="26e35-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="26e35-130">displayName</span><span class="sxs-lookup"><span data-stu-id="26e35-130">displayName</span></span>|<span data-ttu-id="26e35-131">String</span><span class="sxs-lookup"><span data-stu-id="26e35-131">String</span></span>|<span data-ttu-id="26e35-132">Представляет локальное имя опубликованного ресурса.</span><span class="sxs-lookup"><span data-stu-id="26e35-132">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="26e35-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="26e35-133">Response</span></span>

<span data-ttu-id="26e35-134">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="26e35-134">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="26e35-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="26e35-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26e35-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="26e35-136">Request</span></span>

<span data-ttu-id="26e35-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26e35-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="26e35-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="26e35-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_publishedresource"
}-->

```http
PATCH https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d

{
    "displayName": "Demo provisioning (updated)"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="26e35-139">C#</span><span class="sxs-lookup"><span data-stu-id="26e35-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26e35-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="26e35-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="26e35-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="26e35-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="26e35-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="26e35-142">Response</span></span>

<span data-ttu-id="26e35-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26e35-143">The following is an example of the response.</span></span>

> <span data-ttu-id="26e35-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26e35-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update publishedresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
