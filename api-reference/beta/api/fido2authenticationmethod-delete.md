---
title: Удаление fido2AuthenticationMethod
description: Удаляет объект fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 3d92da843b6e18a07cf98e42dee685a1d692d6ef
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436080"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="b37cc-103">Удаление fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b37cc-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="b37cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b37cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b37cc-105">Удаляет объект метода проверки подлинности [ключа безопасности FIDO2 пользователя.](../resources/fido2authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b37cc-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b37cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b37cc-106">Permissions</span></span>
<span data-ttu-id="b37cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b37cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b37cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b37cc-109">Permission type</span></span>|<span data-ttu-id="b37cc-110">Разрешения, действующие на себя (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="b37cc-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="b37cc-111">Разрешения, действующие на других (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="b37cc-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="b37cc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b37cc-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b37cc-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b37cc-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="b37cc-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b37cc-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="b37cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b37cc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b37cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b37cc-116">Not supported.</span></span> | <span data-ttu-id="b37cc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b37cc-117">Not supported.</span></span> |
| <span data-ttu-id="b37cc-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="b37cc-118">Application</span></span>                            | <span data-ttu-id="b37cc-119">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="b37cc-119">Not applicable.</span></span> | <span data-ttu-id="b37cc-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b37cc-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="b37cc-121">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="b37cc-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="b37cc-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b37cc-122">Global admin</span></span>
* <span data-ttu-id="b37cc-123">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b37cc-123">Privileged authentication admin</span></span>
* <span data-ttu-id="b37cc-124">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="b37cc-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="b37cc-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b37cc-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b37cc-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b37cc-126">Request headers</span></span>
|<span data-ttu-id="b37cc-127">Имя</span><span class="sxs-lookup"><span data-stu-id="b37cc-127">Name</span></span>|<span data-ttu-id="b37cc-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b37cc-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b37cc-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b37cc-129">Authorization</span></span>|<span data-ttu-id="b37cc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b37cc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b37cc-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b37cc-132">Request body</span></span>
<span data-ttu-id="b37cc-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b37cc-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b37cc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b37cc-134">Response</span></span>

<span data-ttu-id="b37cc-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b37cc-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b37cc-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="b37cc-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b37cc-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b37cc-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b37cc-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b37cc-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="b37cc-140">C#</span><span class="sxs-lookup"><span data-stu-id="b37cc-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b37cc-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b37cc-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b37cc-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b37cc-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b37cc-143">Java</span><span class="sxs-lookup"><span data-stu-id="b37cc-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b37cc-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b37cc-144">Response</span></span>
<span data-ttu-id="b37cc-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b37cc-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

