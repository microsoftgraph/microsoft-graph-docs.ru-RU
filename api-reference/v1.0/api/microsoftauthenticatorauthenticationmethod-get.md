---
title: Get microsoftAuthenticatorAuthenticationMethod
description: Ознакомьтесь с свойствами и отношениями объекта MicrosoftAuthenticatorAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 828288f71a553c8ee6b7603b4af505c07dedf74d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202815"
---
# <a name="get-microsoftauthenticatorauthenticationmethod"></a><span data-ttu-id="6276c-103">Get microsoftAuthenticatorAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6276c-103">Get microsoftAuthenticatorAuthenticationMethod</span></span>
<span data-ttu-id="6276c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6276c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6276c-105">Ознакомьтесь с свойствами и отношениями объекта [MicrosoftAuthenticatorAuthenticationMethod.](../resources/microsoftauthenticatorauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="6276c-105">Read the properties and relationships of a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6276c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6276c-106">Permissions</span></span>

<span data-ttu-id="6276c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6276c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="6276c-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="6276c-109">Permissions acting on self</span></span>

|<span data-ttu-id="6276c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6276c-110">Permission type</span></span>      | <span data-ttu-id="6276c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6276c-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="6276c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6276c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6276c-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6276c-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="6276c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6276c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6276c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6276c-115">Not supported.</span></span> |
| <span data-ttu-id="6276c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6276c-116">Application</span></span>                            | <span data-ttu-id="6276c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6276c-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="6276c-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="6276c-118">Permissions acting on other users</span></span>

|<span data-ttu-id="6276c-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6276c-119">Permission type</span></span>      | <span data-ttu-id="6276c-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6276c-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="6276c-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6276c-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="6276c-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6276c-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="6276c-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6276c-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6276c-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6276c-124">Not supported.</span></span> |
| <span data-ttu-id="6276c-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6276c-125">Application</span></span>                            | <span data-ttu-id="6276c-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6276c-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="6276c-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="6276c-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="6276c-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6276c-128">Global admin</span></span>
* <span data-ttu-id="6276c-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="6276c-129">Global reader</span></span>
* <span data-ttu-id="6276c-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="6276c-130">Privileged authentication admin</span></span>
* <span data-ttu-id="6276c-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="6276c-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="6276c-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6276c-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods/{microsoftAuthenticatorAuthenticationMethodId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6276c-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6276c-133">Optional query parameters</span></span>
<span data-ttu-id="6276c-134">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="6276c-134">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6276c-135">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6276c-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6276c-136">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6276c-136">Request headers</span></span>
|<span data-ttu-id="6276c-137">Имя</span><span class="sxs-lookup"><span data-stu-id="6276c-137">Name</span></span>|<span data-ttu-id="6276c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="6276c-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6276c-139">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6276c-139">Authorization</span></span>|<span data-ttu-id="6276c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6276c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6276c-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6276c-142">Request body</span></span>
<span data-ttu-id="6276c-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6276c-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6276c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6276c-144">Response</span></span>

<span data-ttu-id="6276c-145">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект MicrosoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6276c-145">If successful, this method returns a `200 OK` response code and a [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6276c-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="6276c-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6276c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="6276c-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6276c-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="6276c-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/users/anirban@contoso.com/authentication/microsoftAuthenticatorMethods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="6276c-149">C#</span><span class="sxs-lookup"><span data-stu-id="6276c-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-microsoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6276c-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6276c-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-microsoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6276c-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6276c-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-microsoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6276c-152">Java</span><span class="sxs-lookup"><span data-stu-id="6276c-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-microsoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6276c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6276c-153">Response</span></span>
<span data-ttu-id="6276c-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6276c-154">**Note:** The response object shown here might be shortened for readability.</span></span>
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
