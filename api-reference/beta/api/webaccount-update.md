---
title: Обновление учетной записи
description: Обновление свойств объекта учетной записи.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: f13a7a350bb3fa2214061c3f8bc1c08a64267223
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996176"
---
# <a name="update-webaccount"></a><span data-ttu-id="15f60-103">Обновление учетной записи</span><span class="sxs-lookup"><span data-stu-id="15f60-103">Update webAccount</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15f60-104">Обновление свойств объекта [учетной записи](../resources/webaccount.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="15f60-104">Update the properties of a [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="15f60-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15f60-105">Permissions</span></span>

<span data-ttu-id="15f60-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15f60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15f60-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15f60-108">Permission type</span></span>                        | <span data-ttu-id="15f60-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15f60-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="15f60-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15f60-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="15f60-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="15f60-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="15f60-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15f60-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15f60-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="15f60-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="15f60-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15f60-114">Application</span></span>                            | <span data-ttu-id="15f60-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15f60-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="15f60-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15f60-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="15f60-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15f60-117">Request headers</span></span>

| <span data-ttu-id="15f60-118">Имя</span><span class="sxs-lookup"><span data-stu-id="15f60-118">Name</span></span>           |<span data-ttu-id="15f60-119">Описание</span><span class="sxs-lookup"><span data-stu-id="15f60-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="15f60-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15f60-120">Authorization</span></span>  | <span data-ttu-id="15f60-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15f60-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="15f60-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15f60-123">Content-Type</span></span>   | <span data-ttu-id="15f60-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15f60-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="15f60-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15f60-126">Request body</span></span>

<span data-ttu-id="15f60-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="15f60-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="15f60-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="15f60-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="15f60-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="15f60-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="15f60-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="15f60-130">Property</span></span>     | <span data-ttu-id="15f60-131">Тип</span><span class="sxs-lookup"><span data-stu-id="15f60-131">Type</span></span>                                                    | <span data-ttu-id="15f60-132">Описание</span><span class="sxs-lookup"><span data-stu-id="15f60-132">Description</span></span>                                                                                     |
|:-------------|:--------------------------------------------------------|:------------------------------------------------------------------------------------------------|
|<span data-ttu-id="15f60-133">description</span><span class="sxs-lookup"><span data-stu-id="15f60-133">description</span></span>   |<span data-ttu-id="15f60-134">String</span><span class="sxs-lookup"><span data-stu-id="15f60-134">String</span></span>                                                   | <span data-ttu-id="15f60-135">Содержит описание, предоставленное пользователем для учетной записи службы, на которую выполняется ссылка.</span><span class="sxs-lookup"><span data-stu-id="15f60-135">Contains the description the user has provided for the account on the service being referenced.</span></span> |
|<span data-ttu-id="15f60-136">service</span><span class="sxs-lookup"><span data-stu-id="15f60-136">service</span></span>       |[<span data-ttu-id="15f60-137">сервицеинформатион</span><span class="sxs-lookup"><span data-stu-id="15f60-137">serviceInformation</span></span>](../resources/serviceinformation.md) | <span data-ttu-id="15f60-138">Представляет основные описательные данные об облачной службе, предоставленной пользователем.</span><span class="sxs-lookup"><span data-stu-id="15f60-138">Represents the basic descriptive data about cloud service provided by a user.</span></span>                   |
|<span data-ttu-id="15f60-139">статусмессаже</span><span class="sxs-lookup"><span data-stu-id="15f60-139">statusMessage</span></span> |<span data-ttu-id="15f60-140">String</span><span class="sxs-lookup"><span data-stu-id="15f60-140">String</span></span>                                                   | <span data-ttu-id="15f60-141">Содержит сообщение о состоянии от облачной службы, если оно предоставлено или синхронизировано.</span><span class="sxs-lookup"><span data-stu-id="15f60-141">Contains a status message from the cloud service if provided or synchronized.</span></span>                   |
|<span data-ttu-id="15f60-142">userId</span><span class="sxs-lookup"><span data-stu-id="15f60-142">userId</span></span>        |<span data-ttu-id="15f60-143">String</span><span class="sxs-lookup"><span data-stu-id="15f60-143">String</span></span>                                                   | <span data-ttu-id="15f60-144">Имя пользователя, отображаемое для учетной записи Account (например, @kevinb).</span><span class="sxs-lookup"><span data-stu-id="15f60-144">The user name  displayed for the webaccount (for example, @kevinb).</span></span>                                       |
|<span data-ttu-id="15f60-145">webUrl</span><span class="sxs-lookup"><span data-stu-id="15f60-145">webUrl</span></span>        |<span data-ttu-id="15f60-146">String</span><span class="sxs-lookup"><span data-stu-id="15f60-146">String</span></span>                                                   | <span data-ttu-id="15f60-147">Содержит ссылку на профиль пользователя в облачной службе, если она существует.</span><span class="sxs-lookup"><span data-stu-id="15f60-147">Contains a link to the users profile on the cloud service if one exists.</span></span>                        |

## <a name="response"></a><span data-ttu-id="15f60-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="15f60-148">Response</span></span>

<span data-ttu-id="15f60-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [учетной записи](../resources/webaccount.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15f60-149">If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15f60-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="15f60-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="15f60-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="15f60-151">Request</span></span>

<span data-ttu-id="15f60-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15f60-152">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="15f60-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="15f60-153">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="15f60-154">C#</span><span class="sxs-lookup"><span data-stu-id="15f60-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="15f60-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15f60-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="15f60-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15f60-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="15f60-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="15f60-157">Response</span></span>

<span data-ttu-id="15f60-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="15f60-158">The following is an example of the response.</span></span>

> <span data-ttu-id="15f60-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15f60-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
