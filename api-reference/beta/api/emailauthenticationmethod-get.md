---
title: Get emailAuthenticationMethod
description: Ознакомьтесь с свойствами и отношениями объекта emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3e5e8f4b4de1ab3bbbd82bade81b98c480295d9c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951018"
---
# <a name="get-emailauthenticationmethod"></a><span data-ttu-id="f836a-103">Get emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f836a-103">Get emailAuthenticationMethod</span></span>
<span data-ttu-id="f836a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f836a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f836a-105">Извлечение одного объекта метода проверки подлинности [электронной почты.](../resources/emailauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="f836a-105">Retrieve a user's single [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f836a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f836a-106">Permissions</span></span>
<span data-ttu-id="f836a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f836a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f836a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f836a-109">Permission type</span></span>|<span data-ttu-id="f836a-110">Разрешения, действующие на себя (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="f836a-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="f836a-111">Разрешения, действующие на других (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="f836a-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="f836a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f836a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f836a-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f836a-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="f836a-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f836a-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="f836a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f836a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f836a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f836a-116">Not supported.</span></span> | <span data-ttu-id="f836a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f836a-117">Not supported.</span></span> |
| <span data-ttu-id="f836a-118">Application</span><span class="sxs-lookup"><span data-stu-id="f836a-118">Application</span></span>                            | <span data-ttu-id="f836a-119">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="f836a-119">Not applicable.</span></span> | <span data-ttu-id="f836a-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f836a-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="f836a-121">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="f836a-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="f836a-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f836a-122">Global admin</span></span>
* <span data-ttu-id="f836a-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="f836a-123">Global reader</span></span>
* <span data-ttu-id="f836a-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="f836a-124">Privileged authentication admin</span></span>
* <span data-ttu-id="f836a-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="f836a-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="f836a-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f836a-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods/{id}
GET /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f836a-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f836a-127">Request headers</span></span>
|<span data-ttu-id="f836a-128">Имя</span><span class="sxs-lookup"><span data-stu-id="f836a-128">Name</span></span>|<span data-ttu-id="f836a-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f836a-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f836a-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f836a-130">Authorization</span></span>|<span data-ttu-id="f836a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f836a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f836a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f836a-133">Request body</span></span>
<span data-ttu-id="f836a-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f836a-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f836a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="f836a-135">Response</span></span>

<span data-ttu-id="f836a-136">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f836a-136">If successful, this method returns a `200 OK` response code and the requested [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f836a-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="f836a-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f836a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f836a-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f836a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="f836a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="f836a-140">C#</span><span class="sxs-lookup"><span data-stu-id="f836a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f836a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f836a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f836a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f836a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f836a-143">Java</span><span class="sxs-lookup"><span data-stu-id="f836a-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethod-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f836a-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="f836a-144">Response</span></span>
<span data-ttu-id="f836a-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f836a-145">The following is an example of the response.</span></span>

<span data-ttu-id="f836a-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f836a-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "value": {
      "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
      "emailAddress": "Kim@contoso.com"
  }
}
```

