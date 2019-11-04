---
title: Создание Едукатионалактивити
description: Создание нового Едукатионалактивити.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 9d860955227de6b85f110c794e264559586fa172
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937716"
---
# <a name="create-educationalactivity"></a><span data-ttu-id="79881-103">Создание Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="79881-103">Create educationalActivity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79881-104">Создайте новый [едукатионалактивити](../resources/educationalactivity.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="79881-104">Create a new [educationalActivity](../resources/educationalactivity.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="79881-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="79881-105">Permissions</span></span>

<span data-ttu-id="79881-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79881-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79881-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="79881-108">Permission type</span></span>                        | <span data-ttu-id="79881-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="79881-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="79881-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="79881-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="79881-111">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="79881-111">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="79881-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="79881-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79881-113">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="79881-113">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="79881-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="79881-114">Application</span></span>                            | <span data-ttu-id="79881-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79881-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79881-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="79881-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /user/profile/educationalActivities
```

## <a name="request-headers"></a><span data-ttu-id="79881-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="79881-117">Request headers</span></span>

| <span data-ttu-id="79881-118">Имя</span><span class="sxs-lookup"><span data-stu-id="79881-118">Name</span></span>      |<span data-ttu-id="79881-119">Описание</span><span class="sxs-lookup"><span data-stu-id="79881-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="79881-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="79881-120">Authorization</span></span>  | <span data-ttu-id="79881-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79881-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="79881-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="79881-123">Content-Type</span></span>   | <span data-ttu-id="79881-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="79881-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79881-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="79881-126">Request body</span></span>

<span data-ttu-id="79881-127">В тексте запроса добавьте представление объекта [едукатионалактивити](../resources/educationalactivity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79881-127">In the request body, supply a JSON representation of an [educationalActivity](../resources/educationalactivity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="79881-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="79881-128">Response</span></span>

<span data-ttu-id="79881-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [едукатионалактивити](../resources/educationalactivity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="79881-129">If successful, this method returns a `201 Created` response code and a new [educationalActivity](../resources/educationalactivity.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79881-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="79881-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="79881-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="79881-131">Request</span></span>

<span data-ttu-id="79881-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="79881-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationalactivity_from_profile"
}-->

```http
POST /me/profile/educationalActivities
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
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
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```

### <a name="response"></a><span data-ttu-id="79881-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="79881-133">Response</span></span>

<span data-ttu-id="79881-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="79881-134">The following is an example of the response.</span></span>

> <span data-ttu-id="79881-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="79881-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationalActivity"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "completionMonthYear": "datetime-value",
  "endMonthYear": "datetime-value",
  "institution": {
    "description": "description-value",
    "displayName": "displayName-value",
    "location": {
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
  "program": {
    "abbreviation": "abbreviation-value",
    "activities": "activities-value",
    "awards": "awards-value",
    "description": "description-value",
    "displayName": "displayName-value",
    "fieldsOfStudy": "fieldsOfStudy-value",
    "grade": "grade-value",
    "notes": "notes-value",
    "webUrl": "webUrl-value"
  },
  "startMonthYear": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationalActivity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
