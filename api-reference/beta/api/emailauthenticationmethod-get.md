---
title: Get emailAuthenticationMethod
description: Ознакомьтесь с свойствами и отношениями объекта emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 46189eb8bb465ea0e436e71fa3c9129094d3ece0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436350"
---
# <a name="get-emailauthenticationmethod"></a><span data-ttu-id="b26fa-103">Get emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b26fa-103">Get emailAuthenticationMethod</span></span>
<span data-ttu-id="b26fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b26fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b26fa-105">Извлечение одного объекта метода проверки подлинности [электронной почты.](../resources/emailauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b26fa-105">Retrieve a user's single [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b26fa-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b26fa-106">Permissions</span></span>
<span data-ttu-id="b26fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b26fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b26fa-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b26fa-109">Permission type</span></span>|<span data-ttu-id="b26fa-110">Разрешения, действующие на себя (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="b26fa-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="b26fa-111">Разрешения, действующие на других (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="b26fa-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="b26fa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b26fa-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b26fa-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b26fa-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="b26fa-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b26fa-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b26fa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b26fa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b26fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b26fa-116">Not supported.</span></span> | <span data-ttu-id="b26fa-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b26fa-117">Not supported.</span></span> |
| <span data-ttu-id="b26fa-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="b26fa-118">Application</span></span>                            | <span data-ttu-id="b26fa-119">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b26fa-119">Not applicable.</span></span> | <span data-ttu-id="b26fa-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b26fa-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b26fa-121">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="b26fa-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b26fa-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b26fa-122">Global admin</span></span>
* <span data-ttu-id="b26fa-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="b26fa-123">Global reader</span></span>
* <span data-ttu-id="b26fa-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b26fa-124">Privileged authentication admin</span></span>
* <span data-ttu-id="b26fa-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b26fa-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b26fa-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b26fa-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods/{id}
GET /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b26fa-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b26fa-127">Request headers</span></span>
|<span data-ttu-id="b26fa-128">Имя</span><span class="sxs-lookup"><span data-stu-id="b26fa-128">Name</span></span>|<span data-ttu-id="b26fa-129">Описание</span><span class="sxs-lookup"><span data-stu-id="b26fa-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b26fa-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b26fa-130">Authorization</span></span>|<span data-ttu-id="b26fa-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b26fa-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b26fa-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b26fa-133">Request body</span></span>
<span data-ttu-id="b26fa-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b26fa-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b26fa-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b26fa-135">Response</span></span>

<span data-ttu-id="b26fa-136">В случае успешной работы этот метод возвращает код ответа и запрашиваемого объекта `200 OK` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b26fa-136">If successful, this method returns a `200 OK` response code and the requested [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b26fa-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="b26fa-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b26fa-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b26fa-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b26fa-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b26fa-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="b26fa-140">C#</span><span class="sxs-lookup"><span data-stu-id="b26fa-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b26fa-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b26fa-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b26fa-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b26fa-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b26fa-143">Java</span><span class="sxs-lookup"><span data-stu-id="b26fa-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b26fa-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b26fa-144">Response</span></span>
<span data-ttu-id="b26fa-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b26fa-145">The following is an example of the response.</span></span>

<span data-ttu-id="b26fa-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b26fa-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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

