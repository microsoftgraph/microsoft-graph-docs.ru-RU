---
title: Обновление Персонанниверсари
description: Обновление свойств объекта персонанниверсари.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: fd3ba313d992f2904ac57a1d650af6245a337b3d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455934"
---
# <a name="update-personanniversary"></a><span data-ttu-id="57eb5-103">Обновление Персонанниверсари</span><span class="sxs-lookup"><span data-stu-id="57eb5-103">Update personAnniversary</span></span>

<span data-ttu-id="57eb5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="57eb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57eb5-105">Обновление свойств объекта [персонанниверсари](../resources/personanniversary.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="57eb5-105">Update the properties of a [personAnniversary](../resources/personanniversary.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="57eb5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57eb5-106">Permissions</span></span>

<span data-ttu-id="57eb5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57eb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57eb5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57eb5-109">Permission type</span></span>                        | <span data-ttu-id="57eb5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57eb5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="57eb5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57eb5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="57eb5-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="57eb5-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="57eb5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57eb5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57eb5-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="57eb5-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="57eb5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57eb5-115">Application</span></span>                            | <span data-ttu-id="57eb5-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57eb5-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="57eb5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57eb5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/anniversaries/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="57eb5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57eb5-118">Request headers</span></span>

| <span data-ttu-id="57eb5-119">Имя</span><span class="sxs-lookup"><span data-stu-id="57eb5-119">Name</span></span>           |<span data-ttu-id="57eb5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="57eb5-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="57eb5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57eb5-121">Authorization</span></span>  | <span data-ttu-id="57eb5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57eb5-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="57eb5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57eb5-124">Content-Type</span></span>   | <span data-ttu-id="57eb5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57eb5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="57eb5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="57eb5-127">Request body</span></span>

<span data-ttu-id="57eb5-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="57eb5-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="57eb5-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="57eb5-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="57eb5-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="57eb5-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="57eb5-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="57eb5-131">Property</span></span>     | <span data-ttu-id="57eb5-132">Тип</span><span class="sxs-lookup"><span data-stu-id="57eb5-132">Type</span></span>        | <span data-ttu-id="57eb5-133">Описание</span><span class="sxs-lookup"><span data-stu-id="57eb5-133">Description</span></span>                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|<span data-ttu-id="57eb5-134">date</span><span class="sxs-lookup"><span data-stu-id="57eb5-134">date</span></span>          |<span data-ttu-id="57eb5-135">Date</span><span class="sxs-lookup"><span data-stu-id="57eb5-135">Date</span></span>         | <span data-ttu-id="57eb5-136">Содержит дату, связанную с типом юбилея.</span><span class="sxs-lookup"><span data-stu-id="57eb5-136">Contains the date associated with the anniversary type.</span></span>          |
|<span data-ttu-id="57eb5-137">type</span><span class="sxs-lookup"><span data-stu-id="57eb5-137">type</span></span>          |<span data-ttu-id="57eb5-138">string</span><span class="sxs-lookup"><span data-stu-id="57eb5-138">string</span></span>       | <span data-ttu-id="57eb5-139">Возможные значения: `birthday`, `wedding`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="57eb5-139">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="57eb5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="57eb5-140">Response</span></span>

<span data-ttu-id="57eb5-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [персонанниверсари](../resources/personanniversary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57eb5-141">If successful, this method returns a `200 OK` response code and an updated [personAnniversary](../resources/personanniversary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57eb5-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="57eb5-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="57eb5-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="57eb5-143">Request</span></span>

<span data-ttu-id="57eb5-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57eb5-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="57eb5-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="57eb5-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personanniversary"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/anniversaries/{id}
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```
# <a name="c"></a>[<span data-ttu-id="57eb5-146">C#</span><span class="sxs-lookup"><span data-stu-id="57eb5-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personanniversary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57eb5-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57eb5-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personanniversary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57eb5-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57eb5-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personanniversary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="57eb5-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="57eb5-149">Response</span></span>

<span data-ttu-id="57eb5-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="57eb5-150">The following is an example of the response.</span></span>

> <span data-ttu-id="57eb5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="57eb5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnniversary"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "type": "type-value",
  "date": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personanniversary",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
