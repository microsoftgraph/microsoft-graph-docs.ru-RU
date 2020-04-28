---
title: Обновление Персонинтерест
description: Обновление свойств объекта Персонинтерест.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: d5692b973e3c50e67f99efea971d19ade6d2699b
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228522"
---
# <a name="update-personinterest"></a><span data-ttu-id="4b8f6-103">Обновление персонинтерест</span><span class="sxs-lookup"><span data-stu-id="4b8f6-103">Update personinterest</span></span>

<span data-ttu-id="4b8f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b8f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b8f6-105">Обновление свойств объекта [персонинтерест](../resources/personinterest.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-105">Update the properties of a [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4b8f6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4b8f6-106">Permissions</span></span>

<span data-ttu-id="4b8f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b8f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4b8f6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b8f6-109">Permission type</span></span>                        | <span data-ttu-id="4b8f6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b8f6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4b8f6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b8f6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4b8f6-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4b8f6-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4b8f6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b8f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b8f6-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4b8f6-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="4b8f6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b8f6-115">Application</span></span>                            | <span data-ttu-id="4b8f6-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b8f6-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="4b8f6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b8f6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/interests/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4b8f6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b8f6-118">Request headers</span></span>

| <span data-ttu-id="4b8f6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4b8f6-119">Name</span></span>           |<span data-ttu-id="4b8f6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4b8f6-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="4b8f6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b8f6-121">Authorization</span></span>  | <span data-ttu-id="4b8f6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="4b8f6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4b8f6-124">Content-Type</span></span>   | <span data-ttu-id="4b8f6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b8f6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b8f6-127">Request body</span></span>

<span data-ttu-id="4b8f6-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4b8f6-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4b8f6-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4b8f6-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b8f6-131">Property</span></span>     | <span data-ttu-id="4b8f6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4b8f6-132">Type</span></span>             | <span data-ttu-id="4b8f6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4b8f6-133">Description</span></span>                                                                         |
|:-------------|:-----------------|:------------------------------------------------------------------------------------|
|<span data-ttu-id="4b8f6-134">categories</span><span class="sxs-lookup"><span data-stu-id="4b8f6-134">categories</span></span>    |<span data-ttu-id="4b8f6-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b8f6-135">String collection</span></span> | <span data-ttu-id="4b8f6-136">Содержит категории, которые пользователь связал с интересом (например: личное, реЦипиес)</span><span class="sxs-lookup"><span data-stu-id="4b8f6-136">Contains categories a user has associated with the interest (eg: personal, recipies)</span></span>|
|<span data-ttu-id="4b8f6-137">description</span><span class="sxs-lookup"><span data-stu-id="4b8f6-137">description</span></span>   |<span data-ttu-id="4b8f6-138">String</span><span class="sxs-lookup"><span data-stu-id="4b8f6-138">String</span></span>            | <span data-ttu-id="4b8f6-139">Содержит описание интереса.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-139">Contains a description of the interest.</span></span>                                             |
|<span data-ttu-id="4b8f6-140">displayName</span><span class="sxs-lookup"><span data-stu-id="4b8f6-140">displayName</span></span>   |<span data-ttu-id="4b8f6-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4b8f6-141">String</span></span>            | <span data-ttu-id="4b8f6-142">Содержит понятное имя для интереса.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-142">Contains a friendly name for the interest.</span></span>                                          |
|<span data-ttu-id="4b8f6-143">webUrl</span><span class="sxs-lookup"><span data-stu-id="4b8f6-143">webUrl</span></span>        |<span data-ttu-id="4b8f6-144">String</span><span class="sxs-lookup"><span data-stu-id="4b8f6-144">String</span></span>            | <span data-ttu-id="4b8f6-145">Содержит ссылку на источник информации о процентах.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-145">Contains a link to an information source about the interest.</span></span>                        |

## <a name="response"></a><span data-ttu-id="4b8f6-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="4b8f6-146">Response</span></span>

<span data-ttu-id="4b8f6-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [персонинтерест](../resources/personinterest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-147">If successful, this method returns a `200 OK` response code and an updated [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4b8f6-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="4b8f6-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4b8f6-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b8f6-149">Request</span></span>

<span data-ttu-id="4b8f6-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4b8f6-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b8f6-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_personinterest"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/interests/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```
# <a name="c"></a>[<span data-ttu-id="4b8f6-152">C#</span><span class="sxs-lookup"><span data-stu-id="4b8f6-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-personinterest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b8f6-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b8f6-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-personinterest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b8f6-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b8f6-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-personinterest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b8f6-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b8f6-155">Response</span></span>

<span data-ttu-id="4b8f6-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-156">The following is an example of the response.</span></span>

> <span data-ttu-id="4b8f6-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b8f6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "description": "description-value",
  "displayName": "displayName-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update personinterest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
