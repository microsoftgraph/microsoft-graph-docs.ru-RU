---
title: Обновление Персонреспонсибилити
description: Обновление свойств объекта Персонреспонсибилити.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9c4696ae3c9f97a6f256c65844b062e0f7882c3e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46813157"
---
# <a name="update-personresponsibility"></a><span data-ttu-id="f649a-103">Обновление Персонреспонсибилити</span><span class="sxs-lookup"><span data-stu-id="f649a-103">Update personResponsibility</span></span>
<span data-ttu-id="f649a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f649a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f649a-105">Обновление свойств объекта [персонреспонсибилити](../resources/personresponsibility.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="f649a-105">Update the properties of a [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f649a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f649a-106">Permissions</span></span>

<span data-ttu-id="f649a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f649a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f649a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f649a-109">Permission type</span></span>                        | <span data-ttu-id="f649a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f649a-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f649a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f649a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f649a-112">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f649a-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f649a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f649a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f649a-114">User. Read, User. ReadWrite, User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f649a-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f649a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f649a-115">Application</span></span>                            | <span data-ttu-id="f649a-116">User. ReadBasic. ALL, User. Read. ALL, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f649a-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f649a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f649a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/profile/responsibilities/{id}
PATCH /users/{id | userPrincipalName}/profile/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f649a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f649a-118">Request headers</span></span>
|<span data-ttu-id="f649a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f649a-119">Name</span></span>|<span data-ttu-id="f649a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f649a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f649a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f649a-121">Authorization</span></span>|<span data-ttu-id="f649a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f649a-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f649a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f649a-124">Content-Type</span></span>|<span data-ttu-id="f649a-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f649a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f649a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f649a-127">Request body</span></span>
<span data-ttu-id="f649a-128">В тексте запроса добавьте представление объекта [персонреспонсибилити](../resources/personresponsibility.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f649a-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="f649a-129">В следующей таблице приведены свойства, необходимые при создании [персонреспонсибилити](../resources/personresponsibility.md).</span><span class="sxs-lookup"><span data-stu-id="f649a-129">The following table shows the properties that are required when you create the [personResponsibility](../resources/personresponsibility.md).</span></span>

|<span data-ttu-id="f649a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f649a-130">Property</span></span>|<span data-ttu-id="f649a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f649a-131">Type</span></span>|<span data-ttu-id="f649a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f649a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f649a-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="f649a-133">allowedAudiences</span></span>|<span data-ttu-id="f649a-134">String</span><span class="sxs-lookup"><span data-stu-id="f649a-134">String</span></span>|<span data-ttu-id="f649a-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="f649a-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="f649a-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f649a-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="f649a-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f649a-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f649a-138">коллаборатионтагс</span><span class="sxs-lookup"><span data-stu-id="f649a-138">collaborationTags</span></span>|<span data-ttu-id="f649a-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f649a-139">String collection</span></span>|<span data-ttu-id="f649a-140">Содержит теги сценариев, с которыми пользователь связан с интересом.</span><span class="sxs-lookup"><span data-stu-id="f649a-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="f649a-141">Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="f649a-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="f649a-142">description</span><span class="sxs-lookup"><span data-stu-id="f649a-142">description</span></span>|<span data-ttu-id="f649a-143">String</span><span class="sxs-lookup"><span data-stu-id="f649a-143">String</span></span>|<span data-ttu-id="f649a-144">Описание ответственности.</span><span class="sxs-lookup"><span data-stu-id="f649a-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="f649a-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f649a-145">displayName</span></span>|<span data-ttu-id="f649a-146">String</span><span class="sxs-lookup"><span data-stu-id="f649a-146">String</span></span>|<span data-ttu-id="f649a-147">Содержит понятное имя для ответственности.</span><span class="sxs-lookup"><span data-stu-id="f649a-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="f649a-148">выводов</span><span class="sxs-lookup"><span data-stu-id="f649a-148">inference</span></span>|[<span data-ttu-id="f649a-149">инференцедата</span><span class="sxs-lookup"><span data-stu-id="f649a-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="f649a-150">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="f649a-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="f649a-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f649a-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f649a-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="f649a-152">webUrl</span></span>|<span data-ttu-id="f649a-153">String</span><span class="sxs-lookup"><span data-stu-id="f649a-153">String</span></span>|<span data-ttu-id="f649a-154">Содержит ссылку на веб-страницу или ресурс, отвечающие за ответственность.</span><span class="sxs-lookup"><span data-stu-id="f649a-154">Contains a link to a web page or resource about the responsibility.</span></span>|



## <a name="response"></a><span data-ttu-id="f649a-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="f649a-155">Response</span></span>

<span data-ttu-id="f649a-156">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [персонреспонсибилити](../resources/personresponsibility.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f649a-156">If successful, this method returns a `200 OK` response code and an updated [personResponsibility](../resources/personresponsibility.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f649a-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="f649a-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f649a-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="f649a-158">Request</span></span>
# <a name="http"></a>[<span data-ttu-id="f649a-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="f649a-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f649a-160">C#</span><span class="sxs-lookup"><span data-stu-id="f649a-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f649a-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f649a-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f649a-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f649a-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f649a-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="f649a-163">Response</span></span>
<span data-ttu-id="f649a-164">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f649a-164">**Note:** The response object shown here might be shortened for readability.</span></span>
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
