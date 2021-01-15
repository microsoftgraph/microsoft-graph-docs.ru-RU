---
title: Создание emailAuthenticationMethod
description: Создание объекта emailAuthenticationMethod.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 451b49ddcabb72736a67cbcb08391fb0bd45cf27
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872172"
---
# <a name="create-emailauthenticationmethod"></a><span data-ttu-id="fed44-103">Создание emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fed44-103">Create emailAuthenticationMethod</span></span>
<span data-ttu-id="fed44-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fed44-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fed44-105">Настройка объекта [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="fed44-105">Set a user's [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object.</span></span> <span data-ttu-id="fed44-106">Проверка подлинности электронной почты — это метод самостоятельного сброса пароля.</span><span class="sxs-lookup"><span data-stu-id="fed44-106">Email authentication is a self-service password reset method.</span></span> <span data-ttu-id="fed44-107">У пользователя может быть только один метод проверки подлинности электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fed44-107">A user may only have one email authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="fed44-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fed44-108">Permissions</span></span>
<span data-ttu-id="fed44-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fed44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fed44-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fed44-111">Permission type</span></span>|<span data-ttu-id="fed44-112">Разрешения, действующие на себя (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="fed44-112">Permissions acting on self (from least to most privileged)</span></span>|<span data-ttu-id="fed44-113">Разрешения, действующие над другими (от наименее привилегированных)</span><span class="sxs-lookup"><span data-stu-id="fed44-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
| <span data-ttu-id="fed44-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fed44-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="fed44-115">UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fed44-115">UserAuthenticationMethod.ReadWrite</span></span> | <span data-ttu-id="fed44-116">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fed44-116">UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="fed44-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fed44-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fed44-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fed44-118">Not supported.</span></span> | <span data-ttu-id="fed44-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fed44-119">Not supported.</span></span> |
| <span data-ttu-id="fed44-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="fed44-120">Application</span></span>                            | <span data-ttu-id="fed44-121">Не применимо.</span><span class="sxs-lookup"><span data-stu-id="fed44-121">Not applicable.</span></span> | <span data-ttu-id="fed44-122">UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fed44-122">UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="fed44-123">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна из следующих [ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="fed44-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="fed44-124">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="fed44-124">Global admin</span></span>
* <span data-ttu-id="fed44-125">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="fed44-125">Privileged authentication admin</span></span>
* <span data-ttu-id="fed44-126">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="fed44-126">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="fed44-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fed44-127">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a><span data-ttu-id="fed44-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fed44-128">Request headers</span></span>
|<span data-ttu-id="fed44-129">Имя</span><span class="sxs-lookup"><span data-stu-id="fed44-129">Name</span></span>|<span data-ttu-id="fed44-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fed44-130">Description</span></span>|
|:---|:---|
|<span data-ttu-id="fed44-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fed44-131">Authorization</span></span>|<span data-ttu-id="fed44-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fed44-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="fed44-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fed44-134">Content-Type</span></span>|<span data-ttu-id="fed44-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fed44-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fed44-137">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="fed44-137">Request body</span></span>
<span data-ttu-id="fed44-138">В теле запроса укажите представление объекта [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в JSON с нужным адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fed44-138">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the desired email address.</span></span>

<span data-ttu-id="fed44-139">В следующей таблице показаны свойства, необходимые при создании [объекта emailAuthenticationMethod.](../resources/emailauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="fed44-139">The following table shows the properties that are required when you create the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="fed44-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="fed44-140">Property</span></span>|<span data-ttu-id="fed44-141">Тип</span><span class="sxs-lookup"><span data-stu-id="fed44-141">Type</span></span>|<span data-ttu-id="fed44-142">Описание</span><span class="sxs-lookup"><span data-stu-id="fed44-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fed44-143">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fed44-143">emailAddress</span></span>|<span data-ttu-id="fed44-144">String</span><span class="sxs-lookup"><span data-stu-id="fed44-144">String</span></span>|<span data-ttu-id="fed44-145">адрес электронной почты;</span><span class="sxs-lookup"><span data-stu-id="fed44-145">Email address</span></span>|



## <a name="response"></a><span data-ttu-id="fed44-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="fed44-146">Response</span></span>

<span data-ttu-id="fed44-147">В случае успеха этот метод возвращает код отклика и новый объект `201 Created` [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fed44-147">If successful, this method returns a `201 Created` response code and a new [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fed44-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="fed44-148">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fed44-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="fed44-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="fed44-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="fed44-150">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="fed44-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fed44-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-emailauthenticationmethod-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fed44-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fed44-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-emailauthenticationmethod-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="fed44-153">C#</span><span class="sxs-lookup"><span data-stu-id="fed44-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-emailauthenticationmethod-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fed44-154">Java</span><span class="sxs-lookup"><span data-stu-id="fed44-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-emailauthenticationmethod-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="fed44-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="fed44-155">Response</span></span>
<span data-ttu-id="fed44-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fed44-156">The following is an example of the response.</span></span>

<span data-ttu-id="fed44-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fed44-157">**Note:** The response object shown here might be shortened for readability.</span></span>
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
