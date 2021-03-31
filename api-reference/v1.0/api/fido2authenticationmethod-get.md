---
title: Get fido2AuthenticationMethod
description: Ознакомьтесь с свойствами и отношениями объекта fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b641e1c2afdbf01a3999c50f76497ac7a1417382
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51467962"
---
# <a name="get-fido2authenticationmethod"></a><span data-ttu-id="75dd8-103">Get fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="75dd8-103">Get fido2AuthenticationMethod</span></span>
<span data-ttu-id="75dd8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75dd8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75dd8-105">Извлечение единого объекта проверки подлинности [ключа безопасности FIDO2 пользователя.](../resources/fido2authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="75dd8-105">Retrieve a user's single [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="75dd8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="75dd8-106">Permissions</span></span>

<span data-ttu-id="75dd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75dd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="75dd8-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="75dd8-109">Permissions acting on self</span></span>

|<span data-ttu-id="75dd8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75dd8-110">Permission type</span></span>      | <span data-ttu-id="75dd8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75dd8-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="75dd8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75dd8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="75dd8-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="75dd8-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="75dd8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75dd8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75dd8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75dd8-115">Not supported.</span></span> |
| <span data-ttu-id="75dd8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75dd8-116">Application</span></span>                            | <span data-ttu-id="75dd8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75dd8-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="75dd8-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="75dd8-118">Permissions acting on other users</span></span>

|<span data-ttu-id="75dd8-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75dd8-119">Permission type</span></span>      | <span data-ttu-id="75dd8-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="75dd8-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="75dd8-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75dd8-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="75dd8-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75dd8-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="75dd8-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75dd8-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75dd8-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75dd8-124">Not supported.</span></span> |
| <span data-ttu-id="75dd8-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="75dd8-125">Application</span></span>                            | <span data-ttu-id="75dd8-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75dd8-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="75dd8-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="75dd8-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="75dd8-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="75dd8-128">Global admin</span></span>
* <span data-ttu-id="75dd8-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="75dd8-129">Global reader</span></span>
* <span data-ttu-id="75dd8-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="75dd8-130">Privileged authentication admin</span></span>
* <span data-ttu-id="75dd8-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="75dd8-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="75dd8-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75dd8-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2AuthenticationMethod/{id}
GET /users/{id | userPrincipalName}/authentication/fido2AuthenticationMethod/{id}
```

## <a name="request-headers"></a><span data-ttu-id="75dd8-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75dd8-133">Request headers</span></span>
|<span data-ttu-id="75dd8-134">Имя</span><span class="sxs-lookup"><span data-stu-id="75dd8-134">Name</span></span>|<span data-ttu-id="75dd8-135">Описание</span><span class="sxs-lookup"><span data-stu-id="75dd8-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="75dd8-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75dd8-136">Authorization</span></span>|<span data-ttu-id="75dd8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75dd8-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75dd8-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75dd8-139">Request body</span></span>
<span data-ttu-id="75dd8-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="75dd8-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75dd8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="75dd8-141">Response</span></span>

<span data-ttu-id="75dd8-142">В случае успешной работы этот метод возвращает код ответа и запрашиваемого `200 OK` [объекта fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="75dd8-142">If successful, this method returns a `200 OK` response code and the requested [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="75dd8-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="75dd8-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="75dd8-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="75dd8-144">Request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/me/authentication/fido2AuthenticationMethod/-2_GRUg2-HYz6_1YG4YRAQ2
```

### <a name="response"></a><span data-ttu-id="75dd8-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="75dd8-145">Response</span></span>
<span data-ttu-id="75dd8-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="75dd8-146">The following is an example of the response.</span></span>

<span data-ttu-id="75dd8-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75dd8-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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

