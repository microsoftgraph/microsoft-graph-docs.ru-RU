---
title: Обновление Публишедресаурце
description: Обновление свойств объекта [публишедресаурце](../resources/publishedresource.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f73a78c3d22e900a4c114dc07edded66bfc91318
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454824"
---
# <a name="update-publishedresource"></a><span data-ttu-id="454be-103">Обновление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="454be-103">Update publishedResource</span></span>

<span data-ttu-id="454be-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="454be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="454be-105">Обновление свойств объекта публишедресаурце [публишедресаурце](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="454be-105">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="454be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="454be-106">Permissions</span></span>

<span data-ttu-id="454be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="454be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="454be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="454be-109">Permission type</span></span>                        | <span data-ttu-id="454be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="454be-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="454be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="454be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="454be-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="454be-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="454be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="454be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="454be-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="454be-114">Not supported.</span></span> |
| <span data-ttu-id="454be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="454be-115">Application</span></span>                            | <span data-ttu-id="454be-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="454be-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="454be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="454be-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="454be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="454be-118">Request headers</span></span>

| <span data-ttu-id="454be-119">Имя</span><span class="sxs-lookup"><span data-stu-id="454be-119">Name</span></span>       | <span data-ttu-id="454be-120">Описание</span><span class="sxs-lookup"><span data-stu-id="454be-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="454be-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="454be-121">Authorization</span></span> | <span data-ttu-id="454be-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="454be-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="454be-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="454be-123">Request body</span></span>

<span data-ttu-id="454be-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="454be-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="454be-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="454be-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="454be-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="454be-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="454be-127">В следующей таблице перечислены свойства, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="454be-127">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="454be-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="454be-128">Property</span></span>     | <span data-ttu-id="454be-129">Тип</span><span class="sxs-lookup"><span data-stu-id="454be-129">Type</span></span>        | <span data-ttu-id="454be-130">Описание</span><span class="sxs-lookup"><span data-stu-id="454be-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="454be-131">displayName</span><span class="sxs-lookup"><span data-stu-id="454be-131">displayName</span></span>|<span data-ttu-id="454be-132">String</span><span class="sxs-lookup"><span data-stu-id="454be-132">String</span></span>|<span data-ttu-id="454be-133">Представляет локальное имя опубликованного ресурса.</span><span class="sxs-lookup"><span data-stu-id="454be-133">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="454be-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="454be-134">Response</span></span>

<span data-ttu-id="454be-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="454be-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="454be-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="454be-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="454be-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="454be-137">Request</span></span>

<span data-ttu-id="454be-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="454be-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="454be-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="454be-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="454be-140">C#</span><span class="sxs-lookup"><span data-stu-id="454be-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="454be-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="454be-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="454be-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="454be-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="454be-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="454be-143">Response</span></span>

<span data-ttu-id="454be-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="454be-144">The following is an example of the response.</span></span>

> <span data-ttu-id="454be-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="454be-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
