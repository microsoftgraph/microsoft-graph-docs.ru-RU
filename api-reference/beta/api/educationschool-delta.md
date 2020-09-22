---
title: 'educationSchool: Delta'
description: Получите новые или обновленные учебные заведения, не требующие полного прочтения всей коллекции учебных заведений.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f8dc7f61d7455e5579d41d8a4e6fbf7d14ec60e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007418"
---
# <a name="educationschool-delta"></a><span data-ttu-id="fe732-103">educationSchool: Delta</span><span class="sxs-lookup"><span data-stu-id="fe732-103">educationSchool: delta</span></span>

<span data-ttu-id="fe732-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe732-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe732-105">Получите новые или обновленные учебные заведения, не требующие полного прочтения всей коллекции учебных заведений.</span><span class="sxs-lookup"><span data-stu-id="fe732-105">Get newly created or updated schools without having to perform a full read of the entire school collection.</span></span> <span data-ttu-id="fe732-106">Дополнительные сведения: [use Query Delta Query](/graph/delta-query-overview) .</span><span class="sxs-lookup"><span data-stu-id="fe732-106">See [Use delta query](/graph/delta-query-overview) for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe732-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe732-107">Permissions</span></span>

<span data-ttu-id="fe732-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe732-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe732-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe732-110">Permission type</span></span>                        | <span data-ttu-id="fe732-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe732-111">Permissions (from least to most privileged)</span></span>                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="fe732-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe732-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe732-113">EduRoster. ReadBasic, EduRoster. Read или EduRoster. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe732-113">EduRoster.ReadBasic, EduRoster.Read, or EduRoster.ReadWrite</span></span>              |
| <span data-ttu-id="fe732-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe732-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe732-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe732-115">Not supported.</span></span>                                                           |
| <span data-ttu-id="fe732-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe732-116">Application</span></span>                            | <span data-ttu-id="fe732-117">EduRoster. ReadBasic. ALL, EduRoster. Read. ALL или EduRoster. Вритеврите. ALL</span><span class="sxs-lookup"><span data-stu-id="fe732-117">EduRoster.ReadBasic.All, EduRoster.Read.All, or EduRoster.WriteWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe732-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe732-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/schools/delta
```

## <a name="request-headers"></a><span data-ttu-id="fe732-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe732-119">Request headers</span></span>

| <span data-ttu-id="fe732-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fe732-120">Name</span></span>          | <span data-ttu-id="fe732-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fe732-121">Description</span></span>   |
| :------------ | :------------ |
| <span data-ttu-id="fe732-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe732-122">Authorization</span></span> | <span data-ttu-id="fe732-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fe732-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe732-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe732-124">Request body</span></span>

<span data-ttu-id="fe732-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe732-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe732-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe732-126">Response</span></span>

<span data-ttu-id="fe732-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект коллекции [educationSchool](../resources/educationschool.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fe732-127">If successful, this method returns a `200 OK` response code and an [educationSchool](../resources/educationschool.md) collection object in the response body.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="fe732-128">разности educationSchool не включают удаленные школы.</span><span class="sxs-lookup"><span data-stu-id="fe732-128">educationSchool deltas do not include deleted schools.</span></span>

## <a name="example"></a><span data-ttu-id="fe732-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fe732-129">Example</span></span>

<span data-ttu-id="fe732-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="fe732-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="fe732-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe732-131">Request</span></span>

<span data-ttu-id="fe732-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe732-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fe732-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe732-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/delta
```
# <a name="c"></a>[<span data-ttu-id="fe732-134">C#</span><span class="sxs-lookup"><span data-stu-id="fe732-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe732-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe732-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe732-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe732-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fe732-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe732-137">Response</span></span>

<span data-ttu-id="fe732-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fe732-138">The following is an example of the response.</span></span>

> <span data-ttu-id="fe732-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe732-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 313

{
  "value": [
    {
      "address": { "@odata.type": "microsoft.graph.physicalAddress" },
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "description": "String",
      "displayName": "String",
      "externalId": "String",
      "externalPrincipalId": "String",
      "externalSource": "string",
      "highestGrade": "String",
      "id": "String (identifier)",
      "lowestGrade": "String",
      "phone": "String",
      "principalEmail": "String",
      "principalName": "String",
      "schoolNumber": "String"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


