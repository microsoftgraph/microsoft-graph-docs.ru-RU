---
title: Перечисление преподавателей
description: Получение списка преподавателей для класса. Чтобы делегированные маркеры могли получить список преподавателей, они должны принадлежать к классу.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9e07ea3deb1cf8ec683a331ac3d76abb576be181
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550534"
---
# <a name="list-teachers"></a><span data-ttu-id="474a2-104">Перечисление преподавателей</span><span class="sxs-lookup"><span data-stu-id="474a2-104">List teachers</span></span>

<span data-ttu-id="474a2-105">Получение списка преподавателей для класса.</span><span class="sxs-lookup"><span data-stu-id="474a2-105">Retrieve a list teachers for a class.</span></span> <span data-ttu-id="474a2-106">Чтобы делегированные маркеры могли получить список преподавателей, они должны принадлежать к классу.</span><span class="sxs-lookup"><span data-stu-id="474a2-106">Delegated tokens must be members of the class to get the teacher list.</span></span>

## <a name="permissions"></a><span data-ttu-id="474a2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="474a2-107">Permissions</span></span>
<span data-ttu-id="474a2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="474a2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="474a2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="474a2-110">Permission type</span></span>      | <span data-ttu-id="474a2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="474a2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="474a2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="474a2-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="474a2-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="474a2-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="474a2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="474a2-114">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="474a2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="474a2-115">Not supported.</span></span>  |
|<span data-ttu-id="474a2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="474a2-116">Application</span></span> | <span data-ttu-id="474a2-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="474a2-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="474a2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="474a2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/teachers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="474a2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="474a2-119">Optional query parameters</span></span>
<span data-ttu-id="474a2-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="474a2-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="474a2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="474a2-121">Request headers</span></span>
| <span data-ttu-id="474a2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="474a2-122">Header</span></span>       | <span data-ttu-id="474a2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="474a2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="474a2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="474a2-124">Authorization</span></span>  | <span data-ttu-id="474a2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="474a2-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="474a2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="474a2-127">Request body</span></span>
<span data-ttu-id="474a2-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="474a2-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="474a2-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="474a2-129">Response</span></span>
<span data-ttu-id="474a2-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="474a2-130">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="474a2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="474a2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="474a2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="474a2-132">Request</span></span>
<span data-ttu-id="474a2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="474a2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_teachers"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers
```
##### <a name="response"></a><span data-ttu-id="474a2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="474a2-134">Response</span></span>
<span data-ttu-id="474a2-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="474a2-135">The following is an example of the response.</span></span> 

><span data-ttu-id="474a2-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="474a2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "14006",
      "displayName": "Kristie Mitchell",
      "givenName": "Kristie",
      "middleName": "Anne",
      "surname": "Mitchell",
      "mail": "kristiem@Contoso.com",
      "mobilePhone": "+1 (253) 555-0101",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalSource": "Edu",
      "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "primaryRole": "Teacher",
      "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List teachers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
