---
title: Обновление итемемаил
description: Обновление свойств объекта Итемемаил в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: e304ce5e92a4ef0fa64b2b7e2044887d86477255
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229040"
---
# <a name="update-itememail"></a><span data-ttu-id="0e20a-103">Обновление итемемаил</span><span class="sxs-lookup"><span data-stu-id="0e20a-103">Update itememail</span></span>

<span data-ttu-id="0e20a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e20a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e20a-105">Обновление свойств объекта [итемемаил](../resources/itememail.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="0e20a-105">Update the properties of an [itemEmail](../resources/itememail.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e20a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e20a-106">Permissions</span></span>

<span data-ttu-id="0e20a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e20a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e20a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e20a-109">Permission type</span></span>                        | <span data-ttu-id="0e20a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e20a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0e20a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e20a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e20a-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0e20a-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0e20a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e20a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e20a-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0e20a-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0e20a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e20a-115">Application</span></span>                            | <span data-ttu-id="0e20a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e20a-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="0e20a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e20a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/emails/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0e20a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e20a-118">Request headers</span></span>

| <span data-ttu-id="0e20a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0e20a-119">Name</span></span>           |<span data-ttu-id="0e20a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0e20a-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="0e20a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e20a-121">Authorization</span></span>  | <span data-ttu-id="0e20a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e20a-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="0e20a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e20a-124">Content-Type</span></span>   | <span data-ttu-id="0e20a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e20a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e20a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e20a-127">Request body</span></span>

<span data-ttu-id="0e20a-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="0e20a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0e20a-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="0e20a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0e20a-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="0e20a-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0e20a-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e20a-131">Property</span></span>     | <span data-ttu-id="0e20a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="0e20a-132">Type</span></span>        | <span data-ttu-id="0e20a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="0e20a-133">Description</span></span>                                                              |
|:-------------|:------------|:-------------------------------------------------------------------------|
|<span data-ttu-id="0e20a-134">address</span><span class="sxs-lookup"><span data-stu-id="0e20a-134">address</span></span>       |<span data-ttu-id="0e20a-135">String</span><span class="sxs-lookup"><span data-stu-id="0e20a-135">String</span></span>       | <span data-ttu-id="0e20a-136">Сам адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0e20a-136">The email address itself.</span></span>                                                |
|<span data-ttu-id="0e20a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0e20a-137">displayName</span></span>   |<span data-ttu-id="0e20a-138">Строка</span><span class="sxs-lookup"><span data-stu-id="0e20a-138">String</span></span>       | <span data-ttu-id="0e20a-139">Имя или метка, с которыми пользователь связан с определенным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0e20a-139">The name or label a user has associated with a particular email address.</span></span> |
|<span data-ttu-id="0e20a-140">type</span><span class="sxs-lookup"><span data-stu-id="0e20a-140">type</span></span>          |<span data-ttu-id="0e20a-141">строка</span><span class="sxs-lookup"><span data-stu-id="0e20a-141">string</span></span>       | <span data-ttu-id="0e20a-142">Возможные значения: `unknown`, `work`, `personal`, `main`, `other`.</span><span class="sxs-lookup"><span data-stu-id="0e20a-142">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>     |

## <a name="response"></a><span data-ttu-id="0e20a-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e20a-143">Response</span></span>

<span data-ttu-id="0e20a-144">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [итемемаил](../resources/itememail.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0e20a-144">If successful, this method returns a `200 OK` response code and an updated [itemEmail](../resources/itememail.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e20a-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="0e20a-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e20a-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e20a-146">Request</span></span>

<span data-ttu-id="0e20a-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e20a-147">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e20a-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e20a-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_itememail"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/emails/{id}
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

# <a name="c"></a>[<span data-ttu-id="0e20a-149">C#</span><span class="sxs-lookup"><span data-stu-id="0e20a-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-itememail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e20a-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e20a-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-itememail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e20a-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e20a-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-itememail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="0e20a-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e20a-152">Response</span></span>

<span data-ttu-id="0e20a-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0e20a-153">The following is an example of the response.</span></span>

> <span data-ttu-id="0e20a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e20a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemEmail"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "address": "address-value",
  "displayName": "displayName-value",
  "type": "type-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update itememail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
