---
title: Удаление пользователя
description: Удаление пользователя.
author: dkershaw10
ms.openlocfilehash: 44e0439a95b0104472101b43adfae39b2c553d58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301178"
---
# <a name="delete-a-user"></a><span data-ttu-id="ae4ac-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="ae4ac-103">Delete a user</span></span>

<span data-ttu-id="ae4ac-104">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="ae4ac-104">Delete user.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae4ac-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae4ac-105">Permissions</span></span>
<span data-ttu-id="ae4ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae4ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae4ac-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae4ac-108">Permission type</span></span>      | <span data-ttu-id="ae4ac-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae4ac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae4ac-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae4ac-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ae4ac-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae4ac-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae4ac-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae4ac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae4ac-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae4ac-113">Not supported.</span></span>    |
|<span data-ttu-id="ae4ac-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae4ac-114">Application</span></span> | <span data-ttu-id="ae4ac-115">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae4ac-115">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae4ac-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae4ac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="ae4ac-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae4ac-117">Request headers</span></span>
| <span data-ttu-id="ae4ac-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ae4ac-118">Header</span></span>       | <span data-ttu-id="ae4ac-119">Значение</span><span class="sxs-lookup"><span data-stu-id="ae4ac-119">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="ae4ac-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ae4ac-120">Authorization</span></span>  | <span data-ttu-id="ae4ac-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ae4ac-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ae4ac-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ae4ac-123">Request body</span></span>
<span data-ttu-id="ae4ac-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ae4ac-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae4ac-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae4ac-125">Response</span></span>

<span data-ttu-id="ae4ac-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ae4ac-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae4ac-128">Пример</span><span class="sxs-lookup"><span data-stu-id="ae4ac-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae4ac-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae4ac-129">Request</span></span>
<span data-ttu-id="ae4ac-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae4ac-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{user-id}
```
##### <a name="response"></a><span data-ttu-id="ae4ac-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ae4ac-131">Response</span></span>
<span data-ttu-id="ae4ac-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae4ac-132">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->