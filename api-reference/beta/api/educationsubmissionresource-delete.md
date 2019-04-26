---
title: Удаление Едукатионсубмиссионресаурце
description: Удаляет ресурс из отправки. Это может сделать только студентом. Если ресурс был скопирован из назначения, то после удаления текущей копии будет создан новый экземпляр ресурса.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 077434e269300617cf239ef82084439c8109adc5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322344"
---
# <a name="delete-educationsubmissionresource"></a><span data-ttu-id="47ebb-105">Удаление Едукатионсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="47ebb-105">Delete educationSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47ebb-106">Удаляет ресурс из отправки.</span><span class="sxs-lookup"><span data-stu-id="47ebb-106">Deletes a resource from the submission.</span></span> <span data-ttu-id="47ebb-107">Это может сделать только студентом.</span><span class="sxs-lookup"><span data-stu-id="47ebb-107">This can only be done by the student.</span></span> <span data-ttu-id="47ebb-108">Если ресурс был скопирован из назначения, то после удаления текущей копии будет создан новый экземпляр ресурса.</span><span class="sxs-lookup"><span data-stu-id="47ebb-108">If the resource was copied from the assignment, a new copy of the resource will be created after the current copy is deleted.</span></span> <span data-ttu-id="47ebb-109">Это позволяет «сбросить» ресурс в исходное состояние.</span><span class="sxs-lookup"><span data-stu-id="47ebb-109">This allows you to "reset" the resource to its original state.</span></span> <span data-ttu-id="47ebb-110">Если ресурс не был скопирован из назначения, но добавлен из учащегося, ресурс просто удаляется.</span><span class="sxs-lookup"><span data-stu-id="47ebb-110">If the resource was not copied from the assignment but was added from the student, the resource is simply deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="47ebb-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47ebb-111">Permissions</span></span>
<span data-ttu-id="47ebb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47ebb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47ebb-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47ebb-114">Permission type</span></span>      | <span data-ttu-id="47ebb-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47ebb-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47ebb-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47ebb-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="47ebb-117">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47ebb-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="47ebb-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47ebb-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="47ebb-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47ebb-119">Not supported.</span></span>  |
|<span data-ttu-id="47ebb-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47ebb-120">Application</span></span> | <span data-ttu-id="47ebb-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47ebb-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="47ebb-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47ebb-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /educationClasses/assignments/{id}/submissions/{id}/resources/{id}

```
## <a name="request-headers"></a><span data-ttu-id="47ebb-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47ebb-123">Request headers</span></span>
| <span data-ttu-id="47ebb-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47ebb-124">Header</span></span>       | <span data-ttu-id="47ebb-125">Значение</span><span class="sxs-lookup"><span data-stu-id="47ebb-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47ebb-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47ebb-126">Authorization</span></span>  | <span data-ttu-id="47ebb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47ebb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47ebb-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47ebb-129">Request body</span></span>
<span data-ttu-id="47ebb-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47ebb-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="47ebb-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="47ebb-131">Response</span></span>
<span data-ttu-id="47ebb-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="47ebb-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47ebb-134">Пример</span><span class="sxs-lookup"><span data-stu-id="47ebb-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47ebb-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="47ebb-135">Request</span></span>
<span data-ttu-id="47ebb-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47ebb-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationsubmissionresource"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="47ebb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="47ebb-137">Response</span></span>
<span data-ttu-id="47ebb-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47ebb-138">The following is an example of the response.</span></span> 

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
  "suppressions": []
}
-->
