---
title: Создание ПрожектпартиЦипатион
description: Используйте этот API для создания нового ПрожектпартиЦипатион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: b3e2cae6b14f3e7f8ea336bb3000bfa8e4894ac2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034408"
---
# <a name="create-projectparticipation"></a><span data-ttu-id="d6fa7-103">Создание ПрожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="d6fa7-103">Create projectParticipation</span></span>

<span data-ttu-id="d6fa7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6fa7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6fa7-105">Используйте этот API, чтобы создать новый объект [прожектпартиЦипатион](../resources/projectParticipation.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-105">Use this API to create a new [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6fa7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6fa7-106">Permissions</span></span>

<span data-ttu-id="d6fa7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6fa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6fa7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6fa7-109">Permission type</span></span>                        | <span data-ttu-id="d6fa7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6fa7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d6fa7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6fa7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6fa7-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d6fa7-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d6fa7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6fa7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6fa7-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d6fa7-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="d6fa7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6fa7-115">Application</span></span>                            | <span data-ttu-id="d6fa7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6fa7-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="d6fa7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6fa7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/projects
POST /users/{id | userPrincipalName}/profile/projects
```

## <a name="request-headers"></a><span data-ttu-id="d6fa7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6fa7-118">Request headers</span></span>

| <span data-ttu-id="d6fa7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d6fa7-119">Name</span></span>           |<span data-ttu-id="d6fa7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d6fa7-120">Description</span></span>                  |
|:---------------|:----------                  |
| <span data-ttu-id="d6fa7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6fa7-121">Authorization</span></span>  | <span data-ttu-id="d6fa7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="d6fa7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6fa7-124">Content-Type</span></span>   | <span data-ttu-id="d6fa7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6fa7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6fa7-127">Request body</span></span>

<span data-ttu-id="d6fa7-128">В тексте запроса добавьте представление объекта [прожектпартиЦипатион](../resources/projectparticipation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-128">In the request body, supply a JSON representation of [projectParticipation](../resources/projectparticipation.md) object.</span></span>

<span data-ttu-id="d6fa7-129">В следующей таблице приведены свойства, которые можно задать при создании нового объекта [прожектпартиЦипатион](../resources/projectParticipation.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-129">The following table shows the properties that are possible to set when you create a new [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="d6fa7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6fa7-130">Property</span></span>|<span data-ttu-id="d6fa7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d6fa7-131">Type</span></span>|<span data-ttu-id="d6fa7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d6fa7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6fa7-133">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="d6fa7-133">allowedAudiences</span></span>|<span data-ttu-id="d6fa7-134">String</span><span class="sxs-lookup"><span data-stu-id="d6fa7-134">String</span></span>|<span data-ttu-id="d6fa7-135">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="d6fa7-136">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d6fa7-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="d6fa7-137">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d6fa7-138">categories</span><span class="sxs-lookup"><span data-stu-id="d6fa7-138">categories</span></span>|<span data-ttu-id="d6fa7-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d6fa7-139">String collection</span></span>|<span data-ttu-id="d6fa7-140">Содержит категории, связанные с проектом пользователем (например, цифровое преобразование, гидростенд).</span><span class="sxs-lookup"><span data-stu-id="d6fa7-140">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="d6fa7-141">Клиенты</span><span class="sxs-lookup"><span data-stu-id="d6fa7-141">client</span></span>|[<span data-ttu-id="d6fa7-142">компанидетаил</span><span class="sxs-lookup"><span data-stu-id="d6fa7-142">companyDetail</span></span>](../resources/companydetail.md)|<span data-ttu-id="d6fa7-143">Содержит подробные сведения о клиенте, для которого выполнялся проект.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-143">Contains detailed information about the client the project was for.</span></span> |
|<span data-ttu-id="d6fa7-144">коллаборатионтагс</span><span class="sxs-lookup"><span data-stu-id="d6fa7-144">collaborationTags</span></span>|<span data-ttu-id="d6fa7-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d6fa7-145">String collection</span></span>|<span data-ttu-id="d6fa7-146">Содержит теги сценариев, с которыми пользователь связан с интересом.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-146">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="d6fa7-147">Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="d6fa7-147">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="d6fa7-148">коллег</span><span class="sxs-lookup"><span data-stu-id="d6fa7-148">colleagues</span></span>|<span data-ttu-id="d6fa7-149">Коллекция [релатедперсон](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="d6fa7-149">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="d6fa7-150">Список людей, которые также работали над проектом.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-150">Lists people that also worked on the project.</span></span> |
|<span data-ttu-id="d6fa7-151">описаны</span><span class="sxs-lookup"><span data-stu-id="d6fa7-151">detail</span></span>|[<span data-ttu-id="d6fa7-152">поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="d6fa7-152">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="d6fa7-153">Содержит подробные сведения о роли пользователя в проекте.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-153">Contains detail about the user's role on the project.</span></span>|
|<span data-ttu-id="d6fa7-154">displayName</span><span class="sxs-lookup"><span data-stu-id="d6fa7-154">displayName</span></span>|<span data-ttu-id="d6fa7-155">String</span><span class="sxs-lookup"><span data-stu-id="d6fa7-155">String</span></span>|<span data-ttu-id="d6fa7-156">Содержит понятное имя проекта.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-156">Contains a friendly name for the project.</span></span>|
|<span data-ttu-id="d6fa7-157">выводов</span><span class="sxs-lookup"><span data-stu-id="d6fa7-157">inference</span></span>|[<span data-ttu-id="d6fa7-158">инференцедата</span><span class="sxs-lookup"><span data-stu-id="d6fa7-158">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="d6fa7-159">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-159">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="d6fa7-160">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d6fa7-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d6fa7-161">source</span><span class="sxs-lookup"><span data-stu-id="d6fa7-161">source</span></span>|[<span data-ttu-id="d6fa7-162">персондатасаурце</span><span class="sxs-lookup"><span data-stu-id="d6fa7-162">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="d6fa7-163">Источник значений при синхронизации от другой службы.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-163">Where the values originated if synced from another service.</span></span> <span data-ttu-id="d6fa7-164">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d6fa7-164">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="d6fa7-165">спонсорами</span><span class="sxs-lookup"><span data-stu-id="d6fa7-165">sponsors</span></span>|<span data-ttu-id="d6fa7-166">Коллекция [релатедперсон](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="d6fa7-166">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="d6fa7-167">Пользователь или люди, которые спонсорируют проект.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-167">The Person or people who sponsored the project.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="d6fa7-168">Отношения</span><span class="sxs-lookup"><span data-stu-id="d6fa7-168">Relationships</span></span>

## <a name="response"></a><span data-ttu-id="d6fa7-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6fa7-169">Response</span></span>

<span data-ttu-id="d6fa7-170">В случае успешного выполнения этот метод возвращает `201, Created` код отклика и новый объект [прожектпартиЦипатион](../resources/projectparticipation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-170">If successful, this method returns `201, Created` response code and a new [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d6fa7-171">Примеры</span><span class="sxs-lookup"><span data-stu-id="d6fa7-171">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d6fa7-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6fa7-172">Request</span></span>

<span data-ttu-id="d6fa7-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6fa7-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6fa7-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_projectparticipation_from_profile"
}-->

```http
POST https://graph.microsoft.com/beta/me/profile/projects
Content-type: application/json

{
  "categories": [
    "Branding"
  ],
  "client": {
    "displayName": "Contoso Ltd.",
    "department": "Corporate Marketing",
    "webUrl": "https://www.contoso.com"
  },
  "displayName": "Contoso Re-branding Project",
  "detail": {
    "company": {
      "displayName": "Adventureworks Inc.",
      "department": "Consulting",
      "webUrl": "https://adventureworks.com"
    },
    "description": "Rebranding of Contoso Ltd.",
    "jobTitle": "Lead PM Rebranding",
    "role": "project management",
    "summary": "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
  }
}
```
# <a name="c"></a>[<span data-ttu-id="d6fa7-175">C#</span><span class="sxs-lookup"><span data-stu-id="d6fa7-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-projectparticipation-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6fa7-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6fa7-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-projectparticipation-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6fa7-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6fa7-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-projectparticipation-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d6fa7-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6fa7-178">Response</span></span>

<span data-ttu-id="d6fa7-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-179">The following is an example of the response.</span></span>

> <span data-ttu-id="d6fa7-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6fa7-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
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
  "categories": [
    "Branding"
  ],
  "client": {
    "displayName": "Contoso Ltd.",
    "pronunciation": null,
    "department": "Corporate Marketing",
    "officeLocation": null,
    "address": null,
    "webUrl": "https://www.contoso.com"
  },
  "displayName": "Contoso Re-branding Project",
  "detail": {
    "company": {
      "displayName": "Adventureworks Inc.",
      "pronunciation": null,
      "department": "Consulting",
      "officeLocation": null,
      "address": null,
      "webUrl": "https://adventureworks.com"
    },
    "description": "Rebranding of Contoso Ltd.",
    "endMonthYear": "datetime-value",
    "jobTitle": "Lead PM Rebranding",
    "role": "project management",
    "startMonthYear": "datetime-value",
    "summary": "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
  },
  "colleagues": null,
  "sponsors": null
}
```


