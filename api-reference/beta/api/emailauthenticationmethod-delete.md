---
title: Удаление emailAuthenticationMethod
description: Удаляет объект emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 25a05ff6b4ad6639c7be87a88135fc2cebd8c2cb
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796390"
---
# <a name="delete-emailauthenticationmethod"></a><span data-ttu-id="a4f38-103">Удаление emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a4f38-103">Delete emailAuthenticationMethod</span></span>
<span data-ttu-id="a4f38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4f38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4f38-105">Удаляет объект метода проверки [подлинности электронной почты](../resources/emailauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="a4f38-105">Deletes a user's [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4f38-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4f38-106">Permissions</span></span>
<span data-ttu-id="a4f38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4f38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4f38-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4f38-109">Permission type</span></span>|<span data-ttu-id="a4f38-110">Разрешения, действующие на себя (от большинства до наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="a4f38-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="a4f38-111">Разрешения, действующие над другими (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="a4f38-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="a4f38-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4f38-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4f38-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4f38-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="a4f38-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f38-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="a4f38-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4f38-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4f38-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4f38-116">Not supported.</span></span> | <span data-ttu-id="a4f38-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4f38-117">Not supported.</span></span> |
| <span data-ttu-id="a4f38-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4f38-118">Application</span></span>                            | <span data-ttu-id="a4f38-119">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="a4f38-119">Not applicable.</span></span> | <span data-ttu-id="a4f38-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4f38-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="a4f38-121">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="a4f38-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="a4f38-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a4f38-122">Global admin</span></span>
* <span data-ttu-id="a4f38-123">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="a4f38-123">Privileged authentication admin</span></span>
* <span data-ttu-id="a4f38-124">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="a4f38-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="a4f38-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4f38-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a4f38-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4f38-126">Request headers</span></span>
|<span data-ttu-id="a4f38-127">Имя</span><span class="sxs-lookup"><span data-stu-id="a4f38-127">Name</span></span>|<span data-ttu-id="a4f38-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a4f38-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4f38-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4f38-129">Authorization</span></span>|<span data-ttu-id="a4f38-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4f38-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4f38-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4f38-132">Request body</span></span>
<span data-ttu-id="a4f38-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4f38-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4f38-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4f38-134">Response</span></span>

<span data-ttu-id="a4f38-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a4f38-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4f38-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="a4f38-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4f38-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4f38-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a4f38-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4f38-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="a4f38-140">C#</span><span class="sxs-lookup"><span data-stu-id="a4f38-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4f38-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4f38-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4f38-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4f38-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a4f38-143">Java</span><span class="sxs-lookup"><span data-stu-id="a4f38-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a4f38-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4f38-144">Response</span></span>
<span data-ttu-id="a4f38-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a4f38-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

