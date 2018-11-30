---
title: Удаление пользователя
description: Удаление пользователя.
ms.openlocfilehash: f7f72ae91c636ef005768c2c4933ed2786ced91d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080338"
---
# <a name="delete-a-user"></a><span data-ttu-id="9d21f-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="9d21f-103">Delete a user</span></span>

> <span data-ttu-id="9d21f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9d21f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d21f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d21f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d21f-106">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="9d21f-106">Delete user.</span></span>
## <a name="permissions"></a><span data-ttu-id="9d21f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d21f-107">Permissions</span></span>
<span data-ttu-id="9d21f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d21f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d21f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d21f-110">Permission type</span></span>      | <span data-ttu-id="9d21f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d21f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d21f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d21f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d21f-113">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d21f-113">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9d21f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d21f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d21f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d21f-115">Not supported.</span></span>    |
|<span data-ttu-id="9d21f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d21f-116">Application</span></span> | <span data-ttu-id="9d21f-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d21f-117">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d21f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d21f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="9d21f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d21f-119">Request headers</span></span>
| <span data-ttu-id="9d21f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d21f-120">Header</span></span>       | <span data-ttu-id="9d21f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9d21f-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="9d21f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d21f-122">Authorization</span></span>  | <span data-ttu-id="9d21f-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d21f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9d21f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d21f-125">Request body</span></span>
<span data-ttu-id="9d21f-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d21f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d21f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d21f-127">Response</span></span>

<span data-ttu-id="9d21f-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9d21f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d21f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9d21f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d21f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d21f-131">Request</span></span>
<span data-ttu-id="9d21f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d21f-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
##### <a name="response"></a><span data-ttu-id="9d21f-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d21f-133">Response</span></span>
<span data-ttu-id="9d21f-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9d21f-134">Here is an example of the response.</span></span> 
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