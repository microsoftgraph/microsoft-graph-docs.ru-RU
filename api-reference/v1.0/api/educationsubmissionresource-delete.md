---
title: Удаление educationSubmissionResource
description: Удаляет ресурс из отправки. Это может быть сделано только студентом. Если ресурс был скопирован из назначения, после удаления текущей копии будет создана новая копия ресурса.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 45b165ab8f2a9c07d657ea56b3118f5e14ba5e4b
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912657"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="7eb35-105">Удаление educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="7eb35-105">Delete educationSubmissionResource</span></span>

<span data-ttu-id="7eb35-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eb35-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7eb35-107">Удаляет ресурс из отправки.</span><span class="sxs-lookup"><span data-stu-id="7eb35-107">Deletes a resource from the submission.</span></span> <span data-ttu-id="7eb35-108">Это может быть сделано только студентом.</span><span class="sxs-lookup"><span data-stu-id="7eb35-108">This can only be done by the student.</span></span> <span data-ttu-id="7eb35-109">Если ресурс был скопирован из назначения, после удаления текущей копии будет создана новая копия ресурса.</span><span class="sxs-lookup"><span data-stu-id="7eb35-109">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="7eb35-110">Это позволяет "сбросить" ресурс в исходное состояние.</span><span class="sxs-lookup"><span data-stu-id="7eb35-110">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="7eb35-111">Если ресурс не был скопирован из назначения, а добавлен из студента, ресурс просто удаляется.</span><span class="sxs-lookup"><span data-stu-id="7eb35-111">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="7eb35-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7eb35-112">Permissions</span></span>
<span data-ttu-id="7eb35-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7eb35-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7eb35-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7eb35-115">Permission type</span></span>      | <span data-ttu-id="7eb35-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7eb35-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7eb35-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7eb35-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="7eb35-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7eb35-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="7eb35-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7eb35-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7eb35-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eb35-120">Not supported.</span></span>  |
|<span data-ttu-id="7eb35-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7eb35-121">Application</span></span> | <span data-ttu-id="7eb35-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eb35-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7eb35-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7eb35-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c
```

## <a name="request-headers"></a><span data-ttu-id="7eb35-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7eb35-124">Request headers</span></span>
| <span data-ttu-id="7eb35-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7eb35-125">Header</span></span>       | <span data-ttu-id="7eb35-126">Значение</span><span class="sxs-lookup"><span data-stu-id="7eb35-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7eb35-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7eb35-127">Authorization</span></span>  | <span data-ttu-id="7eb35-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7eb35-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7eb35-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7eb35-130">Request body</span></span>
<span data-ttu-id="7eb35-131">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7eb35-131">Don't supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7eb35-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7eb35-132">Response</span></span>
<span data-ttu-id="7eb35-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7eb35-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7eb35-135">Пример</span><span class="sxs-lookup"><span data-stu-id="7eb35-135">Example</span></span>
### <a name="request"></a><span data-ttu-id="7eb35-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="7eb35-136">Request</span></span>
<span data-ttu-id="7eb35-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7eb35-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```

### <a name="response"></a><span data-ttu-id="7eb35-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="7eb35-138">Response</span></span>
<span data-ttu-id="7eb35-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7eb35-139">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


