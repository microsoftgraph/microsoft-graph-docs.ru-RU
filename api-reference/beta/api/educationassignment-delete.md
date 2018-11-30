---
title: Удаление educationAssignment
description: Удаление существующего назначения. Назначения можно удалить только учителя внутри класса.
ms.openlocfilehash: e9965efa458459cff0c3914dbc12b37153a6ab51
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079733"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="950a0-104">Удаление educationAssignment</span><span class="sxs-lookup"><span data-stu-id="950a0-104">Delete educationAssignment</span></span>

> <span data-ttu-id="950a0-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="950a0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="950a0-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="950a0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="950a0-107">Удаление существующего назначения.</span><span class="sxs-lookup"><span data-stu-id="950a0-107">Delete an existing assignment.</span></span> <span data-ttu-id="950a0-108">Назначения можно удалить только учителя внутри класса.</span><span class="sxs-lookup"><span data-stu-id="950a0-108">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="950a0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="950a0-109">Permissions</span></span>
<span data-ttu-id="950a0-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="950a0-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="950a0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="950a0-112">Permission type</span></span>      | <span data-ttu-id="950a0-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="950a0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="950a0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="950a0-114">Delegated (work or school account)</span></span>| <span data-ttu-id="950a0-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="950a0-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="950a0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="950a0-116">Delegated (personal Microsoft account)</span></span> |   <span data-ttu-id="950a0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="950a0-117">Not Supported.</span></span> |
|<span data-ttu-id="950a0-118">Для приложения</span><span class="sxs-lookup"><span data-stu-id="950a0-118">Application</span></span> | <span data-ttu-id="950a0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="950a0-119">Not Supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="950a0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="950a0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/<id>/assignments/<id>
```
## <a name="request-headers"></a><span data-ttu-id="950a0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="950a0-121">Request headers</span></span>
| <span data-ttu-id="950a0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="950a0-122">Header</span></span>       | <span data-ttu-id="950a0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="950a0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="950a0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="950a0-124">Authorization</span></span>  | <span data-ttu-id="950a0-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="950a0-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="950a0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="950a0-127">Request body</span></span>
<span data-ttu-id="950a0-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="950a0-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="950a0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="950a0-129">Response</span></span>
<span data-ttu-id="950a0-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="950a0-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="950a0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="950a0-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="950a0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="950a0-133">Request</span></span>
<span data-ttu-id="950a0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="950a0-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
### <a name="response"></a><span data-ttu-id="950a0-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="950a0-135">Response</span></span>
<span data-ttu-id="950a0-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="950a0-136">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->