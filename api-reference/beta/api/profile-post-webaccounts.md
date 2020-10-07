---
title: Создание учетной записи
description: Создайте новый объект учетной записи.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 23990dd1022985a91953d714eeab5f886b5cca6d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034352"
---
# <a name="create-webaccount"></a><span data-ttu-id="1a150-103">Создание учетной записи</span><span class="sxs-lookup"><span data-stu-id="1a150-103">Create webAccount</span></span>

<span data-ttu-id="1a150-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a150-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a150-105">Создайте новый объект [учетной записи](../resources/webaccount.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="1a150-105">Create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1a150-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1a150-106">Permissions</span></span>

<span data-ttu-id="1a150-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a150-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a150-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1a150-109">Permission type</span></span>                        | <span data-ttu-id="1a150-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1a150-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a150-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1a150-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a150-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1a150-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1a150-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1a150-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a150-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1a150-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="1a150-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1a150-115">Application</span></span>                            | <span data-ttu-id="1a150-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a150-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="1a150-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1a150-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/webAccounts
POST /users/{id | userPrincipalName}/profile/webAccounts
```

## <a name="request-headers"></a><span data-ttu-id="1a150-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1a150-118">Request headers</span></span>

| <span data-ttu-id="1a150-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1a150-119">Name</span></span>           | <span data-ttu-id="1a150-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1a150-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="1a150-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1a150-121">Authorization</span></span>  | <span data-ttu-id="1a150-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a150-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1a150-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a150-124">Content-Type</span></span>   | <span data-ttu-id="1a150-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1a150-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a150-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1a150-127">Request body</span></span>

<span data-ttu-id="1a150-128">В тексте запроса добавьте представление объекта [учетной записи](../resources/webaccount.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a150-128">In the request body, supply a JSON representation of [webAccount](../resources/webaccount.md) object.</span></span>

<span data-ttu-id="1a150-129">В следующей таблице приведены свойства, которые можно задать при создании нового объекта [учетной записи](../resources/webaccount.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="1a150-129">The following table shows the properties that are possible to set when you create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="1a150-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a150-130">Property</span></span>|<span data-ttu-id="1a150-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1a150-131">Type</span></span>|<span data-ttu-id="1a150-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1a150-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a150-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="1a150-133">allowedAudiences</span></span>|<span data-ttu-id="1a150-134">String</span><span class="sxs-lookup"><span data-stu-id="1a150-134">String</span></span>|<span data-ttu-id="1a150-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="1a150-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="1a150-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1a150-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="1a150-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1a150-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1a150-138">description</span><span class="sxs-lookup"><span data-stu-id="1a150-138">description</span></span>|<span data-ttu-id="1a150-139">String</span><span class="sxs-lookup"><span data-stu-id="1a150-139">String</span></span>|<span data-ttu-id="1a150-140">Содержит описание, предоставленное пользователем для учетной записи службы, на которую выполняется ссылка.</span><span class="sxs-lookup"><span data-stu-id="1a150-140">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="1a150-141">выводов</span><span class="sxs-lookup"><span data-stu-id="1a150-141">inference</span></span>|[<span data-ttu-id="1a150-142">инференцедата</span><span class="sxs-lookup"><span data-stu-id="1a150-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="1a150-143">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="1a150-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="1a150-144">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1a150-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="1a150-145">служба</span><span class="sxs-lookup"><span data-stu-id="1a150-145">service</span></span>|[<span data-ttu-id="1a150-146">сервицеинформатион</span><span class="sxs-lookup"><span data-stu-id="1a150-146">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="1a150-147">Содержит основные сведения о связанной службе.</span><span class="sxs-lookup"><span data-stu-id="1a150-147">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="1a150-148">source</span><span class="sxs-lookup"><span data-stu-id="1a150-148">source</span></span>|[<span data-ttu-id="1a150-149">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="1a150-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="1a150-150">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="1a150-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="1a150-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="1a150-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="1a150-152">статусмессаже</span><span class="sxs-lookup"><span data-stu-id="1a150-152">statusMessage</span></span>|<span data-ttu-id="1a150-153">String</span><span class="sxs-lookup"><span data-stu-id="1a150-153">String</span></span>|<span data-ttu-id="1a150-154">Содержит сообщение о состоянии от облачной службы, если оно предоставлено или синхронизировано.</span><span class="sxs-lookup"><span data-stu-id="1a150-154">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="1a150-155">userId</span><span class="sxs-lookup"><span data-stu-id="1a150-155">userId</span></span>|<span data-ttu-id="1a150-156">String</span><span class="sxs-lookup"><span data-stu-id="1a150-156">String</span></span>|<span data-ttu-id="1a150-157">Имя пользователя, отображаемое для учетной записи Account.</span><span class="sxs-lookup"><span data-stu-id="1a150-157">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="1a150-158">webUrl</span><span class="sxs-lookup"><span data-stu-id="1a150-158">webUrl</span></span>|<span data-ttu-id="1a150-159">String</span><span class="sxs-lookup"><span data-stu-id="1a150-159">String</span></span>|<span data-ttu-id="1a150-160">Содержит ссылку на профиль пользователя в облачной службе, если она существует.</span><span class="sxs-lookup"><span data-stu-id="1a150-160">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="response"></a><span data-ttu-id="1a150-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a150-161">Response</span></span>

<span data-ttu-id="1a150-162">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и новый объект [учетной записи](../resources/webaccount.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1a150-162">If successful, this method returns `201, Created` response code and a new [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a150-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="1a150-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a150-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="1a150-164">Request</span></span>

<span data-ttu-id="1a150-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1a150-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a150-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a150-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_webaccount_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/webAccounts
Content-type: application/json

{
  "description": "My Github contributions!",
  "userId": "innocenty.popov",
  "service": {
    "name": "GitHub",
    "webUrl": "https://github.com"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="1a150-167">C#</span><span class="sxs-lookup"><span data-stu-id="1a150-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-webaccount-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a150-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a150-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-webaccount-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a150-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a150-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-webaccount-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a150-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="1a150-170">Response</span></span>

<span data-ttu-id="1a150-171">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1a150-171">The following is an example of the response.</span></span>

> <span data-ttu-id="1a150-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1a150-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.webAccount"
} -->

```http
HTTP/1.1 201 Created
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


