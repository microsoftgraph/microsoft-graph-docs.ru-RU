---
title: Get microsoftAuthenticatorAuthenticationMethod
description: Ознакомьтесь с свойствами и отношениями объекта MicrosoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c912f3cf6dced6fc2f95c2e677515dc9bdc1f5ca
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335676"
---
# <a name="get-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="7581b-103">Get microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7581b-103">Get microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="7581b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7581b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7581b-105">Ознакомьтесь с свойствами и отношениями объекта [MicrosoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="7581b-105">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7581b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7581b-106">Permissions</span></span>

<span data-ttu-id="7581b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7581b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="7581b-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="7581b-109">Permissions acting on self</span></span>

|<span data-ttu-id="7581b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7581b-110">Permission type</span></span>      | <span data-ttu-id="7581b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7581b-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="7581b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7581b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7581b-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7581b-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="7581b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7581b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7581b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7581b-115">Not supported.</span></span> |
| <span data-ttu-id="7581b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7581b-116">Application</span></span>                            | <span data-ttu-id="7581b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7581b-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="7581b-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="7581b-118">Permissions acting on other users</span></span>

|<span data-ttu-id="7581b-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7581b-119">Permission type</span></span>      | <span data-ttu-id="7581b-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7581b-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="7581b-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7581b-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="7581b-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7581b-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="7581b-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7581b-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7581b-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7581b-124">Not supported.</span></span> |
| <span data-ttu-id="7581b-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7581b-125">Application</span></span>                            | <span data-ttu-id="7581b-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7581b-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="7581b-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="7581b-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="7581b-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="7581b-128">Global admin</span></span>
* <span data-ttu-id="7581b-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="7581b-129">Global reader</span></span>
* <span data-ttu-id="7581b-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="7581b-130">Privileged authentication admin</span></span>
* <span data-ttu-id="7581b-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="7581b-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="7581b-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7581b-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7581b-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7581b-133">Optional query parameters</span></span>
<span data-ttu-id="7581b-134">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7581b-134">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7581b-135">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7581b-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7581b-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7581b-136">Request headers</span></span>
|<span data-ttu-id="7581b-137">Имя</span><span class="sxs-lookup"><span data-stu-id="7581b-137">Name</span></span>|<span data-ttu-id="7581b-138">Описание</span><span class="sxs-lookup"><span data-stu-id="7581b-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7581b-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7581b-139">Authorization</span></span>|<span data-ttu-id="7581b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7581b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7581b-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7581b-142">Request body</span></span>
<span data-ttu-id="7581b-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7581b-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7581b-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="7581b-144">Response</span></span>

<span data-ttu-id="7581b-145">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект MicrosoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7581b-145">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7581b-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="7581b-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7581b-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="7581b-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7581b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="7581b-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="7581b-149">C#</span><span class="sxs-lookup"><span data-stu-id="7581b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-microsoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7581b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7581b-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-microsoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7581b-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7581b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-microsoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7581b-152">Java</span><span class="sxs-lookup"><span data-stu-id="7581b-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-microsoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7581b-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="7581b-153">Response</span></span>
<span data-ttu-id="7581b-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7581b-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftAuthenticatorAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
    "id": "6803c096-c096-6803-96c0-036896c00368",
    "displayName": "Sandeep's iPhone",
    "deviceTag": "",
    "phoneAppVersion": "6.5.4",
    "createdDateTime": "2020-12-03T23:16:12Z"
  }
}
```
