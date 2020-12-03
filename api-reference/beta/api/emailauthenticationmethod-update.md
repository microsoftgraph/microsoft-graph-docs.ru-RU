---
title: Обновление Емаилаусентикатионмесод
description: Обновление свойств объекта Емаилаусентикатионмесод.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ebb0ab053aab69a3e795ea575f6862e86ccec19c
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521301"
---
# <a name="update-emailauthenticationmethod"></a><span data-ttu-id="9d359-103">Обновление Емаилаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="9d359-103">Update emailAuthenticationMethod</span></span>
<span data-ttu-id="9d359-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d359-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d359-105">Обновление адреса электронной почты пользователя, связанного с объектом [метода проверки подлинности электронной почты](../resources/emailauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="9d359-105">Update a user's email address associated with an [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d359-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d359-106">Permissions</span></span>
<span data-ttu-id="9d359-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d359-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d359-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d359-109">Permission type</span></span>|<span data-ttu-id="9d359-110">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d359-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="9d359-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="9d359-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="9d359-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d359-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d359-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d359-113">Not supported.</span></span>|<span data-ttu-id="9d359-114">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="9d359-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="9d359-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d359-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d359-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d359-116">Not supported.</span></span>|<span data-ttu-id="9d359-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d359-117">Not supported.</span></span>
|<span data-ttu-id="9d359-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d359-118">Application</span></span>|<span data-ttu-id="9d359-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d359-119">Not supported.</span></span>|<span data-ttu-id="9d359-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d359-120">Not supported.</span></span>

<span data-ttu-id="9d359-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="9d359-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="9d359-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="9d359-122">Global admin</span></span>
* <span data-ttu-id="9d359-123">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="9d359-123">Privileged authentication admin</span></span>
* <span data-ttu-id="9d359-124">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="9d359-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="9d359-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d359-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9d359-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d359-126">Request headers</span></span>
|<span data-ttu-id="9d359-127">Имя</span><span class="sxs-lookup"><span data-stu-id="9d359-127">Name</span></span>|<span data-ttu-id="9d359-128">Описание</span><span class="sxs-lookup"><span data-stu-id="9d359-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9d359-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d359-129">Authorization</span></span>|<span data-ttu-id="9d359-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d359-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="9d359-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9d359-132">Content-Type</span></span>|<span data-ttu-id="9d359-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d359-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d359-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d359-135">Request body</span></span>
<span data-ttu-id="9d359-136">В теле запроса добавьте представление объекта [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в формате JSON с обновленным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9d359-136">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the updated email address.</span></span>

<span data-ttu-id="9d359-137">В следующей таблице приведены свойства, необходимые при обновлении [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="9d359-137">The following table shows the properties that are required when you update the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="9d359-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d359-138">Property</span></span>|<span data-ttu-id="9d359-139">Тип</span><span class="sxs-lookup"><span data-stu-id="9d359-139">Type</span></span>|<span data-ttu-id="9d359-140">Описание</span><span class="sxs-lookup"><span data-stu-id="9d359-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d359-141">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9d359-141">emailAddress</span></span>|<span data-ttu-id="9d359-142">String</span><span class="sxs-lookup"><span data-stu-id="9d359-142">String</span></span>|<span data-ttu-id="9d359-143">Обновленный адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="9d359-143">Updated email address</span></span>|



## <a name="response"></a><span data-ttu-id="9d359-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d359-144">Response</span></span>

<span data-ttu-id="9d359-145">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d359-145">If successful, this method returns a `200 OK` response code and an updated [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9d359-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="9d359-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9d359-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d359-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="9d359-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d359-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethod"
}
-->
``` http
PUT https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="9d359-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d359-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d359-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d359-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="9d359-151">C#</span><span class="sxs-lookup"><span data-stu-id="9d359-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d359-152">Java</span><span class="sxs-lookup"><span data-stu-id="9d359-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9d359-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d359-153">Response</span></span>

<span data-ttu-id="9d359-154">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9d359-154">The following is an example of the response.</span></span>

<span data-ttu-id="9d359-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9d359-155">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
  "emailAddress": "kim@contoso.com"
}
```
