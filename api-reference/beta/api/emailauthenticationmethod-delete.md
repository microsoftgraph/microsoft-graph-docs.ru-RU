---
title: Удаление Емаилаусентикатионмесод
description: Удаляет объект Емаилаусентикатионмесод.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a99c8faf5540310640b8321ea7a7bc30eaded624
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921643"
---
# <a name="delete-emailauthenticationmethod"></a><span data-ttu-id="0afd2-103">Удаление Емаилаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="0afd2-103">Delete emailAuthenticationMethod</span></span>
<span data-ttu-id="0afd2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0afd2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0afd2-105">Удаляет объект [метода проверки подлинности электронной почты](../resources/emailauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="0afd2-105">Deletes a user's [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0afd2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0afd2-106">Permissions</span></span>
<span data-ttu-id="0afd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0afd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0afd2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0afd2-109">Permission type</span></span>|<span data-ttu-id="0afd2-110">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="0afd2-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="0afd2-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="0afd2-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="0afd2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0afd2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0afd2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0afd2-113">Not supported.</span></span>|<span data-ttu-id="0afd2-114">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0afd2-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="0afd2-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0afd2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0afd2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0afd2-116">Not supported.</span></span>|<span data-ttu-id="0afd2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0afd2-117">Not supported.</span></span>
|<span data-ttu-id="0afd2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0afd2-118">Application</span></span>|<span data-ttu-id="0afd2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0afd2-119">Not supported.</span></span>|<span data-ttu-id="0afd2-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0afd2-120">Not supported.</span></span>

<span data-ttu-id="0afd2-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима [одна из следующих ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="0afd2-121">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="0afd2-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0afd2-122">Global admin</span></span>
* <span data-ttu-id="0afd2-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="0afd2-123">Global reader</span></span>
* <span data-ttu-id="0afd2-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="0afd2-124">Privileged authentication admin</span></span>
* <span data-ttu-id="0afd2-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="0afd2-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="0afd2-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0afd2-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0afd2-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0afd2-127">Request headers</span></span>
|<span data-ttu-id="0afd2-128">Имя</span><span class="sxs-lookup"><span data-stu-id="0afd2-128">Name</span></span>|<span data-ttu-id="0afd2-129">Описание</span><span class="sxs-lookup"><span data-stu-id="0afd2-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0afd2-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0afd2-130">Authorization</span></span>|<span data-ttu-id="0afd2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0afd2-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0afd2-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0afd2-133">Request body</span></span>
<span data-ttu-id="0afd2-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0afd2-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0afd2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0afd2-135">Response</span></span>

<span data-ttu-id="0afd2-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0afd2-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0afd2-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="0afd2-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0afd2-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0afd2-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0afd2-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="0afd2-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_emailauthenticationmethod"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
```
# <a name="c"></a>[<span data-ttu-id="0afd2-141">C#</span><span class="sxs-lookup"><span data-stu-id="0afd2-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0afd2-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0afd2-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0afd2-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0afd2-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0afd2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0afd2-144">Response</span></span>
<span data-ttu-id="0afd2-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0afd2-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

