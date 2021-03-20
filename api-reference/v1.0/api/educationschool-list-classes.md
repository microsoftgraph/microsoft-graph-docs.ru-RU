---
title: Перечисление educationClasses
description: Получение списка курсов учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f4b67f9d97245b2f5749af33ce36a59a1cc85ec6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945412"
---
# <a name="list-educationclasses"></a><span data-ttu-id="723a7-103">Перечисление educationClasses</span><span class="sxs-lookup"><span data-stu-id="723a7-103">List educationClasses</span></span>

<span data-ttu-id="723a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="723a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="723a7-105">Получение списка курсов учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="723a7-105">Retrieve a list of classes owned by a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="723a7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="723a7-106">Permissions</span></span>
<span data-ttu-id="723a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="723a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="723a7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="723a7-109">Permission type</span></span>      | <span data-ttu-id="723a7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="723a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="723a7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="723a7-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="723a7-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="723a7-112">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="723a7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="723a7-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="723a7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="723a7-114">Not supported.</span></span>  |
|<span data-ttu-id="723a7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="723a7-115">Application</span></span> | <span data-ttu-id="723a7-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="723a7-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="723a7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="723a7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools/{id}/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="723a7-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="723a7-118">Optional query parameters</span></span>
<span data-ttu-id="723a7-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="723a7-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="723a7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="723a7-120">Request headers</span></span>
| <span data-ttu-id="723a7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="723a7-121">Header</span></span>       | <span data-ttu-id="723a7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="723a7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="723a7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="723a7-123">Authorization</span></span>  | <span data-ttu-id="723a7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="723a7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="723a7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="723a7-126">Request body</span></span>
<span data-ttu-id="723a7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="723a7-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="723a7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="723a7-128">Response</span></span>
<span data-ttu-id="723a7-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="723a7-129">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="723a7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="723a7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="723a7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="723a7-131">Request</span></span>
<span data-ttu-id="723a7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="723a7-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="723a7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="723a7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes
```
# <a name="c"></a>[<span data-ttu-id="723a7-134">C#</span><span class="sxs-lookup"><span data-stu-id="723a7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="723a7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="723a7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="723a7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="723a7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="723a7-137">Java</span><span class="sxs-lookup"><span data-stu-id="723a7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="723a7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="723a7-138">Response</span></span>
<span data-ttu-id="723a7-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="723a7-139">The following is an example of the response.</span></span> 

><span data-ttu-id="723a7-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="723a7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
