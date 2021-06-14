---
title: Get educationRubric
description: Извлечение свойств и связей образовательного объекта.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5a38617b1256d9ab187c4a35efb27b6470490213
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912733"
---
# <a name="get-educationrubric"></a><span data-ttu-id="95a6c-103">Get educationRubric</span><span class="sxs-lookup"><span data-stu-id="95a6c-103">Get educationRubric</span></span>

<span data-ttu-id="95a6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95a6c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95a6c-105">Извлечение свойств и связей [объекта educationRubric.](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="95a6c-105">Retrieve the properties and relationships of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="95a6c-106">Обратите внимание, что при получении [рубрики](educationassignment-get-rubric.md)назначения возвращается неосязуемая копия исходной рубрики, которая существует под `/education/users/{id}/rubrics` .</span><span class="sxs-lookup"><span data-stu-id="95a6c-106">Note that when getting the [rubric of an assignment](educationassignment-get-rubric.md), what is returned is an immutable copy of the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="95a6c-107">Копия связана с этим конкретным назначением.</span><span class="sxs-lookup"><span data-stu-id="95a6c-107">The copy is associated with that specific assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="95a6c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95a6c-108">Permissions</span></span>

<span data-ttu-id="95a6c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95a6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="95a6c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95a6c-111">Permission type</span></span>                        | <span data-ttu-id="95a6c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95a6c-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="95a6c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95a6c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="95a6c-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95a6c-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="95a6c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95a6c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95a6c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95a6c-116">Not supported.</span></span> |
| <span data-ttu-id="95a6c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="95a6c-117">Application</span></span>                            | <span data-ttu-id="95a6c-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="95a6c-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="95a6c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95a6c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
```

## <a name="request-headers"></a><span data-ttu-id="95a6c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95a6c-120">Request headers</span></span>

| <span data-ttu-id="95a6c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="95a6c-121">Name</span></span>      |<span data-ttu-id="95a6c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="95a6c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="95a6c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95a6c-123">Authorization</span></span> | <span data-ttu-id="95a6c-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="95a6c-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="95a6c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="95a6c-125">Request body</span></span>

<span data-ttu-id="95a6c-126">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="95a6c-126">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95a6c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="95a6c-127">Response</span></span>

<span data-ttu-id="95a6c-128">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [educationRubric](../resources/educationrubric.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="95a6c-128">If successful, this method returns a `200 OK` response code and the requested [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="95a6c-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="95a6c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="95a6c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="95a6c-130">Request</span></span>

<span data-ttu-id="95a6c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95a6c-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
```

### <a name="response"></a><span data-ttu-id="95a6c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="95a6c-132">Response</span></span>

<span data-ttu-id="95a6c-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="95a6c-133">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="95a6c-134">Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="95a6c-134">The response object shown here might be shortened for readability.</span></span>

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


