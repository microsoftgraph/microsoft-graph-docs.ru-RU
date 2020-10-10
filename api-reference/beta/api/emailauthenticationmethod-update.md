---
title: Обновление Емаилаусентикатионмесод
description: Обновление свойств объекта Емаилаусентикатионмесод.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9da21f027d69f12f0548f7cce720ce1bea83f577
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418455"
---
# <a name="update-emailauthenticationmethod"></a><span data-ttu-id="2ae54-103">Обновление Емаилаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="2ae54-103">Update emailAuthenticationMethod</span></span>
<span data-ttu-id="2ae54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ae54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ae54-105">Обновление адреса электронной почты пользователя, связанного с объектом [метода проверки подлинности электронной почты](../resources/emailauthenticationmethod.md) .</span><span class="sxs-lookup"><span data-stu-id="2ae54-105">Update a user's email address associated with an [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ae54-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ae54-106">Permissions</span></span>
<span data-ttu-id="2ae54-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ae54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ae54-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ae54-109">Permission type</span></span>|<span data-ttu-id="2ae54-110">Разрешения, действующие на себя (от большинства до минимальных привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ae54-110">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="2ae54-111">Разрешения, действующие на других (по крайней мере для самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="2ae54-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="2ae54-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ae54-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ae54-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ae54-113">Not supported.</span></span>|<span data-ttu-id="2ae54-114">Усераусентикатионмесод. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2ae54-114">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="2ae54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ae54-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ae54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ae54-116">Not supported.</span></span>|<span data-ttu-id="2ae54-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ae54-117">Not supported.</span></span>
|<span data-ttu-id="2ae54-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ae54-118">Application</span></span>|<span data-ttu-id="2ae54-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ae54-119">Not supported.</span></span>|<span data-ttu-id="2ae54-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ae54-120">Not supported.</span></span>

<span data-ttu-id="2ae54-121">Для делегированных сценариев, в которых администратор работает с другим пользователем, администратору необходима одна из следующих [ролей](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span><span class="sxs-lookup"><span data-stu-id="2ae54-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="2ae54-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2ae54-122">Global admin</span></span>
* <span data-ttu-id="2ae54-123">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="2ae54-123">Global reader</span></span>
* <span data-ttu-id="2ae54-124">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2ae54-124">Privileged authentication admin</span></span>
* <span data-ttu-id="2ae54-125">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2ae54-125">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="2ae54-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ae54-126">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2ae54-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ae54-127">Request headers</span></span>
|<span data-ttu-id="2ae54-128">Имя</span><span class="sxs-lookup"><span data-stu-id="2ae54-128">Name</span></span>|<span data-ttu-id="2ae54-129">Описание</span><span class="sxs-lookup"><span data-stu-id="2ae54-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2ae54-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ae54-130">Authorization</span></span>|<span data-ttu-id="2ae54-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ae54-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2ae54-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ae54-133">Content-Type</span></span>|<span data-ttu-id="2ae54-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2ae54-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ae54-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ae54-136">Request body</span></span>
<span data-ttu-id="2ae54-137">В теле запроса добавьте представление объекта [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в формате JSON с обновленным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2ae54-137">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the updated email address.</span></span>

<span data-ttu-id="2ae54-138">В следующей таблице приведены свойства, необходимые при обновлении [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="2ae54-138">The following table shows the properties that are required when you update the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="2ae54-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ae54-139">Property</span></span>|<span data-ttu-id="2ae54-140">Тип</span><span class="sxs-lookup"><span data-stu-id="2ae54-140">Type</span></span>|<span data-ttu-id="2ae54-141">Описание</span><span class="sxs-lookup"><span data-stu-id="2ae54-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ae54-142">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2ae54-142">emailAddress</span></span>|<span data-ttu-id="2ae54-143">String</span><span class="sxs-lookup"><span data-stu-id="2ae54-143">String</span></span>|<span data-ttu-id="2ae54-144">Обновленный адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="2ae54-144">Updated email address</span></span>|



## <a name="response"></a><span data-ttu-id="2ae54-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ae54-145">Response</span></span>

<span data-ttu-id="2ae54-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [емаилаусентикатионмесод](../resources/emailauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2ae54-146">If successful, this method returns a `200 OK` response code and an updated [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ae54-147">Примеры</span><span class="sxs-lookup"><span data-stu-id="2ae54-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ae54-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ae54-148">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="2ae54-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ae54-149">Response</span></span>

<span data-ttu-id="2ae54-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2ae54-150">The following is an example of the response.</span></span>

<span data-ttu-id="2ae54-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2ae54-151">**Note:** The response object shown here might be shortened for readability.</span></span>

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
