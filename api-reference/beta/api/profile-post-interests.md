---
title: Создание Персонинтерест
description: Создание нового Персонинтерест.
localization_priority: Normal
author: kevinbellinger
ms.prod: People
doc_type: apiPageType
ms.openlocfilehash: 7428f696db38815d025f8e9fe56510489713b7f8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034494"
---
# <a name="create-personinterest"></a><span data-ttu-id="176c4-103">Создание Персонинтерест</span><span class="sxs-lookup"><span data-stu-id="176c4-103">Create personInterest</span></span>

<span data-ttu-id="176c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="176c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="176c4-105">Создание нового объекта [Персонинтерест] (.. /ресаурцес/персонинтерест.МД] в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="176c4-105">Create a new [personInterest](../resources/personinterest.md] in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="176c4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="176c4-106">Permissions</span></span>

<span data-ttu-id="176c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="176c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="176c4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="176c4-109">Permission type</span></span>                        | <span data-ttu-id="176c4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="176c4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="176c4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="176c4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="176c4-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="176c4-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="176c4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="176c4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="176c4-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="176c4-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="176c4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="176c4-115">Application</span></span>                            | <span data-ttu-id="176c4-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="176c4-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="176c4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="176c4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/interests
POST /users/{id | userPrincipalName}/profile/interests
```

## <a name="request-headers"></a><span data-ttu-id="176c4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="176c4-118">Request headers</span></span>

| <span data-ttu-id="176c4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="176c4-119">Name</span></span>      |<span data-ttu-id="176c4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="176c4-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="176c4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="176c4-121">Authorization</span></span>  | <span data-ttu-id="176c4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="176c4-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="176c4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="176c4-124">Content-Type</span></span>   | <span data-ttu-id="176c4-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="176c4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="176c4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="176c4-127">Request body</span></span>

<span data-ttu-id="176c4-128">В тексте запроса добавьте представление объекта [персонинтерест](../resources/personinterest.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="176c4-128">In the request body, supply a JSON representation of the [personInterest](../resources/personinterest.md) object.</span></span>

<span data-ttu-id="176c4-129">В следующей таблице приведены свойства, которые можно задать в новом объекте [персонинтерест](../resources/personinterest.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="176c4-129">The following table shows the properties that are possible to set within a new [personInterest](../resources/personinterest.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="176c4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="176c4-130">Property</span></span>|<span data-ttu-id="176c4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="176c4-131">Type</span></span>|<span data-ttu-id="176c4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="176c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="176c4-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="176c4-133">allowedAudiences</span></span>|<span data-ttu-id="176c4-134">String</span><span class="sxs-lookup"><span data-stu-id="176c4-134">String</span></span>|<span data-ttu-id="176c4-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="176c4-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="176c4-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="176c4-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="176c4-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="176c4-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="176c4-138">categories</span><span class="sxs-lookup"><span data-stu-id="176c4-138">categories</span></span>|<span data-ttu-id="176c4-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="176c4-139">String collection</span></span>|<span data-ttu-id="176c4-140">Содержит категории, которые пользователь связал с интересом (например, персональный, реЦипиес).</span><span class="sxs-lookup"><span data-stu-id="176c4-140">Contains categories a user has associated with the interest (for example, personal, recipies).</span></span> |
|<span data-ttu-id="176c4-141">коллаборатионтагс</span><span class="sxs-lookup"><span data-stu-id="176c4-141">collaborationTags</span></span>|<span data-ttu-id="176c4-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="176c4-142">String collection</span></span>|<span data-ttu-id="176c4-143">Содержит теги сценариев, с которыми пользователь связан с интересом.</span><span class="sxs-lookup"><span data-stu-id="176c4-143">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="176c4-144">Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="176c4-144">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="176c4-145">description</span><span class="sxs-lookup"><span data-stu-id="176c4-145">description</span></span>|<span data-ttu-id="176c4-146">String</span><span class="sxs-lookup"><span data-stu-id="176c4-146">String</span></span>|<span data-ttu-id="176c4-147">Содержит описание интереса.</span><span class="sxs-lookup"><span data-stu-id="176c4-147">Contains a description of the interest.</span></span>|
|<span data-ttu-id="176c4-148">displayName</span><span class="sxs-lookup"><span data-stu-id="176c4-148">displayName</span></span>|<span data-ttu-id="176c4-149">String</span><span class="sxs-lookup"><span data-stu-id="176c4-149">String</span></span>|<span data-ttu-id="176c4-150">Содержит понятное имя для интереса.</span><span class="sxs-lookup"><span data-stu-id="176c4-150">Contains a friendly name for the interest.</span></span>  |
|<span data-ttu-id="176c4-151">выводов</span><span class="sxs-lookup"><span data-stu-id="176c4-151">inference</span></span>|[<span data-ttu-id="176c4-152">инференцедата</span><span class="sxs-lookup"><span data-stu-id="176c4-152">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="176c4-153">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="176c4-153">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="176c4-154">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="176c4-154">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="176c4-155">source</span><span class="sxs-lookup"><span data-stu-id="176c4-155">source</span></span>|[<span data-ttu-id="176c4-156">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="176c4-156">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="176c4-157">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="176c4-157">Where the values originated if synced from another service.</span></span> <span data-ttu-id="176c4-158">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="176c4-158">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="176c4-159">webUrl</span><span class="sxs-lookup"><span data-stu-id="176c4-159">webUrl</span></span>|<span data-ttu-id="176c4-160">String</span><span class="sxs-lookup"><span data-stu-id="176c4-160">String</span></span>|<span data-ttu-id="176c4-161">Содержит ссылку на веб-страницу или ресурс, представляющие интерес.</span><span class="sxs-lookup"><span data-stu-id="176c4-161">Contains a link to a web page or resource about the interest.</span></span> |

## <a name="response"></a><span data-ttu-id="176c4-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="176c4-162">Response</span></span>

<span data-ttu-id="176c4-163">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [персонинтерест](../resources/personinterest.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="176c4-163">If successful, this method returns a `201 Created` response code and a new [personInterest](../resources/personinterest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="176c4-164">Примеры</span><span class="sxs-lookup"><span data-stu-id="176c4-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="176c4-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="176c4-165">Request</span></span>

<span data-ttu-id="176c4-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="176c4-166">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="176c4-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="176c4-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personinterest_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/interests
Content-type: application/json

{
  "categories": [
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com"
}
```
# <a name="c"></a>[<span data-ttu-id="176c4-168">C#</span><span class="sxs-lookup"><span data-stu-id="176c4-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personinterest-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="176c4-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="176c4-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personinterest-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="176c4-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="176c4-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personinterest-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="176c4-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="176c4-171">Response</span></span>

<span data-ttu-id="176c4-172">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="176c4-172">The following is an example of the response.</span></span>

> <span data-ttu-id="176c4-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="176c4-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personInterest"
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
  "categories": [
    "Sports"
  ],
  "description": "World's greatest football club",
  "displayName": "Chelsea FC",
  "webUrl": "https://www.chelseafc.com",
  "collaborationTags": null
}
```


