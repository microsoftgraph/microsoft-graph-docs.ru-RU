---
title: Создание обязанностей
description: Создание нового объекта обязанностей.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9c0907217bd75b79bc7e200dfc5d9deb901a2bfe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034349"
---
# <a name="create-personresponsibility"></a><span data-ttu-id="f32c3-103">Создание Персонреспонсибилити</span><span class="sxs-lookup"><span data-stu-id="f32c3-103">Create personResponsibility</span></span>
<span data-ttu-id="f32c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f32c3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f32c3-105">Создание нового объекта [персонреспонсибилити](../resources/personresponsibility.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="f32c3-105">Create a new [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f32c3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f32c3-106">Permissions</span></span>

<span data-ttu-id="f32c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f32c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f32c3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f32c3-109">Permission type</span></span>                        | <span data-ttu-id="f32c3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f32c3-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="f32c3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f32c3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f32c3-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f32c3-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f32c3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f32c3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f32c3-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="f32c3-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="f32c3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f32c3-115">Application</span></span>                            | <span data-ttu-id="f32c3-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f32c3-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="f32c3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f32c3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/responsibilities
POST /users/{id | userPrincipalName}/profile/responsibilities
```

## <a name="request-headers"></a><span data-ttu-id="f32c3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f32c3-118">Request headers</span></span>
|<span data-ttu-id="f32c3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f32c3-119">Name</span></span>|<span data-ttu-id="f32c3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f32c3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f32c3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f32c3-121">Authorization</span></span>|<span data-ttu-id="f32c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f32c3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f32c3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f32c3-124">Content-Type</span></span>|<span data-ttu-id="f32c3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f32c3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f32c3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f32c3-127">Request body</span></span>
<span data-ttu-id="f32c3-128">В тексте запроса добавьте представление объекта [персонреспонсибилити](../resources/personresponsibility.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f32c3-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="f32c3-129">В следующей таблице приведены свойства, которые можно задать в новом объекте [персонреспонсибилити](../resources/personresponsibility.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="f32c3-129">The following table shows the properties that are possible to set within a new [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="f32c3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f32c3-130">Property</span></span>|<span data-ttu-id="f32c3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f32c3-131">Type</span></span>|<span data-ttu-id="f32c3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f32c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f32c3-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="f32c3-133">allowedAudiences</span></span>|<span data-ttu-id="f32c3-134">String</span><span class="sxs-lookup"><span data-stu-id="f32c3-134">String</span></span>|<span data-ttu-id="f32c3-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="f32c3-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="f32c3-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f32c3-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="f32c3-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="f32c3-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="f32c3-138">коллаборатионтагс</span><span class="sxs-lookup"><span data-stu-id="f32c3-138">collaborationTags</span></span>|<span data-ttu-id="f32c3-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f32c3-139">String collection</span></span>|<span data-ttu-id="f32c3-140">Содержит теги сценариев, с которыми пользователь связан с интересом.</span><span class="sxs-lookup"><span data-stu-id="f32c3-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="f32c3-141">Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="f32c3-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="f32c3-142">description</span><span class="sxs-lookup"><span data-stu-id="f32c3-142">description</span></span>|<span data-ttu-id="f32c3-143">String</span><span class="sxs-lookup"><span data-stu-id="f32c3-143">String</span></span>|<span data-ttu-id="f32c3-144">Описание ответственности.</span><span class="sxs-lookup"><span data-stu-id="f32c3-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="f32c3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="f32c3-145">displayName</span></span>|<span data-ttu-id="f32c3-146">String</span><span class="sxs-lookup"><span data-stu-id="f32c3-146">String</span></span>|<span data-ttu-id="f32c3-147">Содержит понятное имя для ответственности.</span><span class="sxs-lookup"><span data-stu-id="f32c3-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="f32c3-148">выводов</span><span class="sxs-lookup"><span data-stu-id="f32c3-148">inference</span></span>|[<span data-ttu-id="f32c3-149">инференцедата</span><span class="sxs-lookup"><span data-stu-id="f32c3-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="f32c3-150">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="f32c3-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="f32c3-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f32c3-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f32c3-152">source</span><span class="sxs-lookup"><span data-stu-id="f32c3-152">source</span></span>|[<span data-ttu-id="f32c3-153">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="f32c3-153">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="f32c3-154">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="f32c3-154">Where the values originated if synced from another service.</span></span> <span data-ttu-id="f32c3-155">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="f32c3-155">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="f32c3-156">webUrl</span><span class="sxs-lookup"><span data-stu-id="f32c3-156">webUrl</span></span>|<span data-ttu-id="f32c3-157">String</span><span class="sxs-lookup"><span data-stu-id="f32c3-157">String</span></span>|<span data-ttu-id="f32c3-158">Содержит ссылку на веб-страницу или ресурс, отвечающие за ответственность.</span><span class="sxs-lookup"><span data-stu-id="f32c3-158">Contains a link to a web page or resource about the responsibility.</span></span>|

## <a name="response"></a><span data-ttu-id="f32c3-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="f32c3-159">Response</span></span>

<span data-ttu-id="f32c3-160">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [персонреспонсибилити](../resources/personannotation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f32c3-160">If successful, this method returns a `201 Created` response code and a [personResponsibility](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f32c3-161">Примеры</span><span class="sxs-lookup"><span data-stu-id="f32c3-161">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="f32c3-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="f32c3-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personresponsibility_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/responsibilities
Content-Type: application/json
Content-length: 413

{
  "description": "Member of the Microsoft API Council",
  "displayName": "API Council",
  "collaborationTags": [
    "askMeAbout"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="f32c3-163">C#</span><span class="sxs-lookup"><span data-stu-id="f32c3-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-interests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f32c3-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f32c3-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-interests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f32c3-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f32c3-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-interests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="f32c3-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="f32c3-166">Response</span></span>
<span data-ttu-id="f32c3-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f32c3-167">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personResponsibility"
}
-->
``` http
HTTP/1.1 201 Created
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


