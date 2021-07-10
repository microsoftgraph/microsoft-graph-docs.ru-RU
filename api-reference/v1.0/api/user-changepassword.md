---
title: 'пользователь: changePassword'
description: Обновление собственного пароля.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1ece0fb33e241900356a367233dfee0a5bb0c90a
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351348"
---
# <a name="user-changepassword"></a><span data-ttu-id="a25c6-103">пользователь: changePassword</span><span class="sxs-lookup"><span data-stu-id="a25c6-103">user: changePassword</span></span>

<span data-ttu-id="a25c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a25c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a25c6-105">Внося пользователю возможность обновить пароль.</span><span class="sxs-lookup"><span data-stu-id="a25c6-105">Enable the user to update their password.</span></span> <span data-ttu-id="a25c6-106">Любой пользователь может обновить пароль, не относясь к роли администратора.</span><span class="sxs-lookup"><span data-stu-id="a25c6-106">Any user can update their password without belonging to any administrator role.</span></span>

## <a name="permissions"></a><span data-ttu-id="a25c6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a25c6-107">Permissions</span></span>
<span data-ttu-id="a25c6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a25c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a25c6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a25c6-110">Permission type</span></span>      | <span data-ttu-id="a25c6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a25c6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a25c6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a25c6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a25c6-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a25c6-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a25c6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a25c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a25c6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a25c6-115">Not supported.</span></span>    |
|<span data-ttu-id="a25c6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a25c6-116">Application</span></span> | <span data-ttu-id="a25c6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a25c6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a25c6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a25c6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/changePassword
```
## <a name="request-headers"></a><span data-ttu-id="a25c6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a25c6-119">Request headers</span></span>
| <span data-ttu-id="a25c6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a25c6-120">Header</span></span>       | <span data-ttu-id="a25c6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a25c6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a25c6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a25c6-122">Authorization</span></span>  | <span data-ttu-id="a25c6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a25c6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a25c6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a25c6-125">Content-type</span></span>  | <span data-ttu-id="a25c6-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a25c6-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a25c6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a25c6-128">Request body</span></span>
<span data-ttu-id="a25c6-129">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a25c6-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a25c6-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="a25c6-130">Parameter</span></span>    | <span data-ttu-id="a25c6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a25c6-131">Type</span></span>   |<span data-ttu-id="a25c6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a25c6-132">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a25c6-133">currentPassword</span><span class="sxs-lookup"><span data-stu-id="a25c6-133">currentPassword</span></span> | <span data-ttu-id="a25c6-134">String</span><span class="sxs-lookup"><span data-stu-id="a25c6-134">String</span></span> | <span data-ttu-id="a25c6-135">Текущий пароль.</span><span class="sxs-lookup"><span data-stu-id="a25c6-135">Your current password.</span></span>|
| <span data-ttu-id="a25c6-136">newPassword</span><span class="sxs-lookup"><span data-stu-id="a25c6-136">newPassword</span></span> | <span data-ttu-id="a25c6-137">String</span><span class="sxs-lookup"><span data-stu-id="a25c6-137">String</span></span> | <span data-ttu-id="a25c6-138">Новый пароль.</span><span class="sxs-lookup"><span data-stu-id="a25c6-138">Your new password.</span></span>|

## <a name="response"></a><span data-ttu-id="a25c6-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a25c6-139">Response</span></span>

<span data-ttu-id="a25c6-140">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a25c6-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a25c6-141">Пример</span><span class="sxs-lookup"><span data-stu-id="a25c6-141">Example</span></span>
<span data-ttu-id="a25c6-142">В следующем примере показан запрос на обновление собственного пароля.</span><span class="sxs-lookup"><span data-stu-id="a25c6-142">The following example shows a request to update your own password.</span></span>

### <a name="request"></a><span data-ttu-id="a25c6-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="a25c6-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "user_changepassword"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/changePassword
Content-type: application/json

{
    "currentPassword": "xWwvJ]6NMw+bWH-d",
    "newPassword": "0eM85N54wFxWwvJ]"
}
```


### <a name="response"></a><span data-ttu-id="a25c6-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a25c6-144">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="a25c6-145">См. также</span><span class="sxs-lookup"><span data-stu-id="a25c6-145">See also</span></span>
+ [<span data-ttu-id="a25c6-146">Обновление passwordProfile пользователя для сброса пароля</span><span class="sxs-lookup"><span data-stu-id="a25c6-146">Update the passwordProfile of a user to reset their password</span></span>](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password)

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


