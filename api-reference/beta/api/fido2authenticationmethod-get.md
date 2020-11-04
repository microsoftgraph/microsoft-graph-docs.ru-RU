---
title: Получение fido2AuthenticationMethod
description: Чтение свойств и связей объекта fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2175bfbb0af1960fe64efacb47f34914ac553618
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904151"
---
# <a name="get-fido2authenticationmethod"></a><span data-ttu-id="7c040-103">Получение fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7c040-103">Get fido2AuthenticationMethod</span></span>
<span data-ttu-id="7c040-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c040-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c040-105">Получение объекта [метода проверки подлинности для одного FIDO2ного ключа безопасности](../resources/fido2authenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="7c040-105">Retrieve a user's single [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7c040-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c040-106">Permissions</span></span>
<span data-ttu-id="7c040-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c040-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c040-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c040-109">Permission type</span></span>|<span data-ttu-id="7c040-110">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c040-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="7c040-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="7c040-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="7c040-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c040-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c040-113">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7c040-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="7c040-114">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7c040-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="7c040-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c040-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c040-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c040-116">Not supported.</span></span>|<span data-ttu-id="7c040-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c040-117">Not supported.</span></span>
|<span data-ttu-id="7c040-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c040-118">Application</span></span>|<span data-ttu-id="7c040-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c040-119">Not supported.</span></span>|<span data-ttu-id="7c040-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c040-120">Not supported.</span></span>

<span data-ttu-id="7c040-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="7c040-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="7c040-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="7c040-122">Global admin</span></span>
* <span data-ttu-id="7c040-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="7c040-123">Global reader</span></span>
* <span data-ttu-id="7c040-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="7c040-124">Privileged authentication admin</span></span>
* <span data-ttu-id="7c040-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="7c040-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="7c040-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c040-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2AuthenticationMethod/{id}
GET /users/{id | userPrincipalName}/authentication/fido2AuthenticationMethod/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7c040-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7c040-127">Request headers</span></span>
|<span data-ttu-id="7c040-128">Имя</span><span class="sxs-lookup"><span data-stu-id="7c040-128">Name</span></span>|<span data-ttu-id="7c040-129">Описание</span><span class="sxs-lookup"><span data-stu-id="7c040-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7c040-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c040-130">Authorization</span></span>|<span data-ttu-id="7c040-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c040-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c040-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7c040-133">Request body</span></span>
<span data-ttu-id="7c040-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7c040-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c040-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c040-135">Response</span></span>

<span data-ttu-id="7c040-136">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c040-136">If successful, this method returns a `200 OK` response code and the requested [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7c040-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="7c040-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7c040-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c040-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7c040-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c040-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2AuthenticationMethod/-2_GRUg2-HYz6_1YG4YRAQ2
```
# <a name="c"></a>[<span data-ttu-id="7c040-140">C#</span><span class="sxs-lookup"><span data-stu-id="7c040-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c040-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c040-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c040-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c040-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7c040-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c040-143">Response</span></span>
<span data-ttu-id="7c040-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7c040-144">The following is an example of the response.</span></span>

<span data-ttu-id="7c040-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7c040-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fido2AuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "-2_GRUg2-HYz6_1YG4YRAQ2",
      "displayName": "Red key",
      "creationDateTime": "2020-08-10T06:44:09Z",
      "aaGuid": "2fc0579f-8113-47ea-b116-555a8db9202a",
      "model": "NFC key",
      "attestationCertificates": [
          "dbe793efdf1945e2df25d93653a1e8a3268a9075"
      ],
      "attestationLevel": "attested"
  }
}
```

