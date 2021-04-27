---
title: Get temporaryAccessPassAuthenticationMethod
description: Ознакомьтесь с свойствами и отношениями объекта temporaryAccessPassAuthenticationMethod.
author: inbarckMS
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ccaa0d574c2fb2261c8cb0e0e0091473ec389f1f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049676"
---
# <a name="get-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="55290-103">Get temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="55290-103">Get temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="55290-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55290-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55290-105">Извлечение отдельного объекта [temporaryAccessPassAuthenticationMethod.](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="55290-105">Retrieve a user's single  [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="55290-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="55290-106">Permissions</span></span>
<span data-ttu-id="55290-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55290-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="55290-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="55290-109">Permissions acting on self</span></span>

|<span data-ttu-id="55290-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55290-110">Permission type</span></span>      | <span data-ttu-id="55290-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55290-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="55290-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55290-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="55290-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55290-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="55290-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55290-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55290-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55290-115">Not supported.</span></span> |
| <span data-ttu-id="55290-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55290-116">Application</span></span>                            | <span data-ttu-id="55290-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55290-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="55290-118">Разрешения, действующие на других пользователей</span><span class="sxs-lookup"><span data-stu-id="55290-118">Permissions acting on other users</span></span>

|<span data-ttu-id="55290-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55290-119">Permission type</span></span>      | <span data-ttu-id="55290-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="55290-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="55290-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55290-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="55290-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55290-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="55290-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55290-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55290-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55290-124">Not supported.</span></span> |
| <span data-ttu-id="55290-125">Приложение</span><span class="sxs-lookup"><span data-stu-id="55290-125">Application</span></span>                            | <span data-ttu-id="55290-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55290-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="55290-127">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="55290-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="55290-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="55290-128">Global admin</span></span>
* <span data-ttu-id="55290-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="55290-129">Global reader</span></span>
* <span data-ttu-id="55290-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="55290-130">Privileged authentication admin</span></span>
* <span data-ttu-id="55290-131">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="55290-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="55290-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55290-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
```


## <a name="request-headers"></a><span data-ttu-id="55290-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="55290-133">Request headers</span></span>
|<span data-ttu-id="55290-134">Имя</span><span class="sxs-lookup"><span data-stu-id="55290-134">Name</span></span>|<span data-ttu-id="55290-135">Описание</span><span class="sxs-lookup"><span data-stu-id="55290-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="55290-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="55290-136">Authorization</span></span>|<span data-ttu-id="55290-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55290-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="55290-139">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="55290-139">Request body</span></span>
<span data-ttu-id="55290-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="55290-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55290-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="55290-141">Response</span></span>

<span data-ttu-id="55290-142">В случае успешной работы этот метод возвращает код ответа и временный `200 OK` [объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="55290-142">If successful, this method returns a `200 OK` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55290-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="55290-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="55290-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="55290-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="55290-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="55290-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30
```
# <a name="c"></a>[<span data-ttu-id="55290-146">C#</span><span class="sxs-lookup"><span data-stu-id="55290-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-temporaryaccesspassauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="55290-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="55290-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-temporaryaccesspassauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="55290-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="55290-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-temporaryaccesspassauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="55290-149">Java</span><span class="sxs-lookup"><span data-stu-id="55290-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-temporaryaccesspassauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="55290-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="55290-150">Response</span></span>
<span data-ttu-id="55290-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="55290-151">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30",
    "temporaryAccessPass": null,
    "createdDateTime": "String (timestamp)",
    "startDateTime": "String (timestamp)",
    "lifetimeInMinutes": "Integer",
    "isUsableOnce": "Boolean",
    "isUsable": "Boolean",
    "methodUsabilityReason": "String"
  }
}
```
