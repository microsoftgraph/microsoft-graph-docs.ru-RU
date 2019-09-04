---
title: Получение Едукатионрубрик, подключенных к educationAssignment
description: Получение Едукаитонрубрик, присоединенного к educationAssignment, если таковой существует.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7fd0524affaec2da6a9e21ef679dce539113d8b2
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718004"
---
# <a name="get-educationrubric-attached-to-educationassignment"></a><span data-ttu-id="0772c-103">Получение Едукатионрубрик, подключенных к educationAssignment</span><span class="sxs-lookup"><span data-stu-id="0772c-103">Get educationRubric attached to educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0772c-104">Получение объекта [едукатионрубрик](../resources/educationrubric.md) , присоединенного к [educationAssignment](../resources/educationassignment.md), если он существует.</span><span class="sxs-lookup"><span data-stu-id="0772c-104">Get the [educationRubric](../resources/educationrubric.md) object attached to an [educationAssignment](../resources/educationassignment.md), if one exists.</span></span>

## <a name="permissions"></a><span data-ttu-id="0772c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0772c-105">Permissions</span></span>

<span data-ttu-id="0772c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0772c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0772c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0772c-108">Permission type</span></span>                        | <span data-ttu-id="0772c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0772c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0772c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0772c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0772c-111">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0772c-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="0772c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0772c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0772c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0772c-113">Not supported.</span></span> |
| <span data-ttu-id="0772c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0772c-114">Application</span></span>                            | <span data-ttu-id="0772c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0772c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0772c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0772c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="0772c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0772c-117">Request headers</span></span>

| <span data-ttu-id="0772c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0772c-118">Name</span></span>      |<span data-ttu-id="0772c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0772c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0772c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0772c-120">Authorization</span></span> | <span data-ttu-id="0772c-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="0772c-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="0772c-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0772c-122">Request body</span></span>

<span data-ttu-id="0772c-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0772c-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0772c-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="0772c-124">Response</span></span>

<span data-ttu-id="0772c-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [едукатионрубрик](../resources/educationrubric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0772c-125">If successful, this method returns a `200 OK` response code and an [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0772c-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="0772c-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0772c-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="0772c-127">Request</span></span>

<span data-ttu-id="0772c-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0772c-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0772c-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="0772c-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rubric"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0772c-130">C#</span><span class="sxs-lookup"><span data-stu-id="0772c-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0772c-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0772c-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0772c-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0772c-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0772c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0772c-133">Response</span></span>

<span data-ttu-id="0772c-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0772c-134">The following is an example of the response.</span></span>

> <span data-ttu-id="0772c-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0772c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
