---
title: Создание Емаилаусентикатионмесод
description: Создание нового объекта Емаилаусентикатионмесод.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 52aabdcd45791e1ba1d2dcfc1d9faa63b7dda37a
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522484"
---
# <a name="create-emailauthenticationmethod"></a><span data-ttu-id="d403e-103">Создание Емаилаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="d403e-103">Create emailAuthenticationMethod</span></span>
<span data-ttu-id="d403e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d403e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d403e-105">Задайте объект [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="d403e-105">Set a user's [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object.</span></span> <span data-ttu-id="d403e-106">Проверка подлинности электронной почты — это метод самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="d403e-106">Email authentication is a self-service password reset method.</span></span> <span data-ttu-id="d403e-107">Пользователь может иметь только один метод проверки подлинности электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d403e-107">A user may only have one email authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="d403e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d403e-108">Permissions</span></span>
<span data-ttu-id="d403e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d403e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d403e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d403e-111">Permission type</span></span>|<span data-ttu-id="d403e-112">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="d403e-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="d403e-113">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="d403e-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="d403e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d403e-114">Delegated (work or school account)</span></span>|<span data-ttu-id="d403e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d403e-115">Not supported.</span></span>|<span data-ttu-id="d403e-116">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d403e-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="d403e-117">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d403e-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d403e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d403e-118">Not supported.</span></span>|<span data-ttu-id="d403e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d403e-119">Not supported.</span></span>
|<span data-ttu-id="d403e-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d403e-120">Application</span></span>|<span data-ttu-id="d403e-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d403e-121">Not supported.</span></span>|<span data-ttu-id="d403e-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d403e-122">Not supported.</span></span>

<span data-ttu-id="d403e-123">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="d403e-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="d403e-124">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="d403e-124">Global admin</span></span>
* <span data-ttu-id="d403e-125">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="d403e-125">Privileged authentication admin</span></span>
* <span data-ttu-id="d403e-126">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="d403e-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="d403e-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d403e-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a><span data-ttu-id="d403e-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d403e-128">Request headers</span></span>
|<span data-ttu-id="d403e-129">Имя</span><span class="sxs-lookup"><span data-stu-id="d403e-129">Name</span></span>|<span data-ttu-id="d403e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d403e-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d403e-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d403e-131">Authorization</span></span>|<span data-ttu-id="d403e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d403e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d403e-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d403e-134">Content-Type</span></span>|<span data-ttu-id="d403e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d403e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d403e-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d403e-137">Request body</span></span>
<span data-ttu-id="d403e-138">В тексте запроса добавьте представление объекта [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в формате JSON с нужным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d403e-138">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the desired email address.</span></span>

<span data-ttu-id="d403e-139">В следующей таблице приведены свойства, необходимые при создании [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="d403e-139">The following table shows the properties that are required when you create the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="d403e-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="d403e-140">Property</span></span>|<span data-ttu-id="d403e-141">Тип</span><span class="sxs-lookup"><span data-stu-id="d403e-141">Type</span></span>|<span data-ttu-id="d403e-142">Описание</span><span class="sxs-lookup"><span data-stu-id="d403e-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d403e-143">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d403e-143">emailAddress</span></span>|<span data-ttu-id="d403e-144">String</span><span class="sxs-lookup"><span data-stu-id="d403e-144">String</span></span>|<span data-ttu-id="d403e-145">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="d403e-145">Email address</span></span>|



## <a name="response"></a><span data-ttu-id="d403e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="d403e-146">Response</span></span>

<span data-ttu-id="d403e-147">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d403e-147">If successful, this method returns a `201 Created` response code and a new [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d403e-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="d403e-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d403e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="d403e-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d403e-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="d403e-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_emailauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="d403e-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d403e-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d403e-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d403e-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d403e-153">C#</span><span class="sxs-lookup"><span data-stu-id="d403e-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d403e-154">Java</span><span class="sxs-lookup"><span data-stu-id="d403e-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-emailauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d403e-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="d403e-155">Response</span></span>
<span data-ttu-id="d403e-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d403e-156">The following is an example of the response.</span></span>

<span data-ttu-id="d403e-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d403e-157">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
  "emailAddress": "kim@contoso.com"
}
```
