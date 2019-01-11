---
title: Создание educationUser
description: Создание пользователя.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 1636d137ae1a5b8938a59acf60a5eaae578e83f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892157"
---
# <a name="create-educationuser"></a><span data-ttu-id="72a68-103">Создание educationUser</span><span class="sxs-lookup"><span data-stu-id="72a68-103">Create educationUser</span></span>

> <span data-ttu-id="72a68-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="72a68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="72a68-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72a68-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="72a68-106">Создание пользователя.</span><span class="sxs-lookup"><span data-stu-id="72a68-106">Create a new user.</span></span>

<!-- Add some additional text to better distinguish this method from the user_post_users (https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/user_post_users) topic. -->

## <a name="permissions"></a><span data-ttu-id="72a68-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72a68-107">Permissions</span></span>
<span data-ttu-id="72a68-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72a68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72a68-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72a68-110">Permission type</span></span>      | <span data-ttu-id="72a68-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72a68-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72a68-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72a68-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="72a68-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72a68-113">Not supported.</span></span>  |
|<span data-ttu-id="72a68-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72a68-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="72a68-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72a68-115">Not supported.</span></span>  |
|<span data-ttu-id="72a68-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72a68-116">Application</span></span> | <span data-ttu-id="72a68-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72a68-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="72a68-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72a68-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/users
```
## <a name="request-headers"></a><span data-ttu-id="72a68-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72a68-119">Request headers</span></span>
| <span data-ttu-id="72a68-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72a68-120">Header</span></span>       | <span data-ttu-id="72a68-121">Значение</span><span class="sxs-lookup"><span data-stu-id="72a68-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="72a68-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72a68-122">Authorization</span></span>  | <span data-ttu-id="72a68-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72a68-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="72a68-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="72a68-125">Content-Type</span></span>  | <span data-ttu-id="72a68-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72a68-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="72a68-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="72a68-127">Request body</span></span>
<span data-ttu-id="72a68-128">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72a68-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="72a68-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="72a68-129">Response</span></span>
<span data-ttu-id="72a68-130">При успешном выполнении этот метод возвратит код отклика `201 Created` и объект [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="72a68-130">If successful, this method returns a `201 Created` response code and an [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72a68-131">Пример</span><span class="sxs-lookup"><span data-stu-id="72a68-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72a68-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="72a68-132">Request</span></span>
<span data-ttu-id="72a68-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72a68-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/users
Content-type: application/json
Content-length: 508

{
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": null,
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  }
}
```

##### <a name="response"></a><span data-ttu-id="72a68-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="72a68-134">Response</span></span>
<span data-ttu-id="72a68-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="72a68-135">The following is an example of the response.</span></span> 

><span data-ttu-id="72a68-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72a68-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 508

{
  "id": "13012",
  "displayName": "Dion Matheson",
  "givenName": "Dion",
  "middleName": " ",
  "surname": "Matheson",
  "mail": "DionM@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "externalSource": "sis",
  "mailingAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "primaryRole": "student",
  "residenceAddress": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
