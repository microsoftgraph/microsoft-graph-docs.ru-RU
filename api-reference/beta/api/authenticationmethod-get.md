---
title: Получение параметра authenticationMethod
description: Получение свойств и связей объекта authenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e0847447d3559c2e4bbee77ef4096de0762b5bcd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961352"
---
# <a name="get-authenticationmethod"></a><span data-ttu-id="0b416-103">Получение параметра authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0b416-103">Get authenticationMethod</span></span>

<span data-ttu-id="0b416-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b416-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b416-105">Получение свойств и связей объекта [authenticationMethod](../resources/authenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="0b416-105">Retrieve the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b416-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0b416-106">Permissions</span></span>

<span data-ttu-id="0b416-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b416-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b416-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b416-109">Permission type</span></span>                        | <span data-ttu-id="0b416-110">Разрешения, действующие на себя (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="0b416-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="0b416-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="0b416-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="0b416-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b416-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b416-113">Усераусентикатионмесод. Read, Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0b416-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite, UserAuthenticationMethod.ReadWrite.All</span></span> | <span data-ttu-id="0b416-114">Усераусентикатионмесод. Read. ALL, Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0b416-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="0b416-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b416-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b416-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b416-116">Not supported.</span></span> | <span data-ttu-id="0b416-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b416-117">Not supported.</span></span> |
| <span data-ttu-id="0b416-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b416-118">Application</span></span>                            | <span data-ttu-id="0b416-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b416-119">Not supported.</span></span> | <span data-ttu-id="0b416-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b416-120">Not supported.</span></span> |

<span data-ttu-id="0b416-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="0b416-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="0b416-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0b416-122">Global admin</span></span>
* <span data-ttu-id="0b416-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="0b416-123">Global reader</span></span>
* <span data-ttu-id="0b416-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="0b416-124">Privileged authentication admin</span></span>
* <span data-ttu-id="0b416-125">Администратор проверки подлинности (видит только скрытые номера телефонов)</span><span class="sxs-lookup"><span data-stu-id="0b416-125">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="0b416-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b416-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods/{id}
GET /users/{id | userPrincipalName}/authentication/methods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b416-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0b416-127">Optional query parameters</span></span>

<span data-ttu-id="0b416-128">Этот метод не поддерживает дополнительные параметры запроса для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0b416-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b416-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b416-129">Request headers</span></span>

| <span data-ttu-id="0b416-130">Имя</span><span class="sxs-lookup"><span data-stu-id="0b416-130">Name</span></span>      |<span data-ttu-id="0b416-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0b416-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0b416-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b416-132">Authorization</span></span> | <span data-ttu-id="0b416-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0b416-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b416-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0b416-135">Request body</span></span>

<span data-ttu-id="0b416-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0b416-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b416-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b416-137">Response</span></span>

<span data-ttu-id="0b416-138">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [authenticationMethod](../resources/authenticationmethod.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0b416-138">If successful, this method returns a `200 OK` response code and the requested [authenticationMethod](../resources/authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b416-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="0b416-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b416-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b416-140">Request</span></span>

<span data-ttu-id="0b416-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b416-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b416-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b416-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods/{id}
```
# <a name="c"></a>[<span data-ttu-id="0b416-143">C#</span><span class="sxs-lookup"><span data-stu-id="0b416-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b416-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b416-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b416-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b416-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b416-146">Java</span><span class="sxs-lookup"><span data-stu-id="0b416-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0b416-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b416-147">Response</span></span>

<span data-ttu-id="0b416-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0b416-148">The following is an example of the response.</span></span>

> <span data-ttu-id="0b416-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0b416-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "odata.type": "#microsoft.graph.phoneAuthenticationMethod",
  "id": "3179e48a-750b-4051-897c-87b9720928f7",
  "phoneNumber": "+1 2065555555",
  "authenticationPhoneType": "mobile",
  "smsSignInState": "ready"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get authenticationMethod",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
