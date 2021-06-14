---
title: Удаление educationCategory
description: Удаление существующей категории.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eed94985bfa1de66215f7afd1ca64d236846a118
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911546"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="6728a-103">Удаление educationCategory</span><span class="sxs-lookup"><span data-stu-id="6728a-103">Delete educationCategory</span></span>

<span data-ttu-id="6728a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6728a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6728a-105">Удаление существующей [категории](../resources/educationcategory.md).</span><span class="sxs-lookup"><span data-stu-id="6728a-105">Delete an existing [category](../resources/educationcategory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6728a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6728a-106">Permissions</span></span>

<span data-ttu-id="6728a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6728a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6728a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6728a-109">Permission type</span></span>                        | <span data-ttu-id="6728a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6728a-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="6728a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6728a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6728a-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6728a-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="6728a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6728a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6728a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6728a-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="6728a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6728a-115">Application</span></span>                            | <span data-ttu-id="6728a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6728a-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="6728a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6728a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6728a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6728a-118">Request headers</span></span>

| <span data-ttu-id="6728a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6728a-119">Header</span></span>        | <span data-ttu-id="6728a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6728a-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="6728a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6728a-121">Authorization</span></span> | <span data-ttu-id="6728a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6728a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6728a-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6728a-124">Request body</span></span>

<span data-ttu-id="6728a-125">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6728a-125">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6728a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="6728a-126">Response</span></span>

<span data-ttu-id="6728a-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6728a-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6728a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6728a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6728a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6728a-130">Request</span></span>

<span data-ttu-id="6728a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6728a-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment_2"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/c42f493f-42b4-4e7d-8148-af894cbc518b/assignmentCategories/b93d3b6b-360c-45c0-8764-e8bb622a9504
```

### <a name="response"></a><span data-ttu-id="6728a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6728a-132">Response</span></span>

<span data-ttu-id="6728a-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6728a-133">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


