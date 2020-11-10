---
title: Обновление учетной записи
description: Обновление свойств объекта учетной записи.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 6df75e05761d47e513272a222e956ee64235bde3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973962"
---
# <a name="update-webaccount"></a><span data-ttu-id="845d6-103">Обновление учетной записи</span><span class="sxs-lookup"><span data-stu-id="845d6-103">Update webAccount</span></span>

<span data-ttu-id="845d6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="845d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="845d6-105">Обновление свойств объекта [учетной записи](../resources/webaccount.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="845d6-105">Update the properties of a [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="845d6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="845d6-106">Permissions</span></span>

<span data-ttu-id="845d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="845d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="845d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="845d6-109">Permission type</span></span>                        | <span data-ttu-id="845d6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="845d6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="845d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="845d6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="845d6-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="845d6-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="845d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="845d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="845d6-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="845d6-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="845d6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="845d6-115">Application</span></span>                            | <span data-ttu-id="845d6-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="845d6-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="845d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="845d6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/webAccounts/{id}
PATCH /users/{id | userPrincipalName}/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="845d6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="845d6-118">Request headers</span></span>

| <span data-ttu-id="845d6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="845d6-119">Name</span></span>           |<span data-ttu-id="845d6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="845d6-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="845d6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="845d6-121">Authorization</span></span>  | <span data-ttu-id="845d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="845d6-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="845d6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="845d6-124">Content-Type</span></span>   | <span data-ttu-id="845d6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="845d6-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="845d6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="845d6-127">Request body</span></span>

<span data-ttu-id="845d6-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="845d6-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="845d6-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="845d6-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="845d6-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="845d6-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="845d6-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="845d6-131">Property</span></span>|<span data-ttu-id="845d6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="845d6-132">Type</span></span>|<span data-ttu-id="845d6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="845d6-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="845d6-134">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="845d6-134">allowedAudiences</span></span>|<span data-ttu-id="845d6-135">String</span><span class="sxs-lookup"><span data-stu-id="845d6-135">String</span></span>|<span data-ttu-id="845d6-136">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="845d6-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="845d6-137">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="845d6-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="845d6-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="845d6-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="845d6-139">description</span><span class="sxs-lookup"><span data-stu-id="845d6-139">description</span></span>|<span data-ttu-id="845d6-140">String</span><span class="sxs-lookup"><span data-stu-id="845d6-140">String</span></span>|<span data-ttu-id="845d6-141">Содержит описание, предоставленное пользователем для учетной записи службы, на которую выполняется ссылка.</span><span class="sxs-lookup"><span data-stu-id="845d6-141">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="845d6-142">выводов</span><span class="sxs-lookup"><span data-stu-id="845d6-142">inference</span></span>|[<span data-ttu-id="845d6-143">инференцедата</span><span class="sxs-lookup"><span data-stu-id="845d6-143">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="845d6-144">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="845d6-144">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="845d6-145">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="845d6-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="845d6-146">служба</span><span class="sxs-lookup"><span data-stu-id="845d6-146">service</span></span>|[<span data-ttu-id="845d6-147">сервицеинформатион</span><span class="sxs-lookup"><span data-stu-id="845d6-147">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="845d6-148">Содержит основные сведения о связанной службе.</span><span class="sxs-lookup"><span data-stu-id="845d6-148">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="845d6-149">статусмессаже</span><span class="sxs-lookup"><span data-stu-id="845d6-149">statusMessage</span></span>|<span data-ttu-id="845d6-150">String</span><span class="sxs-lookup"><span data-stu-id="845d6-150">String</span></span>|<span data-ttu-id="845d6-151">Содержит сообщение о состоянии от облачной службы, если оно предоставлено или синхронизировано.</span><span class="sxs-lookup"><span data-stu-id="845d6-151">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="845d6-152">userId</span><span class="sxs-lookup"><span data-stu-id="845d6-152">userId</span></span>|<span data-ttu-id="845d6-153">String</span><span class="sxs-lookup"><span data-stu-id="845d6-153">String</span></span>|<span data-ttu-id="845d6-154">Имя пользователя, отображаемое для учетной записи Account.</span><span class="sxs-lookup"><span data-stu-id="845d6-154">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="845d6-155">webUrl</span><span class="sxs-lookup"><span data-stu-id="845d6-155">webUrl</span></span>|<span data-ttu-id="845d6-156">String</span><span class="sxs-lookup"><span data-stu-id="845d6-156">String</span></span>|<span data-ttu-id="845d6-157">Содержит ссылку на профиль пользователя в облачной службе, если она существует.</span><span class="sxs-lookup"><span data-stu-id="845d6-157">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="response"></a><span data-ttu-id="845d6-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="845d6-158">Response</span></span>

<span data-ttu-id="845d6-159">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [учетной записи](../resources/webaccount.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="845d6-159">If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="845d6-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="845d6-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="845d6-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="845d6-161">Request</span></span>

<span data-ttu-id="845d6-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="845d6-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="845d6-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="845d6-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="845d6-164">C#</span><span class="sxs-lookup"><span data-stu-id="845d6-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="845d6-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="845d6-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="845d6-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="845d6-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="845d6-167">Java</span><span class="sxs-lookup"><span data-stu-id="845d6-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-webaccount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="845d6-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="845d6-168">Response</span></span>

<span data-ttu-id="845d6-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="845d6-169">The following is an example of the response.</span></span>

> <span data-ttu-id="845d6-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="845d6-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


