---
title: Обновление publishedResource
description: Обновление свойств объекта [publishedResource.](../resources/publishedresource.md)
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8c8a6cfe8eead7219918daf5ac2e87090cc18888
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137678"
---
# <a name="update-publishedresource"></a><span data-ttu-id="21513-103">Обновление publishedResource</span><span class="sxs-lookup"><span data-stu-id="21513-103">Update publishedResource</span></span>

<span data-ttu-id="21513-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21513-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21513-105">Обновление свойств объекта publishedresource [publishedResource.](../resources/publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="21513-105">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="21513-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21513-106">Permissions</span></span>

<span data-ttu-id="21513-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21513-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21513-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21513-109">Permission type</span></span>                        | <span data-ttu-id="21513-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21513-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="21513-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21513-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="21513-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21513-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="21513-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21513-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21513-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21513-114">Not supported.</span></span> |
| <span data-ttu-id="21513-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21513-115">Application</span></span>                            | <span data-ttu-id="21513-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21513-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21513-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21513-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="21513-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21513-118">Request headers</span></span>

| <span data-ttu-id="21513-119">Имя</span><span class="sxs-lookup"><span data-stu-id="21513-119">Name</span></span>       | <span data-ttu-id="21513-120">Описание</span><span class="sxs-lookup"><span data-stu-id="21513-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="21513-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21513-121">Authorization</span></span> | <span data-ttu-id="21513-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="21513-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="21513-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="21513-123">Request body</span></span>

<span data-ttu-id="21513-124">В теле запроса укавите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="21513-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="21513-125">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="21513-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="21513-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="21513-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="21513-127">В следующей таблице перечислены свойства, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="21513-127">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="21513-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="21513-128">Property</span></span>     | <span data-ttu-id="21513-129">Тип</span><span class="sxs-lookup"><span data-stu-id="21513-129">Type</span></span>        | <span data-ttu-id="21513-130">Описание</span><span class="sxs-lookup"><span data-stu-id="21513-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21513-131">displayName</span><span class="sxs-lookup"><span data-stu-id="21513-131">displayName</span></span>|<span data-ttu-id="21513-132">Строка</span><span class="sxs-lookup"><span data-stu-id="21513-132">String</span></span>|<span data-ttu-id="21513-133">Представляет локально опубликованное имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="21513-133">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="21513-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="21513-134">Response</span></span>

<span data-ttu-id="21513-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="21513-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="21513-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="21513-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="21513-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="21513-137">Request</span></span>

<span data-ttu-id="21513-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21513-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21513-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="21513-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="21513-140">C#</span><span class="sxs-lookup"><span data-stu-id="21513-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21513-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21513-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21513-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21513-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21513-143">Java</span><span class="sxs-lookup"><span data-stu-id="21513-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="21513-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="21513-144">Response</span></span>

<span data-ttu-id="21513-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21513-145">The following is an example of the response.</span></span>

> <span data-ttu-id="21513-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21513-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



