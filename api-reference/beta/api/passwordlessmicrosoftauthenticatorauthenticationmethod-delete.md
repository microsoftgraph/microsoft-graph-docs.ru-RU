---
title: Удаление Пассвордлессмикрософтаусентикатораусентикатионмесод
description: Удаляет объект Пассвордлессмикрософтаусентикатораусентикатионмесод.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e7931c0524662397e25f97a0c53426b243226be
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457531"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethod"></a><span data-ttu-id="daede-103">Удаление Пассвордлессмикрософтаусентикатораусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="daede-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="daede-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daede-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daede-105">Удаляет объект метода входа без пароля пользователя для средства [проверки подлинности Майкрософт](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="daede-105">Deletes a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="daede-106">Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии.</span><span class="sxs-lookup"><span data-stu-id="daede-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="daede-107">Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.</span><span class="sxs-lookup"><span data-stu-id="daede-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>


## <a name="permissions"></a><span data-ttu-id="daede-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="daede-108">Permissions</span></span>
<span data-ttu-id="daede-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daede-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daede-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="daede-111">Permission type</span></span>|<span data-ttu-id="daede-112">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="daede-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="daede-113">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="daede-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="daede-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="daede-114">Delegated (work or school account)</span></span>|<span data-ttu-id="daede-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daede-115">Not supported.</span></span>|<span data-ttu-id="daede-116">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="daede-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="daede-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="daede-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daede-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daede-118">Not supported.</span></span>|<span data-ttu-id="daede-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daede-119">Not supported.</span></span>
|<span data-ttu-id="daede-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="daede-120">Application</span></span>|<span data-ttu-id="daede-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daede-121">Not supported.</span></span>|<span data-ttu-id="daede-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daede-122">Not supported.</span></span>

<span data-ttu-id="daede-123">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="daede-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="daede-124">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="daede-124">Global admin</span></span>
* <span data-ttu-id="daede-125">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="daede-125">Global reader</span></span>
* <span data-ttu-id="daede-126">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="daede-126">Privileged authentication admin</span></span>
* <span data-ttu-id="daede-127">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="daede-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="daede-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="daede-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="daede-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="daede-129">Request headers</span></span>
|<span data-ttu-id="daede-130">Имя</span><span class="sxs-lookup"><span data-stu-id="daede-130">Name</span></span>|<span data-ttu-id="daede-131">Описание</span><span class="sxs-lookup"><span data-stu-id="daede-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="daede-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="daede-132">Authorization</span></span>|<span data-ttu-id="daede-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="daede-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="daede-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="daede-135">Request body</span></span>
<span data-ttu-id="daede-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="daede-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daede-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="daede-137">Response</span></span>

<span data-ttu-id="daede-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="daede-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="daede-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="daede-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="daede-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="daede-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="daede-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="daede-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="daede-143">C#</span><span class="sxs-lookup"><span data-stu-id="daede-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="daede-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="daede-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="daede-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="daede-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="daede-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="daede-146">Response</span></span>
<span data-ttu-id="daede-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="daede-147">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

