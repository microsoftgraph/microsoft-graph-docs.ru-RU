---
title: Получение Едукатионрубрик
description: Получение свойств и связей объекта едукатионрубрик.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4a42c07859a01db350722eb4e7f35ce02d1e4f63
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36720406"
---
# <a name="get-educationrubric"></a><span data-ttu-id="76e71-103">Получение Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="76e71-103">Get educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76e71-104">Получение свойств и связей объекта [едукатионрубрик](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="76e71-104">Retrieve the properties and relationships of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="76e71-105">Обратите внимание, что возвращаемое значение Rubric (`GET /education/me/assignments/{id}/rubric`) является неизменяемой копией исходного Rubric, который существует в разделе `/education/users/{id}/rubrics`.</span><span class="sxs-lookup"><span data-stu-id="76e71-105">Note that when getting the rubric of an assignment (`GET /education/me/assignments/{id}/rubric`), what is returned is an immutable copy of the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="76e71-106">Копия связана с этим конкретным назначением.</span><span class="sxs-lookup"><span data-stu-id="76e71-106">The copy is associated with that specific assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="76e71-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76e71-107">Permissions</span></span>

<span data-ttu-id="76e71-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76e71-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76e71-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76e71-110">Permission type</span></span>                        | <span data-ttu-id="76e71-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76e71-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="76e71-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76e71-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="76e71-113">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76e71-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="76e71-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76e71-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76e71-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76e71-115">Not supported.</span></span> |
| <span data-ttu-id="76e71-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76e71-116">Application</span></span>                            | <span data-ttu-id="76e71-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76e71-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76e71-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76e71-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="76e71-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76e71-119">Request headers</span></span>

| <span data-ttu-id="76e71-120">Имя</span><span class="sxs-lookup"><span data-stu-id="76e71-120">Name</span></span>      |<span data-ttu-id="76e71-121">Описание</span><span class="sxs-lookup"><span data-stu-id="76e71-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76e71-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76e71-122">Authorization</span></span> | <span data-ttu-id="76e71-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="76e71-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="76e71-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="76e71-124">Request body</span></span>

<span data-ttu-id="76e71-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76e71-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76e71-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="76e71-126">Response</span></span>

<span data-ttu-id="76e71-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [едукатионрубрик](../resources/educationrubric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76e71-127">If successful, this method returns a `200 OK` response code and the requested [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76e71-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="76e71-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76e71-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="76e71-129">Request</span></span>

<span data-ttu-id="76e71-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76e71-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="76e71-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="76e71-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="76e71-132">C#</span><span class="sxs-lookup"><span data-stu-id="76e71-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="76e71-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76e71-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="76e71-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="76e71-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="76e71-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="76e71-135">Response</span></span>

<span data-ttu-id="76e71-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="76e71-136">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="76e71-137">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="76e71-137">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="76e71-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76e71-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
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
  "description": "Get educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
