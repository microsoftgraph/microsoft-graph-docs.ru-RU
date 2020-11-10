---
title: Удаление Пассвордлессмикрософтаусентикатораусентикатионмесод
description: Удаляет объект Пассвордлессмикрософтаусентикатораусентикатионмесод.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ce55978f153bca32fb2f34a33947d612340f2dc6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968651"
---
# <a name="delete-passwordlessmicrosoftauthenticatorauthenticationmethod"></a><span data-ttu-id="ee3e5-103">Удаление Пассвордлессмикрософтаусентикатораусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="ee3e5-103">Delete passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="ee3e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee3e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee3e5-105">Удаляет объект метода входа без пароля пользователя для средства [проверки подлинности Майкрософт](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="ee3e5-105">Deletes a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="ee3e5-106">Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии.</span><span class="sxs-lookup"><span data-stu-id="ee3e5-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="ee3e5-107">Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.</span><span class="sxs-lookup"><span data-stu-id="ee3e5-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>


## <a name="permissions"></a><span data-ttu-id="ee3e5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee3e5-108">Permissions</span></span>
<span data-ttu-id="ee3e5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee3e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee3e5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee3e5-111">Permission type</span></span>|<span data-ttu-id="ee3e5-112">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee3e5-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="ee3e5-113">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="ee3e5-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="ee3e5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee3e5-114">Delegated (work or school account)</span></span>|<span data-ttu-id="ee3e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee3e5-115">Not supported.</span></span>|<span data-ttu-id="ee3e5-116">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ee3e5-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="ee3e5-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee3e5-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee3e5-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee3e5-118">Not supported.</span></span>|<span data-ttu-id="ee3e5-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee3e5-119">Not supported.</span></span>
|<span data-ttu-id="ee3e5-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee3e5-120">Application</span></span>|<span data-ttu-id="ee3e5-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee3e5-121">Not supported.</span></span>|<span data-ttu-id="ee3e5-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee3e5-122">Not supported.</span></span>

<span data-ttu-id="ee3e5-123">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="ee3e5-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="ee3e5-124">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ee3e5-124">Global admin</span></span>
* <span data-ttu-id="ee3e5-125">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="ee3e5-125">Global reader</span></span>
* <span data-ttu-id="ee3e5-126">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="ee3e5-126">Privileged authentication admin</span></span>
* <span data-ttu-id="ee3e5-127">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="ee3e5-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="ee3e5-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee3e5-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ee3e5-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee3e5-129">Request headers</span></span>
|<span data-ttu-id="ee3e5-130">Имя</span><span class="sxs-lookup"><span data-stu-id="ee3e5-130">Name</span></span>|<span data-ttu-id="ee3e5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ee3e5-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ee3e5-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee3e5-132">Authorization</span></span>|<span data-ttu-id="ee3e5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee3e5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee3e5-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee3e5-135">Request body</span></span>
<span data-ttu-id="ee3e5-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee3e5-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee3e5-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee3e5-137">Response</span></span>

<span data-ttu-id="ee3e5-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ee3e5-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee3e5-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="ee3e5-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee3e5-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee3e5-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ee3e5-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee3e5-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="ee3e5-143">C#</span><span class="sxs-lookup"><span data-stu-id="ee3e5-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee3e5-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee3e5-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee3e5-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee3e5-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee3e5-146">Java</span><span class="sxs-lookup"><span data-stu-id="ee3e5-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ee3e5-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee3e5-147">Response</span></span>
<span data-ttu-id="ee3e5-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ee3e5-148">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

