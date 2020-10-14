---
title: Получение Пассвордлессмикрософтаусентикатораусентикатионмесод
description: Чтение свойств и связей объекта Пассвордлессмикрософтаусентикатораусентикатионмесод.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1a92e7669df96efe69d8e793fc327a8c578ffcde
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457501"
---
# <a name="get-passwordlessmicrosoftauthenticatorauthenticationmethod"></a><span data-ttu-id="eacdf-103">Получение Пассвордлессмикрософтаусентикатораусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="eacdf-103">Get passwordlessMicrosoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="eacdf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eacdf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eacdf-105">Получение одного объекта [метода входа без пароля для проверки подлинности пользователя (Майкрософт)](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="eacdf-105">Retrieve a user's single [Microsoft Authenticator Passwordless Phone Sign-in method](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="eacdf-106">Существенные изменения схемы запланированы для API, которые управляют приложением для проверки подлинности (Майкрософт), а API в Мирософт Graph бета-версии.</span><span class="sxs-lookup"><span data-stu-id="eacdf-106">Substantial schema changes are planned for APIs that manage the Microsoft Authenticator app while the APIs are in Mirosoft Graph beta.</span></span> <span data-ttu-id="eacdf-107">Так как шаблоны звонков будут изменены, мы не рекомендуем задействовать производственную зависимость от этих API.</span><span class="sxs-lookup"><span data-stu-id="eacdf-107">Because the calling patterns will change, we recommend that you do not take a production dependency on these APIs.</span></span>

## <a name="permissions"></a><span data-ttu-id="eacdf-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eacdf-108">Permissions</span></span>
<span data-ttu-id="eacdf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eacdf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eacdf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eacdf-111">Permission type</span></span>|<span data-ttu-id="eacdf-112">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="eacdf-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="eacdf-113">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="eacdf-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="eacdf-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eacdf-114">Delegated (work or school account)</span></span>|<span data-ttu-id="eacdf-115">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="eacdf-115">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="eacdf-116">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="eacdf-116">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="eacdf-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eacdf-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eacdf-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eacdf-118">Not supported.</span></span>|<span data-ttu-id="eacdf-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eacdf-119">Not supported.</span></span>
|<span data-ttu-id="eacdf-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eacdf-120">Application</span></span>|<span data-ttu-id="eacdf-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eacdf-121">Not supported.</span></span>|<span data-ttu-id="eacdf-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eacdf-122">Not supported.</span></span>

<span data-ttu-id="eacdf-123">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="eacdf-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="eacdf-124">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="eacdf-124">Global admin</span></span>
* <span data-ttu-id="eacdf-125">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="eacdf-125">Global reader</span></span>
* <span data-ttu-id="eacdf-126">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="eacdf-126">Privileged authentication admin</span></span>
* <span data-ttu-id="eacdf-127">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="eacdf-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="eacdf-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eacdf-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
GET /users/{id | userPrincipalName}/authentication/passwordlessMicrosoftAuthenticatorMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eacdf-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eacdf-129">Request headers</span></span>
|<span data-ttu-id="eacdf-130">Имя</span><span class="sxs-lookup"><span data-stu-id="eacdf-130">Name</span></span>|<span data-ttu-id="eacdf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="eacdf-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eacdf-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eacdf-132">Authorization</span></span>|<span data-ttu-id="eacdf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eacdf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eacdf-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eacdf-135">Request body</span></span>
<span data-ttu-id="eacdf-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eacdf-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eacdf-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="eacdf-137">Response</span></span>

<span data-ttu-id="eacdf-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [пассвордлессмикрософтаусентикатораусентикатионмесод](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eacdf-138">If successful, this method returns a `200 OK` response code and the requested [passwordlessMicrosoftAuthenticatorAuthenticationMethod](../resources/passwordlessmicrosoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eacdf-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="eacdf-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eacdf-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="eacdf-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="eacdf-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="eacdf-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_passwordlessmicrosoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/passwordlessMicrosoftAuthenticatorMethods/R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1
```
# <a name="c"></a>[<span data-ttu-id="eacdf-142">C#</span><span class="sxs-lookup"><span data-stu-id="eacdf-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-passwordlessmicrosoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eacdf-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eacdf-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-passwordlessmicrosoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eacdf-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eacdf-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-passwordlessmicrosoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="eacdf-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="eacdf-145">Response</span></span>
<span data-ttu-id="eacdf-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="eacdf-146">The following is an example of the response.</span></span>

<span data-ttu-id="eacdf-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="eacdf-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "R18B3t8Ogh9XIOGmPt81d6p_KXJs1YTxfGgGqeVFJSM1",
      "displayName": "My mobile phone",
      "creationDateTime": "2020-09-02T04:16:49Z"
  }
}
```

