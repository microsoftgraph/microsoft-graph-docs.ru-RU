---
title: Список Пассвордлессмикрософтаусентикатораусентикатионмесодс
description: Получение списка объектов Пассвордлессмикрософтаусентикатораусентикатионмесод и их свойств.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ae837eb7938a1734f30402e24db31c96cb0f587
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968616"
---
# <a name="list-passwordlessmicrosoftauthenticatorauthenticationmethods"></a><span data-ttu-id="5a692-103">Список Пассвордлессмикрософтаусентикатораусентикатионмесодс</span><span class="sxs-lookup"><span data-stu-id="5a692-103">List passwordlessMicrosoftAuthenticatorAuthenticationMethods</span></span>
<span data-ttu-id="5a692-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a692-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a692-105">Получение списка объектов [методов входа без пароля пользователя (Майкрософт) для проверки подлинности](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) пользователя и их свойств.</span><span class="sxs-lookup"><span data-stu-id="5a692-105">Retrieve a list of a user's [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

> [!NOTE]
> <span data-ttu-id="5a692-106">Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии.</span><span class="sxs-lookup"><span data-stu-id="5a692-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="5a692-107">Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.</span><span class="sxs-lookup"><span data-stu-id="5a692-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a692-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a692-108">Permissions</span></span>
<span data-ttu-id="5a692-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a692-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a692-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a692-111">Permission type</span></span>|<span data-ttu-id="5a692-112">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a692-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="5a692-113">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="5a692-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="5a692-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a692-114">Delegated (work or school account)</span></span>|<span data-ttu-id="5a692-115">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5a692-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="5a692-116">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5a692-116">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="5a692-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a692-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a692-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a692-118">Not supported.</span></span>|<span data-ttu-id="5a692-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a692-119">Not supported.</span></span>
|<span data-ttu-id="5a692-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a692-120">Application</span></span>|<span data-ttu-id="5a692-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a692-121">Not supported.</span></span>|<span data-ttu-id="5a692-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a692-122">Not supported.</span></span>

<span data-ttu-id="5a692-123">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="5a692-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="5a692-124">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="5a692-124">Global admin</span></span>
* <span data-ttu-id="5a692-125">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="5a692-125">Global reader</span></span>
* <span data-ttu-id="5a692-126">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="5a692-126">Privileged authentication admin</span></span>
* <span data-ttu-id="5a692-127">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="5a692-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="5a692-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a692-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a692-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5a692-129">Optional query parameters</span></span>
<span data-ttu-id="5a692-130">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5a692-130">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5a692-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a692-131">Request headers</span></span>
|<span data-ttu-id="5a692-132">Имя</span><span class="sxs-lookup"><span data-stu-id="5a692-132">Name</span></span>|<span data-ttu-id="5a692-133">Описание</span><span class="sxs-lookup"><span data-stu-id="5a692-133">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5a692-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a692-134">Authorization</span></span>|<span data-ttu-id="5a692-135">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="5a692-135">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a692-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a692-136">Request body</span></span>
<span data-ttu-id="5a692-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5a692-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a692-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a692-138">Response</span></span>

<span data-ttu-id="5a692-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [пассвордлессмикрософтаусентикатораусентикатионмесод](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5a692-139">If successful, this method returns a `200 OK` response code and a collection of [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5a692-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="5a692-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5a692-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a692-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5a692-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a692-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods
```
# <a name="c"></a>[<span data-ttu-id="5a692-143">C#</span><span class="sxs-lookup"><span data-stu-id="5a692-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a692-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a692-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a692-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a692-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a692-146">Java</span><span class="sxs-lookup"><span data-stu-id="5a692-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-passwordlessmicrosoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5a692-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a692-147">Response</span></span>
<span data-ttu-id="5a692-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5a692-148">The following is an example of the response.</span></span>

<span data-ttu-id="5a692-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5a692-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1",
      "displayName": "My mobile phone",
      "creationDateTime": "2020-09-02T04:16:49Z"
    },
    {
      "id": "J18B378Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJGM1",
      "displayName": "My tablet",
      "creationDateTime": "2020-09-02T03:36:19Z"
    }
  ]
}
```

