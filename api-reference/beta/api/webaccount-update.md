---
title: Обновление webAccount
description: Обновление свойств объекта webAccount.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b2eb21947edb12693ba44cdb2d19ba535df03306
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819608"
---
# <a name="update-webaccount"></a><span data-ttu-id="d4a1b-103">Обновление webAccount</span><span class="sxs-lookup"><span data-stu-id="d4a1b-103">Update webAccount</span></span>

<span data-ttu-id="d4a1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4a1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4a1b-105">Обновление свойств объекта [webAccount](../resources/webaccount.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="d4a1b-105">Update the properties of a [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4a1b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d4a1b-106">Permissions</span></span>

<span data-ttu-id="d4a1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4a1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4a1b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d4a1b-109">Permission type</span></span>                        | <span data-ttu-id="d4a1b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d4a1b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4a1b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d4a1b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4a1b-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a1b-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d4a1b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d4a1b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4a1b-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a1b-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d4a1b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d4a1b-115">Application</span></span>                            | <span data-ttu-id="d4a1b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4a1b-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="d4a1b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d4a1b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/webAccounts/{id}
PATCH /users/{id | userPrincipalName}/profile/webAccounts/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d4a1b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d4a1b-118">Request headers</span></span>

| <span data-ttu-id="d4a1b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d4a1b-119">Name</span></span>           |<span data-ttu-id="d4a1b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d4a1b-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="d4a1b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d4a1b-121">Authorization</span></span>  | <span data-ttu-id="d4a1b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d4a1b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4a1b-124">Content-Type</span></span>   | <span data-ttu-id="d4a1b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d4a1b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d4a1b-127">Request body</span></span>

<span data-ttu-id="d4a1b-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d4a1b-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d4a1b-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="d4a1b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4a1b-131">Property</span></span>|<span data-ttu-id="d4a1b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="d4a1b-132">Type</span></span>|<span data-ttu-id="d4a1b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="d4a1b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4a1b-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="d4a1b-134">allowedAudiences</span></span>|<span data-ttu-id="d4a1b-135">String</span><span class="sxs-lookup"><span data-stu-id="d4a1b-135">String</span></span>|<span data-ttu-id="d4a1b-136">Аудитории, которые могут просматривать значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="d4a1b-137">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="d4a1b-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="d4a1b-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d4a1b-139">description</span><span class="sxs-lookup"><span data-stu-id="d4a1b-139">description</span></span>|<span data-ttu-id="d4a1b-140">String</span><span class="sxs-lookup"><span data-stu-id="d4a1b-140">String</span></span>|<span data-ttu-id="d4a1b-141">Содержит описание, предоставленное пользователем для учетной записи в службе, на которую указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-141">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="d4a1b-142">inference</span><span class="sxs-lookup"><span data-stu-id="d4a1b-142">inference</span></span>|[<span data-ttu-id="d4a1b-143">inferenceData</span><span class="sxs-lookup"><span data-stu-id="d4a1b-143">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="d4a1b-144">Содержит подробные данные о подобных значениях, если сущность задана созданием или изменением приложения.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-144">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="d4a1b-145">Наследуется от [itemFacet.](../resources/itemfacet.md)</span><span class="sxs-lookup"><span data-stu-id="d4a1b-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d4a1b-146">service</span><span class="sxs-lookup"><span data-stu-id="d4a1b-146">service</span></span>|[<span data-ttu-id="d4a1b-147">serviceInformation</span><span class="sxs-lookup"><span data-stu-id="d4a1b-147">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="d4a1b-148">Содержит основные сведения о связанной службе.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-148">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="d4a1b-149">statusMessage</span><span class="sxs-lookup"><span data-stu-id="d4a1b-149">statusMessage</span></span>|<span data-ttu-id="d4a1b-150">String</span><span class="sxs-lookup"><span data-stu-id="d4a1b-150">String</span></span>|<span data-ttu-id="d4a1b-151">Содержит сообщение о состоянии из облачной службы, если она указана или синхронизирована.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-151">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="d4a1b-152">userId</span><span class="sxs-lookup"><span data-stu-id="d4a1b-152">userId</span></span>|<span data-ttu-id="d4a1b-153">String</span><span class="sxs-lookup"><span data-stu-id="d4a1b-153">String</span></span>|<span data-ttu-id="d4a1b-154">Имя пользователя, отображаемое для учетной записи веб-сайта.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-154">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="d4a1b-155">webUrl</span><span class="sxs-lookup"><span data-stu-id="d4a1b-155">webUrl</span></span>|<span data-ttu-id="d4a1b-156">String</span><span class="sxs-lookup"><span data-stu-id="d4a1b-156">String</span></span>|<span data-ttu-id="d4a1b-157">Содержит ссылку на профиль пользователя в облачной службе, если она есть.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-157">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="response"></a><span data-ttu-id="d4a1b-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4a1b-158">Response</span></span>

<span data-ttu-id="d4a1b-159">При успешном выполнении этот метод возвращает код `200 OK` ответа и обновленный [объект webAccount](../resources/webaccount.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-159">If successful, this method returns a `200 OK` response code and an updated [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4a1b-160">Примеры</span><span class="sxs-lookup"><span data-stu-id="d4a1b-160">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4a1b-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="d4a1b-161">Request</span></span>

<span data-ttu-id="d4a1b-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-162">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4a1b-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4a1b-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d4a1b-164">C#</span><span class="sxs-lookup"><span data-stu-id="d4a1b-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-webaccount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4a1b-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4a1b-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-webaccount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4a1b-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4a1b-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-webaccount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d4a1b-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="d4a1b-167">Response</span></span>

<span data-ttu-id="d4a1b-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-168">The following is an example of the response.</span></span>

> <span data-ttu-id="d4a1b-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d4a1b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
