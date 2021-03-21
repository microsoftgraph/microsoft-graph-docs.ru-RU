---
title: Get fido2AuthenticationMethod
description: Ознакомьтесь с свойствами и отношениями объекта fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4b5bad06b344db8355b1c73c7bf7886517795027
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959240"
---
# <a name="get-fido2authenticationmethod"></a><span data-ttu-id="02f4a-103">Get fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="02f4a-103">Get fido2AuthenticationMethod</span></span>
<span data-ttu-id="02f4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02f4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02f4a-105">Извлечение единого объекта проверки подлинности [ключа безопасности FIDO2 пользователя.](../resources/fido2authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="02f4a-105">Retrieve a user's single [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02f4a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02f4a-106">Permissions</span></span>
<span data-ttu-id="02f4a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02f4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02f4a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02f4a-109">Permission type</span></span>|<span data-ttu-id="02f4a-110">Разрешения, действующие на себя (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="02f4a-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="02f4a-111">Разрешения, действующие на других (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="02f4a-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="02f4a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02f4a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="02f4a-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02f4a-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="02f4a-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02f4a-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="02f4a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02f4a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02f4a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02f4a-116">Not supported.</span></span> | <span data-ttu-id="02f4a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02f4a-117">Not supported.</span></span> |
| <span data-ttu-id="02f4a-118">Application</span><span class="sxs-lookup"><span data-stu-id="02f4a-118">Application</span></span>                            | <span data-ttu-id="02f4a-119">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="02f4a-119">Not applicable.</span></span> | <span data-ttu-id="02f4a-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02f4a-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="02f4a-121">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="02f4a-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="02f4a-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="02f4a-122">Global admin</span></span>
* <span data-ttu-id="02f4a-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="02f4a-123">Global reader</span></span>
* <span data-ttu-id="02f4a-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="02f4a-124">Privileged authentication admin</span></span>
* <span data-ttu-id="02f4a-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="02f4a-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="02f4a-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02f4a-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods/{id}
GET /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="02f4a-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02f4a-127">Request headers</span></span>
|<span data-ttu-id="02f4a-128">Имя</span><span class="sxs-lookup"><span data-stu-id="02f4a-128">Name</span></span>|<span data-ttu-id="02f4a-129">Описание</span><span class="sxs-lookup"><span data-stu-id="02f4a-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="02f4a-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02f4a-130">Authorization</span></span>|<span data-ttu-id="02f4a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02f4a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02f4a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02f4a-133">Request body</span></span>
<span data-ttu-id="02f4a-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02f4a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02f4a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="02f4a-135">Response</span></span>

<span data-ttu-id="02f4a-136">В случае успешной работы этот метод возвращает код ответа и запрашиваемого `200 OK` [объекта fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="02f4a-136">If successful, this method returns a `200 OK` response code and the requested [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02f4a-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="02f4a-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02f4a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="02f4a-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="02f4a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="02f4a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2Methods/-2_GRUg2-HYz6_1YG4YRAQ2
```
# <a name="c"></a>[<span data-ttu-id="02f4a-140">C#</span><span class="sxs-lookup"><span data-stu-id="02f4a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethod-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02f4a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02f4a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethod-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02f4a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02f4a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethod-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02f4a-143">Java</span><span class="sxs-lookup"><span data-stu-id="02f4a-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fido2authenticationmethod-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02f4a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="02f4a-144">Response</span></span>
<span data-ttu-id="02f4a-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="02f4a-145">The following is an example of the response.</span></span>

<span data-ttu-id="02f4a-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="02f4a-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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

