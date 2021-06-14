---
title: Удаление educationRubric из educationAssignment
description: Удаление educationRubric из educationAssignment
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9ce6eb7090c75fab942fc9cd5e317b5526a6dd7b
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912924"
---
# <a name="delete-educationrubric-from-educationassignment"></a><span data-ttu-id="fe29e-103">Удаление educationRubric из educationAssignment</span><span class="sxs-lookup"><span data-stu-id="fe29e-103">Delete educationRubric from educationAssignment</span></span>

<span data-ttu-id="fe29e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe29e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe29e-105">Удаление [educationRubric](../resources/educationrubric.md) из [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fe29e-105">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>
<span data-ttu-id="fe29e-106">Этот метод не удаляет сам рубрику.</span><span class="sxs-lookup"><span data-stu-id="fe29e-106">This method does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe29e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe29e-107">Permissions</span></span>

<span data-ttu-id="fe29e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe29e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe29e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe29e-110">Permission type</span></span>                        | <span data-ttu-id="fe29e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe29e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fe29e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe29e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe29e-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe29e-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="fe29e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe29e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe29e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe29e-115">Not supported.</span></span> |
| <span data-ttu-id="fe29e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe29e-116">Application</span></span>                            | <span data-ttu-id="fe29e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe29e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe29e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe29e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="fe29e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe29e-119">Request headers</span></span>

| <span data-ttu-id="fe29e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fe29e-120">Name</span></span>          | <span data-ttu-id="fe29e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fe29e-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fe29e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe29e-122">Authorization</span></span> | <span data-ttu-id="fe29e-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="fe29e-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe29e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe29e-124">Request body</span></span>

<span data-ttu-id="fe29e-125">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe29e-125">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe29e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe29e-126">Response</span></span>

<span data-ttu-id="fe29e-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fe29e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fe29e-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="fe29e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fe29e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe29e-130">Request</span></span>

<span data-ttu-id="fe29e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe29e-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric/$ref
```

### <a name="response"></a><span data-ttu-id="fe29e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe29e-132">Response</span></span>

<span data-ttu-id="fe29e-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fe29e-133">The following is an example of the response.</span></span>

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


