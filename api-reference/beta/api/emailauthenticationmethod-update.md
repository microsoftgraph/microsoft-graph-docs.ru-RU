---
title: Обновление Емаилаусентикатионмесод
description: Обновление свойств объекта Емаилаусентикатионмесод.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cc4fc3c7900482e4444465a406e7c8b4319bcf0f
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458139"
---
# <a name="update-emailauthenticationmethod"></a><span data-ttu-id="ca466-103">Обновление Емаилаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="ca466-103">Update emailAuthenticationMethod</span></span>
<span data-ttu-id="ca466-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca466-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca466-105">Обновление адреса электронной почты пользователя, связанного с объектом [метода проверки подлинности электронной почты](../resources/emailauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="ca466-105">Update a user's email address associated with an [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca466-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ca466-106">Permissions</span></span>
<span data-ttu-id="ca466-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca466-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca466-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca466-109">Permission type</span></span>|<span data-ttu-id="ca466-110">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca466-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="ca466-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="ca466-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="ca466-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca466-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca466-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca466-113">Not supported.</span></span>|<span data-ttu-id="ca466-114">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ca466-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="ca466-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca466-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca466-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca466-116">Not supported.</span></span>|<span data-ttu-id="ca466-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca466-117">Not supported.</span></span>
|<span data-ttu-id="ca466-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca466-118">Application</span></span>|<span data-ttu-id="ca466-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca466-119">Not supported.</span></span>|<span data-ttu-id="ca466-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca466-120">Not supported.</span></span>

<span data-ttu-id="ca466-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="ca466-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="ca466-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="ca466-122">Global admin</span></span>
* <span data-ttu-id="ca466-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="ca466-123">Global reader</span></span>
* <span data-ttu-id="ca466-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="ca466-124">Privileged authentication admin</span></span>
* <span data-ttu-id="ca466-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="ca466-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="ca466-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca466-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ca466-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca466-127">Request headers</span></span>
|<span data-ttu-id="ca466-128">Имя</span><span class="sxs-lookup"><span data-stu-id="ca466-128">Name</span></span>|<span data-ttu-id="ca466-129">Описание</span><span class="sxs-lookup"><span data-stu-id="ca466-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ca466-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ca466-130">Authorization</span></span>|<span data-ttu-id="ca466-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca466-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ca466-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca466-133">Content-Type</span></span>|<span data-ttu-id="ca466-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca466-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca466-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca466-136">Request body</span></span>
<span data-ttu-id="ca466-137">В теле запроса добавьте представление объекта [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в формате JSON с обновленным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ca466-137">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the updated email address.</span></span>

<span data-ttu-id="ca466-138">В следующей таблице приведены свойства, необходимые при обновлении [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="ca466-138">The following table shows the properties that are required when you update the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="ca466-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca466-139">Property</span></span>|<span data-ttu-id="ca466-140">Тип</span><span class="sxs-lookup"><span data-stu-id="ca466-140">Type</span></span>|<span data-ttu-id="ca466-141">Описание</span><span class="sxs-lookup"><span data-stu-id="ca466-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca466-142">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ca466-142">emailAddress</span></span>|<span data-ttu-id="ca466-143">String</span><span class="sxs-lookup"><span data-stu-id="ca466-143">String</span></span>|<span data-ttu-id="ca466-144">Обновленный адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="ca466-144">Updated email address</span></span>|



## <a name="response"></a><span data-ttu-id="ca466-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca466-145">Response</span></span>

<span data-ttu-id="ca466-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ca466-146">If successful, this method returns a `200 OK` response code and an updated [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ca466-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="ca466-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ca466-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca466-148">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ca466-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca466-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_emailauthenticationmethod"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods/3ddfcfc8-9383-446f-83cc-3ab9be4be18f
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```
# <a name="javascript"></a>[<span data-ttu-id="ca466-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca466-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca466-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca466-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ca466-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca466-152">Response</span></span>

<span data-ttu-id="ca466-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ca466-153">The following is an example of the response.</span></span>

<span data-ttu-id="ca466-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ca466-154">**Note:** The response object shown here might be shortened for readability.</span></span>

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
