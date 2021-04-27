---
title: 'educationClass: delta'
description: Получите новые или обновленные классы, в том числе изменения членства, без выполнения полного чтения всей коллекции классов.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e8b93c8ddd251bbc25efc9203417d6736e6bf62c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044087"
---
# <a name="educationclass-delta"></a><span data-ttu-id="6ef10-103">educationClass: delta</span><span class="sxs-lookup"><span data-stu-id="6ef10-103">educationClass: delta</span></span>

<span data-ttu-id="6ef10-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ef10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ef10-105">Получите новые или обновленные классы, в том числе изменения членства, без выполнения полного чтения всей коллекции классов.</span><span class="sxs-lookup"><span data-stu-id="6ef10-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="6ef10-106">Подробные [сведения см. в запросе Use Delta.](/graph/delta-query-overview)</span><span class="sxs-lookup"><span data-stu-id="6ef10-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ef10-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ef10-107">Permissions</span></span>

<span data-ttu-id="6ef10-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ef10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ef10-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ef10-110">Permission type</span></span>                        | <span data-ttu-id="6ef10-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ef10-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="6ef10-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ef10-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ef10-113">EduRoster.ReadBasic, EduRoster.Read или EduRoster.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6ef10-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="6ef10-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ef10-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ef10-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ef10-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="6ef10-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ef10-116">Application</span></span>                            | <span data-ttu-id="6ef10-117">EduRoster.ReadBasic.All, EduRoster.Read.All или EduRoster.WriteWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ef10-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ef10-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ef10-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/delta
```

## <a name="request-headers"></a><span data-ttu-id="6ef10-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ef10-119">Request headers</span></span>

| <span data-ttu-id="6ef10-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6ef10-120">Name</span></span>          | <span data-ttu-id="6ef10-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6ef10-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="6ef10-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ef10-122">Authorization</span></span> | <span data-ttu-id="6ef10-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6ef10-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ef10-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ef10-124">Request body</span></span>

<span data-ttu-id="6ef10-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ef10-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ef10-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ef10-126">Response</span></span>

<span data-ttu-id="6ef10-127">В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [коллекции educationClass](../resources/educationclass.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6ef10-127">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6ef10-128">дельты educationClass не включают удаленные классы.</span><span class="sxs-lookup"><span data-stu-id="6ef10-128">educationClass deltas do not include deleted classes.</span></span>

## <a name="example"></a><span data-ttu-id="6ef10-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6ef10-129">Example</span></span>

<span data-ttu-id="6ef10-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="6ef10-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6ef10-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ef10-131">Request</span></span>

<span data-ttu-id="6ef10-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ef10-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6ef10-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ef10-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/delta
```
# <a name="c"></a>[<span data-ttu-id="6ef10-134">C#</span><span class="sxs-lookup"><span data-stu-id="6ef10-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ef10-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ef10-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ef10-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ef10-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ef10-137">Java</span><span class="sxs-lookup"><span data-stu-id="6ef10-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationclass-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6ef10-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ef10-138">Response</span></span>

<span data-ttu-id="6ef10-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6ef10-139">The following is an example of the response.</span></span>

> <span data-ttu-id="6ef10-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6ef10-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 585

{
  "value": [
    {
      "classCode": "String",
      "course": { "@odata.type": "microsoft.graph.educationCourse" },
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "description": "String",
      "displayName": "String",
      "externalId": "String",
      "externalName": "String",
      "externalSource": "string",
      "grade": "string",
      "id": "String (identifier)",
      "mailNickname": "String",
      "term": { "@odata.type": "microsoft.graph.educationTerm" }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


