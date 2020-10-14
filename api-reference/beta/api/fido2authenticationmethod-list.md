---
title: Список fido2AuthenticationMethod
description: Получение списка объектов fido2AuthenticationMethod и их свойств.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad8a3d3c90299dcf72bb5103059420a4db4ec514
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458885"
---
# <a name="list-fido2authenticationmethod"></a><span data-ttu-id="bb295-103">Список fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="bb295-103">List fido2AuthenticationMethod</span></span>
<span data-ttu-id="bb295-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb295-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb295-105">Получение списка объектов [метода проверки подлинности FIDO2 для ключа безопасности](../resources/fido2authenticationmethod.md) пользователя и их свойств.</span><span class="sxs-lookup"><span data-stu-id="bb295-105">Retrieve a list of a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb295-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bb295-106">Permissions</span></span>
<span data-ttu-id="bb295-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb295-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb295-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb295-109">Permission type</span></span>|<span data-ttu-id="bb295-110">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb295-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="bb295-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="bb295-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="bb295-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb295-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb295-113">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bb295-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span>|<span data-ttu-id="bb295-114">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="bb295-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="bb295-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb295-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb295-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb295-116">Not supported.</span></span>|<span data-ttu-id="bb295-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb295-117">Not supported.</span></span>
|<span data-ttu-id="bb295-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb295-118">Application</span></span>|<span data-ttu-id="bb295-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb295-119">Not supported.</span></span>|<span data-ttu-id="bb295-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb295-120">Not supported.</span></span>

<span data-ttu-id="bb295-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="bb295-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="bb295-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="bb295-122">Global admin</span></span>
* <span data-ttu-id="bb295-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="bb295-123">Global reader</span></span>
* <span data-ttu-id="bb295-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="bb295-124">Privileged authentication admin</span></span>
* <span data-ttu-id="bb295-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="bb295-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="bb295-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb295-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods
GET /users/{id | userPrincipalName}/authentication/fido2Methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bb295-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bb295-127">Optional query parameters</span></span>
<span data-ttu-id="bb295-128">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bb295-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb295-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb295-129">Request headers</span></span>
|<span data-ttu-id="bb295-130">Имя</span><span class="sxs-lookup"><span data-stu-id="bb295-130">Name</span></span>|<span data-ttu-id="bb295-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bb295-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bb295-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bb295-132">Authorization</span></span>|<span data-ttu-id="bb295-133">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="bb295-133">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb295-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb295-134">Request body</span></span>
<span data-ttu-id="bb295-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bb295-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb295-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb295-136">Response</span></span>

<span data-ttu-id="bb295-137">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb295-137">If successful, this method returns a `200 OK` response code and a collection of [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bb295-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="bb295-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb295-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb295-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="bb295-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb295-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2Methods
```
# <a name="c"></a>[<span data-ttu-id="bb295-141">C#</span><span class="sxs-lookup"><span data-stu-id="bb295-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb295-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb295-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb295-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb295-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="bb295-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb295-144">Response</span></span>
<span data-ttu-id="bb295-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bb295-145">The following is an example of the response.</span></span>

<span data-ttu-id="bb295-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bb295-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.fido2AuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "-2_GRUg2-HYz6_1YG4YRAQ2",
      "displayName": "Red key",
      "creationDateTime": "2020-08-10T06:44:09Z",
      "aaGuid": "2fc0579f-8113-47ea-b116-555a8db9202a",
      "model": "NFC key",
      "attestationCertificates": [
          "dbe793efdf1945e2df25d93653a1e8a3268a9075"
      ],
      "attestationLevel": "attested"
    },
    {
      "id": "_jpuR-TGZgk6aQCLF3BQjA2",
      "displayName": "Blue key",
      "creationDateTime": "2020-08-10T06:25:38Z",
      "aaGuid": "c5ef55ff-ad9a-4b9f-b580-ababafe026d0",
      "model": "USB key",
      "attestationCertificates": [
          "b479e7652167f574296e76bfa76731b8ccd22ed7"
      ],
      "attestationLevel": "attested"
    }
  ]
}
```

