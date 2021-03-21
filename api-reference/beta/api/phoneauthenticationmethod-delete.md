---
title: Удаление phoneAuthenticationMethod
description: Удаление метода проверки подлинности телефона пользователя.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bbd08b9da7a75c471e90b9846e3aaa2c1a503879
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957489"
---
# <a name="delete-phoneauthenticationmethod"></a><span data-ttu-id="9ed50-103">Удаление phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9ed50-103">Delete phoneAuthenticationMethod</span></span>

<span data-ttu-id="9ed50-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ed50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ed50-105">Удаление метода проверки подлинности [телефона пользователя.](../resources/phoneauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="9ed50-105">Delete a user's [phone authentication method](../resources/phoneauthenticationmethod.md).</span></span> 

><span data-ttu-id="9ed50-106">**Примечание:** Это удаляет номер телефона у пользователя, и он больше не сможет использовать его для проверки подлинности, будь то с помощью SMS или голосовых вызовов.</span><span class="sxs-lookup"><span data-stu-id="9ed50-106">**Note:** This removes the phone number from the user and they will no longer be able to use the number for authentication, whether via SMS or voice calls.</span></span>

<span data-ttu-id="9ed50-107">Помните, что пользователь не может иметь `alternateMobile` номер без `mobile` номера.</span><span class="sxs-lookup"><span data-stu-id="9ed50-107">Remember that a user cannot have an `alternateMobile` number without a `mobile` number.</span></span> <span data-ttu-id="9ed50-108">Если вы хотите удалить номер пользователя, который также имеет номер, сначала обновите номер на новый `mobile` `alternateMobile` [](phoneauthenticationmethod-update.md) `mobile` номер, а затем удалите `alternateMobile` номер.</span><span class="sxs-lookup"><span data-stu-id="9ed50-108">If you want to remove a `mobile` number from a user that also has an `alternateMobile` number, first [update](phoneauthenticationmethod-update.md) the `mobile` number to the new number, then delete the `alternateMobile` number.</span></span>

<span data-ttu-id="9ed50-109">Если номер телефона является методом многофакторной проверки подлинности Azure по умолчанию, его невозможно удалить.</span><span class="sxs-lookup"><span data-stu-id="9ed50-109">If the phone number is the user's default Azure multi-factor authentication (MFA) authentication method, it cannot be deleted.</span></span> <span data-ttu-id="9ed50-110">Измените метод проверки подлинности по умолчанию, а затем удалите номер.</span><span class="sxs-lookup"><span data-stu-id="9ed50-110">Have the user change their default authentication method, and then delete the number.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ed50-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ed50-111">Permissions</span></span>

<span data-ttu-id="9ed50-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ed50-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="9ed50-114">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="9ed50-114">Permissions acting on self</span></span>

|<span data-ttu-id="9ed50-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ed50-115">Permission type</span></span>      | <span data-ttu-id="9ed50-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ed50-116">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9ed50-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ed50-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ed50-118">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9ed50-118">UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="9ed50-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ed50-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ed50-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ed50-120">Not supported.</span></span> |
| <span data-ttu-id="9ed50-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ed50-121">Application</span></span>                            | <span data-ttu-id="9ed50-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ed50-122">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="9ed50-123">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="9ed50-123">Permissions acting on other users</span></span>

|<span data-ttu-id="9ed50-124">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ed50-124">Permission type</span></span>      | <span data-ttu-id="9ed50-125">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ed50-125">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="9ed50-126">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ed50-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ed50-127">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ed50-127">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="9ed50-128">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ed50-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ed50-129">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ed50-129">Not supported.</span></span> |
| <span data-ttu-id="9ed50-130">Application</span><span class="sxs-lookup"><span data-stu-id="9ed50-130">Application</span></span>                            | <span data-ttu-id="9ed50-131">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ed50-131">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="9ed50-132">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="9ed50-132">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="9ed50-133">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="9ed50-133">Global admin</span></span>
* <span data-ttu-id="9ed50-134">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="9ed50-134">Privileged authentication admin</span></span>
* <span data-ttu-id="9ed50-135">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="9ed50-135">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="9ed50-136">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ed50-136">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/authentication/phoneMethods/{id}
DELETE /users/{id | userPrincipalName}/authentication/phoneMethods/{id}
```
<span data-ttu-id="9ed50-137">Значение, `id` соответствующее удаляемой phoneType, является одним из следующих:</span><span class="sxs-lookup"><span data-stu-id="9ed50-137">The value of `id` corresponding to the phoneType to delete is one of the following:</span></span>
+ <span data-ttu-id="9ed50-138">`b6332ec1-7057-4abe-9331-3d72feddfe41` удаление `alternateMobile` **phoneType**.</span><span class="sxs-lookup"><span data-stu-id="9ed50-138">`b6332ec1-7057-4abe-9331-3d72feddfe41` to delete the `alternateMobile` **phoneType**.</span></span>
+ <span data-ttu-id="9ed50-139">`e37fc753-ff3b-4958-9484-eaa9425c82bc` удаление `office` **phoneType**.</span><span class="sxs-lookup"><span data-stu-id="9ed50-139">`e37fc753-ff3b-4958-9484-eaa9425c82bc` to delete the `office` **phoneType**.</span></span>
+ <span data-ttu-id="9ed50-140">`3179e48a-750b-4051-897c-87b9720928f7` удаление `mobile` **phoneType**.</span><span class="sxs-lookup"><span data-stu-id="9ed50-140">`3179e48a-750b-4051-897c-87b9720928f7` to delete the `mobile` **phoneType**.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ed50-141">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ed50-141">Request headers</span></span>

| <span data-ttu-id="9ed50-142">Имя</span><span class="sxs-lookup"><span data-stu-id="9ed50-142">Name</span></span>          | <span data-ttu-id="9ed50-143">Описание</span><span class="sxs-lookup"><span data-stu-id="9ed50-143">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="9ed50-144">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ed50-144">Authorization</span></span> | <span data-ttu-id="9ed50-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ed50-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ed50-147">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ed50-147">Request body</span></span>

<span data-ttu-id="9ed50-148">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ed50-148">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ed50-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ed50-149">Response</span></span>

<span data-ttu-id="9ed50-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9ed50-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ed50-152">Примеры</span><span class="sxs-lookup"><span data-stu-id="9ed50-152">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ed50-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ed50-153">Request</span></span>

<span data-ttu-id="9ed50-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ed50-154">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ed50-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ed50-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_phoneauthenticationmethod"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7
```
# <a name="c"></a>[<span data-ttu-id="9ed50-156">C#</span><span class="sxs-lookup"><span data-stu-id="9ed50-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-phoneauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ed50-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ed50-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-phoneauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ed50-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ed50-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-phoneauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ed50-159">Java</span><span class="sxs-lookup"><span data-stu-id="9ed50-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-phoneauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ed50-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ed50-160">Response</span></span>

<span data-ttu-id="9ed50-161">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9ed50-161">The following is an example of the response.</span></span>

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
