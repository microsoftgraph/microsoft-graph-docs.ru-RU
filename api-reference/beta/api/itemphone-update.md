---
title: Обновление итемфоне
description: Обновление свойств объекта итемфоне.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a7959b4233323b8987a36f67fb3b4eb13a384972
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42457233"
---
# <a name="update-itemphonenumber"></a><span data-ttu-id="6e58c-103">Обновление итемфоненумбер</span><span class="sxs-lookup"><span data-stu-id="6e58c-103">Update itemphonenumber</span></span>

<span data-ttu-id="6e58c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6e58c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e58c-105">Обновление свойств объекта [итемфоне](../resources/itemphone.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e58c-105">Update the properties of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6e58c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e58c-106">Permissions</span></span>

<span data-ttu-id="6e58c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e58c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e58c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e58c-109">Permission type</span></span>                        | <span data-ttu-id="6e58c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e58c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6e58c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e58c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e58c-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6e58c-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6e58c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e58c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e58c-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6e58c-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="6e58c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e58c-115">Application</span></span>                            | <span data-ttu-id="6e58c-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e58c-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="6e58c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e58c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/phones/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="6e58c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e58c-118">Request headers</span></span>

| <span data-ttu-id="6e58c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6e58c-119">Name</span></span>           |<span data-ttu-id="6e58c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6e58c-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="6e58c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e58c-121">Authorization</span></span>  | <span data-ttu-id="6e58c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e58c-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="6e58c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e58c-124">Content-Type</span></span>   | <span data-ttu-id="6e58c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e58c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e58c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e58c-127">Request body</span></span>

<span data-ttu-id="6e58c-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6e58c-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6e58c-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="6e58c-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6e58c-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6e58c-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6e58c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e58c-131">Property</span></span>     | <span data-ttu-id="6e58c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="6e58c-132">Type</span></span>        | <span data-ttu-id="6e58c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="6e58c-133">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="6e58c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6e58c-134">displayName</span></span>   |<span data-ttu-id="6e58c-135">Строка</span><span class="sxs-lookup"><span data-stu-id="6e58c-135">String</span></span>       | <span data-ttu-id="6e58c-136">Содержит понятное имя для номера телефона.</span><span class="sxs-lookup"><span data-stu-id="6e58c-136">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="6e58c-137">число</span><span class="sxs-lookup"><span data-stu-id="6e58c-137">number</span></span>        |<span data-ttu-id="6e58c-138">String</span><span class="sxs-lookup"><span data-stu-id="6e58c-138">String</span></span>       | <span data-ttu-id="6e58c-139">Содержит номер телефона.</span><span class="sxs-lookup"><span data-stu-id="6e58c-139">Contains the phone number.</span></span>                                                                                                      |
|<span data-ttu-id="6e58c-140">type</span><span class="sxs-lookup"><span data-stu-id="6e58c-140">type</span></span>          |<span data-ttu-id="6e58c-141">string</span><span class="sxs-lookup"><span data-stu-id="6e58c-141">string</span></span>       | <span data-ttu-id="6e58c-142">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="6e58c-142">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="6e58c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e58c-143">Response</span></span>

<span data-ttu-id="6e58c-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [итемфоне](../resources/itemphone.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6e58c-144">If successful, this method returns a `200 OK` response code and an updated [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e58c-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="6e58c-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e58c-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e58c-146">Request</span></span>

<span data-ttu-id="6e58c-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e58c-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6e58c-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e58c-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itemphone"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/phones/{id}
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6e58c-149">C#</span><span class="sxs-lookup"><span data-stu-id="6e58c-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-itemphone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6e58c-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e58c-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-itemphone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6e58c-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e58c-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-itemphone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6e58c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e58c-152">Response</span></span>

<span data-ttu-id="6e58c-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6e58c-153">The following is an example of the response.</span></span>

> <span data-ttu-id="6e58c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e58c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemPhone"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "displayName-value",
  "type": "type-value",
  "number": "number-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update itemphone",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
