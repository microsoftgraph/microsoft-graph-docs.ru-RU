---
title: Удаление fido2AuthenticationMethod
description: Удаляет объект fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 187503ad87bb7dc8e71c201e7086ff3858d0247d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954481"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="1bdfe-103">Удаление fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1bdfe-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="1bdfe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bdfe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bdfe-105">Удаляет объект [метода проверки подлинности для ключа безопасности FIDO2](../resources/fido2authenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bdfe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1bdfe-106">Permissions</span></span>
<span data-ttu-id="1bdfe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bdfe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bdfe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bdfe-109">Permission type</span></span>|<span data-ttu-id="1bdfe-110">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bdfe-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="1bdfe-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="1bdfe-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="1bdfe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bdfe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1bdfe-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-113">Not supported.</span></span>|<span data-ttu-id="1bdfe-114">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1bdfe-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="1bdfe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bdfe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bdfe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-116">Not supported.</span></span>|<span data-ttu-id="1bdfe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-117">Not supported.</span></span>
|<span data-ttu-id="1bdfe-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bdfe-118">Application</span></span>|<span data-ttu-id="1bdfe-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-119">Not supported.</span></span>|<span data-ttu-id="1bdfe-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-120">Not supported.</span></span>

<span data-ttu-id="1bdfe-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="1bdfe-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="1bdfe-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1bdfe-122">Global admin</span></span>
* <span data-ttu-id="1bdfe-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="1bdfe-123">Global reader</span></span>
* <span data-ttu-id="1bdfe-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="1bdfe-124">Privileged authentication admin</span></span>
* <span data-ttu-id="1bdfe-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="1bdfe-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="1bdfe-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bdfe-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1bdfe-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bdfe-127">Request headers</span></span>
|<span data-ttu-id="1bdfe-128">Имя</span><span class="sxs-lookup"><span data-stu-id="1bdfe-128">Name</span></span>|<span data-ttu-id="1bdfe-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1bdfe-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1bdfe-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1bdfe-130">Authorization</span></span>|<span data-ttu-id="1bdfe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bdfe-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bdfe-133">Request body</span></span>
<span data-ttu-id="1bdfe-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bdfe-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bdfe-135">Response</span></span>

<span data-ttu-id="1bdfe-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1bdfe-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="1bdfe-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1bdfe-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bdfe-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1bdfe-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1bdfe-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="1bdfe-141">C#</span><span class="sxs-lookup"><span data-stu-id="1bdfe-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1bdfe-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1bdfe-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1bdfe-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1bdfe-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1bdfe-144">Java</span><span class="sxs-lookup"><span data-stu-id="1bdfe-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1bdfe-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bdfe-145">Response</span></span>
<span data-ttu-id="1bdfe-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1bdfe-146">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

