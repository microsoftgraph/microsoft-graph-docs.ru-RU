---
title: Список fido2AuthenticationMethod
description: Извлечение списка объектов fido2AuthenticationMethod и их свойств.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c9c735a12bba47baaddcfbed0359a3f794c473b8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964869"
---
# <a name="list-fido2authenticationmethod"></a><span data-ttu-id="26b15-103">Список fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="26b15-103">List fido2AuthenticationMethod</span></span>
<span data-ttu-id="26b15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26b15-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26b15-105">Извлечение списка объектов метода проверки подлинности [ключей безопасности FIDO2](../resources/fido2authenticationmethod.md) пользователя и их свойств.</span><span class="sxs-lookup"><span data-stu-id="26b15-105">Retrieve a list of a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="26b15-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26b15-106">Permissions</span></span>

<span data-ttu-id="26b15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26b15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="26b15-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="26b15-109">Permissions acting on self</span></span>

|<span data-ttu-id="26b15-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26b15-110">Permission type</span></span>      | <span data-ttu-id="26b15-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26b15-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="26b15-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26b15-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="26b15-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26b15-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="26b15-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26b15-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26b15-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26b15-115">Not supported.</span></span> |
| <span data-ttu-id="26b15-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26b15-116">Application</span></span>                            | <span data-ttu-id="26b15-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26b15-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="26b15-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="26b15-118">Permissions acting on other users</span></span>

|<span data-ttu-id="26b15-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26b15-119">Permission type</span></span>      | <span data-ttu-id="26b15-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26b15-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="26b15-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26b15-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="26b15-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b15-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="26b15-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26b15-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26b15-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26b15-124">Not supported.</span></span> |
| <span data-ttu-id="26b15-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26b15-125">Application</span></span>                            | <span data-ttu-id="26b15-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b15-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="26b15-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="26b15-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="26b15-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="26b15-128">Global admin</span></span>
* <span data-ttu-id="26b15-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="26b15-129">Global reader</span></span>
* <span data-ttu-id="26b15-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="26b15-130">Privileged authentication admin</span></span>
* <span data-ttu-id="26b15-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="26b15-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="26b15-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26b15-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/fido2Methods
GET /users/{id | userPrincipalName}/authentication/fido2Methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="26b15-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="26b15-133">Optional query parameters</span></span>
<span data-ttu-id="26b15-134">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="26b15-134">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26b15-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26b15-135">Request headers</span></span>
|<span data-ttu-id="26b15-136">Имя</span><span class="sxs-lookup"><span data-stu-id="26b15-136">Name</span></span>|<span data-ttu-id="26b15-137">Описание</span><span class="sxs-lookup"><span data-stu-id="26b15-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="26b15-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26b15-138">Authorization</span></span>|<span data-ttu-id="26b15-139">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="26b15-139">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="26b15-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="26b15-140">Request body</span></span>
<span data-ttu-id="26b15-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="26b15-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26b15-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b15-142">Response</span></span>

<span data-ttu-id="26b15-143">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="26b15-143">If successful, this method returns a `200 OK` response code and a collection of [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="26b15-144">Примеры</span><span class="sxs-lookup"><span data-stu-id="26b15-144">Examples</span></span>

### <a name="request"></a><span data-ttu-id="26b15-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="26b15-145">Request</span></span>


``` http
GET https://graph.microsoft.com/v1.0/me/authentication/fido2Methods
```

### <a name="response"></a><span data-ttu-id="26b15-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="26b15-146">Response</span></span>
<span data-ttu-id="26b15-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26b15-147">The following is an example of the response.</span></span>

<span data-ttu-id="26b15-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="26b15-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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

