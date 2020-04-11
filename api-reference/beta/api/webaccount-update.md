---
title: Обновление учетной записи
description: Обновление свойств объекта учетной записи.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bf31a230d9e77a64905bf04b2ee26215bb47375f
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229061"
---
# <a name="update-webaccount"></a><span data-ttu-id="e9ed1-103">Обновление учетной записи</span><span class="sxs-lookup"><span data-stu-id="e9ed1-103">Update webAccount</span></span>

<span data-ttu-id="e9ed1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9ed1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9ed1-105">Обновление свойств объекта [учетной записи](../resources/webaccount.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-105">Update the properties of a [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e9ed1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e9ed1-106">Permissions</span></span>

<span data-ttu-id="e9ed1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9ed1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e9ed1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9ed1-109">Permission type</span></span>                        | <span data-ttu-id="e9ed1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9ed1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e9ed1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9ed1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e9ed1-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e9ed1-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e9ed1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9ed1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9ed1-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e9ed1-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="e9ed1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9ed1-115">Application</span></span>                            | <span data-ttu-id="e9ed1-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9ed1-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="e9ed1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9ed1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e9ed1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e9ed1-118">Request headers</span></span>

| <span data-ttu-id="e9ed1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e9ed1-119">Name</span></span>           |<span data-ttu-id="e9ed1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e9ed1-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="e9ed1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9ed1-121">Authorization</span></span>  | <span data-ttu-id="e9ed1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="e9ed1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9ed1-124">Content-Type</span></span>   | <span data-ttu-id="e9ed1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e9ed1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e9ed1-127">Request body</span></span>

<span data-ttu-id="e9ed1-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e9ed1-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e9ed1-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e9ed1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9ed1-131">Property</span></span>     | <span data-ttu-id="e9ed1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="e9ed1-132">Type</span></span>                                                    | <span data-ttu-id="e9ed1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="e9ed1-133">Description</span></span>                                                                                     |
|:-------------|:--------------------------------------------------------|:------------------------------------------------------------------------------------------------|
|<span data-ttu-id="e9ed1-134">description</span><span class="sxs-lookup"><span data-stu-id="e9ed1-134">description</span></span>   |<span data-ttu-id="e9ed1-135">String</span><span class="sxs-lookup"><span data-stu-id="e9ed1-135">String</span></span>                                                   | <span data-ttu-id="e9ed1-136">Содержит описание, предоставленное пользователем для учетной записи службы, на которую выполняется ссылка.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-136">Contains the description the user has provided for the account on the service being referenced.</span></span> |
|<span data-ttu-id="e9ed1-137">service</span><span class="sxs-lookup"><span data-stu-id="e9ed1-137">service</span></span>       |[<span data-ttu-id="e9ed1-138">сервицеинформатион</span><span class="sxs-lookup"><span data-stu-id="e9ed1-138">serviceInformation</span></span>](../resources/serviceinformation.md) | <span data-ttu-id="e9ed1-139">Представляет основные описательные данные об облачной службе, предоставленной пользователем.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-139">Represents the basic descriptive data about cloud service provided by a user.</span></span>                   |
|<span data-ttu-id="e9ed1-140">статусмессаже</span><span class="sxs-lookup"><span data-stu-id="e9ed1-140">statusMessage</span></span> |<span data-ttu-id="e9ed1-141">String</span><span class="sxs-lookup"><span data-stu-id="e9ed1-141">String</span></span>                                                   | <span data-ttu-id="e9ed1-142">Содержит сообщение о состоянии от облачной службы, если оно предоставлено или синхронизировано.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-142">Contains a status message from the cloud service if provided or synchronized.</span></span>                   |
|<span data-ttu-id="e9ed1-143">userId</span><span class="sxs-lookup"><span data-stu-id="e9ed1-143">userId</span></span>        |<span data-ttu-id="e9ed1-144">String</span><span class="sxs-lookup"><span data-stu-id="e9ed1-144">String</span></span>                                                   | <span data-ttu-id="e9ed1-145">Имя пользователя, отображаемое для учетной записи Account (например, @kevinb).</span><span class="sxs-lookup"><span data-stu-id="e9ed1-145">The user name  displayed for the webaccount (for example, @kevinb).</span></span>                             |
|<span data-ttu-id="e9ed1-146">webUrl</span><span class="sxs-lookup"><span data-stu-id="e9ed1-146">webUrl</span></span>        |<span data-ttu-id="e9ed1-147">String</span><span class="sxs-lookup"><span data-stu-id="e9ed1-147">String</span></span>                                                   | <span data-ttu-id="e9ed1-148">Содержит ссылку на профиль пользователя в облачной службе, если она существует.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-148">Contains a link to the users profile on the cloud service if one exists.</span></span>                        |

## <a name="response"></a><span data-ttu-id="e9ed1-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9ed1-149">Response</span></span>

<span data-ttu-id="e9ed1-150">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [учетной записи](../resources/webaccount.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-150">If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9ed1-151">Примеры</span><span class="sxs-lookup"><span data-stu-id="e9ed1-151">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9ed1-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9ed1-152">Request</span></span>

<span data-ttu-id="e9ed1-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-153">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e9ed1-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="e9ed1-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_webaccount"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```
# <a name="c"></a>[<span data-ttu-id="e9ed1-155">C#</span><span class="sxs-lookup"><span data-stu-id="e9ed1-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e9ed1-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e9ed1-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e9ed1-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e9ed1-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e9ed1-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9ed1-158">Response</span></span>

<span data-ttu-id="e9ed1-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-159">The following is an example of the response.</span></span>

> <span data-ttu-id="e9ed1-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9ed1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "description": "description-value",
  "userId": "userId-value",
  "service": {
    "name": "name-value",
    "webUrl": "webUrl-value"
  },
  "statusMessage": "statusMessage-value",
  "webUrl": "webUrl-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update webaccount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
