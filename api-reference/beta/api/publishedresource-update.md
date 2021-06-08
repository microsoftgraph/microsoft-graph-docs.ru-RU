---
title: Update publishedResource
description: Обновление свойств объекта [publishedResource.](../resources/publishedresource.md)
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 776893669989e135a781e19aca6f344cf4015ce0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787382"
---
# <a name="update-publishedresource"></a><span data-ttu-id="ac421-103">Update publishedResource</span><span class="sxs-lookup"><span data-stu-id="ac421-103">Update publishedResource</span></span>

<span data-ttu-id="ac421-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac421-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac421-105">Обновление свойств объекта publishedresource [publishedResource.](../resources/publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="ac421-105">Update the properties of publishedresource  [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac421-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac421-106">Permissions</span></span>

<span data-ttu-id="ac421-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac421-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac421-109">Permission type</span></span>                        | <span data-ttu-id="ac421-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac421-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="ac421-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac421-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac421-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac421-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="ac421-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac421-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac421-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac421-114">Not supported.</span></span> |
| <span data-ttu-id="ac421-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac421-115">Application</span></span>                            | <span data-ttu-id="ac421-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac421-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac421-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac421-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="ac421-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac421-118">Request headers</span></span>

| <span data-ttu-id="ac421-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ac421-119">Name</span></span>       | <span data-ttu-id="ac421-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ac421-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ac421-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac421-121">Authorization</span></span> | <span data-ttu-id="ac421-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ac421-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac421-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ac421-123">Request body</span></span>

<span data-ttu-id="ac421-124">В теле запроса укажи значения для обновления соответствующих полей.</span><span class="sxs-lookup"><span data-stu-id="ac421-124">In the request body, supply the values for relevant fields to update.</span></span> <span data-ttu-id="ac421-125">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="ac421-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ac421-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ac421-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="ac421-127">В следующей таблице перечислены свойства, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="ac421-127">The following table lists the properties that can be updated.</span></span>

| <span data-ttu-id="ac421-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac421-128">Property</span></span>     | <span data-ttu-id="ac421-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ac421-129">Type</span></span>        | <span data-ttu-id="ac421-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ac421-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac421-131">displayName</span><span class="sxs-lookup"><span data-stu-id="ac421-131">displayName</span></span>|<span data-ttu-id="ac421-132">String</span><span class="sxs-lookup"><span data-stu-id="ac421-132">String</span></span>|<span data-ttu-id="ac421-133">Представляет локальное имя опубликованного ресурса.</span><span class="sxs-lookup"><span data-stu-id="ac421-133">Represents an on-premises published resource name.</span></span>|

## <a name="response"></a><span data-ttu-id="ac421-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac421-134">Response</span></span>

<span data-ttu-id="ac421-135">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ac421-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ac421-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="ac421-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac421-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac421-137">Request</span></span>

<span data-ttu-id="ac421-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac421-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ac421-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac421-139">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ac421-140">C#</span><span class="sxs-lookup"><span data-stu-id="ac421-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ac421-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac421-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac421-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac421-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ac421-143">Java</span><span class="sxs-lookup"><span data-stu-id="ac421-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac421-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac421-144">Response</span></span>

<span data-ttu-id="ac421-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ac421-145">The following is an example of the response.</span></span>

> <span data-ttu-id="ac421-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac421-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "description": "Update publishedresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



