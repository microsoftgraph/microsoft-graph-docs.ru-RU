---
title: Get fido2AuthenticationMethod
description: Чтение свойств и связей объекта fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 86dad6ea65abfe66491096148e55a0bac5806b88
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291918"
---
# <a name="get-fido2authenticationmethod"></a><span data-ttu-id="b92ca-103">Get fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b92ca-103">Get fido2AuthenticationMethod</span></span>
<span data-ttu-id="b92ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b92ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b92ca-105">Получить один объект метода проверки подлинности ключа безопасности [FIDO2](../resources/fido2authenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="b92ca-105">Retrieve a user's single [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b92ca-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b92ca-106">Permissions</span></span>
<span data-ttu-id="b92ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b92ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b92ca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b92ca-109">Permission type</span></span>|<span data-ttu-id="b92ca-110">Разрешения, действующие на себя (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="b92ca-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="b92ca-111">Разрешения, действующие над другими (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="b92ca-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="b92ca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b92ca-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b92ca-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b92ca-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="b92ca-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b92ca-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b92ca-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b92ca-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b92ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b92ca-116">Not supported.</span></span> | <span data-ttu-id="b92ca-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b92ca-117">Not supported.</span></span> |
| <span data-ttu-id="b92ca-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b92ca-118">Application</span></span>                            | <span data-ttu-id="b92ca-119">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b92ca-119">Not applicable.</span></span> | <span data-ttu-id="b92ca-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b92ca-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b92ca-121">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="b92ca-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b92ca-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b92ca-122">Global admin</span></span>
* <span data-ttu-id="b92ca-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="b92ca-123">Global reader</span></span>
* <span data-ttu-id="b92ca-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b92ca-124">Privileged authentication admin</span></span>
* <span data-ttu-id="b92ca-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b92ca-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b92ca-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b92ca-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods/{id}
GET /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b92ca-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b92ca-127">Request headers</span></span>
|<span data-ttu-id="b92ca-128">Имя</span><span class="sxs-lookup"><span data-stu-id="b92ca-128">Name</span></span>|<span data-ttu-id="b92ca-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b92ca-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b92ca-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b92ca-130">Authorization</span></span>|<span data-ttu-id="b92ca-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b92ca-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b92ca-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b92ca-133">Request body</span></span>
<span data-ttu-id="b92ca-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b92ca-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b92ca-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b92ca-135">Response</span></span>

<span data-ttu-id="b92ca-136">В случае успеха этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b92ca-136">If successful, this method returns a `200 OK` response code and the requested [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b92ca-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="b92ca-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b92ca-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b92ca-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_fido2authenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/fido2Methods/-2_GRUg2-HYz6_1YG4YRAQ2
```

### <a name="response"></a><span data-ttu-id="b92ca-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="b92ca-139">Response</span></span>
<span data-ttu-id="b92ca-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b92ca-140">The following is an example of the response.</span></span>

<span data-ttu-id="b92ca-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b92ca-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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

