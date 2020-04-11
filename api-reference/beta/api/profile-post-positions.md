---
title: Создание Воркпоситион
description: Используйте этот API для создания нового Воркпоситион.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 0344dc0d0f861fb653f1ed26e2b951978148c8b8
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229313"
---
# <a name="create-workposition"></a><span data-ttu-id="ffd0b-103">Создание Воркпоситион</span><span class="sxs-lookup"><span data-stu-id="ffd0b-103">Create workPosition</span></span>

<span data-ttu-id="ffd0b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffd0b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffd0b-105">Используйте этот API, чтобы создать новый [воркпоситион](../resources/workposition.md) в [профиле](../resources/profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="ffd0b-105">Use this API to create a new [workPosition](../resources/workposition.md) in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ffd0b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffd0b-106">Permissions</span></span>

<span data-ttu-id="ffd0b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffd0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ffd0b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffd0b-109">Permission type</span></span>                        | <span data-ttu-id="ffd0b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffd0b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ffd0b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffd0b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ffd0b-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ffd0b-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ffd0b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffd0b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffd0b-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ffd0b-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="ffd0b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffd0b-115">Application</span></span>                            | <span data-ttu-id="ffd0b-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffd0b-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="ffd0b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffd0b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/profile/positions
```

## <a name="request-headers"></a><span data-ttu-id="ffd0b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffd0b-118">Request headers</span></span>

| <span data-ttu-id="ffd0b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ffd0b-119">Name</span></span>      |<span data-ttu-id="ffd0b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ffd0b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ffd0b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffd0b-121">Authorization</span></span>  | <span data-ttu-id="ffd0b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffd0b-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ffd0b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ffd0b-124">Content-Type</span></span>   | <span data-ttu-id="ffd0b-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffd0b-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffd0b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffd0b-127">Request body</span></span>

<span data-ttu-id="ffd0b-128">В тексте запроса добавьте представление объекта [воркпоситион](../resources/workposition.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffd0b-128">In the request body, supply a JSON representation of [workPosition](../resources/workposition.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ffd0b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffd0b-129">Response</span></span>

<span data-ttu-id="ffd0b-130">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [воркпоситион](../resources/workposition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ffd0b-130">If successful, this method returns `201, Created` response code and a new [workPosition](../resources/workposition.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ffd0b-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="ffd0b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ffd0b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffd0b-132">Request</span></span>

<span data-ttu-id="ffd0b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffd0b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_workposition_from_profile"
}-->

```http
POST https://graph.microsoft.com/Beta/me/profile/positions
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
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
  }
}
```

### <a name="response"></a><span data-ttu-id="ffd0b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffd0b-134">Response</span></span>

<span data-ttu-id="ffd0b-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ffd0b-135">The following is an example of the response.</span></span>

> <span data-ttu-id="ffd0b-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ffd0b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workPosition"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "categories": [
    "categories-value"
  ],
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
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workPosition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->