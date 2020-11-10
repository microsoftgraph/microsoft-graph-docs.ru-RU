---
title: Обновление типа ресурса ПрожектпартиЦипатион
description: Обновление свойств объекта ПрожектпартиЦипатион в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 61e03f2a63a5654486e88b7b2f8588680cac3999
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968974"
---
# <a name="update-projectparticipation"></a><span data-ttu-id="28c0b-103">Обновление прожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="28c0b-103">Update projectparticipation</span></span>

<span data-ttu-id="28c0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28c0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28c0b-105">Обновление свойств объекта [прожектпартиЦипатион](../resources/projectParticipation.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="28c0b-105">Update the properties of a [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="28c0b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28c0b-106">Permissions</span></span>

<span data-ttu-id="28c0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28c0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28c0b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28c0b-109">Permission type</span></span>                        | <span data-ttu-id="28c0b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28c0b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="28c0b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28c0b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="28c0b-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="28c0b-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="28c0b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28c0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28c0b-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="28c0b-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="28c0b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28c0b-115">Application</span></span>                            | <span data-ttu-id="28c0b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28c0b-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="28c0b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28c0b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
PATCH /users/{id | userPrincipalName}/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="28c0b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28c0b-118">Request headers</span></span>

| <span data-ttu-id="28c0b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="28c0b-119">Name</span></span>           |<span data-ttu-id="28c0b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="28c0b-120">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="28c0b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28c0b-121">Authorization</span></span>  | <span data-ttu-id="28c0b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28c0b-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="28c0b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28c0b-124">Content-Type</span></span>   | <span data-ttu-id="28c0b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28c0b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28c0b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28c0b-127">Request body</span></span>

<span data-ttu-id="28c0b-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="28c0b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="28c0b-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="28c0b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="28c0b-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="28c0b-130">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="28c0b-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="28c0b-131">Property</span></span>|<span data-ttu-id="28c0b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="28c0b-132">Type</span></span>|<span data-ttu-id="28c0b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="28c0b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28c0b-134">алловедаудиенцес</span><span class="sxs-lookup"><span data-stu-id="28c0b-134">allowedAudiences</span></span>|<span data-ttu-id="28c0b-135">String</span><span class="sxs-lookup"><span data-stu-id="28c0b-135">String</span></span>|<span data-ttu-id="28c0b-136">Аудитории, которые могут видеть значения, содержащиеся в сущности.</span><span class="sxs-lookup"><span data-stu-id="28c0b-136">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="28c0b-137">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="28c0b-137">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="28c0b-138">Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="28c0b-138">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="28c0b-139">categories</span><span class="sxs-lookup"><span data-stu-id="28c0b-139">categories</span></span>|<span data-ttu-id="28c0b-140">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="28c0b-140">String collection</span></span>|<span data-ttu-id="28c0b-141">Содержит категории, связанные с проектом пользователем (например, цифровое преобразование, гидростенд).</span><span class="sxs-lookup"><span data-stu-id="28c0b-141">Contains categories a user has associated with the project (for example, digital transformation, oil rig).</span></span> |
|<span data-ttu-id="28c0b-142">Клиенты</span><span class="sxs-lookup"><span data-stu-id="28c0b-142">client</span></span>|[<span data-ttu-id="28c0b-143">компанидетаил</span><span class="sxs-lookup"><span data-stu-id="28c0b-143">companyDetail</span></span>](../resources/companydetail.md)|<span data-ttu-id="28c0b-144">Содержит подробные сведения о клиенте, для которого выполнялся проект.</span><span class="sxs-lookup"><span data-stu-id="28c0b-144">Contains detailed information about the client the project was for.</span></span> |
|<span data-ttu-id="28c0b-145">коллаборатионтагс</span><span class="sxs-lookup"><span data-stu-id="28c0b-145">collaborationTags</span></span>|<span data-ttu-id="28c0b-146">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="28c0b-146">String collection</span></span>|<span data-ttu-id="28c0b-147">Содержит теги сценариев, с которыми пользователь связан с интересом.</span><span class="sxs-lookup"><span data-stu-id="28c0b-147">Contains experience scenario tags a user has associated with the interest.</span></span> <span data-ttu-id="28c0b-148">Допустимые значения в коллекции: `askMeAbout` ,, `ableToMentor` `wantsToLearn` , `wantsToImprove` .</span><span class="sxs-lookup"><span data-stu-id="28c0b-148">Allowed values in the collection are: `askMeAbout`, `ableToMentor`, `wantsToLearn`, `wantsToImprove`.</span></span>|
|<span data-ttu-id="28c0b-149">коллег</span><span class="sxs-lookup"><span data-stu-id="28c0b-149">colleagues</span></span>|<span data-ttu-id="28c0b-150">Коллекция [релатедперсон](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="28c0b-150">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="28c0b-151">Список людей, которые также работали над проектом.</span><span class="sxs-lookup"><span data-stu-id="28c0b-151">Lists people that also worked on the project.</span></span> |
|<span data-ttu-id="28c0b-152">описаны</span><span class="sxs-lookup"><span data-stu-id="28c0b-152">detail</span></span>|[<span data-ttu-id="28c0b-153">поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="28c0b-153">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="28c0b-154">Содержит подробные сведения о роли пользователя в проекте.</span><span class="sxs-lookup"><span data-stu-id="28c0b-154">Contains detail about the user's role on the project.</span></span>|
|<span data-ttu-id="28c0b-155">displayName</span><span class="sxs-lookup"><span data-stu-id="28c0b-155">displayName</span></span>|<span data-ttu-id="28c0b-156">String</span><span class="sxs-lookup"><span data-stu-id="28c0b-156">String</span></span>|<span data-ttu-id="28c0b-157">Содержит понятное имя проекта.</span><span class="sxs-lookup"><span data-stu-id="28c0b-157">Contains a friendly name for the project.</span></span>|
|<span data-ttu-id="28c0b-158">выводов</span><span class="sxs-lookup"><span data-stu-id="28c0b-158">inference</span></span>|[<span data-ttu-id="28c0b-159">инференцедата</span><span class="sxs-lookup"><span data-stu-id="28c0b-159">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="28c0b-160">Содержит сведения о выводе, если объект создается или изменяется приложением.</span><span class="sxs-lookup"><span data-stu-id="28c0b-160">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="28c0b-161">Наследуется от [итемфацет](../resources/itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="28c0b-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="28c0b-162">спонсорами</span><span class="sxs-lookup"><span data-stu-id="28c0b-162">sponsors</span></span>|<span data-ttu-id="28c0b-163">Коллекция [релатедперсон](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="28c0b-163">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="28c0b-164">Пользователь или люди, которые спонсорируют проект.</span><span class="sxs-lookup"><span data-stu-id="28c0b-164">The Person or people who sponsored the project.</span></span>    |

## <a name="response"></a><span data-ttu-id="28c0b-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="28c0b-165">Response</span></span>

<span data-ttu-id="28c0b-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [прожектпартиЦипатион](../resources/projectparticipation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="28c0b-166">If successful, this method returns a `200 OK` response code and an updated [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28c0b-167">Примеры</span><span class="sxs-lookup"><span data-stu-id="28c0b-167">Examples</span></span>

### <a name="request"></a><span data-ttu-id="28c0b-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="28c0b-168">Request</span></span>

<span data-ttu-id="28c0b-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28c0b-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28c0b-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="28c0b-170">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="28c0b-171">C#</span><span class="sxs-lookup"><span data-stu-id="28c0b-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-projectparticipation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28c0b-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28c0b-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-projectparticipation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28c0b-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28c0b-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-projectparticipation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28c0b-174">Java</span><span class="sxs-lookup"><span data-stu-id="28c0b-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-projectparticipation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="28c0b-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="28c0b-175">Response</span></span>

<span data-ttu-id="28c0b-176">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28c0b-176">The following is an example of the response.</span></span>

> <span data-ttu-id="28c0b-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28c0b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


