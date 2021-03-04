---
title: Список emailAuthenticationMethods
description: Получите список объектов emailAuthenticationMethod и их свойств.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 90e815be865619b7e6cb1874b0b6008620705ce8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436346"
---
# <a name="list-emailauthenticationmethods"></a><span data-ttu-id="cb00d-103">Список emailAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="cb00d-103">List emailAuthenticationMethods</span></span>
<span data-ttu-id="cb00d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb00d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb00d-105">Извлечение списка объектов [](../resources/emailauthenticationmethod.md) метода проверки подлинности электронной почты пользователя и их свойств.</span><span class="sxs-lookup"><span data-stu-id="cb00d-105">Retrieve a list of a user's [email Authentication Method](../resources/emailauthenticationmethod.md) objects and their properties.</span></span> <span data-ttu-id="cb00d-106">Этот вызов возвращает только один объект, так как для пользователей может быть заданной только один метод электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cb00d-106">This call will only return a single object as only one email method can be set on users.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb00d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb00d-107">Permissions</span></span>
<span data-ttu-id="cb00d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb00d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb00d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb00d-110">Permission type</span></span>|<span data-ttu-id="cb00d-111">Разрешения, действующие на себя (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="cb00d-111">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="cb00d-112">Разрешения, действующие на других (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="cb00d-112">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="cb00d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb00d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cb00d-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb00d-114">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="cb00d-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb00d-115">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="cb00d-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb00d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb00d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb00d-117">Not supported.</span></span> | <span data-ttu-id="cb00d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb00d-118">Not supported.</span></span> |
| <span data-ttu-id="cb00d-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="cb00d-119">Application</span></span>                            | <span data-ttu-id="cb00d-120">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="cb00d-120">Not applicable.</span></span> | <span data-ttu-id="cb00d-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb00d-121">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="cb00d-122">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="cb00d-122">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="cb00d-123">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="cb00d-123">Global admin</span></span>
* <span data-ttu-id="cb00d-124">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="cb00d-124">Global reader</span></span>
* <span data-ttu-id="cb00d-125">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="cb00d-125">Privileged authentication admin</span></span>
* <span data-ttu-id="cb00d-126">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="cb00d-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="cb00d-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb00d-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods
GET /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb00d-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cb00d-128">Optional query parameters</span></span>
<span data-ttu-id="cb00d-129">Этот метод не поддерживает необязательные параметры запроса для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cb00d-129">This method does not support optional query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb00d-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb00d-130">Request headers</span></span>
|<span data-ttu-id="cb00d-131">Имя</span><span class="sxs-lookup"><span data-stu-id="cb00d-131">Name</span></span>|<span data-ttu-id="cb00d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cb00d-132">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cb00d-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb00d-133">Authorization</span></span>|<span data-ttu-id="cb00d-134">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="cb00d-134">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb00d-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cb00d-135">Request body</span></span>
<span data-ttu-id="cb00d-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb00d-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb00d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb00d-137">Response</span></span>

<span data-ttu-id="cb00d-138">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cb00d-138">If successful, this method returns a `200 OK` response code and a collection of [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb00d-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="cb00d-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb00d-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb00d-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cb00d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb00d-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods
```
# <a name="c"></a>[<span data-ttu-id="cb00d-142">C#</span><span class="sxs-lookup"><span data-stu-id="cb00d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb00d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb00d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb00d-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb00d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb00d-145">Java</span><span class="sxs-lookup"><span data-stu-id="cb00d-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="cb00d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb00d-146">Response</span></span>
<span data-ttu-id="cb00d-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cb00d-147">The following is an example of the response.</span></span>

<span data-ttu-id="cb00d-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cb00d-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.emailAuthenticationMethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": [
    {
      "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
      "emailAddress": "Kim@contoso.com"
    }
  ]
}
```

