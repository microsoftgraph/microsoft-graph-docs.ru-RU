---
title: Создание emailAuthenticationMethod
description: Создание нового объекта emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b9ec2d40253faa72fd1f8d354de2649c4487e47e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436330"
---
# <a name="create-emailauthenticationmethod"></a><span data-ttu-id="4f208-103">Создание emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4f208-103">Create emailAuthenticationMethod</span></span>
<span data-ttu-id="4f208-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f208-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f208-105">Установите объект [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f208-105">Set a user's [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object.</span></span> <span data-ttu-id="4f208-106">Проверка подлинности электронной почты — это метод сброса пароля самообслуживления.</span><span class="sxs-lookup"><span data-stu-id="4f208-106">Email authentication is a self-service password reset method.</span></span> <span data-ttu-id="4f208-107">У пользователя может быть только один метод проверки подлинности электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4f208-107">A user may only have one email authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f208-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f208-108">Permissions</span></span>
<span data-ttu-id="4f208-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f208-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f208-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f208-111">Permission type</span></span>|<span data-ttu-id="4f208-112">Разрешения, действующие на себя (от наименее до самых привилегированных)</span><span class="sxs-lookup"><span data-stu-id="4f208-112">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="4f208-113">Разрешения, действующие на других (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="4f208-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="4f208-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f208-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f208-115">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4f208-115">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="4f208-116">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f208-116">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="4f208-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f208-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f208-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f208-118">Not supported.</span></span> | <span data-ttu-id="4f208-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f208-119">Not supported.</span></span> |
| <span data-ttu-id="4f208-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="4f208-120">Application</span></span>                            | <span data-ttu-id="4f208-121">Неприменимо.</span><span class="sxs-lookup"><span data-stu-id="4f208-121">Not applicable.</span></span> | <span data-ttu-id="4f208-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f208-122">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="4f208-123">Для делегирования сценариев, в которых администратор действует на другого пользователя, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="4f208-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="4f208-124">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="4f208-124">Global admin</span></span>
* <span data-ttu-id="4f208-125">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="4f208-125">Privileged authentication admin</span></span>
* <span data-ttu-id="4f208-126">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="4f208-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="4f208-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f208-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a><span data-ttu-id="4f208-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f208-128">Request headers</span></span>
|<span data-ttu-id="4f208-129">Имя</span><span class="sxs-lookup"><span data-stu-id="4f208-129">Name</span></span>|<span data-ttu-id="4f208-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4f208-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4f208-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f208-131">Authorization</span></span>|<span data-ttu-id="4f208-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f208-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4f208-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f208-134">Content-Type</span></span>|<span data-ttu-id="4f208-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f208-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f208-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f208-137">Request body</span></span>
<span data-ttu-id="4f208-138">В теле запроса укажи JSON-представление объекта [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) с нужным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4f208-138">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the desired email address.</span></span>

<span data-ttu-id="4f208-139">В следующей таблице показаны свойства, необходимые при создании [электронной почтыAuthenticationMethod.](../resources/emailauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="4f208-139">The following table shows the properties that are required when you create the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="4f208-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f208-140">Property</span></span>|<span data-ttu-id="4f208-141">Тип</span><span class="sxs-lookup"><span data-stu-id="4f208-141">Type</span></span>|<span data-ttu-id="4f208-142">Описание</span><span class="sxs-lookup"><span data-stu-id="4f208-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f208-143">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4f208-143">emailAddress</span></span>|<span data-ttu-id="4f208-144">String</span><span class="sxs-lookup"><span data-stu-id="4f208-144">String</span></span>|<span data-ttu-id="4f208-145">Адрес электронной почты</span><span class="sxs-lookup"><span data-stu-id="4f208-145">Email address</span></span>|



## <a name="response"></a><span data-ttu-id="4f208-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f208-146">Response</span></span>

<span data-ttu-id="4f208-147">В случае успешной работы этот метод возвращает код отклика и новый объект `201 Created` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4f208-147">If successful, this method returns a `201 Created` response code and a new [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f208-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="4f208-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f208-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f208-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4f208-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f208-150">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="4f208-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f208-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f208-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f208-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="4f208-153">C#</span><span class="sxs-lookup"><span data-stu-id="4f208-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f208-154">Java</span><span class="sxs-lookup"><span data-stu-id="4f208-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-emailauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="4f208-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f208-155">Response</span></span>
<span data-ttu-id="4f208-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4f208-156">The following is an example of the response.</span></span>

<span data-ttu-id="4f208-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4f208-157">**Note:** The response object shown here might be shortened for readability.</span></span>
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
