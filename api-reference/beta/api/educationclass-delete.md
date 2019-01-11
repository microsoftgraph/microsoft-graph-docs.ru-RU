---
title: Удаление educationClass
description: Удаление класса. Так как класс также является универсальной группой, удаление класса приводит к удалению группы.
localization_priority: Normal
ms.openlocfilehash: f042d7290b99f54efc6809162647ecbb6395f006
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864640"
---
# <a name="delete-educationclass"></a><span data-ttu-id="d2f4f-104">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="d2f4f-104">Delete educationClass</span></span>

> <span data-ttu-id="d2f4f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d2f4f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2f4f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f4f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d2f4f-107">Удаление класса.</span><span class="sxs-lookup"><span data-stu-id="d2f4f-107">Delete a class.</span></span> <span data-ttu-id="d2f4f-108">Так как класс также является универсальной группой, удаление класса приводит к удалению группы.</span><span class="sxs-lookup"><span data-stu-id="d2f4f-108">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2f4f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f4f-109">Permissions</span></span>
<span data-ttu-id="d2f4f-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2f4f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2f4f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2f4f-112">Permission type</span></span>      | <span data-ttu-id="d2f4f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2f4f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2f4f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2f4f-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="d2f4f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f4f-115">Not supported.</span></span>  |
|<span data-ttu-id="d2f4f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2f4f-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d2f4f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2f4f-117">Not supported.</span></span>  |
|<span data-ttu-id="d2f4f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2f4f-118">Application</span></span> | <span data-ttu-id="d2f4f-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2f4f-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d2f4f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2f4f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d2f4f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2f4f-121">Request headers</span></span>
| <span data-ttu-id="d2f4f-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2f4f-122">Header</span></span>       | <span data-ttu-id="d2f4f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d2f4f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d2f4f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2f4f-124">Authorization</span></span>  | <span data-ttu-id="d2f4f-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2f4f-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2f4f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2f4f-127">Request body</span></span>
<span data-ttu-id="d2f4f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2f4f-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d2f4f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2f4f-129">Response</span></span>
<span data-ttu-id="d2f4f-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d2f4f-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2f4f-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d2f4f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2f4f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2f4f-133">Request</span></span>
<span data-ttu-id="d2f4f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2f4f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="d2f4f-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d2f4f-135">Response</span></span>
<span data-ttu-id="d2f4f-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d2f4f-136">The following is an example of the response.</span></span> 

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
