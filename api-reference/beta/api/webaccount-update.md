---
title: Обновление webAccount
description: Обновление свойств объекта webAccount.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: bc907445655085ff863094f58d2afe337a9074fe
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050712"
---
# <a name="update-webaccount"></a><span data-ttu-id="71dd3-103">Обновление webAccount</span><span class="sxs-lookup"><span data-stu-id="71dd3-103">Update webAccount</span></span>

<span data-ttu-id="71dd3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71dd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71dd3-105">Обновление свойств объекта [webAccount](../resources/webaccount.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="71dd3-105">Update the properties of a [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="71dd3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71dd3-106">Permissions</span></span>

<span data-ttu-id="71dd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71dd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71dd3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71dd3-109">Permission type</span></span>                        | <span data-ttu-id="71dd3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71dd3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="71dd3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71dd3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="71dd3-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71dd3-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="71dd3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71dd3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71dd3-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71dd3-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="71dd3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71dd3-115">Application</span></span>                            | <span data-ttu-id="71dd3-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71dd3-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="71dd3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71dd3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/webAccounts/{id}
PATCH /users/{id | userPrincipalName}/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="71dd3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71dd3-118">Request headers</span></span>

| <span data-ttu-id="71dd3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="71dd3-119">Name</span></span>           |<span data-ttu-id="71dd3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="71dd3-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="71dd3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71dd3-121">Authorization</span></span>  | <span data-ttu-id="71dd3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71dd3-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="71dd3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71dd3-124">Content-Type</span></span>   | <span data-ttu-id="71dd3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71dd3-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="71dd3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71dd3-127">Request body</span></span>

<span data-ttu-id="71dd3-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="71dd3-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="71dd3-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="71dd3-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="71dd3-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="71dd3-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="71dd3-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="71dd3-131">Property</span></span>|<span data-ttu-id="71dd3-132">Тип</span><span class="sxs-lookup"><span data-stu-id="71dd3-132">Type</span></span>|<span data-ttu-id="71dd3-133">Описание</span><span class="sxs-lookup"><span data-stu-id="71dd3-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71dd3-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="71dd3-134">allowedAudiences</span></span>|<span data-ttu-id="71dd3-135">String</span><span class="sxs-lookup"><span data-stu-id="71dd3-135">String</span></span>|<span data-ttu-id="71dd3-136">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="71dd3-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="71dd3-137">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="71dd3-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="71dd3-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="71dd3-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="71dd3-139">description</span><span class="sxs-lookup"><span data-stu-id="71dd3-139">description</span></span>|<span data-ttu-id="71dd3-140">String</span><span class="sxs-lookup"><span data-stu-id="71dd3-140">String</span></span>|<span data-ttu-id="71dd3-141">Содержит описание, предоставленное пользователем для учетной записи в службе, на который ссылается.</span><span class="sxs-lookup"><span data-stu-id="71dd3-141">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="71dd3-142">вывод</span><span class="sxs-lookup"><span data-stu-id="71dd3-142">inference</span></span>|[<span data-ttu-id="71dd3-143">inferenceData</span><span class="sxs-lookup"><span data-stu-id="71dd3-143">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="71dd3-144">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="71dd3-144">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="71dd3-145">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="71dd3-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="71dd3-146">служба</span><span class="sxs-lookup"><span data-stu-id="71dd3-146">service</span></span>|[<span data-ttu-id="71dd3-147">serviceInformation</span><span class="sxs-lookup"><span data-stu-id="71dd3-147">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="71dd3-148">Содержит основные сведения о связанной службе.</span><span class="sxs-lookup"><span data-stu-id="71dd3-148">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="71dd3-149">statusMessage</span><span class="sxs-lookup"><span data-stu-id="71dd3-149">statusMessage</span></span>|<span data-ttu-id="71dd3-150">String</span><span class="sxs-lookup"><span data-stu-id="71dd3-150">String</span></span>|<span data-ttu-id="71dd3-151">Содержит сообщение о состоянии облачной службы при условии или синхронизации.</span><span class="sxs-lookup"><span data-stu-id="71dd3-151">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="71dd3-152">userId</span><span class="sxs-lookup"><span data-stu-id="71dd3-152">userId</span></span>|<span data-ttu-id="71dd3-153">String</span><span class="sxs-lookup"><span data-stu-id="71dd3-153">String</span></span>|<span data-ttu-id="71dd3-154">Имя пользователя, отображаемая для webaccount.</span><span class="sxs-lookup"><span data-stu-id="71dd3-154">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="71dd3-155">webUrl</span><span class="sxs-lookup"><span data-stu-id="71dd3-155">webUrl</span></span>|<span data-ttu-id="71dd3-156">String</span><span class="sxs-lookup"><span data-stu-id="71dd3-156">String</span></span>|<span data-ttu-id="71dd3-157">Содержит ссылку на профиль пользователя в облачной службе, если она существует.</span><span class="sxs-lookup"><span data-stu-id="71dd3-157">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="response"></a><span data-ttu-id="71dd3-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="71dd3-158">Response</span></span>

<span data-ttu-id="71dd3-159">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект webAccount](../resources/webaccount.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="71dd3-159">If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="71dd3-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="71dd3-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="71dd3-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="71dd3-161">Request</span></span>

<span data-ttu-id="71dd3-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71dd3-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71dd3-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="71dd3-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_webaccount"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/webAccounts/{id}
Content-type: application/json

{
  "webUrl": "https://github.com/innocenty.popov"
}
```
# <a name="c"></a>[<span data-ttu-id="71dd3-164">C#</span><span class="sxs-lookup"><span data-stu-id="71dd3-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71dd3-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71dd3-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71dd3-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71dd3-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71dd3-167">Java</span><span class="sxs-lookup"><span data-stu-id="71dd3-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-webaccount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="71dd3-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="71dd3-168">Response</span></span>

<span data-ttu-id="71dd3-169">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="71dd3-169">The following is an example of the response.</span></span>

> <span data-ttu-id="71dd3-170">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71dd3-170">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "description": "My Github contributions!",
  "userId": "innocenty.popov",
  "service": {
    "name": "GitHub",
    "webUrl": "https://github.com"
  },
  "statusMessage": null,
  "webUrl": "https://github.com/innocenty.popov"
}
```


