---
title: Создание СкиллпрофиЦиенци
description: Используйте этот API для создания нового СкиллпрофиЦиенци.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: a13713904da19cc4b13729633e63e81275596833
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034359"
---
# <a name="create-skillproficiency"></a><span data-ttu-id="ef2b7-103">Создание СкиллпрофиЦиенци</span><span class="sxs-lookup"><span data-stu-id="ef2b7-103">Create skillProficiency</span></span>

<span data-ttu-id="ef2b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef2b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef2b7-105">Используйте этот API, чтобы создать новый объект [скиллпрофиЦиенци](../resources/skillproficiency.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-105">Use this API to create a new [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef2b7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef2b7-106">Permissions</span></span>

<span data-ttu-id="ef2b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef2b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef2b7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef2b7-109">Permission type</span></span>                        | <span data-ttu-id="ef2b7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef2b7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ef2b7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef2b7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef2b7-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ef2b7-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ef2b7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef2b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef2b7-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ef2b7-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ef2b7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef2b7-115">Application</span></span>                            | <span data-ttu-id="ef2b7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef2b7-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="ef2b7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef2b7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/skills
POST /users/{id | userPrincipalName}/profile/skills
```

## <a name="request-headers"></a><span data-ttu-id="ef2b7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef2b7-118">Request headers</span></span>

| <span data-ttu-id="ef2b7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ef2b7-119">Name</span></span>           | <span data-ttu-id="ef2b7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ef2b7-120">Description</span></span>                 |
|:---------------|:----------------------------|
| <span data-ttu-id="ef2b7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef2b7-121">Authorization</span></span>  | <span data-ttu-id="ef2b7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ef2b7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef2b7-124">Content-Type</span></span>   | <span data-ttu-id="ef2b7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef2b7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef2b7-127">Request body</span></span>

<span data-ttu-id="ef2b7-128">В тексте запроса добавьте представление объекта [скиллпрофиЦиенци](../resources/skillproficiency.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-128">In the request body, supply a JSON representation of [skillProficiency](../resources/skillproficiency.md) object.</span></span>

<span data-ttu-id="ef2b7-129">В следующей таблице приведены свойства, которые можно задать при создании нового объекта [скиллпрофиЦиенци](../resources/skillproficiency.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-129">The following table shows the properties that are possible to set when you create a new [skillProficiency](../resources/skillproficiency.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="ef2b7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef2b7-130">Property</span></span>|<span data-ttu-id="ef2b7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ef2b7-131">Type</span></span>|<span data-ttu-id="ef2b7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ef2b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef2b7-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="ef2b7-133">allowedAudiences</span></span>|<span data-ttu-id="ef2b7-134">String</span><span class="sxs-lookup"><span data-stu-id="ef2b7-134">String</span></span>|<span data-ttu-id="ef2b7-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="ef2b7-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ef2b7-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="ef2b7-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ef2b7-138">categories</span><span class="sxs-lookup"><span data-stu-id="ef2b7-138">categories</span></span>|<span data-ttu-id="ef2b7-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ef2b7-139">String collection</span></span>|<span data-ttu-id="ef2b7-140">Содержит категории, связанные с навыком пользователя (например, персональный, профессиональный, увлеченный).</span><span class="sxs-lookup"><span data-stu-id="ef2b7-140">Contains categories a user has associated with the skill (for example, personal, professional, hobby).</span></span> |
|<span data-ttu-id="ef2b7-141">коллаборатионтагс</span><span class="sxs-lookup"><span data-stu-id="ef2b7-141">collaborationTags</span></span>|<span data-ttu-id="ef2b7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ef2b7-142">String collection</span></span>|<span data-ttu-id="ef2b7-143">Содержит теги сценариев, с которыми пользователь связан с интересом.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-143">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="ef2b7-144">Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="ef2b7-144">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="ef2b7-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ef2b7-145">displayName</span></span>|<span data-ttu-id="ef2b7-146">String</span><span class="sxs-lookup"><span data-stu-id="ef2b7-146">String</span></span>|<span data-ttu-id="ef2b7-147">Содержит понятное имя для навыка.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-147">Contains a friendly name for the skill.</span></span> |
|<span data-ttu-id="ef2b7-148">выводов</span><span class="sxs-lookup"><span data-stu-id="ef2b7-148">inference</span></span>|[<span data-ttu-id="ef2b7-149">инференцедата</span><span class="sxs-lookup"><span data-stu-id="ef2b7-149">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="ef2b7-150">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-150">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="ef2b7-151">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ef2b7-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ef2b7-152">навыки</span><span class="sxs-lookup"><span data-stu-id="ef2b7-152">proficiency</span></span>|<span data-ttu-id="ef2b7-153">скиллпрофиЦиенцилевел</span><span class="sxs-lookup"><span data-stu-id="ef2b7-153">skillProficiencyLevel</span></span>|<span data-ttu-id="ef2b7-154">Сведения о пользователях, которые подключают этот навык.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-154">Detail of the users proficiency with this skill.</span></span> <span data-ttu-id="ef2b7-155">Возможные значения: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-155">Possible values are: `elementary`, `limitedWorking`, `generalProfessional`, `advancedProfessional`, `expert`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="ef2b7-156">source</span><span class="sxs-lookup"><span data-stu-id="ef2b7-156">source</span></span>|[<span data-ttu-id="ef2b7-157">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="ef2b7-157">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="ef2b7-158">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-158">Where the values originated if synced from another service.</span></span> <span data-ttu-id="ef2b7-159">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="ef2b7-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="ef2b7-160">webUrl</span><span class="sxs-lookup"><span data-stu-id="ef2b7-160">webUrl</span></span>|<span data-ttu-id="ef2b7-161">String</span><span class="sxs-lookup"><span data-stu-id="ef2b7-161">String</span></span>|<span data-ttu-id="ef2b7-162">Содержит ссылку на источник информации о навыке.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-162">Contains a link to an information source about the skill.</span></span> |

## <a name="response"></a><span data-ttu-id="ef2b7-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef2b7-163">Response</span></span>

<span data-ttu-id="ef2b7-164">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и новый объект [скиллпрофиЦиенци](../resources/skillproficiency.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-164">If successful, this method returns `201, Created` response code and a new [skillProficiency](../resources/skillproficiency.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef2b7-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="ef2b7-165">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ef2b7-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef2b7-166">Request</span></span>

<span data-ttu-id="ef2b7-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ef2b7-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef2b7-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_skillproficiency_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/skills
Content-type: application/json

{
  "categories": [
    "Professional"
  ],
  "allowedAudiences": "organization",
  "displayName": "API Design",
  "proficiency": "generalProfessional",
  "collaborationTags": [
    "ableToMentor"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ef2b7-169">C#</span><span class="sxs-lookup"><span data-stu-id="ef2b7-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-skillproficiency-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef2b7-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef2b7-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-skillproficiency-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef2b7-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef2b7-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-skillproficiency-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ef2b7-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef2b7-172">Response</span></span>
<span data-ttu-id="ef2b7-173">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ef2b7-173">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skillProficiency"
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


