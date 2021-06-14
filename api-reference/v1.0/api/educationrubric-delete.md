---
title: Удаление educationRubric
description: Удаление объекта educationRubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0b488c7c3307a7ac2388d36861eb4895fec44484
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912913"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="a9fa0-103">Удаление educationRubric</span><span class="sxs-lookup"><span data-stu-id="a9fa0-103">Delete educationRubric</span></span>

<span data-ttu-id="a9fa0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9fa0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9fa0-105">Удаление [объекта educationRubric.](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="a9fa0-105">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9fa0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9fa0-106">Permissions</span></span>

<span data-ttu-id="a9fa0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9fa0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9fa0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9fa0-109">Permission type</span></span>                        | <span data-ttu-id="a9fa0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9fa0-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a9fa0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9fa0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9fa0-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9fa0-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="a9fa0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9fa0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9fa0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9fa0-114">Not supported.</span></span> |
| <span data-ttu-id="a9fa0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9fa0-115">Application</span></span>                            | <span data-ttu-id="a9fa0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9fa0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9fa0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9fa0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
```

## <a name="request-headers"></a><span data-ttu-id="a9fa0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9fa0-118">Request headers</span></span>

| <span data-ttu-id="a9fa0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a9fa0-119">Name</span></span>          | <span data-ttu-id="a9fa0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a9fa0-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a9fa0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9fa0-121">Authorization</span></span> | <span data-ttu-id="a9fa0-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a9fa0-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9fa0-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a9fa0-123">Request body</span></span>

<span data-ttu-id="a9fa0-124">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9fa0-124">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9fa0-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9fa0-125">Response</span></span>

<span data-ttu-id="a9fa0-p102">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a9fa0-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9fa0-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a9fa0-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9fa0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9fa0-129">Request</span></span>

<span data-ttu-id="a9fa0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9fa0-130">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
```

### <a name="response"></a><span data-ttu-id="a9fa0-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9fa0-131">Response</span></span>

<span data-ttu-id="a9fa0-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a9fa0-132">The following is an example of the response.</span></span>

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


