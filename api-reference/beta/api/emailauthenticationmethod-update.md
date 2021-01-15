---
title: Обновление emailAuthenticationMethod
description: Обновление свойств объекта emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 87671a3c0a3bb5c663beb50ce740c8d25631f1c0
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872074"
---
# <a name="update-emailauthenticationmethod"></a><span data-ttu-id="0f5df-103">Обновление emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="0f5df-103">Update emailAuthenticationMethod</span></span>
<span data-ttu-id="0f5df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f5df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f5df-105">Обновление адреса электронной почты пользователя, связанного с объектом [метода проверки подлинности электронной почты.](../resources/emailauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="0f5df-105">Update a user's email address associated with an [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f5df-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f5df-106">Permissions</span></span>
<span data-ttu-id="0f5df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f5df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f5df-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f5df-109">Permission type</span></span>|<span data-ttu-id="0f5df-110">Разрешения, действующие на себя (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="0f5df-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="0f5df-111">Разрешения, действующие над другими (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="0f5df-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="0f5df-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f5df-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="0f5df-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0f5df-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="0f5df-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f5df-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="0f5df-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f5df-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f5df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f5df-116">Not supported.</span></span> | <span data-ttu-id="0f5df-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f5df-117">Not supported.</span></span> |
| <span data-ttu-id="0f5df-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="0f5df-118">Application</span></span>                            | <span data-ttu-id="0f5df-119">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="0f5df-119">Not applicable.</span></span> | <span data-ttu-id="0f5df-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f5df-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="0f5df-121">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="0f5df-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="0f5df-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="0f5df-122">Global admin</span></span>
* <span data-ttu-id="0f5df-123">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="0f5df-123">Privileged authentication admin</span></span>
* <span data-ttu-id="0f5df-124">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="0f5df-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="0f5df-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f5df-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0f5df-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f5df-126">Request headers</span></span>
|<span data-ttu-id="0f5df-127">Имя</span><span class="sxs-lookup"><span data-stu-id="0f5df-127">Name</span></span>|<span data-ttu-id="0f5df-128">Описание</span><span class="sxs-lookup"><span data-stu-id="0f5df-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0f5df-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f5df-129">Authorization</span></span>|<span data-ttu-id="0f5df-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f5df-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0f5df-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0f5df-132">Content-Type</span></span>|<span data-ttu-id="0f5df-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f5df-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f5df-135">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f5df-135">Request body</span></span>
<span data-ttu-id="0f5df-136">В теле запроса укажу представление объекта [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в JSON с обновленным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0f5df-136">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the updated email address.</span></span>

<span data-ttu-id="0f5df-137">В следующей таблице показаны свойства, необходимые при обновлении [объекта emailAuthenticationMethod.](../resources/emailauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="0f5df-137">The following table shows the properties that are required when you update the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="0f5df-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f5df-138">Property</span></span>|<span data-ttu-id="0f5df-139">Тип</span><span class="sxs-lookup"><span data-stu-id="0f5df-139">Type</span></span>|<span data-ttu-id="0f5df-140">Описание</span><span class="sxs-lookup"><span data-stu-id="0f5df-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f5df-141">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0f5df-141">emailAddress</span></span>|<span data-ttu-id="0f5df-142">String</span><span class="sxs-lookup"><span data-stu-id="0f5df-142">String</span></span>|<span data-ttu-id="0f5df-143">Обновленный адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="0f5df-143">Updated email address</span></span>|



## <a name="response"></a><span data-ttu-id="0f5df-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f5df-144">Response</span></span>

<span data-ttu-id="0f5df-145">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0f5df-145">If successful, this method returns a `200 OK` response code and an updated [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0f5df-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="0f5df-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0f5df-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f5df-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="0f5df-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="0f5df-148">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="0f5df-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0f5df-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0f5df-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0f5df-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="0f5df-151">C#</span><span class="sxs-lookup"><span data-stu-id="0f5df-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0f5df-152">Java</span><span class="sxs-lookup"><span data-stu-id="0f5df-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="0f5df-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f5df-153">Response</span></span>

<span data-ttu-id="0f5df-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0f5df-154">The following is an example of the response.</span></span>

<span data-ttu-id="0f5df-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0f5df-155">**Note:** The response object shown here might be shortened for readability.</span></span>

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
