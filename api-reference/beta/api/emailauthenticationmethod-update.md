---
title: Обновление emailAuthenticationMethod
description: Обновление свойств объекта emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4e5eeaa1173b6ab5970fe85c472d0e6559ef9cd5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436332"
---
# <a name="update-emailauthenticationmethod"></a><span data-ttu-id="8aefb-103">Обновление emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8aefb-103">Update emailAuthenticationMethod</span></span>
<span data-ttu-id="8aefb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8aefb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8aefb-105">Обновление электронного адреса пользователя, связанного с объектом [метода проверки подлинности электронной](../resources/emailauthenticationmethod.md) почты.</span><span class="sxs-lookup"><span data-stu-id="8aefb-105">Update a user's email address associated with an [email Authentication Method](../resources/emailauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8aefb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8aefb-106">Permissions</span></span>
<span data-ttu-id="8aefb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8aefb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8aefb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8aefb-109">Permission type</span></span>|<span data-ttu-id="8aefb-110">Разрешения, действующие на себя (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="8aefb-110">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="8aefb-111">Разрешения, действующие на других (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="8aefb-111">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="8aefb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8aefb-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="8aefb-113">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8aefb-113">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="8aefb-114">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aefb-114">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="8aefb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8aefb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8aefb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aefb-116">Not supported.</span></span> | <span data-ttu-id="8aefb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8aefb-117">Not supported.</span></span> |
| <span data-ttu-id="8aefb-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="8aefb-118">Application</span></span>                            | <span data-ttu-id="8aefb-119">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="8aefb-119">Not applicable.</span></span> | <span data-ttu-id="8aefb-120">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8aefb-120">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="8aefb-121">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="8aefb-121">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="8aefb-122">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="8aefb-122">Global admin</span></span>
* <span data-ttu-id="8aefb-123">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="8aefb-123">Privileged authentication admin</span></span>
* <span data-ttu-id="8aefb-124">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="8aefb-124">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="8aefb-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8aefb-125">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /users/{id | userPrincipalName}/authentication/emailMethods/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8aefb-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8aefb-126">Request headers</span></span>
|<span data-ttu-id="8aefb-127">Имя</span><span class="sxs-lookup"><span data-stu-id="8aefb-127">Name</span></span>|<span data-ttu-id="8aefb-128">Описание</span><span class="sxs-lookup"><span data-stu-id="8aefb-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8aefb-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8aefb-129">Authorization</span></span>|<span data-ttu-id="8aefb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8aefb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8aefb-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8aefb-132">Content-Type</span></span>|<span data-ttu-id="8aefb-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8aefb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8aefb-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8aefb-135">Request body</span></span>
<span data-ttu-id="8aefb-136">В теле запроса поставляем JSON-представление объекта [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) с обновленным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8aefb-136">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the updated email address.</span></span>

<span data-ttu-id="8aefb-137">В следующей таблице показаны свойства, необходимые при обновлении [электронной почтыAuthenticationMethod.](../resources/emailauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="8aefb-137">The following table shows the properties that are required when you update the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="8aefb-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="8aefb-138">Property</span></span>|<span data-ttu-id="8aefb-139">Тип</span><span class="sxs-lookup"><span data-stu-id="8aefb-139">Type</span></span>|<span data-ttu-id="8aefb-140">Описание</span><span class="sxs-lookup"><span data-stu-id="8aefb-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8aefb-141">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8aefb-141">emailAddress</span></span>|<span data-ttu-id="8aefb-142">String</span><span class="sxs-lookup"><span data-stu-id="8aefb-142">String</span></span>|<span data-ttu-id="8aefb-143">Обновленный адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="8aefb-143">Updated email address</span></span>|



## <a name="response"></a><span data-ttu-id="8aefb-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="8aefb-144">Response</span></span>

<span data-ttu-id="8aefb-145">В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8aefb-145">If successful, this method returns a `200 OK` response code and an updated [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8aefb-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="8aefb-146">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8aefb-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="8aefb-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8aefb-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="8aefb-148">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="8aefb-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8aefb-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-emailauthenticationmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8aefb-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8aefb-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-emailauthenticationmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8aefb-151">C#</span><span class="sxs-lookup"><span data-stu-id="8aefb-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-emailauthenticationmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8aefb-152">Java</span><span class="sxs-lookup"><span data-stu-id="8aefb-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-emailauthenticationmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8aefb-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8aefb-153">Response</span></span>

<span data-ttu-id="8aefb-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8aefb-154">The following is an example of the response.</span></span>

<span data-ttu-id="8aefb-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8aefb-155">**Note:** The response object shown here might be shortened for readability.</span></span>

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
