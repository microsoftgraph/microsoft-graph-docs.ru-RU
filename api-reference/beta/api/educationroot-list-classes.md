---
title: Перечисление классов
description: 'Получение списка всех объектов class. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b5147fe93122eedd164bfe9490e22c6380faa01b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043677"
---
# <a name="list-classes"></a><span data-ttu-id="c2947-103">Перечисление курсов</span><span class="sxs-lookup"><span data-stu-id="c2947-103">List classes</span></span>

<span data-ttu-id="c2947-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2947-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2947-105">Получение списка всех объектов class.</span><span class="sxs-lookup"><span data-stu-id="c2947-105">Retrieve a list of all class objects.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c2947-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2947-106">Permissions</span></span>
<span data-ttu-id="c2947-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2947-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2947-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2947-109">Permission type</span></span>      | <span data-ttu-id="c2947-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2947-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2947-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2947-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c2947-112">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="c2947-112">EduRoster.ReadBasic</span></span> |
|<span data-ttu-id="c2947-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2947-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c2947-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2947-114">Not supported.</span></span>  |
|<span data-ttu-id="c2947-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2947-115">Application</span></span> | <span data-ttu-id="c2947-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2947-116">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c2947-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2947-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c2947-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c2947-118">Optional query parameters</span></span>
<span data-ttu-id="c2947-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c2947-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2947-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2947-120">Request headers</span></span>
| <span data-ttu-id="c2947-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2947-121">Header</span></span>       | <span data-ttu-id="c2947-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2947-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c2947-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2947-123">Authorization</span></span>  | <span data-ttu-id="c2947-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2947-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="c2947-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2947-126">Request body</span></span>
<span data-ttu-id="c2947-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2947-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c2947-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2947-128">Response</span></span>
<span data-ttu-id="c2947-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c2947-129">If successful, this method returns a `200 OK` response code and a collection of [educationClass](../resources/educationclass.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c2947-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c2947-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2947-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2947-131">Request</span></span>
<span data-ttu-id="c2947-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2947-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2947-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2947-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classes_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes
```
# <a name="c"></a>[<span data-ttu-id="c2947-134">C#</span><span class="sxs-lookup"><span data-stu-id="c2947-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classes-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2947-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2947-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classes-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2947-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2947-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classes-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2947-137">Java</span><span class="sxs-lookup"><span data-stu-id="c2947-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classes-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c2947-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2947-138">Response</span></span>
<span data-ttu-id="c2947-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c2947-139">The following is an example of the response.</span></span> 

><span data-ttu-id="c2947-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c2947-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List classes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
