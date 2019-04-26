---
title: Перечисление пользователей
description: Получение списка объектов user. Эти объекты user будут содержать специальные свойства, связанные с образованием.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e03c451f0bc470a166d6c90ef1217c4f0770c799
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322920"
---
# <a name="list-users"></a><span data-ttu-id="8024a-104">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="8024a-104">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8024a-105">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="8024a-105">Retrieve a list of user objects.</span></span> <span data-ttu-id="8024a-106">Эти объекты user будут содержать специальные свойства, связанные с образованием.</span><span class="sxs-lookup"><span data-stu-id="8024a-106">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="8024a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8024a-107">Permissions</span></span>
<span data-ttu-id="8024a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8024a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8024a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8024a-110">Permission type</span></span>      | <span data-ttu-id="8024a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8024a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8024a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8024a-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="8024a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8024a-113">Not supported.</span></span>  |
|<span data-ttu-id="8024a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8024a-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8024a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8024a-115">Not supported.</span></span>  |
|<span data-ttu-id="8024a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8024a-116">Application</span></span> | <span data-ttu-id="8024a-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8024a-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8024a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8024a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8024a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8024a-119">Optional query parameters</span></span>
<span data-ttu-id="8024a-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8024a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8024a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8024a-121">Request headers</span></span>
| <span data-ttu-id="8024a-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8024a-122">Header</span></span>       | <span data-ttu-id="8024a-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8024a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8024a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8024a-124">Authorization</span></span>  | <span data-ttu-id="8024a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8024a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8024a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8024a-127">Request body</span></span>
<span data-ttu-id="8024a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8024a-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8024a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="8024a-129">Response</span></span>
<span data-ttu-id="8024a-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8024a-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8024a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8024a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8024a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8024a-132">Request</span></span>
<span data-ttu-id="8024a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8024a-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/users
```
##### <a name="response"></a><span data-ttu-id="8024a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8024a-134">Response</span></span>
<span data-ttu-id="8024a-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8024a-135">The following is an example of the response.</span></span> 

><span data-ttu-id="8024a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8024a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 593

{
  "value": [
    {
      "id": "13012",
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
