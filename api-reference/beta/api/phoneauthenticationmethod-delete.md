---
title: Удаление phoneAuthenticationMethod
description: Удаление метода проверки подлинности на телефоне пользователя.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b506851ec693b5fe9cba2216910ba635c7d648af
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796600"
---
# <a name="delete-phoneauthenticationmethod"></a><span data-ttu-id="b87a7-103">Удаление phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b87a7-103">Delete phoneAuthenticationMethod</span></span>

<span data-ttu-id="b87a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b87a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b87a7-105">Удаление метода проверки подлинности [на телефоне пользователя.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b87a7-105">Delete a user's [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> 

><span data-ttu-id="b87a7-106">**Примечание.** Это удаляет номер телефона пользователя, и он больше не сможет использовать этот номер для проверки подлинности с помощью SMS или голосовых вызовов.</span><span class="sxs-lookup"><span data-stu-id="b87a7-106">**Note:** This removes the phone number from the user and they will no longer be able to use the number for authentication, whether via SMS or voice calls.</span></span>

<span data-ttu-id="b87a7-107">Помните, что пользователь не может иметь `alternateMobile` номер без `mobile` него.</span><span class="sxs-lookup"><span data-stu-id="b87a7-107">Remember that a user cannot have an `alternateMobile` number without a `mobile` number.</span></span> <span data-ttu-id="b87a7-108">Если вы хотите удалить номер пользователя, который также имеет номер, сначала обновите его до нового номера, а затем `mobile` `alternateMobile` [](phoneauthenticationmethod-update.md) `mobile` `alternateMobile` удалите номер.</span><span class="sxs-lookup"><span data-stu-id="b87a7-108">If you want to remove a `mobile` number from a user that also has an `alternateMobile` number, first [update](phoneauthenticationmethod-update.md) the `mobile` number to the new number, then delete the `alternateMobile` number.</span></span>

<span data-ttu-id="b87a7-109">Если номер телефона является методом многофакторной проверки подлинности Azure (MFA) пользователя по умолчанию, его нельзя удалить.</span><span class="sxs-lookup"><span data-stu-id="b87a7-109">If the phone number is the user's default Azure multi-factor authentication (MFA) authentication method, it cannot be deleted.</span></span> <span data-ttu-id="b87a7-110">Пользователь должен изменить метод проверки подлинности по умолчанию, а затем удалить номер.</span><span class="sxs-lookup"><span data-stu-id="b87a7-110">Have the user change their default authentication method, and then delete the number.</span></span>

## <a name="permissions"></a><span data-ttu-id="b87a7-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b87a7-111">Permissions</span></span>

<span data-ttu-id="b87a7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b87a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="b87a7-114">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="b87a7-114">Permissions acting on self</span></span>

|<span data-ttu-id="b87a7-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b87a7-115">Permission type</span></span>      | <span data-ttu-id="b87a7-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b87a7-116">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="b87a7-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b87a7-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="b87a7-118">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b87a7-118">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="b87a7-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b87a7-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b87a7-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b87a7-120">Not supported.</span></span> |
| <span data-ttu-id="b87a7-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b87a7-121">Application</span></span>                            | <span data-ttu-id="b87a7-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b87a7-122">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="b87a7-123">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="b87a7-123">Permissions acting on other users</span></span>

|<span data-ttu-id="b87a7-124">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b87a7-124">Permission type</span></span>      | <span data-ttu-id="b87a7-125">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b87a7-125">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="b87a7-126">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b87a7-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="b87a7-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b87a7-127">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b87a7-128">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b87a7-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b87a7-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b87a7-129">Not supported.</span></span> |
| <span data-ttu-id="b87a7-130">Приложение</span><span class="sxs-lookup"><span data-stu-id="b87a7-130">Application</span></span>                            | <span data-ttu-id="b87a7-131">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b87a7-131">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b87a7-132">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="b87a7-132">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="b87a7-133">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b87a7-133">Global admin</span></span>
* <span data-ttu-id="b87a7-134">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b87a7-134">Privileged authentication admin</span></span>
* <span data-ttu-id="b87a7-135">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b87a7-135">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b87a7-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b87a7-136">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/authentication/phoneMethods/{id}
DELETE /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b87a7-137">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b87a7-137">Request headers</span></span>

| <span data-ttu-id="b87a7-138">Имя</span><span class="sxs-lookup"><span data-stu-id="b87a7-138">Name</span></span>          | <span data-ttu-id="b87a7-139">Описание</span><span class="sxs-lookup"><span data-stu-id="b87a7-139">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b87a7-140">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b87a7-140">Authorization</span></span> | <span data-ttu-id="b87a7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b87a7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b87a7-143">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b87a7-143">Request body</span></span>

<span data-ttu-id="b87a7-144">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b87a7-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b87a7-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="b87a7-145">Response</span></span>

<span data-ttu-id="b87a7-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b87a7-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b87a7-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="b87a7-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b87a7-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="b87a7-149">Request</span></span>

<span data-ttu-id="b87a7-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b87a7-150">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b87a7-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="b87a7-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_phoneauthenticationmethod"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="b87a7-152">C#</span><span class="sxs-lookup"><span data-stu-id="b87a7-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b87a7-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b87a7-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b87a7-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b87a7-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b87a7-155">Java</span><span class="sxs-lookup"><span data-stu-id="b87a7-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b87a7-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b87a7-156">Response</span></span>

<span data-ttu-id="b87a7-157">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b87a7-157">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete phoneAuthenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
