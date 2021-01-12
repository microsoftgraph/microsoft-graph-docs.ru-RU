---
title: Get emailAuthenticationMethod
description: Чтение свойств и связей объекта emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: edc1eaea88604887a51b8a2a6f527a1128865291
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796393"
---
# <a name="get-emailauthenticationmethod"></a><span data-ttu-id="83197-103">Get emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="83197-103">Get emailAuthenticationMethod</span></span>
<span data-ttu-id="83197-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83197-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83197-105">Получить один объект метода проверки [подлинности электронной почты](../resources/emailauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="83197-105">Retrieve a user's single [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="83197-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83197-106">Permissions</span></span>
<span data-ttu-id="83197-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83197-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83197-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83197-109">Permission type</span></span>|<span data-ttu-id="83197-110">Разрешения, действующие на себя (от большинства до наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="83197-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="83197-111">Разрешения, действующие над другими (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="83197-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="83197-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83197-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="83197-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="83197-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="83197-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83197-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="83197-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83197-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83197-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83197-116">Not supported.</span></span> | <span data-ttu-id="83197-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83197-117">Not supported.</span></span> |
| <span data-ttu-id="83197-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="83197-118">Application</span></span>                            | <span data-ttu-id="83197-119">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="83197-119">Not applicable.</span></span> | <span data-ttu-id="83197-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83197-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="83197-121">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="83197-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="83197-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="83197-122">Global admin</span></span>
* <span data-ttu-id="83197-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="83197-123">Global reader</span></span>
* <span data-ttu-id="83197-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="83197-124">Privileged authentication admin</span></span>
* <span data-ttu-id="83197-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="83197-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="83197-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83197-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods/{id}
GET /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="83197-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83197-127">Request headers</span></span>
|<span data-ttu-id="83197-128">Имя</span><span class="sxs-lookup"><span data-stu-id="83197-128">Name</span></span>|<span data-ttu-id="83197-129">Описание</span><span class="sxs-lookup"><span data-stu-id="83197-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="83197-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83197-130">Authorization</span></span>|<span data-ttu-id="83197-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83197-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="83197-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83197-133">Request body</span></span>
<span data-ttu-id="83197-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="83197-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83197-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="83197-135">Response</span></span>

<span data-ttu-id="83197-136">В случае успеха этот метод возвращает код отклика и объект `200 OK` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="83197-136">If successful, this method returns a `200 OK` response code and the requested [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="83197-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="83197-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="83197-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="83197-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="83197-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="83197-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="83197-140">C#</span><span class="sxs-lookup"><span data-stu-id="83197-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="83197-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="83197-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="83197-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="83197-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="83197-143">Java</span><span class="sxs-lookup"><span data-stu-id="83197-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="83197-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="83197-144">Response</span></span>
<span data-ttu-id="83197-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="83197-145">The following is an example of the response.</span></span>

<span data-ttu-id="83197-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="83197-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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

