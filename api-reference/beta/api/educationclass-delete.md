---
title: Удаление educationClass
description: Удаление класса. Так как класс также является универсальной группой, удаление класса приводит к удалению группы.
ms.openlocfilehash: e63903f1a6db2c223071f04db26f31e3cfbc2168
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079739"
---
# <a name="delete-educationclass"></a><span data-ttu-id="9a3f3-104">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="9a3f3-104">Delete educationClass</span></span>

> <span data-ttu-id="9a3f3-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9a3f3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a3f3-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a3f3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a3f3-107">Удаление класса.</span><span class="sxs-lookup"><span data-stu-id="9a3f3-107">Delete a class.</span></span> <span data-ttu-id="9a3f3-108">Так как класс также является универсальной группой, удаление класса приводит к удалению группы.</span><span class="sxs-lookup"><span data-stu-id="9a3f3-108">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a3f3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a3f3-109">Permissions</span></span>
<span data-ttu-id="9a3f3-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a3f3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a3f3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a3f3-112">Permission type</span></span>      | <span data-ttu-id="9a3f3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a3f3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a3f3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a3f3-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="9a3f3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a3f3-115">Not supported.</span></span>  |
|<span data-ttu-id="9a3f3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a3f3-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9a3f3-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a3f3-117">Not supported.</span></span>  |
|<span data-ttu-id="9a3f3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a3f3-118">Application</span></span> | <span data-ttu-id="9a3f3-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a3f3-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9a3f3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a3f3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9a3f3-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9a3f3-121">Request headers</span></span>
| <span data-ttu-id="9a3f3-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a3f3-122">Header</span></span>       | <span data-ttu-id="9a3f3-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9a3f3-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a3f3-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9a3f3-124">Authorization</span></span>  | <span data-ttu-id="9a3f3-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a3f3-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a3f3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9a3f3-127">Request body</span></span>
<span data-ttu-id="9a3f3-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9a3f3-128">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9a3f3-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a3f3-129">Response</span></span>
<span data-ttu-id="9a3f3-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9a3f3-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a3f3-132">Пример</span><span class="sxs-lookup"><span data-stu-id="9a3f3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a3f3-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a3f3-133">Request</span></span>
<span data-ttu-id="9a3f3-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a3f3-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11022
```
##### <a name="response"></a><span data-ttu-id="9a3f3-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a3f3-135">Response</span></span>
<span data-ttu-id="9a3f3-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9a3f3-136">The following is an example of the response.</span></span> 

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