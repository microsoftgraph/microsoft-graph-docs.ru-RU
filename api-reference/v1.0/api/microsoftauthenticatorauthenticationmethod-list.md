---
title: Список microsoftAuthenticatorAuthenticationMethods
description: Получите список объектов MicrosoftAuthenticatorAuthenticationMethod и их свойств.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5538a954edb69793e693a8cce109e8088b4f5926
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202584"
---
# <a name="list-microsoftauthenticatorauthenticationmethods"></a><span data-ttu-id="ef208-103">Список microsoftAuthenticatorAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="ef208-103">List microsoftAuthenticatorAuthenticationMethods</span></span>
<span data-ttu-id="ef208-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef208-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ef208-105">Получите список объектов [MicrosoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="ef208-105">Get a list of the [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef208-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef208-106">Permissions</span></span>

<span data-ttu-id="ef208-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef208-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="ef208-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="ef208-109">Permissions acting on self</span></span>

|<span data-ttu-id="ef208-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef208-110">Permission type</span></span>      | <span data-ttu-id="ef208-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef208-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="ef208-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef208-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef208-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef208-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="ef208-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef208-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef208-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef208-115">Not supported.</span></span> |
| <span data-ttu-id="ef208-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef208-116">Application</span></span>                            | <span data-ttu-id="ef208-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef208-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="ef208-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="ef208-118">Permissions acting on other users</span></span>

|<span data-ttu-id="ef208-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef208-119">Permission type</span></span>      | <span data-ttu-id="ef208-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef208-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="ef208-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef208-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef208-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef208-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="ef208-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef208-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef208-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef208-124">Not supported.</span></span> |
| <span data-ttu-id="ef208-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef208-125">Application</span></span>                            | <span data-ttu-id="ef208-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef208-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="ef208-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="ef208-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="ef208-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ef208-128">Global admin</span></span>
* <span data-ttu-id="ef208-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="ef208-129">Global reader</span></span>
* <span data-ttu-id="ef208-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="ef208-130">Privileged authentication admin</span></span>
* <span data-ttu-id="ef208-131">Администратор проверки подлинности (видит только номера телефонов в масках)</span><span class="sxs-lookup"><span data-stu-id="ef208-131">Authentication admin (only sees masked phone numbers)</span></span>

## <a name="http-request"></a><span data-ttu-id="ef208-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef208-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/microsoftAuthenticatorMethods
GET /users/{id | userPrincipalName}/authentication/microsoftAuthenticatorMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ef208-133">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ef208-133">Optional query parameters</span></span>

<span data-ttu-id="ef208-134">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef208-134">Not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ef208-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef208-135">Request headers</span></span>

|<span data-ttu-id="ef208-136">Имя</span><span class="sxs-lookup"><span data-stu-id="ef208-136">Name</span></span>|<span data-ttu-id="ef208-137">Описание</span><span class="sxs-lookup"><span data-stu-id="ef208-137">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ef208-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef208-138">Authorization</span></span>|<span data-ttu-id="ef208-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef208-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef208-141">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef208-141">Request body</span></span>

<span data-ttu-id="ef208-142">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef208-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef208-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef208-143">Response</span></span>

<span data-ttu-id="ef208-144">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [MicrosoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ef208-144">If successful, this method returns a `200 OK` response code and a collection of [microsoftAuthenticatorAuthenticationMethod](../resources/microsoftauthenticatorauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ef208-145">Примеры</span><span class="sxs-lookup"><span data-stu-id="ef208-145">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ef208-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef208-146">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ef208-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef208-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_microsoftauthenticatorauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/users/sandeep@contoso.com/authentication/microsoftAuthenticatorMethods
```
# <a name="c"></a>[<span data-ttu-id="ef208-148">C#</span><span class="sxs-lookup"><span data-stu-id="ef208-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-microsoftauthenticatorauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef208-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef208-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-microsoftauthenticatorauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef208-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef208-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-microsoftauthenticatorauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef208-151">Java</span><span class="sxs-lookup"><span data-stu-id="ef208-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-microsoftauthenticatorauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ef208-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef208-152">Response</span></span>
<span data-ttu-id="ef208-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ef208-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.microsoftAuthenticatorAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftAuthenticatorAuthenticationMethod",
      "id": "6803c096-c096-6803-96c0-036896c00368",
      "displayName": "Sandeep's iPhone",
      "deviceTag": "",
      "phoneAppVersion": "6.5.4",
      "createdDateTime": "2020-12-03T23:16:12Z"
    }
  ]
}
```

