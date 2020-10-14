---
title: Список Емаилаусентикатионмесодс
description: Получение списка объектов Емаилаусентикатионмесод и их свойств.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 254b25eec440ba8502293fdb7e51d6377e53b863
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458187"
---
# <a name="list-emailauthenticationmethods"></a><span data-ttu-id="98e35-103">Список Емаилаусентикатионмесодс</span><span class="sxs-lookup"><span data-stu-id="98e35-103">List emailAuthenticationMethods</span></span>
<span data-ttu-id="98e35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98e35-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98e35-105">Получение списка объектов [метода проверки подлинности электронной почты](../resources/emailauthenticationmethod.md) пользователя и их свойств.</span><span class="sxs-lookup"><span data-stu-id="98e35-105">Retrieve a list of a user's [email Authentication Method](../resources/emailauthenticationmethod.md) objects and their properties.</span></span> <span data-ttu-id="98e35-106">Этот вызов будет возвращать только один объект, так как для пользователей можно задать только один метод электронной почты.</span><span class="sxs-lookup"><span data-stu-id="98e35-106">This call will only return a single object as only one email method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="98e35-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98e35-107">Permissions</span></span>
<span data-ttu-id="98e35-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98e35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98e35-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98e35-110">Permission type</span></span>|<span data-ttu-id="98e35-111">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="98e35-111">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="98e35-112">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="98e35-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="98e35-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98e35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98e35-114">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="98e35-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="98e35-115">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="98e35-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="98e35-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98e35-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98e35-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98e35-117">Not supported.</span></span>|<span data-ttu-id="98e35-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98e35-118">Not supported.</span></span>
|<span data-ttu-id="98e35-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98e35-119">Application</span></span>|<span data-ttu-id="98e35-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98e35-120">Not supported.</span></span>|<span data-ttu-id="98e35-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98e35-121">Not supported.</span></span>

<span data-ttu-id="98e35-122">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="98e35-122">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="98e35-123">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="98e35-123">Global admin</span></span>
* <span data-ttu-id="98e35-124">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="98e35-124">Global reader</span></span>
* <span data-ttu-id="98e35-125">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="98e35-125">Privileged authentication admin</span></span>
* <span data-ttu-id="98e35-126">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="98e35-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="98e35-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98e35-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods
GET /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98e35-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98e35-128">Optional query parameters</span></span>
<span data-ttu-id="98e35-129">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="98e35-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98e35-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98e35-130">Request headers</span></span>
|<span data-ttu-id="98e35-131">Имя</span><span class="sxs-lookup"><span data-stu-id="98e35-131">Name</span></span>|<span data-ttu-id="98e35-132">Описание</span><span class="sxs-lookup"><span data-stu-id="98e35-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="98e35-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98e35-133">Authorization</span></span>|<span data-ttu-id="98e35-134">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="98e35-134">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="98e35-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98e35-135">Request body</span></span>
<span data-ttu-id="98e35-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98e35-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98e35-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="98e35-137">Response</span></span>

<span data-ttu-id="98e35-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98e35-138">If successful, this method returns a `200 OK` response code and a collection of [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="98e35-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="98e35-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="98e35-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="98e35-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="98e35-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="98e35-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods
```
# <a name="c"></a>[<span data-ttu-id="98e35-142">C#</span><span class="sxs-lookup"><span data-stu-id="98e35-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98e35-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98e35-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98e35-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98e35-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="98e35-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="98e35-145">Response</span></span>
<span data-ttu-id="98e35-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="98e35-146">The following is an example of the response.</span></span>

<span data-ttu-id="98e35-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="98e35-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.emailAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
      "emailAddress": "Kim@contoso.com"
    }
  ]
}
```

