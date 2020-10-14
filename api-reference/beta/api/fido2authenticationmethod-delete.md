---
title: Удаление fido2AuthenticationMethod
description: Удаляет объект fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 204b29ec29b44c785bce8388dff74866e6620996
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458507"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="6d259-103">Удаление fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="6d259-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="6d259-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d259-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d259-105">Удаляет объект [метода проверки подлинности для ключа безопасности FIDO2](../resources/fido2authenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="6d259-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d259-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d259-106">Permissions</span></span>
<span data-ttu-id="6d259-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d259-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d259-109">Permission type</span></span>|<span data-ttu-id="6d259-110">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d259-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="6d259-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="6d259-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="6d259-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d259-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6d259-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d259-113">Not supported.</span></span>|<span data-ttu-id="6d259-114">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6d259-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="6d259-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d259-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d259-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d259-116">Not supported.</span></span>|<span data-ttu-id="6d259-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d259-117">Not supported.</span></span>
|<span data-ttu-id="6d259-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d259-118">Application</span></span>|<span data-ttu-id="6d259-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d259-119">Not supported.</span></span>|<span data-ttu-id="6d259-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d259-120">Not supported.</span></span>

<span data-ttu-id="6d259-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="6d259-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="6d259-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6d259-122">Global admin</span></span>
* <span data-ttu-id="6d259-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="6d259-123">Global reader</span></span>
* <span data-ttu-id="6d259-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="6d259-124">Privileged authentication admin</span></span>
* <span data-ttu-id="6d259-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="6d259-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="6d259-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d259-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6d259-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d259-127">Request headers</span></span>
|<span data-ttu-id="6d259-128">Имя</span><span class="sxs-lookup"><span data-stu-id="6d259-128">Name</span></span>|<span data-ttu-id="6d259-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6d259-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6d259-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d259-130">Authorization</span></span>|<span data-ttu-id="6d259-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d259-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d259-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6d259-133">Request body</span></span>
<span data-ttu-id="6d259-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6d259-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d259-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d259-135">Response</span></span>

<span data-ttu-id="6d259-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6d259-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d259-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="6d259-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d259-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d259-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6d259-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d259-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="6d259-141">C#</span><span class="sxs-lookup"><span data-stu-id="6d259-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d259-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d259-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d259-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d259-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6d259-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d259-144">Response</span></span>
<span data-ttu-id="6d259-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6d259-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

