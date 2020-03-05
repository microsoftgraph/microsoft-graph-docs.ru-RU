---
title: Получение Едукатионрубрик
description: Получение свойств и связей объекта едукатионрубрик.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e4825a0da4d03b42f85a5dd1582fa9bbe7521b97
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42425795"
---
# <a name="get-educationrubric"></a><span data-ttu-id="90843-103">Получение Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="90843-103">Get educationRubric</span></span>

<span data-ttu-id="90843-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="90843-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90843-105">Получение свойств и связей объекта [едукатионрубрик](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="90843-105">Retrieve the properties and relationships of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="90843-106">Обратите внимание, что возвращаемое значение Rubric (`GET /education/me/assignments/{id}/rubric`) является неизменяемой копией исходного Rubric, который существует в разделе `/education/users/{id}/rubrics`.</span><span class="sxs-lookup"><span data-stu-id="90843-106">Note that when getting the rubric of an assignment (`GET /education/me/assignments/{id}/rubric`), what is returned is an immutable copy of the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="90843-107">Копия связана с этим конкретным назначением.</span><span class="sxs-lookup"><span data-stu-id="90843-107">The copy is associated with that specific assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="90843-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90843-108">Permissions</span></span>

<span data-ttu-id="90843-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90843-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90843-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90843-111">Permission type</span></span>                        | <span data-ttu-id="90843-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90843-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90843-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90843-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="90843-114">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90843-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="90843-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90843-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90843-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90843-116">Not supported.</span></span> |
| <span data-ttu-id="90843-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90843-117">Application</span></span>                            | <span data-ttu-id="90843-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90843-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90843-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90843-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics/{id}
```

## <a name="request-headers"></a><span data-ttu-id="90843-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90843-120">Request headers</span></span>

| <span data-ttu-id="90843-121">Имя</span><span class="sxs-lookup"><span data-stu-id="90843-121">Name</span></span>      |<span data-ttu-id="90843-122">Описание</span><span class="sxs-lookup"><span data-stu-id="90843-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90843-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90843-123">Authorization</span></span> | <span data-ttu-id="90843-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="90843-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="90843-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90843-125">Request body</span></span>

<span data-ttu-id="90843-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90843-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90843-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="90843-127">Response</span></span>

<span data-ttu-id="90843-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [едукатионрубрик](../resources/educationrubric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90843-128">If successful, this method returns a `200 OK` response code and the requested [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90843-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="90843-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="90843-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="90843-130">Request</span></span>

<span data-ttu-id="90843-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90843-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90843-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="90843-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/rubrics/{id}
```
# <a name="c"></a>[<span data-ttu-id="90843-133">C#</span><span class="sxs-lookup"><span data-stu-id="90843-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90843-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90843-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90843-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90843-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="90843-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="90843-136">Response</span></span>

<span data-ttu-id="90843-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90843-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="90843-138">Объект Response, показанный здесь, может быть укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="90843-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="90843-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="90843-139">All the properties will be returned from an actual call.</span></span>

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
