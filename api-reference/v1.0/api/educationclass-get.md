---
title: Получение educationClass
description: "  Администраторы групп представляют преподавателей в классе. Если вы используете делегированный маркер, пользователь увидит только курсы, участником которых является."
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: a4458287c9473e49c55ed2afae981cfaa61ebb69
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886453"
---
# <a name="get-educationclass"></a><span data-ttu-id="2215d-104">Получение educationClass</span><span class="sxs-lookup"><span data-stu-id="2215d-104">Get educationClass</span></span>

<span data-ttu-id="2215d-105">Получение курса из системы.</span><span class="sxs-lookup"><span data-stu-id="2215d-105">Retrieve a class from the system.</span></span> <span data-ttu-id="2215d-106">Курс — это универсальная группа со специальным свойством, которое указывает системе на то, что эта группа представляет собой курс.</span><span class="sxs-lookup"><span data-stu-id="2215d-106">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="2215d-107">Члены группы представляют учащихся, администраторы группы — преподавателей курса.</span><span class="sxs-lookup"><span data-stu-id="2215d-107">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="2215d-108">Если вы используете делегированный маркер, пользователь увидит только курсы, участником которых является.</span><span class="sxs-lookup"><span data-stu-id="2215d-108">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="2215d-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2215d-109">Permissions</span></span>
<span data-ttu-id="2215d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2215d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2215d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2215d-112">Permission type</span></span>      | <span data-ttu-id="2215d-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2215d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2215d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2215d-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="2215d-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="2215d-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="2215d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2215d-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2215d-117">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2215d-117">Not supported</span></span>  |
|<span data-ttu-id="2215d-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2215d-118">Application</span></span> | <span data-ttu-id="2215d-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2215d-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2215d-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2215d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2215d-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2215d-121">Optional query parameters</span></span>
<span data-ttu-id="2215d-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2215d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2215d-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2215d-123">Request headers</span></span>
| <span data-ttu-id="2215d-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2215d-124">Header</span></span>       | <span data-ttu-id="2215d-125">Значение</span><span class="sxs-lookup"><span data-stu-id="2215d-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2215d-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2215d-126">Authorization</span></span>  | <span data-ttu-id="2215d-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2215d-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2215d-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2215d-129">Request body</span></span>
<span data-ttu-id="2215d-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2215d-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2215d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="2215d-131">Response</span></span>
<span data-ttu-id="2215d-132">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2215d-132">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2215d-133">Пример</span><span class="sxs-lookup"><span data-stu-id="2215d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2215d-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="2215d-134">Request</span></span>
<span data-ttu-id="2215d-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2215d-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2215d-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="2215d-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2215d-137">C#</span><span class="sxs-lookup"><span data-stu-id="2215d-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2215d-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="2215d-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2215d-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2215d-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2215d-140">Java</span><span class="sxs-lookup"><span data-stu-id="2215d-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2215d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2215d-141">Response</span></span>
<span data-ttu-id="2215d-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2215d-142">The following is an example of the response.</span></span> 

><span data-ttu-id="2215d-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2215d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11023",
  "description": "English Level 2",
  "classCode": "11023",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "displayName": "English - Language 2",
  "externalId": "301",
  "externalName": "English Level 1",
  "externalSource": "School of Fine Art",
  "mailNickname": "fineartschool.net "
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
