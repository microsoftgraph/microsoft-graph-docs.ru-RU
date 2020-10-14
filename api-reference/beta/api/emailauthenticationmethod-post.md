---
title: Создание Емаилаусентикатионмесод
description: Создание нового объекта Емаилаусентикатионмесод.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0fa084db81af3677f5a6e12c6d90020178653b4f
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458151"
---
# <a name="create-emailauthenticationmethod"></a><span data-ttu-id="9bcf0-103">Создание Емаилаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="9bcf0-103">Create emailAuthenticationMethod</span></span>
<span data-ttu-id="9bcf0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bcf0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bcf0-105">Задайте объект [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-105">Set a user's [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object.</span></span> <span data-ttu-id="9bcf0-106">Проверка подлинности электронной почты — это метод самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-106">Email authentication is a self-service password reset method.</span></span> <span data-ttu-id="9bcf0-107">Пользователь может иметь только один метод проверки подлинности электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-107">A user may only have one email authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bcf0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9bcf0-108">Permissions</span></span>
<span data-ttu-id="9bcf0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9bcf0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bcf0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9bcf0-111">Permission type</span></span>|<span data-ttu-id="9bcf0-112">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="9bcf0-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="9bcf0-113">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="9bcf0-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="9bcf0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9bcf0-114">Delegated (work or school account)</span></span>|<span data-ttu-id="9bcf0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-115">Not supported.</span></span>|<span data-ttu-id="9bcf0-116">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9bcf0-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="9bcf0-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9bcf0-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bcf0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-118">Not supported.</span></span>|<span data-ttu-id="9bcf0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-119">Not supported.</span></span>
|<span data-ttu-id="9bcf0-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9bcf0-120">Application</span></span>|<span data-ttu-id="9bcf0-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-121">Not supported.</span></span>|<span data-ttu-id="9bcf0-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-122">Not supported.</span></span>

<span data-ttu-id="9bcf0-123">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="9bcf0-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="9bcf0-124">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="9bcf0-124">Global admin</span></span>
* <span data-ttu-id="9bcf0-125">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="9bcf0-125">Global reader</span></span>
* <span data-ttu-id="9bcf0-126">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="9bcf0-126">Privileged authentication admin</span></span>
* <span data-ttu-id="9bcf0-127">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="9bcf0-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="9bcf0-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9bcf0-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a><span data-ttu-id="9bcf0-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9bcf0-129">Request headers</span></span>
|<span data-ttu-id="9bcf0-130">Имя</span><span class="sxs-lookup"><span data-stu-id="9bcf0-130">Name</span></span>|<span data-ttu-id="9bcf0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9bcf0-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9bcf0-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9bcf0-132">Authorization</span></span>|<span data-ttu-id="9bcf0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9bcf0-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9bcf0-135">Content-Type</span></span>|<span data-ttu-id="9bcf0-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bcf0-138">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9bcf0-138">Request body</span></span>
<span data-ttu-id="9bcf0-139">В тексте запроса добавьте представление объекта [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в формате JSON с нужным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-139">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the desired email address.</span></span>

<span data-ttu-id="9bcf0-140">В следующей таблице приведены свойства, необходимые при создании [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="9bcf0-140">The following table shows the properties that are required when you create the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="9bcf0-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bcf0-141">Property</span></span>|<span data-ttu-id="9bcf0-142">Тип</span><span class="sxs-lookup"><span data-stu-id="9bcf0-142">Type</span></span>|<span data-ttu-id="9bcf0-143">Описание</span><span class="sxs-lookup"><span data-stu-id="9bcf0-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bcf0-144">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9bcf0-144">emailAddress</span></span>|<span data-ttu-id="9bcf0-145">String</span><span class="sxs-lookup"><span data-stu-id="9bcf0-145">String</span></span>|<span data-ttu-id="9bcf0-146">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="9bcf0-146">Email address</span></span>|



## <a name="response"></a><span data-ttu-id="9bcf0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bcf0-147">Response</span></span>

<span data-ttu-id="9bcf0-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-148">If successful, this method returns a `201 Created` response code and a new [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9bcf0-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="9bcf0-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9bcf0-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="9bcf0-150">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9bcf0-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bcf0-151">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="9bcf0-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bcf0-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bcf0-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bcf0-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9bcf0-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="9bcf0-154">Response</span></span>
<span data-ttu-id="9bcf0-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-155">The following is an example of the response.</span></span>

<span data-ttu-id="9bcf0-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9bcf0-156">**Note:** The response object shown here might be shortened for readability.</span></span>
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
