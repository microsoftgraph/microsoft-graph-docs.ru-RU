---
title: Список пользователей
description: Получение списка объектов user. Эти объекты user будут содержать специальные свойства, связанные с образованием.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c484cab4851fdfccb7b9845f9447b07f669211bf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979539"
---
# <a name="list-users"></a><span data-ttu-id="fbeb9-104">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="fbeb9-104">List users</span></span>

> <span data-ttu-id="fbeb9-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbeb9-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fbeb9-107">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-107">Retrieve a list of user objects.</span></span> <span data-ttu-id="fbeb9-108">Эти объекты user будут содержать специальные свойства, связанные с образованием.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-108">These user objects will include education-specific properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbeb9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbeb9-109">Permissions</span></span>
<span data-ttu-id="fbeb9-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbeb9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbeb9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbeb9-112">Permission type</span></span>      | <span data-ttu-id="fbeb9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbeb9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbeb9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbeb9-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="fbeb9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-115">Not supported.</span></span>  |
|<span data-ttu-id="fbeb9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbeb9-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fbeb9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-117">Not supported.</span></span>  |
|<span data-ttu-id="fbeb9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbeb9-118">Application</span></span> | <span data-ttu-id="fbeb9-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbeb9-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fbeb9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbeb9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fbeb9-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fbeb9-121">Optional query parameters</span></span>
<span data-ttu-id="fbeb9-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fbeb9-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbeb9-123">Request headers</span></span>
| <span data-ttu-id="fbeb9-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbeb9-124">Header</span></span>       | <span data-ttu-id="fbeb9-125">Значение</span><span class="sxs-lookup"><span data-stu-id="fbeb9-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fbeb9-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbeb9-126">Authorization</span></span>  | <span data-ttu-id="fbeb9-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fbeb9-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fbeb9-129">Request body</span></span>
<span data-ttu-id="fbeb9-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="fbeb9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbeb9-131">Response</span></span>
<span data-ttu-id="fbeb9-132">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-132">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fbeb9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="fbeb9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbeb9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbeb9-134">Request</span></span>
<span data-ttu-id="fbeb9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/users
```
##### <a name="response"></a><span data-ttu-id="fbeb9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbeb9-136">Response</span></span>
<span data-ttu-id="fbeb9-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-137">The following is an example of the response.</span></span> 

><span data-ttu-id="fbeb9-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbeb9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
