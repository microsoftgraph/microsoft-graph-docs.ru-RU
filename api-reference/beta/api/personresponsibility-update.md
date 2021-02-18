---
title: Обновление personResponsibility
description: Обновление свойств объекта personResponsibility.
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 62948aa9accfa79997e9a119f32d200cca507051
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292702"
---
# <a name="update-personresponsibility"></a><span data-ttu-id="4cde3-103">Обновление personResponsibility</span><span class="sxs-lookup"><span data-stu-id="4cde3-103">Update personResponsibility</span></span>
<span data-ttu-id="4cde3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cde3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4cde3-105">Обновление свойств объекта [personResponsibility](../resources/personresponsibility.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="4cde3-105">Update the properties of a [personResponsibility](../resources/personresponsibility.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4cde3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4cde3-106">Permissions</span></span>

<span data-ttu-id="4cde3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cde3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4cde3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4cde3-109">Permission type</span></span>                        | <span data-ttu-id="4cde3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4cde3-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="4cde3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4cde3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4cde3-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cde3-112">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4cde3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4cde3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cde3-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cde3-114">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span> |
| <span data-ttu-id="4cde3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4cde3-115">Application</span></span>                            | <span data-ttu-id="4cde3-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cde3-116">User.ReadBasic.All, User.Read.All, User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="4cde3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4cde3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/responsibilities/{id}
PATCH /users/{id | userPrincipalName}/responsibilities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4cde3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4cde3-118">Request headers</span></span>
|<span data-ttu-id="4cde3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4cde3-119">Name</span></span>|<span data-ttu-id="4cde3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4cde3-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4cde3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4cde3-121">Authorization</span></span>|<span data-ttu-id="4cde3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cde3-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4cde3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4cde3-124">Content-Type</span></span>|<span data-ttu-id="4cde3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4cde3-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cde3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4cde3-127">Request body</span></span>
<span data-ttu-id="4cde3-128">В теле запроса укажу представление объекта [personResponsibility](../resources/personresponsibility.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="4cde3-128">In the request body, supply a JSON representation of the [personResponsibility](../resources/personresponsibility.md) object.</span></span>

<span data-ttu-id="4cde3-129">В следующей таблице показаны свойства, необходимые при создании [объекта personResponsibility.](../resources/personresponsibility.md)</span><span class="sxs-lookup"><span data-stu-id="4cde3-129">The following table shows the properties that are required when you create the [personResponsibility](../resources/personresponsibility.md).</span></span>

|<span data-ttu-id="4cde3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cde3-130">Property</span></span>|<span data-ttu-id="4cde3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4cde3-131">Type</span></span>|<span data-ttu-id="4cde3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4cde3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cde3-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="4cde3-133">allowedAudiences</span></span>|<span data-ttu-id="4cde3-134">String</span><span class="sxs-lookup"><span data-stu-id="4cde3-134">String</span></span>|<span data-ttu-id="4cde3-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="4cde3-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="4cde3-136">Наследуется [от itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4cde3-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="4cde3-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4cde3-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4cde3-138">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="4cde3-138">collaborationTags</span></span>|<span data-ttu-id="4cde3-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4cde3-139">String collection</span></span>|<span data-ttu-id="4cde3-140">Содержит теги сценария работы, которые пользователь связал с интересом.</span><span class="sxs-lookup"><span data-stu-id="4cde3-140">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="4cde3-141">Допустимые значения в коллекции: `askMeAbout` , `ableToMentor` , , `wantsToLearn` `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="4cde3-141">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="4cde3-142">description</span><span class="sxs-lookup"><span data-stu-id="4cde3-142">description</span></span>|<span data-ttu-id="4cde3-143">String</span><span class="sxs-lookup"><span data-stu-id="4cde3-143">String</span></span>|<span data-ttu-id="4cde3-144">Описание ответственности.</span><span class="sxs-lookup"><span data-stu-id="4cde3-144">Description of the responsibility.</span></span>|
|<span data-ttu-id="4cde3-145">displayName</span><span class="sxs-lookup"><span data-stu-id="4cde3-145">displayName</span></span>|<span data-ttu-id="4cde3-146">String</span><span class="sxs-lookup"><span data-stu-id="4cde3-146">String</span></span>|<span data-ttu-id="4cde3-147">Содержит удобное имя для ответственности.</span><span class="sxs-lookup"><span data-stu-id="4cde3-147">Contains a friendly name for the responsibility.</span></span> |
|<span data-ttu-id="4cde3-148">вывод</span><span class="sxs-lookup"><span data-stu-id="4cde3-148">inference</span></span>|[<span data-ttu-id="4cde3-149">inferenceData</span><span class="sxs-lookup"><span data-stu-id="4cde3-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="4cde3-150">Содержит сведения о выводе, если сущность создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="4cde3-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="4cde3-151">Наследуется [от itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="4cde3-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="4cde3-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="4cde3-152">webUrl</span></span>|<span data-ttu-id="4cde3-153">String</span><span class="sxs-lookup"><span data-stu-id="4cde3-153">String</span></span>|<span data-ttu-id="4cde3-154">Содержит ссылку на веб-страницу или ресурс об ответственности.</span><span class="sxs-lookup"><span data-stu-id="4cde3-154">Contains a link to a web page or resource about the responsibility.</span></span>|



## <a name="response"></a><span data-ttu-id="4cde3-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="4cde3-155">Response</span></span>

<span data-ttu-id="4cde3-156">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [personResponsibility](../resources/personresponsibility.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4cde3-156">If successful, this method returns a `200 OK` response code and an updated [personResponsibility](../resources/personresponsibility.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4cde3-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="4cde3-157">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4cde3-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="4cde3-158">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f"],
  "name": "update_personresponsibility"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/responsibilities/0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f
Content-Type: application/json
Content-length: 446

{
  "collaborationTags": [
    "askMeAbout"
  ]
}
```

### <a name="response"></a><span data-ttu-id="4cde3-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="4cde3-159">Response</span></span>
<span data-ttu-id="4cde3-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4cde3-160">**Note:** The response object shown here might be shortened for readability.</span></span>
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


