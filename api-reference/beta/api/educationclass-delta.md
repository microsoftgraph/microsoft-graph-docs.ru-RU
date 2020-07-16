---
title: 'educationClass: Delta'
description: Получите новые или обновленные классы, в том числе изменения членства, без необходимости выполнять полное чтение всей коллекции классов.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 34766ce4e6fe210369869f71213fb596432cbaab
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081242"
---
# <a name="educationclass-delta"></a><span data-ttu-id="f2361-103">educationClass: Delta</span><span class="sxs-lookup"><span data-stu-id="f2361-103">educationClass: delta</span></span>

<span data-ttu-id="f2361-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2361-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2361-105">Получите новые или обновленные классы, в том числе изменения членства, без необходимости выполнять полное чтение всей коллекции классов.</span><span class="sxs-lookup"><span data-stu-id="f2361-105">Get newly created or updated classes, including membership changes, without having to perform a full read of the entire class collection.</span></span> <span data-ttu-id="f2361-106">Дополнительные сведения: [use Query Delta Query](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="f2361-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2361-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2361-107">Permissions</span></span>

<span data-ttu-id="f2361-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2361-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f2361-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2361-110">Permission type</span></span>                        | <span data-ttu-id="f2361-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2361-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="f2361-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2361-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f2361-113">EduRoster. ReadBasic, EduRoster. Read или EduRoster. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f2361-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="f2361-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2361-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2361-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2361-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="f2361-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f2361-116">Application</span></span>                            | <span data-ttu-id="f2361-117">EduRoster. ReadBasic. ALL, EduRoster. Read. ALL или EduRoster. Вритеврите. ALL</span><span class="sxs-lookup"><span data-stu-id="f2361-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2361-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2361-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/delta
```

## <a name="request-headers"></a><span data-ttu-id="f2361-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2361-119">Request headers</span></span>

| <span data-ttu-id="f2361-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f2361-120">Name</span></span>          | <span data-ttu-id="f2361-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f2361-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="f2361-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2361-122">Authorization</span></span> | <span data-ttu-id="f2361-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f2361-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2361-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2361-124">Request body</span></span>

<span data-ttu-id="f2361-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2361-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2361-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2361-126">Response</span></span>

<span data-ttu-id="f2361-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [educationClass](../resources/educationclass.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f2361-127">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f2361-128">разность educationClass не включает удаленные классы.</span><span class="sxs-lookup"><span data-stu-id="f2361-128">educationClass deltas do not include deleted classes.</span></span>

## <a name="example"></a><span data-ttu-id="f2361-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f2361-129">Example</span></span>

<span data-ttu-id="f2361-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="f2361-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f2361-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2361-131">Request</span></span>

<span data-ttu-id="f2361-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2361-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2361-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2361-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/delta
```
# <a name="c"></a>[<span data-ttu-id="f2361-134">C#</span><span class="sxs-lookup"><span data-stu-id="f2361-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationclass-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2361-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2361-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationclass-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2361-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2361-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationclass-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2361-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2361-137">Response</span></span>

<span data-ttu-id="f2361-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f2361-138">The following is an example of the response.</span></span>

> <span data-ttu-id="f2361-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2361-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
