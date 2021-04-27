---
title: Update publishedResource
description: Обновление свойств объекта [publishedResource.](../resources/publishedresource.md)
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 22544845ededf639bc71f14dec72a7163ded7c90
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055157"
---
# <a name="update-publishedresource"></a><span data-ttu-id="7b961-103">Update publishedResource</span><span class="sxs-lookup"><span data-stu-id="7b961-103">Update publishedResource</span></span>

<span data-ttu-id="7b961-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b961-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b961-105">Обновление свойств объекта publishedresource [publishedResource.](../resources/publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="7b961-105">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b961-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7b961-106">Permissions</span></span>

<span data-ttu-id="7b961-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b961-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b961-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7b961-109">Permission type</span></span>                        | <span data-ttu-id="7b961-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7b961-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="7b961-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7b961-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b961-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b961-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="7b961-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7b961-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b961-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b961-114">Not supported.</span></span> |
| <span data-ttu-id="7b961-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7b961-115">Application</span></span>                            | <span data-ttu-id="7b961-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b961-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b961-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7b961-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="7b961-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7b961-118">Request headers</span></span>

| <span data-ttu-id="7b961-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7b961-119">Name</span></span>       | <span data-ttu-id="7b961-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7b961-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="7b961-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7b961-121">Authorization</span></span> | <span data-ttu-id="7b961-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="7b961-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b961-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7b961-123">Request body</span></span>

<span data-ttu-id="7b961-124">В теле запроса укажи значения для обновления соответствующих полей.</span><span class="sxs-lookup"><span data-stu-id="7b961-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="7b961-125">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="7b961-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="7b961-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="7b961-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="7b961-127">В следующей таблице перечислены свойства, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="7b961-127">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="7b961-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b961-128">Property</span></span>     | <span data-ttu-id="7b961-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7b961-129">Type</span></span>        | <span data-ttu-id="7b961-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7b961-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7b961-131">displayName</span><span class="sxs-lookup"><span data-stu-id="7b961-131">displayName</span></span>|<span data-ttu-id="7b961-132">String</span><span class="sxs-lookup"><span data-stu-id="7b961-132">String</span></span>|<span data-ttu-id="7b961-133">Представляет локальное имя опубликованного ресурса.</span><span class="sxs-lookup"><span data-stu-id="7b961-133">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="7b961-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b961-134">Response</span></span>

<span data-ttu-id="7b961-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7b961-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7b961-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="7b961-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7b961-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="7b961-137">Request</span></span>

<span data-ttu-id="7b961-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7b961-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7b961-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7b961-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7b961-140">C#</span><span class="sxs-lookup"><span data-stu-id="7b961-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7b961-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7b961-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7b961-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7b961-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7b961-143">Java</span><span class="sxs-lookup"><span data-stu-id="7b961-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7b961-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7b961-144">Response</span></span>

<span data-ttu-id="7b961-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7b961-145">The following is an example of the response.</span></span>

> <span data-ttu-id="7b961-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7b961-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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



