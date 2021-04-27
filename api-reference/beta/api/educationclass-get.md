---
title: Получение educationClass
description: "  Администраторы групп представляют преподавателей в классе. Если вы используете делегированный маркер, пользователь увидит только курсы, участником которых является."
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f5d6dba45d267b85e8edf6d2831338c7aa79084c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044013"
---
# <a name="get-educationclass"></a><span data-ttu-id="54025-104">Получение educationClass</span><span class="sxs-lookup"><span data-stu-id="54025-104">Get educationClass</span></span>

<span data-ttu-id="54025-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54025-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54025-106">Получение курса из системы.</span><span class="sxs-lookup"><span data-stu-id="54025-106">Retrieve a class from the system.</span></span> <span data-ttu-id="54025-107">Курс — это универсальная группа со специальным свойством, которое указывает системе на то, что эта группа представляет собой курс.</span><span class="sxs-lookup"><span data-stu-id="54025-107">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="54025-108">Члены группы представляют учащихся, администраторы группы — преподавателей курса.</span><span class="sxs-lookup"><span data-stu-id="54025-108">Group members represent the students;  group admins represent the teachers in the class.</span></span> <span data-ttu-id="54025-109">Если вы используете делегированный маркер, пользователь увидит только курсы, участником которых является.</span><span class="sxs-lookup"><span data-stu-id="54025-109">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="54025-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54025-110">Permissions</span></span>
<span data-ttu-id="54025-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54025-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54025-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54025-113">Permission type</span></span>      | <span data-ttu-id="54025-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54025-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54025-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54025-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="54025-116">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="54025-116">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="54025-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54025-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="54025-118">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="54025-118">Not supported</span></span>  |
|<span data-ttu-id="54025-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54025-119">Application</span></span> | <span data-ttu-id="54025-120">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54025-120">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="54025-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54025-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="54025-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="54025-122">Optional query parameters</span></span>
<span data-ttu-id="54025-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="54025-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54025-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54025-124">Request headers</span></span>
| <span data-ttu-id="54025-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54025-125">Header</span></span>       | <span data-ttu-id="54025-126">Значение</span><span class="sxs-lookup"><span data-stu-id="54025-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="54025-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54025-127">Authorization</span></span>  | <span data-ttu-id="54025-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54025-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="54025-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54025-130">Request body</span></span>
<span data-ttu-id="54025-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54025-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="54025-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="54025-132">Response</span></span>
<span data-ttu-id="54025-133">При успешном выполнении этот метод возвратит код отклика `200 OK` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="54025-133">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54025-134">Пример</span><span class="sxs-lookup"><span data-stu-id="54025-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54025-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="54025-135">Request</span></span>
<span data-ttu-id="54025-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54025-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54025-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="54025-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11023
```
# <a name="c"></a>[<span data-ttu-id="54025-138">C#</span><span class="sxs-lookup"><span data-stu-id="54025-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54025-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54025-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54025-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54025-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54025-141">Java</span><span class="sxs-lookup"><span data-stu-id="54025-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="54025-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="54025-142">Response</span></span>
<span data-ttu-id="54025-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="54025-143">The following is an example of the response.</span></span> 

><span data-ttu-id="54025-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="54025-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
