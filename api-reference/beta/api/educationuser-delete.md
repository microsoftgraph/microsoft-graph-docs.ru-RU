---
title: Удаление educationUser
description: Удаление пользователя.
ms.openlocfilehash: 9f0eba350026c45f0371c6de5c8db6e76fc71dfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076973"
---
# <a name="delete-educationuser"></a><span data-ttu-id="f57fd-103">Удаление educationUser</span><span class="sxs-lookup"><span data-stu-id="f57fd-103">Delete educationUser</span></span>

> <span data-ttu-id="f57fd-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f57fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f57fd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f57fd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f57fd-106">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="f57fd-106">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="f57fd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f57fd-107">Permissions</span></span>
<span data-ttu-id="f57fd-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f57fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f57fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f57fd-110">Permission type</span></span>      | <span data-ttu-id="f57fd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f57fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f57fd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f57fd-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="f57fd-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f57fd-113">Not supported.</span></span>  |
|<span data-ttu-id="f57fd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f57fd-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f57fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f57fd-115">Not supported.</span></span>  |
|<span data-ttu-id="f57fd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f57fd-116">Application</span></span> | <span data-ttu-id="f57fd-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f57fd-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f57fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f57fd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f57fd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f57fd-119">Request headers</span></span>
| <span data-ttu-id="f57fd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f57fd-120">Header</span></span>       | <span data-ttu-id="f57fd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f57fd-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f57fd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f57fd-122">Authorization</span></span>  | <span data-ttu-id="f57fd-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f57fd-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f57fd-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f57fd-125">Request body</span></span>
<span data-ttu-id="f57fd-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f57fd-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="f57fd-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="f57fd-127">Response</span></span>
<span data-ttu-id="f57fd-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f57fd-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f57fd-130">Пример</span><span class="sxs-lookup"><span data-stu-id="f57fd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f57fd-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="f57fd-131">Request</span></span>
<span data-ttu-id="f57fd-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f57fd-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/users/13019
```
##### <a name="response"></a><span data-ttu-id="f57fd-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="f57fd-133">Response</span></span>
<span data-ttu-id="f57fd-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f57fd-134">The following is an example of the response.</span></span> 
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
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->