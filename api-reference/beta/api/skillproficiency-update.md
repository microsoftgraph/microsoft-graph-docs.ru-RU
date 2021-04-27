---
title: Обновление skillProficiency
description: Обновление свойств объекта skillProficiency в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9da18f3fc53cac80fc4f357083c6dea3c95d5c84
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048990"
---
# <a name="update-skillproficiency"></a><span data-ttu-id="872f7-103">Обновление профессиональных навыков</span><span class="sxs-lookup"><span data-stu-id="872f7-103">Update skillproficiency</span></span>

<span data-ttu-id="872f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="872f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="872f7-105">Обновление свойств объекта [skillProficiency](../resources/skillproficiency.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="872f7-105">Update the properties of a [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="872f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="872f7-106">Permissions</span></span>

<span data-ttu-id="872f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="872f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="872f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="872f7-109">Permission type</span></span>                        | <span data-ttu-id="872f7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="872f7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="872f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="872f7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="872f7-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="872f7-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="872f7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="872f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="872f7-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="872f7-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="872f7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="872f7-115">Application</span></span>                            | <span data-ttu-id="872f7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="872f7-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="872f7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="872f7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/skills/{id}
PATCH /users/{id | userPrincipalName}/profile/skills/{id}
```

## <a name="request-headers"></a><span data-ttu-id="872f7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="872f7-118">Request headers</span></span>

| <span data-ttu-id="872f7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="872f7-119">Name</span></span>           |<span data-ttu-id="872f7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="872f7-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="872f7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="872f7-121">Authorization</span></span>  | <span data-ttu-id="872f7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="872f7-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="872f7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="872f7-124">Content-Type</span></span>   | <span data-ttu-id="872f7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="872f7-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="872f7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="872f7-127">Request body</span></span>

<span data-ttu-id="872f7-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="872f7-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="872f7-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="872f7-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="872f7-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="872f7-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="872f7-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="872f7-131">Property</span></span>|<span data-ttu-id="872f7-132">Тип</span><span class="sxs-lookup"><span data-stu-id="872f7-132">Type</span></span>|<span data-ttu-id="872f7-133">Описание</span><span class="sxs-lookup"><span data-stu-id="872f7-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="872f7-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="872f7-134">allowedAudiences</span></span>|<span data-ttu-id="872f7-135">String</span><span class="sxs-lookup"><span data-stu-id="872f7-135">String</span></span>|<span data-ttu-id="872f7-136">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="872f7-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="872f7-137">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="872f7-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="872f7-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="872f7-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="872f7-139">categories</span><span class="sxs-lookup"><span data-stu-id="872f7-139">categories</span></span>|<span data-ttu-id="872f7-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="872f7-140">String collection</span></span>|<span data-ttu-id="872f7-141">Содержит категории, связанные с навыком пользователя (например, личное, профессиональное, хобби).</span><span class="sxs-lookup"><span data-stu-id="872f7-141">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span> |
|<span data-ttu-id="872f7-142">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="872f7-142">collaborationTags</span></span>|<span data-ttu-id="872f7-143">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="872f7-143">String collection</span></span>|<span data-ttu-id="872f7-144">Содержит теги сценариев работы, которые пользователь связал с интересом.</span><span class="sxs-lookup"><span data-stu-id="872f7-144">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="872f7-145">Допустимые значения в коллекции: `askMeAbout` , `ableToMentor` , `wantsToLearn` `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="872f7-145">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="872f7-146">displayName</span><span class="sxs-lookup"><span data-stu-id="872f7-146">displayName</span></span>|<span data-ttu-id="872f7-147">String</span><span class="sxs-lookup"><span data-stu-id="872f7-147">String</span></span>|<span data-ttu-id="872f7-148">Содержит удобное имя для навыка.</span><span class="sxs-lookup"><span data-stu-id="872f7-148">Contains a friendly name for the skill.</span></span> |
|<span data-ttu-id="872f7-149">вывод</span><span class="sxs-lookup"><span data-stu-id="872f7-149">inference</span></span>|[<span data-ttu-id="872f7-150">inferenceData</span><span class="sxs-lookup"><span data-stu-id="872f7-150">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="872f7-151">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="872f7-151">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="872f7-152">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="872f7-152">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="872f7-153">профессиональный уровень</span><span class="sxs-lookup"><span data-stu-id="872f7-153">proficiency</span></span>|<span data-ttu-id="872f7-154">skillProficiencyLevel</span><span class="sxs-lookup"><span data-stu-id="872f7-154">skillProficiencyLevel</span></span>|<span data-ttu-id="872f7-155">Подробное знание пользователями этого навыка.</span><span class="sxs-lookup"><span data-stu-id="872f7-155">Detail of the users proficiency with this skill.</span></span> <span data-ttu-id="872f7-156">Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="872f7-156">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|

## <a name="response"></a><span data-ttu-id="872f7-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="872f7-157">Response</span></span>

<span data-ttu-id="872f7-158">В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [skillProficiency](../resources/skillproficiency.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="872f7-158">If successful, this method returns a `200 OK` response code and an updated [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="872f7-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="872f7-159">Examples</span></span>

### <a name="request"></a><span data-ttu-id="872f7-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="872f7-160">Request</span></span>

<span data-ttu-id="872f7-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="872f7-161">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="872f7-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="872f7-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_skillproficiency"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/skills/{id}
Content-type: application/json

{
  "categories": [
    "Professional"
  ],
  "proficiency": "advancedProfessional"
}
```
# <a name="c"></a>[<span data-ttu-id="872f7-163">C#</span><span class="sxs-lookup"><span data-stu-id="872f7-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-skillproficiency-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="872f7-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="872f7-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-skillproficiency-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="872f7-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="872f7-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-skillproficiency-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="872f7-166">Java</span><span class="sxs-lookup"><span data-stu-id="872f7-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-skillproficiency-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="872f7-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="872f7-167">Response</span></span>

<span data-ttu-id="872f7-168">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="872f7-168">The following is an example of the response.</span></span>

> <span data-ttu-id="872f7-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="872f7-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
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
  "categories": [
    "Professional"
  ],
  "displayName": "API Design",
  "proficiency": "advancedProfessional",
  "webUrl": null,
  "collaborationTags": [
    "ableToMentor"
  ]
}
```


