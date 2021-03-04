---
title: Список fido2AuthenticationMethod
description: Извлечение списка объектов fido2AuthenticationMethod и их свойств.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 57e63c083e75a84eff13ffc5094041224bdd43d7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436064"
---
# <a name="list-fido2authenticationmethod"></a><span data-ttu-id="16247-103">Список fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="16247-103">List fido2AuthenticationMethod</span></span>
<span data-ttu-id="16247-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16247-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16247-105">Извлечение списка объектов метода проверки подлинности [ключей безопасности FIDO2](../resources/fido2authenticationmethod.md) пользователя и их свойств.</span><span class="sxs-lookup"><span data-stu-id="16247-105">Retrieve a list of a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="16247-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="16247-106">Permissions</span></span>
<span data-ttu-id="16247-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16247-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16247-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16247-109">Permission type</span></span>|<span data-ttu-id="16247-110">Разрешения, действующие на себя (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="16247-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="16247-111">Разрешения, действующие на других (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="16247-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="16247-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16247-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="16247-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="16247-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="16247-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16247-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="16247-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16247-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16247-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16247-116">Not supported.</span></span> | <span data-ttu-id="16247-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16247-117">Not supported.</span></span> |
| <span data-ttu-id="16247-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="16247-118">Application</span></span>                            | <span data-ttu-id="16247-119">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="16247-119">Not applicable.</span></span> | <span data-ttu-id="16247-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16247-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="16247-121">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="16247-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="16247-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="16247-122">Global admin</span></span>
* <span data-ttu-id="16247-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="16247-123">Global reader</span></span>
* <span data-ttu-id="16247-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="16247-124">Privileged authentication admin</span></span>
* <span data-ttu-id="16247-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="16247-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="16247-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16247-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods
GET /users/{id | userPrincipalName}/authentication/fido2Methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="16247-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="16247-127">Optional query parameters</span></span>
<span data-ttu-id="16247-128">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="16247-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16247-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="16247-129">Request headers</span></span>
|<span data-ttu-id="16247-130">Имя</span><span class="sxs-lookup"><span data-stu-id="16247-130">Name</span></span>|<span data-ttu-id="16247-131">Описание</span><span class="sxs-lookup"><span data-stu-id="16247-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="16247-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="16247-132">Authorization</span></span>|<span data-ttu-id="16247-133">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="16247-133">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="16247-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="16247-134">Request body</span></span>
<span data-ttu-id="16247-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="16247-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16247-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="16247-136">Response</span></span>

<span data-ttu-id="16247-137">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="16247-137">If successful, this method returns a `200 OK` response code and a collection of [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="16247-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="16247-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="16247-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="16247-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="16247-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="16247-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2Methods
```
# <a name="c"></a>[<span data-ttu-id="16247-141">C#</span><span class="sxs-lookup"><span data-stu-id="16247-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="16247-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16247-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="16247-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="16247-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="16247-144">Java</span><span class="sxs-lookup"><span data-stu-id="16247-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="16247-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="16247-145">Response</span></span>
<span data-ttu-id="16247-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="16247-146">The following is an example of the response.</span></span>

<span data-ttu-id="16247-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="16247-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

