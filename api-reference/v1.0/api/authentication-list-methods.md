---
title: Методы List
description: Извлечение списка объектов метода проверки подлинности.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e4dd76103f14daad826d78dfbf2dc5be6e333aa0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950242"
---
# <a name="list-methods"></a><span data-ttu-id="47c2f-103">Методы List</span><span class="sxs-lookup"><span data-stu-id="47c2f-103">List methods</span></span>

<span data-ttu-id="47c2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47c2f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47c2f-105">Извлечение списка объектов метода [проверки подлинности.](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="47c2f-105">Retrieve a list of [authentication method](../resources/authenticationmethod.md) objects.</span></span>

> <span data-ttu-id="47c2f-106">**Примечание:** Возвращаются только методы, поддерживаемые в v1.0.</span><span class="sxs-lookup"><span data-stu-id="47c2f-106">**Note:** Only methods supported on v1.0 will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="47c2f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47c2f-107">Permissions</span></span>

<span data-ttu-id="47c2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47c2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="47c2f-110">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="47c2f-110">Permissions acting on self</span></span>

|<span data-ttu-id="47c2f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47c2f-111">Permission type</span></span>      | <span data-ttu-id="47c2f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47c2f-112">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="47c2f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47c2f-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="47c2f-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47c2f-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="47c2f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47c2f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47c2f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47c2f-116">Not supported.</span></span> |
| <span data-ttu-id="47c2f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47c2f-117">Application</span></span>                            | <span data-ttu-id="47c2f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47c2f-118">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="47c2f-119">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="47c2f-119">Permissions acting on other users</span></span>

|<span data-ttu-id="47c2f-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47c2f-120">Permission type</span></span>      | <span data-ttu-id="47c2f-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47c2f-121">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="47c2f-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47c2f-122">Delegated (work or school account)</span></span>     | <span data-ttu-id="47c2f-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c2f-123">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="47c2f-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47c2f-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47c2f-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47c2f-125">Not supported.</span></span> |
| <span data-ttu-id="47c2f-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47c2f-126">Application</span></span>                            | <span data-ttu-id="47c2f-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c2f-127">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="47c2f-128">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="47c2f-128">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="47c2f-129">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="47c2f-129">Global admin</span></span>
* <span data-ttu-id="47c2f-130">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="47c2f-130">Global reader</span></span>
* <span data-ttu-id="47c2f-131">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="47c2f-131">Privileged authentication admin</span></span>
* <span data-ttu-id="47c2f-132">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="47c2f-132">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="47c2f-133">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47c2f-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id | userPrincipalName}/authentication/methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47c2f-134">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="47c2f-134">Optional query parameters</span></span>

<span data-ttu-id="47c2f-135">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="47c2f-135">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47c2f-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47c2f-136">Request headers</span></span>

| <span data-ttu-id="47c2f-137">Имя</span><span class="sxs-lookup"><span data-stu-id="47c2f-137">Name</span></span>      |<span data-ttu-id="47c2f-138">Описание</span><span class="sxs-lookup"><span data-stu-id="47c2f-138">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="47c2f-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47c2f-139">Authorization</span></span> | <span data-ttu-id="47c2f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47c2f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47c2f-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47c2f-142">Request body</span></span>

<span data-ttu-id="47c2f-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47c2f-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47c2f-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="47c2f-144">Response</span></span>

<span data-ttu-id="47c2f-145">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [authenticationMethod](../resources/authenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="47c2f-145">If successful, this method returns a `200 OK` response code and a collection of [authenticationMethod](../resources/authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47c2f-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="47c2f-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47c2f-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="47c2f-147">Request</span></span>

<span data-ttu-id="47c2f-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47c2f-148">The following is an example of the request.</span></span>


```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/authentication/methods
```

### <a name="response"></a><span data-ttu-id="47c2f-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="47c2f-149">Response</span></span>

<span data-ttu-id="47c2f-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47c2f-150">The following is an example of the response.</span></span>

> <span data-ttu-id="47c2f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47c2f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
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
    "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
    "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
    "displayName": "Jordan's Surface Book",
    "createdDateTime": "2020-11-27T23:12:49Z",
    "keyStrength": "normal"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List methods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
