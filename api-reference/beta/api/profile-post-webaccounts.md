---
title: Создание webAccount
description: Создание нового объекта webAccount.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 2d41cb9fe650fa8d506f8ea9c218a01d4f2c0605
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036767"
---
# <a name="create-webaccount"></a><span data-ttu-id="da7be-103">Создание webAccount</span><span class="sxs-lookup"><span data-stu-id="da7be-103">Create webAccount</span></span>

<span data-ttu-id="da7be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da7be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da7be-105">Создание нового [объекта webAccount](../resources/webaccount.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="da7be-105">Create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="da7be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da7be-106">Permissions</span></span>

<span data-ttu-id="da7be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da7be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da7be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da7be-109">Permission type</span></span>                        | <span data-ttu-id="da7be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da7be-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="da7be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da7be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="da7be-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da7be-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="da7be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da7be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da7be-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da7be-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="da7be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da7be-115">Application</span></span>                            | <span data-ttu-id="da7be-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da7be-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="da7be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da7be-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/webAccounts
POST /users/{id | userPrincipalName}/profile/webAccounts
```

## <a name="request-headers"></a><span data-ttu-id="da7be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da7be-118">Request headers</span></span>

| <span data-ttu-id="da7be-119">Имя</span><span class="sxs-lookup"><span data-stu-id="da7be-119">Name</span></span>           | <span data-ttu-id="da7be-120">Описание</span><span class="sxs-lookup"><span data-stu-id="da7be-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="da7be-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da7be-121">Authorization</span></span>  | <span data-ttu-id="da7be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da7be-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="da7be-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da7be-124">Content-Type</span></span>   | <span data-ttu-id="da7be-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da7be-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da7be-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da7be-127">Request body</span></span>

<span data-ttu-id="da7be-128">В теле запроса поставляем представление JSON объекта [webAccount.](../resources/webaccount.md)</span><span class="sxs-lookup"><span data-stu-id="da7be-128">In the request body, supply a JSON representation of [webAccount](../resources/webaccount.md) object.</span></span>

<span data-ttu-id="da7be-129">В следующей таблице показаны свойства, которые можно установить при создании нового объекта [webAccount](../resources/webaccount.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="da7be-129">The following table shows the properties that are possible to set when you create a new [webAccount](../resources/webaccount.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="da7be-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="da7be-130">Property</span></span>|<span data-ttu-id="da7be-131">Тип</span><span class="sxs-lookup"><span data-stu-id="da7be-131">Type</span></span>|<span data-ttu-id="da7be-132">Описание</span><span class="sxs-lookup"><span data-stu-id="da7be-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da7be-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="da7be-133">allowedAudiences</span></span>|<span data-ttu-id="da7be-134">String</span><span class="sxs-lookup"><span data-stu-id="da7be-134">String</span></span>|<span data-ttu-id="da7be-135">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="da7be-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="da7be-136">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="da7be-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="da7be-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="da7be-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="da7be-138">description</span><span class="sxs-lookup"><span data-stu-id="da7be-138">description</span></span>|<span data-ttu-id="da7be-139">String</span><span class="sxs-lookup"><span data-stu-id="da7be-139">String</span></span>|<span data-ttu-id="da7be-140">Содержит описание, предоставленное пользователем для учетной записи в службе, на который ссылается.</span><span class="sxs-lookup"><span data-stu-id="da7be-140">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="da7be-141">вывод</span><span class="sxs-lookup"><span data-stu-id="da7be-141">inference</span></span>|[<span data-ttu-id="da7be-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="da7be-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="da7be-143">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="da7be-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="da7be-144">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="da7be-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="da7be-145">служба</span><span class="sxs-lookup"><span data-stu-id="da7be-145">service</span></span>|[<span data-ttu-id="da7be-146">serviceInformation</span><span class="sxs-lookup"><span data-stu-id="da7be-146">serviceInformation</span></span>](../resources/serviceinformation.md)| <span data-ttu-id="da7be-147">Содержит основные сведения о связанной службе.</span><span class="sxs-lookup"><span data-stu-id="da7be-147">Contains basic detail about the service that is being associated.</span></span> |
|<span data-ttu-id="da7be-148">source</span><span class="sxs-lookup"><span data-stu-id="da7be-148">source</span></span>|[<span data-ttu-id="da7be-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="da7be-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="da7be-150">Где значения возникли, если синхронизированы с другой службы.</span><span class="sxs-lookup"><span data-stu-id="da7be-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="da7be-151">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="da7be-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="da7be-152">statusMessage</span><span class="sxs-lookup"><span data-stu-id="da7be-152">statusMessage</span></span>|<span data-ttu-id="da7be-153">String</span><span class="sxs-lookup"><span data-stu-id="da7be-153">String</span></span>|<span data-ttu-id="da7be-154">Содержит сообщение о состоянии облачной службы при условии или синхронизации.</span><span class="sxs-lookup"><span data-stu-id="da7be-154">Contains a status message from the cloud service if provided or synchronized.</span></span> |
|<span data-ttu-id="da7be-155">userId</span><span class="sxs-lookup"><span data-stu-id="da7be-155">userId</span></span>|<span data-ttu-id="da7be-156">String</span><span class="sxs-lookup"><span data-stu-id="da7be-156">String</span></span>|<span data-ttu-id="da7be-157">Имя пользователя, отображаемая для webaccount.</span><span class="sxs-lookup"><span data-stu-id="da7be-157">The user name  displayed for the webaccount.</span></span>  |
|<span data-ttu-id="da7be-158">webUrl</span><span class="sxs-lookup"><span data-stu-id="da7be-158">webUrl</span></span>|<span data-ttu-id="da7be-159">String</span><span class="sxs-lookup"><span data-stu-id="da7be-159">String</span></span>|<span data-ttu-id="da7be-160">Содержит ссылку на профиль пользователя в облачной службе, если она существует.</span><span class="sxs-lookup"><span data-stu-id="da7be-160">Contains a link to the user's profile on the cloud service if one exists.</span></span>|

## <a name="response"></a><span data-ttu-id="da7be-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="da7be-161">Response</span></span>

<span data-ttu-id="da7be-162">В случае успешной работы этот метод возвращает код отклика и новый `201, Created` [объект webAccount](../resources/webaccount.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="da7be-162">If successful, this method returns `201, Created` response code and a new [webAccount](../resources/webaccount.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="da7be-163">Примеры</span><span class="sxs-lookup"><span data-stu-id="da7be-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="da7be-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="da7be-164">Request</span></span>

<span data-ttu-id="da7be-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da7be-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da7be-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="da7be-166">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="da7be-167">C#</span><span class="sxs-lookup"><span data-stu-id="da7be-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-webaccount-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da7be-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da7be-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-webaccount-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da7be-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da7be-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-webaccount-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da7be-170">Java</span><span class="sxs-lookup"><span data-stu-id="da7be-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-webaccount-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="da7be-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="da7be-171">Response</span></span>

<span data-ttu-id="da7be-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="da7be-172">The following is an example of the response.</span></span>

> <span data-ttu-id="da7be-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="da7be-173">**Note:** The response object shown here might be shortened for readability.</span></span>

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


