---
title: Обновление типа ресурса ПрожектпартиЦипатион
description: Обновление свойств объекта ПрожектпартиЦипатион в профиле пользователя.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 3ee963f30289cb07c96860c2f0aeb5ec6096dac2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938417"
---
# <a name="update-projectparticipation"></a><span data-ttu-id="ca25d-103">Обновление прожектпартиЦипатион</span><span class="sxs-lookup"><span data-stu-id="ca25d-103">Update projectparticipation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca25d-104">Обновление свойств объекта [прожектпартиЦипатион](../resources/projectParticipation.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="ca25d-104">Update the properties of a [projectParticipation](../resources/projectParticipation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca25d-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca25d-105">Permissions</span></span>

<span data-ttu-id="ca25d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca25d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ca25d-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca25d-108">Permission type</span></span>                        | <span data-ttu-id="ca25d-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca25d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ca25d-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca25d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ca25d-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ca25d-111">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ca25d-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca25d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca25d-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ca25d-113">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ca25d-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca25d-114">Application</span></span>                            | <span data-ttu-id="ca25d-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca25d-115">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="ca25d-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca25d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/projects/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ca25d-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca25d-117">Request headers</span></span>

| <span data-ttu-id="ca25d-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ca25d-118">Name</span></span>           |<span data-ttu-id="ca25d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ca25d-119">Description</span></span>                  |
|:---------------|:----------------------------|
| <span data-ttu-id="ca25d-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca25d-120">Authorization</span></span>  | <span data-ttu-id="ca25d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca25d-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ca25d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca25d-123">Content-Type</span></span>   | <span data-ttu-id="ca25d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca25d-p103">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ca25d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca25d-126">Request body</span></span>

<span data-ttu-id="ca25d-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="ca25d-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ca25d-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="ca25d-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ca25d-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="ca25d-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ca25d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca25d-130">Property</span></span>     | <span data-ttu-id="ca25d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ca25d-131">Type</span></span>                                                     | <span data-ttu-id="ca25d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ca25d-132">Description</span></span>                                                                                        |
|:-------------|:---------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
|<span data-ttu-id="ca25d-133">categories</span><span class="sxs-lookup"><span data-stu-id="ca25d-133">categories</span></span>    |<span data-ttu-id="ca25d-134">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ca25d-134">String collection</span></span>                                         | <span data-ttu-id="ca25d-135">Содержит категории, связанные с проектом пользователем (например, цифровое преобразование, на платформе для нефтегазовой платформы)</span><span class="sxs-lookup"><span data-stu-id="ca25d-135">Contains categories a user has associated with the project (eg: digital transformation, oil rig)</span></span>   |
|<span data-ttu-id="ca25d-136">Клиенты</span><span class="sxs-lookup"><span data-stu-id="ca25d-136">client</span></span>        |[<span data-ttu-id="ca25d-137">компанидетаил</span><span class="sxs-lookup"><span data-stu-id="ca25d-137">companyDetail</span></span>](../resources/companydetail.md)            | <span data-ttu-id="ca25d-138">Содержит подробные сведения о клиенте, для которого выполнялся проект.</span><span class="sxs-lookup"><span data-stu-id="ca25d-138">Contains detailed information about the client the project was for.</span></span>                                |
|<span data-ttu-id="ca25d-139">коллег</span><span class="sxs-lookup"><span data-stu-id="ca25d-139">colleagues</span></span>    |<span data-ttu-id="ca25d-140">Коллекция [релатедперсон](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="ca25d-140">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="ca25d-141">Пользователи, которые также работали над проектом.</span><span class="sxs-lookup"><span data-stu-id="ca25d-141">People that also worked on the project.</span></span>                                                            |
|<span data-ttu-id="ca25d-142">описаны</span><span class="sxs-lookup"><span data-stu-id="ca25d-142">detail</span></span>        |[<span data-ttu-id="ca25d-143">поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="ca25d-143">positionDetail</span></span>](../resources/positiondetail.md)          | <span data-ttu-id="ca25d-144">Содержит подробные сведения о роли пользователей в проекте.</span><span class="sxs-lookup"><span data-stu-id="ca25d-144">Contains detail about the users role on the project.</span></span>                                               |
|<span data-ttu-id="ca25d-145">displayName</span><span class="sxs-lookup"><span data-stu-id="ca25d-145">displayName</span></span>   |<span data-ttu-id="ca25d-146">Строка</span><span class="sxs-lookup"><span data-stu-id="ca25d-146">String</span></span>                                                    | <span data-ttu-id="ca25d-147">Содержит понятное имя проекта.</span><span class="sxs-lookup"><span data-stu-id="ca25d-147">Contains a friendly name for the project.</span></span>                                                          |
|<span data-ttu-id="ca25d-148">спонсорами</span><span class="sxs-lookup"><span data-stu-id="ca25d-148">sponsors</span></span>      |<span data-ttu-id="ca25d-149">Коллекция [релатедперсон](../resources/relatedperson.md)</span><span class="sxs-lookup"><span data-stu-id="ca25d-149">[relatedPerson](../resources/relatedperson.md) collection</span></span> | <span data-ttu-id="ca25d-150">Пользователь (люди), который спонсор проекта.</span><span class="sxs-lookup"><span data-stu-id="ca25d-150">Person(People) who sponsored the project.</span></span>                                                          |

## <a name="response"></a><span data-ttu-id="ca25d-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca25d-151">Response</span></span>

<span data-ttu-id="ca25d-152">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [прожектпартиЦипатион](../resources/projectparticipation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca25d-152">If successful, this method returns a `200 OK` response code and an updated [projectParticipation](../resources/projectparticipation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca25d-153">Примеры</span><span class="sxs-lookup"><span data-stu-id="ca25d-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ca25d-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca25d-154">Request</span></span>

<span data-ttu-id="ca25d-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca25d-155">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_projectparticipation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/projects/{id}
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ca25d-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca25d-156">Response</span></span>

<span data-ttu-id="ca25d-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca25d-157">The following is an example of the response.</span></span>

> <span data-ttu-id="ca25d-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca25d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.projectParticipation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
  "client": {
    "displayName": "displayName-value",
    "pronunciation": "pronunciation-value",
    "department": "department-value",
    "officeLocation": "officeLocation-value",
    "address": {
      "type": "type-value",
      "postOfficeBox": "postOfficeBox-value",
      "street": "street-value",
      "city": "city-value",
      "state": "state-value",
      "countryOrRegion": "countryOrRegion-value",
      "postalCode": "postalCode-value"
    },
    "webUrl": "webUrl-value"
  },
  "displayName": "displayName-value",
  "detail": {
    "company": {
      "displayName": "displayName-value",
      "pronunciation": "pronunciation-value",
      "department": "department-value",
      "officeLocation": "officeLocation-value",
      "address": {
        "type": "type-value",
        "postOfficeBox": "postOfficeBox-value",
        "street": "street-value",
        "city": "city-value",
        "state": "state-value",
        "countryOrRegion": "countryOrRegion-value",
        "postalCode": "postalCode-value"
      },
      "webUrl": "webUrl-value"
    },
    "description": "description-value",
    "endMonthYear": "datetime-value",
    "jobTitle": "jobTitle-value",
    "role": "role-value",
    "startMonthYear": "datetime-value",
    "summary": "summary-value"
  },
  "colleagues": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ],
  "sponsors": [
    {
      "displayName": "displayName-value",
      "relationship": "relationship-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update projectparticipation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->