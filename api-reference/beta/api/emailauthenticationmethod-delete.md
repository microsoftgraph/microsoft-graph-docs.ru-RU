---
title: Удаление emailAuthenticationMethod
description: Удаляет объект emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7fbb2f6af414da2c44ca6d68dc688973e9d34bce
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873502"
---
# <a name="delete-emailauthenticationmethod"></a><span data-ttu-id="db7d1-103">Удаление emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="db7d1-103">Delete emailAuthenticationMethod</span></span>
<span data-ttu-id="db7d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db7d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db7d1-105">Удаляет объект метода проверки [подлинности электронной почты](../resources/emailauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="db7d1-105">Deletes a user's [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db7d1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db7d1-106">Permissions</span></span>
<span data-ttu-id="db7d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db7d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db7d1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db7d1-109">Permission type</span></span>|<span data-ttu-id="db7d1-110">Разрешения, действующие на себя (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="db7d1-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="db7d1-111">Разрешения, действующие над другими (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="db7d1-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="db7d1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db7d1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="db7d1-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db7d1-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="db7d1-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db7d1-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="db7d1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db7d1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db7d1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db7d1-116">Not supported.</span></span> | <span data-ttu-id="db7d1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db7d1-117">Not supported.</span></span> |
| <span data-ttu-id="db7d1-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="db7d1-118">Application</span></span>                            | <span data-ttu-id="db7d1-119">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="db7d1-119">Not applicable.</span></span> | <span data-ttu-id="db7d1-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db7d1-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="db7d1-121">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="db7d1-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="db7d1-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="db7d1-122">Global admin</span></span>
* <span data-ttu-id="db7d1-123">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="db7d1-123">Privileged authentication admin</span></span>
* <span data-ttu-id="db7d1-124">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="db7d1-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="db7d1-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db7d1-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="db7d1-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db7d1-126">Request headers</span></span>
|<span data-ttu-id="db7d1-127">Имя</span><span class="sxs-lookup"><span data-stu-id="db7d1-127">Name</span></span>|<span data-ttu-id="db7d1-128">Описание</span><span class="sxs-lookup"><span data-stu-id="db7d1-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="db7d1-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db7d1-129">Authorization</span></span>|<span data-ttu-id="db7d1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db7d1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="db7d1-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db7d1-132">Request body</span></span>
<span data-ttu-id="db7d1-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db7d1-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db7d1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="db7d1-134">Response</span></span>

<span data-ttu-id="db7d1-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="db7d1-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db7d1-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="db7d1-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db7d1-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="db7d1-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="db7d1-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="db7d1-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="db7d1-140">C#</span><span class="sxs-lookup"><span data-stu-id="db7d1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db7d1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db7d1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db7d1-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db7d1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db7d1-143">Java</span><span class="sxs-lookup"><span data-stu-id="db7d1-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="db7d1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="db7d1-144">Response</span></span>
<span data-ttu-id="db7d1-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="db7d1-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

