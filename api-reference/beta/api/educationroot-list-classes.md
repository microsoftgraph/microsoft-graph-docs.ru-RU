---
title: Перечисление классов
description: 'Получение списка всех объектов class. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3152e2f3136bfc2fdf7679f8af4019bcb7dd537a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33588019"
---
# <a name="list-classes"></a><span data-ttu-id="3e7dc-103">Перечисление классов</span><span class="sxs-lookup"><span data-stu-id="3e7dc-103">List classes</span></span>

<span data-ttu-id="3e7dc-104">Получение списка всех объектов class.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-104">Retrieve a list of all class objects.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3e7dc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e7dc-105">Permissions</span></span>
<span data-ttu-id="3e7dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e7dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e7dc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e7dc-108">Permission type</span></span>      | <span data-ttu-id="3e7dc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e7dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e7dc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e7dc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3e7dc-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="3e7dc-111">EduRoster.ReadBasic</span></span> |
|<span data-ttu-id="3e7dc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e7dc-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3e7dc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-113">Not supported.</span></span>  |
|<span data-ttu-id="3e7dc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e7dc-114">Application</span></span> | <span data-ttu-id="3e7dc-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e7dc-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3e7dc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e7dc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3e7dc-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3e7dc-117">Optional query parameters</span></span>
<span data-ttu-id="3e7dc-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e7dc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e7dc-119">Request headers</span></span>
| <span data-ttu-id="3e7dc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e7dc-120">Header</span></span>       | <span data-ttu-id="3e7dc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3e7dc-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3e7dc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e7dc-122">Authorization</span></span>  | <span data-ttu-id="3e7dc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="3e7dc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e7dc-125">Request body</span></span>
<span data-ttu-id="3e7dc-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3e7dc-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e7dc-127">Response</span></span>
<span data-ttu-id="3e7dc-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-128">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3e7dc-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3e7dc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e7dc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e7dc-130">Request</span></span>
<span data-ttu-id="3e7dc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_classes"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes
```
##### <a name="response"></a><span data-ttu-id="3e7dc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e7dc-132">Response</span></span>
<span data-ttu-id="3e7dc-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-133">The following is an example of the response.</span></span> 

><span data-ttu-id="3e7dc-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e7dc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 277

{
  "value": [
    {
      "id": "11019",
      "description": "Health Level 1",
      "classCode": "Health 501",
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "displayName": "Health 1",
      "externalId": "11019",
      "externalName": "Health Level 1",
      "externalSource": "sis",
      "mailNickname": "fineartschool.net"
    }  
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3e7dc-136">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="3e7dc-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3e7dc-137">Языках</span><span class="sxs-lookup"><span data-stu-id="3e7dc-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_classes-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3e7dc-138">Язык</span><span class="sxs-lookup"><span data-stu-id="3e7dc-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_classes-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationroot-list-classes.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/educationroot-list-classes.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
