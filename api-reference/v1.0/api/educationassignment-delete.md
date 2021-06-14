---
title: Удаление educationAssignment
description: Удаление существующего назначения. Удалить назначения могут только преподаватели в классе.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ff82696996c9731209b448245515011e2f9baf2a
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911567"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="f598a-104">Удаление educationAssignment</span><span class="sxs-lookup"><span data-stu-id="f598a-104">Delete educationAssignment</span></span>

<span data-ttu-id="f598a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f598a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f598a-106">Удаление существующего назначения.</span><span class="sxs-lookup"><span data-stu-id="f598a-106">Delete an existing assignment.</span></span> 

<span data-ttu-id="f598a-107">Удалить назначения могут только преподаватели в классе.</span><span class="sxs-lookup"><span data-stu-id="f598a-107">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="f598a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f598a-108">Permissions</span></span>

<span data-ttu-id="f598a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f598a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f598a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f598a-111">Permission type</span></span>                        | <span data-ttu-id="f598a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f598a-112">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="f598a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f598a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f598a-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f598a-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="f598a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f598a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f598a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f598a-116">Not Supported.</span></span>                                          |
| <span data-ttu-id="f598a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f598a-117">Application</span></span>                            | <span data-ttu-id="f598a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f598a-118">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="f598a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f598a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
```

## <a name="request-headers"></a><span data-ttu-id="f598a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f598a-120">Request headers</span></span>

| <span data-ttu-id="f598a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f598a-121">Header</span></span>        | <span data-ttu-id="f598a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f598a-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="f598a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f598a-123">Authorization</span></span> | <span data-ttu-id="f598a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f598a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f598a-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f598a-126">Request body</span></span>

<span data-ttu-id="f598a-127">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f598a-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f598a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="f598a-128">Response</span></span>

<span data-ttu-id="f598a-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f598a-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f598a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f598a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f598a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f598a-132">Request</span></span>

<span data-ttu-id="f598a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f598a-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["1fdf61ee-c129-4960-9b7c-8df159aa64b0"],
  "name": "delete_educationassignment_1"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/c42f493f-42b4-4e7d-8148-af894cbc518b/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8
```

### <a name="response"></a><span data-ttu-id="f598a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f598a-134">Response</span></span>
<span data-ttu-id="f598a-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f598a-135">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


