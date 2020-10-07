---
title: Методы List
description: Получение списка объектов метода проверки подлинности.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 56afff3a8ea1fd7bd2239edfb168598eb2a0bf26
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48372438"
---
# <a name="list-methods"></a><span data-ttu-id="d24c0-103">Методы List</span><span class="sxs-lookup"><span data-stu-id="d24c0-103">List methods</span></span>

<span data-ttu-id="d24c0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d24c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d24c0-105">Получение списка объектов [метода проверки подлинности](../resources/authenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="d24c0-105">Retrieve a list of [authentication method](../resources/authenticationmethod.md) objects.</span></span> <span data-ttu-id="d24c0-106">В настоящее время возвращаются объекты метода [проверки подлинности по телефону](../resources/phoneauthenticationmethod.md) и [метода проверки подлинности пароля](../resources/passwordauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="d24c0-106">Currently only [phone authentication method](../resources/phoneauthenticationmethod.md) and [password authentication method](../resources/passwordauthenticationmethod.md) objects are returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="d24c0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d24c0-107">Permissions</span></span>

<span data-ttu-id="d24c0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d24c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d24c0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d24c0-110">Permission type</span></span>                        | <span data-ttu-id="d24c0-111">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="d24c0-111">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="d24c0-112">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="d24c0-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="d24c0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d24c0-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d24c0-114">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d24c0-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="d24c0-115">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d24c0-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="d24c0-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d24c0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d24c0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d24c0-117">Not supported.</span></span> | <span data-ttu-id="d24c0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d24c0-118">Not supported.</span></span> |
| <span data-ttu-id="d24c0-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d24c0-119">Application</span></span>                            | <span data-ttu-id="d24c0-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d24c0-120">Not supported.</span></span> | <span data-ttu-id="d24c0-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d24c0-121">Not supported.</span></span> |

<span data-ttu-id="d24c0-122">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="d24c0-122">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="d24c0-123">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d24c0-123">Global admin</span></span>
* <span data-ttu-id="d24c0-124">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="d24c0-124">Global reader</span></span>
* <span data-ttu-id="d24c0-125">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="d24c0-125">Privileged authentication admin</span></span>
* <span data-ttu-id="d24c0-126">Администратор проверки подлинности (видит только скрытые номера телефонов)</span><span class="sxs-lookup"><span data-stu-id="d24c0-126">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="d24c0-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d24c0-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id}/authentication/methods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d24c0-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d24c0-128">Optional query parameters</span></span>

<span data-ttu-id="d24c0-129">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d24c0-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d24c0-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d24c0-130">Request headers</span></span>

| <span data-ttu-id="d24c0-131">Имя</span><span class="sxs-lookup"><span data-stu-id="d24c0-131">Name</span></span>      |<span data-ttu-id="d24c0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d24c0-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d24c0-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d24c0-133">Authorization</span></span> | <span data-ttu-id="d24c0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d24c0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d24c0-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d24c0-136">Request body</span></span>

<span data-ttu-id="d24c0-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d24c0-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d24c0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d24c0-138">Response</span></span>

<span data-ttu-id="d24c0-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [authenticationMethod](../resources/authenticationmethod.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d24c0-139">If successful, this method returns a `200 OK` response code and a collection of [authenticationMethod](../resources/authenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d24c0-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="d24c0-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d24c0-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="d24c0-141">Request</span></span>

<span data-ttu-id="d24c0-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d24c0-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d24c0-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d24c0-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_methods"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods
```
# <a name="c"></a>[<span data-ttu-id="d24c0-144">C#</span><span class="sxs-lookup"><span data-stu-id="d24c0-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-methods-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d24c0-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d24c0-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-methods-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d24c0-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d24c0-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-methods-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d24c0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="d24c0-147">Response</span></span>

<span data-ttu-id="d24c0-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d24c0-148">The following is an example of the response.</span></span>

> <span data-ttu-id="d24c0-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d24c0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "odata.type": "#microsoft.graph.passwordAuthenticationMethod",
      "id": "28c10230-6103-485e-b985-444c60001490",
      "password": null,
      "creationDateTime": null
    },
    {
      "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
      "id": "3179e48a-750b-4051-897c-87b9720928f7",
      "phoneNumber": "+1 2065555555",
      "authenticationPhoneType": "mobile",
      "smsSignInState": "ready"
    },
    {
      "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
      "id": "b6332ec1-7057-4abe-9331-3d72feddfe41",
      "phoneNumber": "+1 2065555556",
      "authenticationPhoneType": "alternateMobile",
      "smsSignInState": "notSupported"
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
