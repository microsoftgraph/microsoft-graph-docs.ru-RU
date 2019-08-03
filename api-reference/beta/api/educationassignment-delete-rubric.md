---
title: Удаление Едукатионрубрик из educationAssignment
description: Удаление Едукатионрубрик из educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a6334e24c01db8f32f643f552b1a64cb2c86967d
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173225"
---
# <a name="remove-educationrubric-from-educationassignment"></a><span data-ttu-id="3bce1-103">Удаление Едукатионрубрик из educationAssignment</span><span class="sxs-lookup"><span data-stu-id="3bce1-103">Remove educationRubric from educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bce1-104">Удаление [едукатионрубрик](../resources/educationrubric.md) из [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3bce1-104">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>  <span data-ttu-id="3bce1-105">При этом сам Rubric не удаляется.</span><span class="sxs-lookup"><span data-stu-id="3bce1-105">This does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="3bce1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3bce1-106">Permissions</span></span>

<span data-ttu-id="3bce1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bce1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3bce1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bce1-109">Permission type</span></span>                        | <span data-ttu-id="3bce1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bce1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3bce1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bce1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3bce1-112">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3bce1-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="3bce1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bce1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bce1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bce1-114">Not supported.</span></span> |
| <span data-ttu-id="3bce1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bce1-115">Application</span></span>                            | <span data-ttu-id="3bce1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bce1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bce1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bce1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="3bce1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bce1-118">Request headers</span></span>

| <span data-ttu-id="3bce1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3bce1-119">Name</span></span>          | <span data-ttu-id="3bce1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3bce1-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3bce1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bce1-121">Authorization</span></span> | <span data-ttu-id="3bce1-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="3bce1-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3bce1-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3bce1-123">Request body</span></span>

<span data-ttu-id="3bce1-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3bce1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bce1-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="3bce1-125">Response</span></span>

<span data-ttu-id="3bce1-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3bce1-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3bce1-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="3bce1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3bce1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bce1-129">Request</span></span>

<span data-ttu-id="3bce1-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bce1-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric/$ref
```

### <a name="response"></a><span data-ttu-id="3bce1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bce1-131">Response</span></span>

<span data-ttu-id="3bce1-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3bce1-132">The following is an example of the response.</span></span>

> <span data-ttu-id="3bce1-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3bce1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
