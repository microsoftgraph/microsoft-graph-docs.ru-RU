---
title: Перечисление учебных заведений
description: Получение списка учебных заведений для этого пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 594a38d82de173d3a6a93607fdac61cca60e7cac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508568"
---
# <a name="list-schools"></a><span data-ttu-id="18d29-103">Перечисление учебных заведений</span><span class="sxs-lookup"><span data-stu-id="18d29-103">List schools</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18d29-104">Получение списка учебных заведений для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="18d29-104">Retrieve a list of schools for a user.</span></span>

><span data-ttu-id="18d29-105">**Примечание.** Если используется делегированный маркер, участники могут видеть сведения только о своих учебных заведениях.</span><span class="sxs-lookup"><span data-stu-id="18d29-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="18d29-106">В данном случае используйте ресурс `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="18d29-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="18d29-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18d29-107">Permissions</span></span>
<span data-ttu-id="18d29-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18d29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18d29-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18d29-110">Permission type</span></span>      | <span data-ttu-id="18d29-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18d29-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18d29-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18d29-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="18d29-113">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="18d29-113">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="18d29-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18d29-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="18d29-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18d29-115">Not supported.</span></span>  |
|<span data-ttu-id="18d29-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18d29-116">Application</span></span> | <span data-ttu-id="18d29-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18d29-117">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="18d29-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18d29-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="18d29-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="18d29-119">Optional query parameters</span></span>
<span data-ttu-id="18d29-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="18d29-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18d29-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18d29-121">Request headers</span></span>
| <span data-ttu-id="18d29-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18d29-122">Header</span></span>       | <span data-ttu-id="18d29-123">Значение</span><span class="sxs-lookup"><span data-stu-id="18d29-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18d29-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18d29-124">Authorization</span></span>  | <span data-ttu-id="18d29-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18d29-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18d29-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18d29-127">Request body</span></span>
<span data-ttu-id="18d29-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="18d29-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="18d29-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="18d29-129">Response</span></span>
<span data-ttu-id="18d29-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationSchool](../resources/educationschool.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="18d29-130">If successful, this method returns a `200 OK` response code and a collection of [educationSchool](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18d29-131">Пример</span><span class="sxs-lookup"><span data-stu-id="18d29-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18d29-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="18d29-132">Request</span></span>
<span data-ttu-id="18d29-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18d29-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/beta/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="18d29-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="18d29-134">Response</span></span>
<span data-ttu-id="18d29-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="18d29-135">The following is an example of the response.</span></span> 

><span data-ttu-id="18d29-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18d29-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10001",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationuser-list-schools.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
