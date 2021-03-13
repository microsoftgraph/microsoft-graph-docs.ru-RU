---
title: Дело об обновлении
description: Обновим свойства объекта-кейса.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 79b2e56cdb0e7e6ad4acf09625af54e413291b08
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773657"
---
# <a name="update-case"></a><span data-ttu-id="75b7a-103">Дело об обновлении</span><span class="sxs-lookup"><span data-stu-id="75b7a-103">Update case</span></span>

<span data-ttu-id="75b7a-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="75b7a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75b7a-105">Обновим свойства [объекта-кейса.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="75b7a-105">Update the properties of a [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="75b7a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75b7a-106">Permissions</span></span>

<span data-ttu-id="75b7a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75b7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75b7a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75b7a-109">Permission type</span></span>|<span data-ttu-id="75b7a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75b7a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75b7a-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75b7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75b7a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75b7a-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="75b7a-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75b7a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75b7a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75b7a-114">Not supported.</span></span>|
|<span data-ttu-id="75b7a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75b7a-115">Application</span></span>|<span data-ttu-id="75b7a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75b7a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75b7a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75b7a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /compliance/ediscovery/cases/{id}
```

## <a name="request-headers"></a><span data-ttu-id="75b7a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75b7a-118">Request headers</span></span>

| <span data-ttu-id="75b7a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="75b7a-119">Name</span></span>       | <span data-ttu-id="75b7a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="75b7a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="75b7a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75b7a-121">Authorization</span></span> | <span data-ttu-id="75b7a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75b7a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75b7a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75b7a-124">Request body</span></span>

<span data-ttu-id="75b7a-125">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="75b7a-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="75b7a-126">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="75b7a-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="75b7a-127">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="75b7a-127">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="75b7a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="75b7a-128">Property</span></span>     | <span data-ttu-id="75b7a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="75b7a-129">Type</span></span>        | <span data-ttu-id="75b7a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="75b7a-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="75b7a-131">description</span><span class="sxs-lookup"><span data-stu-id="75b7a-131">description</span></span>|<span data-ttu-id="75b7a-132">String</span><span class="sxs-lookup"><span data-stu-id="75b7a-132">String</span></span>|<span data-ttu-id="75b7a-133">Описание случая.</span><span class="sxs-lookup"><span data-stu-id="75b7a-133">The case description.</span></span>|
|<span data-ttu-id="75b7a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="75b7a-134">displayName</span></span>|<span data-ttu-id="75b7a-135">String</span><span class="sxs-lookup"><span data-stu-id="75b7a-135">String</span></span>|<span data-ttu-id="75b7a-136">Имя случая.</span><span class="sxs-lookup"><span data-stu-id="75b7a-136">The case name.</span></span>|
|<span data-ttu-id="75b7a-137">externalId</span><span class="sxs-lookup"><span data-stu-id="75b7a-137">externalId</span></span>|<span data-ttu-id="75b7a-138">String</span><span class="sxs-lookup"><span data-stu-id="75b7a-138">String</span></span>|<span data-ttu-id="75b7a-139">Внешний номер случая для клиентской ссылки.</span><span class="sxs-lookup"><span data-stu-id="75b7a-139">The external case number for customer reference.</span></span>|

## <a name="response"></a><span data-ttu-id="75b7a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="75b7a-140">Response</span></span>

<span data-ttu-id="75b7a-141">В случае успешного решения этот метод возвращает код ответа и обновленный `200 OK` [объект microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="75b7a-141">If successful, this method returns a `200 OK` response code and an updated [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75b7a-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="75b7a-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="75b7a-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="75b7a-143">Request</span></span>

<span data-ttu-id="75b7a-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75b7a-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="75b7a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="75b7a-145">HTTP</span></span>](#tab/http)

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

# <a name="c"></a>[<span data-ttu-id="75b7a-146">C#</span><span class="sxs-lookup"><span data-stu-id="75b7a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-case-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75b7a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75b7a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-case-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75b7a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75b7a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-case-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="75b7a-149">Java</span><span class="sxs-lookup"><span data-stu-id="75b7a-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-case-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="75b7a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="75b7a-150">Response</span></span>

<span data-ttu-id="75b7a-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="75b7a-151">The following is an example of the response.</span></span>

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
