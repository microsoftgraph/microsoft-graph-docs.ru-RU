---
title: Удаление educationClass
description: Удаление класса. Так как класс также является универсальной группой, удаление класса приводит к удалению группы.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9b25e95dfa109ef48d67374ba7569a32af22ba50
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935068"
---
# <a name="delete-educationclass"></a><span data-ttu-id="8b60b-104">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="8b60b-104">Delete educationClass</span></span>

> <span data-ttu-id="8b60b-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8b60b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b60b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b60b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b60b-107">Удаление класса.</span><span class="sxs-lookup"><span data-stu-id="8b60b-107">Delete a class.</span></span> <span data-ttu-id="8b60b-108">Так как класс также является универсальной группой, удаление класса приводит к удалению группы.</span><span class="sxs-lookup"><span data-stu-id="8b60b-108">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b60b-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b60b-109">Permissions</span></span>
<span data-ttu-id="8b60b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b60b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b60b-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b60b-112">Permission type</span></span>      | <span data-ttu-id="8b60b-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b60b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b60b-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b60b-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="8b60b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b60b-115">Not supported.</span></span>  |
|<span data-ttu-id="8b60b-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b60b-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8b60b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b60b-117">Not supported.</span></span>  |
|<span data-ttu-id="8b60b-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b60b-118">Application</span></span> | <span data-ttu-id="8b60b-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b60b-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8b60b-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b60b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="8b60b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b60b-121">Request headers</span></span>
| <span data-ttu-id="8b60b-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b60b-122">Header</span></span>       | <span data-ttu-id="8b60b-123">Значение</span><span class="sxs-lookup"><span data-stu-id="8b60b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b60b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b60b-124">Authorization</span></span>  | <span data-ttu-id="8b60b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b60b-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b60b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b60b-127">Request body</span></span>
<span data-ttu-id="8b60b-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b60b-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8b60b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b60b-129">Response</span></span>
<span data-ttu-id="8b60b-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8b60b-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b60b-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8b60b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b60b-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b60b-133">Request</span></span>
<span data-ttu-id="8b60b-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b60b-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="8b60b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b60b-135">Response</span></span>
<span data-ttu-id="8b60b-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8b60b-136">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
