---
title: Получение Едукатионрубрик, подключенных к educationAssignment
description: Получение Едукаитонрубрик, присоединенного к educationAssignment, если таковой существует.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ad4e72c2d638e1b07aa1ef363f8d0c406ef9b4bd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427657"
---
# <a name="get-educationrubric-attached-to-educationassignment"></a><span data-ttu-id="72c65-103">Получение Едукатионрубрик, подключенных к educationAssignment</span><span class="sxs-lookup"><span data-stu-id="72c65-103">Get educationRubric attached to educationAssignment</span></span>

<span data-ttu-id="72c65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72c65-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72c65-105">Получение объекта [едукатионрубрик](../resources/educationrubric.md) , присоединенного к [educationAssignment](../resources/educationassignment.md), если он существует.</span><span class="sxs-lookup"><span data-stu-id="72c65-105">Get the [educationRubric](../resources/educationrubric.md) object attached to an [educationAssignment](../resources/educationassignment.md), if one exists.</span></span>

## <a name="permissions"></a><span data-ttu-id="72c65-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72c65-106">Permissions</span></span>

<span data-ttu-id="72c65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72c65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72c65-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72c65-109">Permission type</span></span>                        | <span data-ttu-id="72c65-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72c65-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="72c65-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72c65-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="72c65-112">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72c65-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="72c65-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72c65-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72c65-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72c65-114">Not supported.</span></span> |
| <span data-ttu-id="72c65-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72c65-115">Application</span></span>                            | <span data-ttu-id="72c65-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72c65-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72c65-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72c65-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="72c65-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="72c65-118">Request headers</span></span>

| <span data-ttu-id="72c65-119">Имя</span><span class="sxs-lookup"><span data-stu-id="72c65-119">Name</span></span>      |<span data-ttu-id="72c65-120">Описание</span><span class="sxs-lookup"><span data-stu-id="72c65-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72c65-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="72c65-121">Authorization</span></span> | <span data-ttu-id="72c65-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="72c65-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="72c65-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="72c65-123">Request body</span></span>

<span data-ttu-id="72c65-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="72c65-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72c65-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="72c65-125">Response</span></span>

<span data-ttu-id="72c65-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [едукатионрубрик](../resources/educationrubric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72c65-126">If successful, this method returns a `200 OK` response code and an [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72c65-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="72c65-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="72c65-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="72c65-128">Request</span></span>

<span data-ttu-id="72c65-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72c65-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="72c65-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="72c65-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rubric"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric
```
# <a name="c"></a>[<span data-ttu-id="72c65-131">C#</span><span class="sxs-lookup"><span data-stu-id="72c65-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72c65-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72c65-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72c65-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72c65-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="72c65-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="72c65-134">Response</span></span>

<span data-ttu-id="72c65-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="72c65-135">The following is an example of the response.</span></span>

> <span data-ttu-id="72c65-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72c65-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "displayName": "Example Points Rubric",
    "id": "bf040af7-a5ff-4abe-a8c8-1bdc532344c2",
    "description": {
        "content": "This is an example of a rubric with points",
        "contentType": "text"
    },
    "levels": [
        {
            "levelId": "519cd134-c513-40b9-aa71-fdb0d063c084",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            },
            "grading": {
                "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints": 2
            }
        },
        {
            "levelId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            },
            "grading": {
                "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
                "maxPoints": 1
            }
        }
    ],
    "qualities": [
        {
            "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
            "weight": 50.0,
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "5e637d79-f26b-4ea6-acd7-73824f0c0967",
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "ebdcc27f-d1ec-4aa3-9da7-bd8d7842e3d3",
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
            "weight": 50.0,
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "5417252a-f810-41eb-9a83-09276a258a08",
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "5de220bd-74b9-41a7-85d5-9be7c6cb7933",
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
                }
            ]
        }
    ],
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List rubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
