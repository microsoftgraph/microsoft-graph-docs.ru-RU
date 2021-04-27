---
title: Получить проверку подлинностиMethod
description: Извлечение свойств и связей объекта authenticationMethod.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 7311b1257311a21c70aed08fb86336eba970c95d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047975"
---
# <a name="get-authenticationmethod"></a><span data-ttu-id="ec345-103">Получить проверку подлинностиMethod</span><span class="sxs-lookup"><span data-stu-id="ec345-103">Get authenticationMethod</span></span>

<span data-ttu-id="ec345-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec345-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec345-105">Извлечение свойств и связей объекта [authenticationMethod.](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="ec345-105">Retrieve the properties and relationships of an [authenticationMethod](../resources/authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec345-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ec345-106">Permissions</span></span>

<span data-ttu-id="ec345-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec345-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec345-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ec345-109">Permission type</span></span>                        | <span data-ttu-id="ec345-110">Разрешения, действующие на себя (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="ec345-110">Permissions acting on self (from least to most privileged)</span></span> | <span data-ttu-id="ec345-111">Разрешения, действующие на других (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="ec345-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="ec345-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ec345-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec345-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec345-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="ec345-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec345-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="ec345-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ec345-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec345-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec345-116">Not supported.</span></span> | <span data-ttu-id="ec345-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec345-117">Not supported.</span></span> |
| <span data-ttu-id="ec345-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="ec345-118">Application</span></span>                            | <span data-ttu-id="ec345-119">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="ec345-119">Not applicable.</span></span> | <span data-ttu-id="ec345-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec345-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="ec345-121">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="ec345-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="ec345-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ec345-122">Global admin</span></span>
* <span data-ttu-id="ec345-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="ec345-123">Global reader</span></span>
* <span data-ttu-id="ec345-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="ec345-124">Privileged authentication admin</span></span>
* <span data-ttu-id="ec345-125">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="ec345-125">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="ec345-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ec345-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods/{id}
GET /users/{id | userPrincipalName}/authentication/methods/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec345-127">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ec345-127">Optional query parameters</span></span>

<span data-ttu-id="ec345-128">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ec345-128">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec345-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ec345-129">Request headers</span></span>

| <span data-ttu-id="ec345-130">Имя</span><span class="sxs-lookup"><span data-stu-id="ec345-130">Name</span></span>      |<span data-ttu-id="ec345-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ec345-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec345-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ec345-132">Authorization</span></span> | <span data-ttu-id="ec345-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ec345-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec345-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ec345-135">Request body</span></span>

<span data-ttu-id="ec345-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ec345-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec345-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec345-137">Response</span></span>

<span data-ttu-id="ec345-138">В случае успешной работы этот метод возвращает код ответа и запрашиваемую проверку `200 OK` [подлинностиMethod](../resources/authenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ec345-138">If successful, this method returns a `200 OK` response code and the requested [authenticationMethod](../resources/authenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec345-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="ec345-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ec345-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="ec345-140">Request</span></span>

<span data-ttu-id="ec345-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ec345-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ec345-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec345-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/authentication/methods/{id}
```
# <a name="c"></a>[<span data-ttu-id="ec345-143">C#</span><span class="sxs-lookup"><span data-stu-id="ec345-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ec345-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec345-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ec345-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec345-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ec345-146">Java</span><span class="sxs-lookup"><span data-stu-id="ec345-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec345-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ec345-147">Response</span></span>

<span data-ttu-id="ec345-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ec345-148">The following is an example of the response.</span></span>

> <span data-ttu-id="ec345-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ec345-149">**Note:** The response object shown here might be shortened for readability.</span></span>

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
