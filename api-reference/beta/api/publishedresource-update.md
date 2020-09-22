---
title: Обновление Публишедресаурце
description: Обновление свойств объекта [публишедресаурце](../resources/publishedresource.md) .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 91f7f03e21c4608f8245f56443cea13d6a1c369b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093047"
---
# <a name="update-publishedresource"></a><span data-ttu-id="7ccd1-103">Обновление Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="7ccd1-103">Update publishedResource</span></span>

<span data-ttu-id="7ccd1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ccd1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ccd1-105">Обновление свойств объекта публишедресаурце  [публишедресаурце](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="7ccd1-105">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ccd1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ccd1-106">Permissions</span></span>

<span data-ttu-id="7ccd1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ccd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ccd1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ccd1-109">Permission type</span></span>                        | <span data-ttu-id="7ccd1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ccd1-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="7ccd1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ccd1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ccd1-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ccd1-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="7ccd1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ccd1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ccd1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ccd1-114">Not supported.</span></span> |
| <span data-ttu-id="7ccd1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ccd1-115">Application</span></span>                            | <span data-ttu-id="7ccd1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ccd1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ccd1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ccd1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="7ccd1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ccd1-118">Request headers</span></span>

| <span data-ttu-id="7ccd1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7ccd1-119">Name</span></span>       | <span data-ttu-id="7ccd1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7ccd1-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7ccd1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ccd1-121">Authorization</span></span> | <span data-ttu-id="7ccd1-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="7ccd1-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ccd1-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ccd1-123">Request body</span></span>

<span data-ttu-id="7ccd1-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="7ccd1-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="7ccd1-125">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="7ccd1-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7ccd1-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7ccd1-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="7ccd1-127">В следующей таблице перечислены свойства, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="7ccd1-127">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="7ccd1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ccd1-128">Property</span></span>     | <span data-ttu-id="7ccd1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7ccd1-129">Type</span></span>        | <span data-ttu-id="7ccd1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7ccd1-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7ccd1-131">displayName</span><span class="sxs-lookup"><span data-stu-id="7ccd1-131">displayName</span></span>|<span data-ttu-id="7ccd1-132">Строка</span><span class="sxs-lookup"><span data-stu-id="7ccd1-132">String</span></span>|<span data-ttu-id="7ccd1-133">Представляет локальное имя опубликованного ресурса.</span><span class="sxs-lookup"><span data-stu-id="7ccd1-133">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="7ccd1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ccd1-134">Response</span></span>

<span data-ttu-id="7ccd1-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7ccd1-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7ccd1-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="7ccd1-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7ccd1-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ccd1-137">Request</span></span>

<span data-ttu-id="7ccd1-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ccd1-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ccd1-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ccd1-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7ccd1-140">C#</span><span class="sxs-lookup"><span data-stu-id="7ccd1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ccd1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ccd1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ccd1-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ccd1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7ccd1-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ccd1-143">Response</span></span>

<span data-ttu-id="7ccd1-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7ccd1-144">The following is an example of the response.</span></span>

> <span data-ttu-id="7ccd1-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ccd1-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


