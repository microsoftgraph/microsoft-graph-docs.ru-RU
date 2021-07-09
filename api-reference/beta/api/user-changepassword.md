---
title: 'пользователь: changePassword'
description: Обновите собственный пароль.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 2c582b4465c12aa2ccf86e74e35408ccbe8fc4c0
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351172"
---
# <a name="user-changepassword"></a><span data-ttu-id="d133c-103">пользователь: changePassword</span><span class="sxs-lookup"><span data-stu-id="d133c-103">user: changePassword</span></span>

<span data-ttu-id="d133c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d133c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d133c-105">Внося пользователю возможность обновить пароль.</span><span class="sxs-lookup"><span data-stu-id="d133c-105">Enable the user to update their password.</span></span> <span data-ttu-id="d133c-106">Любой пользователь может обновить пароль, не относясь к роли администратора.</span><span class="sxs-lookup"><span data-stu-id="d133c-106">Any user can update their password without belonging to any administrator role.</span></span>

## <a name="permissions"></a><span data-ttu-id="d133c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d133c-107">Permissions</span></span>
<span data-ttu-id="d133c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d133c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d133c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d133c-110">Permission type</span></span>      | <span data-ttu-id="d133c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d133c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d133c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d133c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d133c-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d133c-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d133c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d133c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d133c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d133c-115">Not supported.</span></span>    |
|<span data-ttu-id="d133c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d133c-116">Application</span></span> | <span data-ttu-id="d133c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d133c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d133c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d133c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/changePassword
```
## <a name="request-headers"></a><span data-ttu-id="d133c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d133c-119">Request headers</span></span>
| <span data-ttu-id="d133c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d133c-120">Header</span></span>       | <span data-ttu-id="d133c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d133c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d133c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d133c-122">Authorization</span></span>  | <span data-ttu-id="d133c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d133c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d133c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d133c-125">Content-type</span></span>  | <span data-ttu-id="d133c-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d133c-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d133c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d133c-128">Request body</span></span>
<span data-ttu-id="d133c-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d133c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d133c-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="d133c-130">Parameter</span></span>    | <span data-ttu-id="d133c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d133c-131">Type</span></span>   |<span data-ttu-id="d133c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d133c-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d133c-133">currentPassword</span><span class="sxs-lookup"><span data-stu-id="d133c-133">currentPassword</span></span> | <span data-ttu-id="d133c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="d133c-134">String</span></span> | <span data-ttu-id="d133c-135">Текущий пароль.</span><span class="sxs-lookup"><span data-stu-id="d133c-135">Your current password.</span></span>|
| <span data-ttu-id="d133c-136">newPassword</span><span class="sxs-lookup"><span data-stu-id="d133c-136">newPassword</span></span> | <span data-ttu-id="d133c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d133c-137">String</span></span> | <span data-ttu-id="d133c-138">Новый пароль.</span><span class="sxs-lookup"><span data-stu-id="d133c-138">Your new password.</span></span>|

## <a name="response"></a><span data-ttu-id="d133c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d133c-139">Response</span></span>

<span data-ttu-id="d133c-140">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d133c-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d133c-141">Пример</span><span class="sxs-lookup"><span data-stu-id="d133c-141">Example</span></span>
<span data-ttu-id="d133c-142">В следующем примере показан запрос на обновление собственного пароля.</span><span class="sxs-lookup"><span data-stu-id="d133c-142">The following example shows a request to update your own password.</span></span>

### <a name="request"></a><span data-ttu-id="d133c-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d133c-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "user_changepassword"
}-->
```http
POST https://graph.microsoft.com/beta/me/changePassword
Content-type: application/json

{
    "currentPassword": "xWwvJ]6NMw+bWH-d",
    "newPassword": "0eM85N54wFxWwvJ]"
}
```


### <a name="response"></a><span data-ttu-id="d133c-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="d133c-144">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="d133c-145">См. также</span><span class="sxs-lookup"><span data-stu-id="d133c-145">See also</span></span>
+ [<span data-ttu-id="d133c-146">Обновление passwordProfile пользователя для сброса пароля</span><span class="sxs-lookup"><span data-stu-id="d133c-146">Update the passwordProfile of a user to reset their password</span></span>](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password)

<!-- uuid: a7c9a0de-8324-4f80-8d88-2e6d5838f3be
2021-06-24 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: changePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


