---
title: Удаление fido2AuthenticationMethod
description: Удаляет объект fido2AuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b173e6ffe7534a6087210b9b412ce00e476034fb
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796396"
---
# <a name="delete-fido2authenticationmethod"></a><span data-ttu-id="02a4e-103">Удаление fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="02a4e-103">Delete fido2AuthenticationMethod</span></span>
<span data-ttu-id="02a4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02a4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02a4e-105">Удаляет объект метода проверки подлинности ключа безопасности [FIDO2](../resources/fido2authenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="02a4e-105">Deletes a user's [FIDO2 Security Key Authentication Method](../resources/fido2authenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02a4e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02a4e-106">Permissions</span></span>
<span data-ttu-id="02a4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02a4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a4e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02a4e-109">Permission type</span></span>|<span data-ttu-id="02a4e-110">Разрешения, действующие на себя (от большинства до наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="02a4e-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="02a4e-111">Разрешения, действующие над другими (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="02a4e-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="02a4e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02a4e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="02a4e-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02a4e-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="02a4e-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a4e-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="02a4e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02a4e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02a4e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02a4e-116">Not supported.</span></span> | <span data-ttu-id="02a4e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02a4e-117">Not supported.</span></span> |
| <span data-ttu-id="02a4e-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="02a4e-118">Application</span></span>                            | <span data-ttu-id="02a4e-119">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="02a4e-119">Not applicable.</span></span> | <span data-ttu-id="02a4e-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a4e-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="02a4e-121">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="02a4e-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="02a4e-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="02a4e-122">Global admin</span></span>
* <span data-ttu-id="02a4e-123">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="02a4e-123">Privileged authentication admin</span></span>
* <span data-ttu-id="02a4e-124">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="02a4e-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="02a4e-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02a4e-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/fido2Methods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="02a4e-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02a4e-126">Request headers</span></span>
|<span data-ttu-id="02a4e-127">Имя</span><span class="sxs-lookup"><span data-stu-id="02a4e-127">Name</span></span>|<span data-ttu-id="02a4e-128">Описание</span><span class="sxs-lookup"><span data-stu-id="02a4e-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="02a4e-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02a4e-129">Authorization</span></span>|<span data-ttu-id="02a4e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02a4e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02a4e-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02a4e-132">Request body</span></span>
<span data-ttu-id="02a4e-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="02a4e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02a4e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="02a4e-134">Response</span></span>

<span data-ttu-id="02a4e-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="02a4e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02a4e-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="02a4e-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02a4e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="02a4e-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="02a4e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="02a4e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_fido2authenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2
```
# <a name="c"></a>[<span data-ttu-id="02a4e-140">C#</span><span class="sxs-lookup"><span data-stu-id="02a4e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-fido2authenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02a4e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02a4e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-fido2authenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02a4e-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02a4e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-fido2authenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02a4e-143">Java</span><span class="sxs-lookup"><span data-stu-id="02a4e-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-fido2authenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="02a4e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="02a4e-144">Response</span></span>
<span data-ttu-id="02a4e-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="02a4e-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

