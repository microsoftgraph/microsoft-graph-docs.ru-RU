---
title: Перечисление EducationUsers
description: Получение списка пользователей в учебном заведении.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1889dfd19ab5ef461cccff5a2dc0103fce79cb29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550275"
---
# <a name="list-educationusers"></a><span data-ttu-id="b1e8e-103">Перечисление EducationUsers</span><span class="sxs-lookup"><span data-stu-id="b1e8e-103">List educationUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1e8e-104">Получение списка пользователей в учебном заведении.</span><span class="sxs-lookup"><span data-stu-id="b1e8e-104">Retrieve a list of users at a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1e8e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1e8e-105">Permissions</span></span>
<span data-ttu-id="b1e8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1e8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1e8e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1e8e-108">Permission type</span></span>      | <span data-ttu-id="b1e8e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1e8e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1e8e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1e8e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b1e8e-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1e8e-111">Not supported.</span></span>  |
|<span data-ttu-id="b1e8e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1e8e-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b1e8e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1e8e-113">Not supported.</span></span>  |
|<span data-ttu-id="b1e8e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1e8e-114">Application</span></span> | <span data-ttu-id="b1e8e-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1e8e-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b1e8e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1e8e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/users
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1e8e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1e8e-117">Optional query parameters</span></span>
<span data-ttu-id="b1e8e-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b1e8e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1e8e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1e8e-119">Request headers</span></span>
| <span data-ttu-id="b1e8e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1e8e-120">Header</span></span>       | <span data-ttu-id="b1e8e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b1e8e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1e8e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1e8e-122">Authorization</span></span>  | <span data-ttu-id="b1e8e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1e8e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1e8e-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1e8e-125">Request body</span></span>
<span data-ttu-id="b1e8e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1e8e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b1e8e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1e8e-127">Response</span></span>
<span data-ttu-id="b1e8e-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationUser](../resources/educationuser.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b1e8e-128">If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1e8e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b1e8e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1e8e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1e8e-130">Request</span></span>
<span data-ttu-id="b1e8e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1e8e-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/education/schools/10002/users
```
##### <a name="response"></a><span data-ttu-id="b1e8e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1e8e-132">Response</span></span>
<span data-ttu-id="b1e8e-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1e8e-133">The following is an example of the response.</span></span> 

><span data-ttu-id="b1e8e-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1e8e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
