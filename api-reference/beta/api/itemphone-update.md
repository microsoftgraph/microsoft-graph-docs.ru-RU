---
title: Обновление итемфоне
description: Обновление свойств объекта итемфоне.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b93d76dabf1aef7b45e77fd9a3020fb5da96ab01
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997342"
---
# <a name="update-itemphonenumber"></a><span data-ttu-id="df104-103">Обновление итемфоненумбер</span><span class="sxs-lookup"><span data-stu-id="df104-103">Update itemphonenumber</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df104-104">Обновление свойств объекта [итемфоне](../resources/itemphone.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="df104-104">Update the properties of an [itemPhone](../resources/itemphone.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df104-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df104-105">Permissions</span></span>

<span data-ttu-id="df104-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df104-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df104-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df104-108">Permission type</span></span>                        | <span data-ttu-id="df104-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df104-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="df104-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df104-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="df104-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="df104-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="df104-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df104-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df104-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="df104-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="df104-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df104-114">Application</span></span>                            | <span data-ttu-id="df104-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df104-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="df104-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df104-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/phones/{id} 
```

## <a name="request-headers"></a><span data-ttu-id="df104-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df104-117">Request headers</span></span>

| <span data-ttu-id="df104-118">Имя</span><span class="sxs-lookup"><span data-stu-id="df104-118">Name</span></span>           |<span data-ttu-id="df104-119">Описание</span><span class="sxs-lookup"><span data-stu-id="df104-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="df104-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df104-120">Authorization</span></span>  | <span data-ttu-id="df104-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df104-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="df104-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df104-123">Content-Type</span></span>   | <span data-ttu-id="df104-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df104-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df104-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df104-126">Request body</span></span>

<span data-ttu-id="df104-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="df104-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="df104-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="df104-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="df104-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="df104-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="df104-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="df104-130">Property</span></span>     | <span data-ttu-id="df104-131">Тип</span><span class="sxs-lookup"><span data-stu-id="df104-131">Type</span></span>        | <span data-ttu-id="df104-132">Описание</span><span class="sxs-lookup"><span data-stu-id="df104-132">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="df104-133">displayName</span><span class="sxs-lookup"><span data-stu-id="df104-133">displayName</span></span>   |<span data-ttu-id="df104-134">Строка</span><span class="sxs-lookup"><span data-stu-id="df104-134">String</span></span>       | <span data-ttu-id="df104-135">Содержит понятное имя для номера телефона.</span><span class="sxs-lookup"><span data-stu-id="df104-135">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="df104-136">число</span><span class="sxs-lookup"><span data-stu-id="df104-136">number</span></span>        |<span data-ttu-id="df104-137">String</span><span class="sxs-lookup"><span data-stu-id="df104-137">String</span></span>       | <span data-ttu-id="df104-138">Содержит номер телефона.</span><span class="sxs-lookup"><span data-stu-id="df104-138">Contains the phone number.</span></span>                                                                                                      |
|<span data-ttu-id="df104-139">type</span><span class="sxs-lookup"><span data-stu-id="df104-139">type</span></span>          |<span data-ttu-id="df104-140">string</span><span class="sxs-lookup"><span data-stu-id="df104-140">string</span></span>       | <span data-ttu-id="df104-141">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="df104-141">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="response"></a><span data-ttu-id="df104-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="df104-142">Response</span></span>

<span data-ttu-id="df104-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [итемфоне](../resources/itemphone.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df104-143">If successful, this method returns a `200 OK` response code and an updated [itemPhone](../resources/itemphone.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df104-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="df104-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df104-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="df104-145">Request</span></span>

<span data-ttu-id="df104-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df104-146">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="df104-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="df104-147">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="df104-148">C#</span><span class="sxs-lookup"><span data-stu-id="df104-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-itemphone-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df104-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df104-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-itemphone-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="df104-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df104-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-itemphone-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df104-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="df104-151">Response</span></span>

<span data-ttu-id="df104-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="df104-152">The following is an example of the response.</span></span>

> <span data-ttu-id="df104-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df104-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
