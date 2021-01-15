---
title: Get emailAuthenticationMethod
description: Чтение свойств и связей объекта emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f4cf44accf9d67da2475079813545bc3a3ce21bf
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872179"
---
# <a name="get-emailauthenticationmethod"></a><span data-ttu-id="97835-103">Get emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="97835-103">Get emailAuthenticationMethod</span></span>
<span data-ttu-id="97835-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97835-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97835-105">Получить один объект метода проверки [подлинности электронной почты](../resources/emailauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="97835-105">Retrieve a user's single [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="97835-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97835-106">Permissions</span></span>
<span data-ttu-id="97835-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97835-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97835-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97835-109">Permission type</span></span>|<span data-ttu-id="97835-110">Разрешения, действующие на себя (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="97835-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="97835-111">Разрешения, действующие над другими (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="97835-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="97835-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97835-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="97835-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97835-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="97835-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97835-114">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="97835-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97835-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97835-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97835-116">Not supported.</span></span> | <span data-ttu-id="97835-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97835-117">Not supported.</span></span> |
| <span data-ttu-id="97835-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="97835-118">Application</span></span>                            | <span data-ttu-id="97835-119">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="97835-119">Not applicable.</span></span> | <span data-ttu-id="97835-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97835-120">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="97835-121">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="97835-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="97835-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="97835-122">Global admin</span></span>
* <span data-ttu-id="97835-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="97835-123">Global reader</span></span>
* <span data-ttu-id="97835-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="97835-124">Privileged authentication admin</span></span>
* <span data-ttu-id="97835-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="97835-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="97835-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97835-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/emailMethods/{id}
GET /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="97835-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97835-127">Request headers</span></span>
|<span data-ttu-id="97835-128">Имя</span><span class="sxs-lookup"><span data-stu-id="97835-128">Name</span></span>|<span data-ttu-id="97835-129">Описание</span><span class="sxs-lookup"><span data-stu-id="97835-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="97835-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97835-130">Authorization</span></span>|<span data-ttu-id="97835-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97835-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97835-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97835-133">Request body</span></span>
<span data-ttu-id="97835-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97835-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97835-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="97835-135">Response</span></span>

<span data-ttu-id="97835-136">В случае успеха этот метод возвращает код отклика и объект `200 OK` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="97835-136">If successful, this method returns a `200 OK` response code and the requested [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="97835-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="97835-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="97835-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="97835-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="97835-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="97835-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_emailauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="97835-140">C#</span><span class="sxs-lookup"><span data-stu-id="97835-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97835-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97835-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97835-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97835-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97835-143">Java</span><span class="sxs-lookup"><span data-stu-id="97835-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="97835-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="97835-144">Response</span></span>
<span data-ttu-id="97835-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="97835-145">The following is an example of the response.</span></span>

<span data-ttu-id="97835-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="97835-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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

