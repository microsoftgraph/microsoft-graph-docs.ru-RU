---
title: Дело об обновлении
description: Обновим свойства объекта-кейса.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 24b2a72efc8e0f36a6cf8f00161a3ca636987805
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447098"
---
# <a name="update-case"></a><span data-ttu-id="f4bf8-103">Дело об обновлении</span><span class="sxs-lookup"><span data-stu-id="f4bf8-103">Update case</span></span>

<span data-ttu-id="f4bf8-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f4bf8-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4bf8-105">Обновим свойства [объекта-кейса.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="f4bf8-105">Update the properties of a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4bf8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4bf8-106">Permissions</span></span>

<span data-ttu-id="f4bf8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4bf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4bf8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4bf8-109">Permission type</span></span>|<span data-ttu-id="f4bf8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4bf8-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4bf8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4bf8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f4bf8-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4bf8-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="f4bf8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4bf8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4bf8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4bf8-114">Not supported.</span></span>|
|<span data-ttu-id="f4bf8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4bf8-115">Application</span></span>|<span data-ttu-id="f4bf8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4bf8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4bf8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4bf8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f4bf8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4bf8-118">Request headers</span></span>

| <span data-ttu-id="f4bf8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f4bf8-119">Name</span></span>       | <span data-ttu-id="f4bf8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f4bf8-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f4bf8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4bf8-121">Authorization</span></span> | <span data-ttu-id="f4bf8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f4bf8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4bf8-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4bf8-124">Request body</span></span>

<span data-ttu-id="f4bf8-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f4bf8-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f4bf8-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="f4bf8-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f4bf8-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f4bf8-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f4bf8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4bf8-128">Property</span></span>     | <span data-ttu-id="f4bf8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f4bf8-129">Type</span></span>        | <span data-ttu-id="f4bf8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f4bf8-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f4bf8-131">description</span><span class="sxs-lookup"><span data-stu-id="f4bf8-131">description</span></span>|<span data-ttu-id="f4bf8-132">String</span><span class="sxs-lookup"><span data-stu-id="f4bf8-132">String</span></span>|<span data-ttu-id="f4bf8-133">Описание случая.</span><span class="sxs-lookup"><span data-stu-id="f4bf8-133">The case description.</span></span>|
|<span data-ttu-id="f4bf8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="f4bf8-134">displayName</span></span>|<span data-ttu-id="f4bf8-135">String</span><span class="sxs-lookup"><span data-stu-id="f4bf8-135">String</span></span>|<span data-ttu-id="f4bf8-136">Имя случая.</span><span class="sxs-lookup"><span data-stu-id="f4bf8-136">The case name.</span></span>|
|<span data-ttu-id="f4bf8-137">externalId</span><span class="sxs-lookup"><span data-stu-id="f4bf8-137">externalId</span></span>|<span data-ttu-id="f4bf8-138">String</span><span class="sxs-lookup"><span data-stu-id="f4bf8-138">String</span></span>|<span data-ttu-id="f4bf8-139">Внешний номер случая для клиентской ссылки.</span><span class="sxs-lookup"><span data-stu-id="f4bf8-139">The external case number for customer reference.</span></span>|

## <a name="response"></a><span data-ttu-id="f4bf8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4bf8-140">Response</span></span>

<span data-ttu-id="f4bf8-141">В случае успешного решения этот метод возвращает код ответа и обновленный `200 OK` [объект microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f4bf8-141">If successful, this method returns a `200 OK` response code and an updated [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4bf8-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="f4bf8-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4bf8-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4bf8-143">Request</span></span>

<span data-ttu-id="f4bf8-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4bf8-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4bf8-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4bf8-145">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_case"
}-->

```http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases/061b9a92-8926-4bd9-b41d-abf35edc7583
Content-type: application/json

{
  "displayName": "My Case 1 - Renamed",
  "description": "Updated description",
  "externalId": "Updated externalId"
}
```

# <a name="c"></a>[<span data-ttu-id="f4bf8-146">C#</span><span class="sxs-lookup"><span data-stu-id="f4bf8-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4bf8-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4bf8-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4bf8-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4bf8-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4bf8-149">Java</span><span class="sxs-lookup"><span data-stu-id="f4bf8-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-ediscoverycase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f4bf8-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4bf8-150">Response</span></span>

<span data-ttu-id="f4bf8-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f4bf8-151">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.case"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update case",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
