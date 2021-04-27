---
title: Обновление типа ресурсов projectParticipation
description: Обновление свойств объекта projectParticipation в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 5665c10cbaeb2968b5a17be3f7d30561ed9573d2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055199"
---
# <a name="update-projectparticipation"></a><span data-ttu-id="06fa7-103">Обновление projectparticipation</span><span class="sxs-lookup"><span data-stu-id="06fa7-103">Update projectparticipation</span></span>

<span data-ttu-id="06fa7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06fa7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06fa7-105">Обновление свойств объекта [projectParticipation](../resources/projectParticipation.md) в профиле [пользователя.](../resources/profile.md)</span><span class="sxs-lookup"><span data-stu-id="06fa7-105">Update the properties of a [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06fa7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06fa7-106">Permissions</span></span>

<span data-ttu-id="06fa7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06fa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="06fa7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06fa7-109">Permission type</span></span>                        | <span data-ttu-id="06fa7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06fa7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="06fa7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06fa7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="06fa7-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06fa7-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="06fa7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06fa7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06fa7-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06fa7-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="06fa7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06fa7-115">Application</span></span>                            | <span data-ttu-id="06fa7-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06fa7-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="06fa7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06fa7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
PATCH /users/{id | userPrincipalName}/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="06fa7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06fa7-118">Request headers</span></span>

| <span data-ttu-id="06fa7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="06fa7-119">Name</span></span>           |<span data-ttu-id="06fa7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="06fa7-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="06fa7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06fa7-121">Authorization</span></span>  | <span data-ttu-id="06fa7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06fa7-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="06fa7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="06fa7-124">Content-Type</span></span>   | <span data-ttu-id="06fa7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06fa7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06fa7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="06fa7-127">Request body</span></span>

<span data-ttu-id="06fa7-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="06fa7-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="06fa7-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="06fa7-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="06fa7-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="06fa7-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="06fa7-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="06fa7-131">Property</span></span>|<span data-ttu-id="06fa7-132">Тип</span><span class="sxs-lookup"><span data-stu-id="06fa7-132">Type</span></span>|<span data-ttu-id="06fa7-133">Описание</span><span class="sxs-lookup"><span data-stu-id="06fa7-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06fa7-134">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="06fa7-134">allowedAudiences</span></span>|<span data-ttu-id="06fa7-135">String</span><span class="sxs-lookup"><span data-stu-id="06fa7-135">String</span></span>|<span data-ttu-id="06fa7-136">Аудитории, которые могут видеть значения, содержащиеся в объекте.</span><span class="sxs-lookup"><span data-stu-id="06fa7-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="06fa7-137">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="06fa7-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="06fa7-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="06fa7-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="06fa7-139">categories</span><span class="sxs-lookup"><span data-stu-id="06fa7-139">categories</span></span>|<span data-ttu-id="06fa7-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="06fa7-140">String collection</span></span>|<span data-ttu-id="06fa7-141">Содержит категории, которые пользователь связал с проектом (например, цифровая трансформация, нефтяная вышка).</span><span class="sxs-lookup"><span data-stu-id="06fa7-141">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="06fa7-142">клиент</span><span class="sxs-lookup"><span data-stu-id="06fa7-142">client</span></span>|[<span data-ttu-id="06fa7-143">companyDetail</span><span class="sxs-lookup"><span data-stu-id="06fa7-143">companyDetail</span></span>](../resources/companydetail.md)|<span data-ttu-id="06fa7-144">Содержит подробные сведения о клиенте, для который был проект.</span><span class="sxs-lookup"><span data-stu-id="06fa7-144">Contains detailed information about the client the project was for.</span></span> |
|<span data-ttu-id="06fa7-145">collaborationTags</span><span class="sxs-lookup"><span data-stu-id="06fa7-145">collaborationTags</span></span>|<span data-ttu-id="06fa7-146">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="06fa7-146">String collection</span></span>|<span data-ttu-id="06fa7-147">Содержит теги сценариев работы, которые пользователь связал с интересом.</span><span class="sxs-lookup"><span data-stu-id="06fa7-147">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="06fa7-148">Допустимые значения в коллекции: `askMeAbout` , `ableToMentor` , `wantsToLearn` `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="06fa7-148">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="06fa7-149">коллеги</span><span class="sxs-lookup"><span data-stu-id="06fa7-149">colleagues</span></span>|<span data-ttu-id="06fa7-150">[коллекция relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="06fa7-150">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="06fa7-151">Списки людей, которые также работали над проектом.</span><span class="sxs-lookup"><span data-stu-id="06fa7-151">Lists people that also worked on the project.</span></span> |
|<span data-ttu-id="06fa7-152">подробные</span><span class="sxs-lookup"><span data-stu-id="06fa7-152">detail</span></span>|[<span data-ttu-id="06fa7-153">positionDetail</span><span class="sxs-lookup"><span data-stu-id="06fa7-153">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="06fa7-154">Содержит сведения о роли пользователя в проекте.</span><span class="sxs-lookup"><span data-stu-id="06fa7-154">Contains detail about the user's role on the project.</span></span>|
|<span data-ttu-id="06fa7-155">displayName</span><span class="sxs-lookup"><span data-stu-id="06fa7-155">displayName</span></span>|<span data-ttu-id="06fa7-156">String</span><span class="sxs-lookup"><span data-stu-id="06fa7-156">String</span></span>|<span data-ttu-id="06fa7-157">Содержит удобное имя для проекта.</span><span class="sxs-lookup"><span data-stu-id="06fa7-157">Contains a friendly name for the project.</span></span>|
|<span data-ttu-id="06fa7-158">вывод</span><span class="sxs-lookup"><span data-stu-id="06fa7-158">inference</span></span>|[<span data-ttu-id="06fa7-159">inferenceData</span><span class="sxs-lookup"><span data-stu-id="06fa7-159">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="06fa7-160">Содержит сведения о выводе, если объект создается или модифицируют приложение.</span><span class="sxs-lookup"><span data-stu-id="06fa7-160">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="06fa7-161">Унаследовано от [itemFacet](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="06fa7-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="06fa7-162">спонсоры</span><span class="sxs-lookup"><span data-stu-id="06fa7-162">sponsors</span></span>|<span data-ttu-id="06fa7-163">[коллекция relatedPerson](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="06fa7-163">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="06fa7-164">Лицо или люди, которые спонсировали проект.</span><span class="sxs-lookup"><span data-stu-id="06fa7-164">The Person or people who sponsored the project.</span></span>    |

## <a name="response"></a><span data-ttu-id="06fa7-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="06fa7-165">Response</span></span>

<span data-ttu-id="06fa7-166">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект projectParticipation](../resources/projectparticipation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="06fa7-166">If successful, this method returns a `200 OK` response code and an updated [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06fa7-167">Примеры</span><span class="sxs-lookup"><span data-stu-id="06fa7-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06fa7-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="06fa7-168">Request</span></span>

<span data-ttu-id="06fa7-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06fa7-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="06fa7-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="06fa7-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_projectparticipation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/projects/{id}
Content-type: application/json

{
  "allowedAudiences": "organization",
  "client": {
    "department": "Corporate Marketing",
    "webUrl": "https://www.contoso.com"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="06fa7-171">C#</span><span class="sxs-lookup"><span data-stu-id="06fa7-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06fa7-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06fa7-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06fa7-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06fa7-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06fa7-174">Java</span><span class="sxs-lookup"><span data-stu-id="06fa7-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-projectparticipation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="06fa7-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="06fa7-175">Response</span></span>

<span data-ttu-id="06fa7-176">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="06fa7-176">The following is an example of the response.</span></span>

> <span data-ttu-id="06fa7-177">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="06fa7-177">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
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


