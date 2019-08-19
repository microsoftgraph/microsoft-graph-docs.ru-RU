---
title: Обновление Едукатионрубрик
description: Обновление свойств объекта Едукатионрубрик.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d45d5c90366aa0bf5e165cc640890d4b4247d7b7
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461021"
---
# <a name="update-educationrubric"></a><span data-ttu-id="2ea8a-103">Обновление Едукатионрубрик</span><span class="sxs-lookup"><span data-stu-id="2ea8a-103">Update educationRubric</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ea8a-104">Обновление свойств объекта [едукатионрубрик](../resources/educationrubric.md) .</span><span class="sxs-lookup"><span data-stu-id="2ea8a-104">Update the properties of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="2ea8a-105">Обновление Rubric, присоединенного к назначению`PATCH /education/me/assignments/{id}/rubric`(), возможно только до публикации назначения, а то, что Обновлено, фактически является исходной Rubric, которая `/education/users/{id}/rubrics`существует в.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-105">Updating a rubric attached to an assignment (`PATCH /education/me/assignments/{id}/rubric`) is only possible before the assignment is published, and what is updated is actually the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="2ea8a-106">После публикации назначения выполняется неизменяемая копия Rubric, которая присоединяется к определенному назначению.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-106">After the assignment is published, an immutable copy of the rubric is made that is attached to that specific assignment.</span></span> <span data-ttu-id="2ea8a-107">Этот Rubric можно получить с помощью [Get/едукатион/ме/ассигнментс/{ИД}/рубрик](educationrubric-get.md), но его невозможно обновить.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-107">That rubric can be retrieved using [GET /education/me/assignments/{id}/rubric](educationrubric-get.md), but it cannot be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ea8a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ea8a-108">Permissions</span></span>

<span data-ttu-id="2ea8a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ea8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ea8a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ea8a-111">Permission type</span></span>                        | <span data-ttu-id="2ea8a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ea8a-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ea8a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ea8a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ea8a-114">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2ea8a-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="2ea8a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ea8a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ea8a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-116">Not supported.</span></span> |
| <span data-ttu-id="2ea8a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ea8a-117">Application</span></span>                            | <span data-ttu-id="2ea8a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ea8a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ea8a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/me/rubrics/{id}
PATCH /education/me/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="2ea8a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ea8a-120">Request headers</span></span>

| <span data-ttu-id="2ea8a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="2ea8a-121">Name</span></span>       | <span data-ttu-id="2ea8a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2ea8a-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2ea8a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ea8a-123">Authorization</span></span> | <span data-ttu-id="2ea8a-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="2ea8a-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ea8a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ea8a-125">Request body</span></span>

<span data-ttu-id="2ea8a-126">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2ea8a-127">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2ea8a-128">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2ea8a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ea8a-129">Property</span></span>     | <span data-ttu-id="2ea8a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2ea8a-130">Type</span></span>        | <span data-ttu-id="2ea8a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2ea8a-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ea8a-132">description</span><span class="sxs-lookup"><span data-stu-id="2ea8a-132">description</span></span>|<span data-ttu-id="2ea8a-133">итембоди</span><span class="sxs-lookup"><span data-stu-id="2ea8a-133">itemBody</span></span>|<span data-ttu-id="2ea8a-134">Описание этого Rubric.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-134">The description of this rubric.</span></span>|
|<span data-ttu-id="2ea8a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2ea8a-135">displayName</span></span>|<span data-ttu-id="2ea8a-136">String</span><span class="sxs-lookup"><span data-stu-id="2ea8a-136">String</span></span>|<span data-ttu-id="2ea8a-137">Имя этого Rubric.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-137">The name of this rubric.</span></span>|
|<span data-ttu-id="2ea8a-138">снижения</span><span class="sxs-lookup"><span data-stu-id="2ea8a-138">grading</span></span>|<span data-ttu-id="2ea8a-139">едукатионассигнментградетипе</span><span class="sxs-lookup"><span data-stu-id="2ea8a-139">educationAssignmentGradeType</span></span>|<span data-ttu-id="2ea8a-140">Указывает, есть ли у этого Rubric баллы.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-140">Whether this rubric has points or not.</span></span>|
|<span data-ttu-id="2ea8a-141">тонов</span><span class="sxs-lookup"><span data-stu-id="2ea8a-141">levels</span></span>|<span data-ttu-id="2ea8a-142">Коллекция Рубриклевел</span><span class="sxs-lookup"><span data-stu-id="2ea8a-142">rubricLevel collection</span></span>|<span data-ttu-id="2ea8a-143">Коллекция уровней, составляющих данный Rubric.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-143">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="2ea8a-144">являются</span><span class="sxs-lookup"><span data-stu-id="2ea8a-144">qualities</span></span>|<span data-ttu-id="2ea8a-145">Коллекция Рубриккуалити</span><span class="sxs-lookup"><span data-stu-id="2ea8a-145">rubricQuality collection</span></span>|<span data-ttu-id="2ea8a-146">Коллекция качеств, составляющих этот Rubric.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-146">The collection of qualities making up this rubric.</span></span>|

## <a name="response"></a><span data-ttu-id="2ea8a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ea8a-147">Response</span></span>

<span data-ttu-id="2ea8a-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [едукатионрубрик](../resources/educationrubric.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-148">If successful, this method returns a `200 OK` response code and an updated [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ea8a-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ea8a-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ea8a-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ea8a-150">Request</span></span>

<span data-ttu-id="2ea8a-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-151">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2ea8a-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ea8a-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationrubric"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/rubrics/{id}
Content-type: application/json

{
  "displayName": "Example Credit Rubric after display name patch"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ea8a-153">C#</span><span class="sxs-lookup"><span data-stu-id="2ea8a-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ea8a-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ea8a-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ea8a-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2ea8a-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ea8a-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ea8a-156">Response</span></span>

<span data-ttu-id="2ea8a-157">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-157">The following is an example of the response.</span></span>

> <span data-ttu-id="2ea8a-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2ea8a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "displayName": "Example Credit Rubric after display name patch",
    "id": "c4459fcb-a761-4f70-ac5b-e9466cb77c2a",
    "description": {
        "content": "This is an example of a credit rubric (no points)",
        "contentType": "text"
    },
    "levels": [
        {
            "levelId": "dec665d4-cf1b-4481-ac61-1d5b6188f4f5",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            }
        },
        {
            "levelId": "3f2e4b0f-508e-4005-984b-17e061bc5377",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            }
        }
    ],
    "qualities": [
        {
            "qualityId": "dc79dcbf-b536-4797-9c5b-902f28129fd0",
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "8937fa15-4a7c-4f27-bd01-ca3471d2d1d5",
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "4dfb5263-1d3f-4f0a-93ef-d24d800d0f69",
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "7e087062-ac25-4629-8386-a946350936db",
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "12276eb2-122c-4ad2-ba92-335ea798c88e",
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "3db7e6b2-2b1b-4f8e-9fca-bea701159145",
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationrubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
