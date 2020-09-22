---
title: Обновление Персонреспонсибилити
description: Обновление свойств объекта Персонреспонсибилити.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 38ca672825c49f0149dcf9b06b4c57d8df92c0e5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017369"
---
# <a name="update-personresponsibility"></a><span data-ttu-id="23d23-103">Обновление Персонреспонсибилити</span><span class="sxs-lookup"><span data-stu-id="23d23-103">Update personResponsibility</span></span>
<span data-ttu-id="23d23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23d23-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23d23-105">Обновление свойств объекта [персонреспонсибилити](../resources/personresponsibility.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="23d23-105">Update the properties of a [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="23d23-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23d23-106">Permissions</span></span>

<span data-ttu-id="23d23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23d23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="23d23-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23d23-109">Permission type</span></span>                        | <span data-ttu-id="23d23-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23d23-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="23d23-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23d23-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="23d23-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="23d23-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="23d23-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23d23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23d23-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="23d23-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="23d23-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23d23-115">Application</span></span>                            | <span data-ttu-id="23d23-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="23d23-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="23d23-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23d23-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/responsibilities/{id}
PATCH /users/{id | userPrincipalName}/profile/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="23d23-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23d23-118">Request headers</span></span>
|<span data-ttu-id="23d23-119">Имя</span><span class="sxs-lookup"><span data-stu-id="23d23-119">Name</span></span>|<span data-ttu-id="23d23-120">Описание</span><span class="sxs-lookup"><span data-stu-id="23d23-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="23d23-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23d23-121">Authorization</span></span>|<span data-ttu-id="23d23-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23d23-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="23d23-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23d23-124">Content-Type</span></span>|<span data-ttu-id="23d23-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23d23-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="23d23-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23d23-127">Request body</span></span>
<span data-ttu-id="23d23-128">В тексте запроса добавьте представление объекта [персонреспонсибилити](../resources/personresponsibility.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23d23-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="23d23-129">В следующей таблице приведены свойства, необходимые при создании [персонреспонсибилити](../resources/personresponsibility.md).</span><span class="sxs-lookup"><span data-stu-id="23d23-129">The following table shows the properties that are required when you create the [personResponsibility](../resources/personresponsibility.md).</span></span>

|<span data-ttu-id="23d23-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="23d23-130">Property</span></span>|<span data-ttu-id="23d23-131">Тип</span><span class="sxs-lookup"><span data-stu-id="23d23-131">Type</span></span>|<span data-ttu-id="23d23-132">Описание</span><span class="sxs-lookup"><span data-stu-id="23d23-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23d23-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="23d23-133">allowedAudiences</span></span>|<span data-ttu-id="23d23-134">String</span><span class="sxs-lookup"><span data-stu-id="23d23-134">String</span></span>|<span data-ttu-id="23d23-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="23d23-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="23d23-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="23d23-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="23d23-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="23d23-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="23d23-138">коллаборатионтагс</span><span class="sxs-lookup"><span data-stu-id="23d23-138">collaborationTags</span></span>|<span data-ttu-id="23d23-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="23d23-139">String collection</span></span>|<span data-ttu-id="23d23-140">Содержит теги сценариев, с которыми пользователь связан с интересом.</span><span class="sxs-lookup"><span data-stu-id="23d23-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="23d23-141">Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="23d23-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="23d23-142">description</span><span class="sxs-lookup"><span data-stu-id="23d23-142">description</span></span>|<span data-ttu-id="23d23-143">String</span><span class="sxs-lookup"><span data-stu-id="23d23-143">String</span></span>|<span data-ttu-id="23d23-144">Описание ответственности.</span><span class="sxs-lookup"><span data-stu-id="23d23-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="23d23-145">displayName</span><span class="sxs-lookup"><span data-stu-id="23d23-145">displayName</span></span>|<span data-ttu-id="23d23-146">String</span><span class="sxs-lookup"><span data-stu-id="23d23-146">String</span></span>|<span data-ttu-id="23d23-147">Содержит понятное имя для ответственности.</span><span class="sxs-lookup"><span data-stu-id="23d23-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="23d23-148">выводов</span><span class="sxs-lookup"><span data-stu-id="23d23-148">inference</span></span>|[<span data-ttu-id="23d23-149">инференцедата</span><span class="sxs-lookup"><span data-stu-id="23d23-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="23d23-150">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="23d23-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="23d23-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="23d23-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="23d23-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="23d23-152">webUrl</span></span>|<span data-ttu-id="23d23-153">String</span><span class="sxs-lookup"><span data-stu-id="23d23-153">String</span></span>|<span data-ttu-id="23d23-154">Содержит ссылку на веб-страницу или ресурс, отвечающие за ответственность.</span><span class="sxs-lookup"><span data-stu-id="23d23-154">Contains a link to a web page or resource about the responsibility.</span></span>|



## <a name="response"></a><span data-ttu-id="23d23-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="23d23-155">Response</span></span>

<span data-ttu-id="23d23-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [персонреспонсибилити](../resources/personresponsibility.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23d23-156">If successful, this method returns a `200 OK` response code and an updated [personResponsibility](../resources/personresponsibility.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="23d23-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="23d23-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="23d23-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="23d23-158">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="23d23-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="23d23-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "update_personresponsibility"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/profile/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
Content-Type: application/json
Content-length: 446

{
  "collaborationTags": [
    "askMeAbout"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="23d23-160">C#</span><span class="sxs-lookup"><span data-stu-id="23d23-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23d23-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23d23-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23d23-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23d23-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="23d23-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="23d23-163">Response</span></span>
<span data-ttu-id="23d23-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="23d23-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

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
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "webUrl": null,
  "collaborationTags": [
    "askMeAbout"
  ]
}
```


