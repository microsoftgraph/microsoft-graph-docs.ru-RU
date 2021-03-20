---
title: Создание языков
description: Создание настраиваемого языка в потоке пользователей Azure AD B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1aa49de8c9e32952921413ca64325b39e0dff5fc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944653"
---
# <a name="create-languages"></a><span data-ttu-id="37f38-103">Создание языков</span><span class="sxs-lookup"><span data-stu-id="37f38-103">Create languages</span></span>

<span data-ttu-id="37f38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37f38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37f38-105">Этот метод используется для создания или обновления настраиваемого языка в потоке пользователей Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="37f38-105">This method is used to create or update a custom language in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="37f38-106">**Примечание:** Прежде чем создать настраиваемый язык, необходимо включить настройку языка в потоке пользователей Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="37f38-106">**Note:** You must enable language customization in the Azure AD B2C user flow before you can create a custom language.</span></span> <span data-ttu-id="37f38-107">Дополнительные сведения см. [в обновлении b2cIdentityUserFlow.](../api/b2cidentityuserflow-update.md)</span><span class="sxs-lookup"><span data-stu-id="37f38-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="37f38-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37f38-108">Permissions</span></span>

<span data-ttu-id="37f38-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37f38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37f38-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37f38-111">Permission type</span></span>      | <span data-ttu-id="37f38-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37f38-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37f38-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37f38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37f38-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37f38-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="37f38-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37f38-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="37f38-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37f38-116">Not supported.</span></span>|
|<span data-ttu-id="37f38-117">Application</span><span class="sxs-lookup"><span data-stu-id="37f38-117">Application</span></span>|<span data-ttu-id="37f38-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37f38-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="37f38-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="37f38-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="37f38-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="37f38-120">Global administrator</span></span>
* <span data-ttu-id="37f38-121">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="37f38-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="37f38-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37f38-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="37f38-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37f38-123">Request headers</span></span>

|<span data-ttu-id="37f38-124">Имя</span><span class="sxs-lookup"><span data-stu-id="37f38-124">Name</span></span>|<span data-ttu-id="37f38-125">Описание</span><span class="sxs-lookup"><span data-stu-id="37f38-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="37f38-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="37f38-126">Authorization</span></span>|<span data-ttu-id="37f38-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37f38-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="37f38-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="37f38-129">Content-Type</span></span>|<span data-ttu-id="37f38-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="37f38-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37f38-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="37f38-132">Request body</span></span>

<span data-ttu-id="37f38-133">В теле запроса предоставляем представление JSON объекта [userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37f38-133">In the request body, supply a JSON representation of the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span>

<span data-ttu-id="37f38-134">В следующей таблице показаны свойства, которые можно дополнительно предоставлять при создании [userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37f38-134">The following table shows the properties that can be optionally provided when you create the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md).</span></span>

|<span data-ttu-id="37f38-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="37f38-135">Property</span></span>|<span data-ttu-id="37f38-136">Тип</span><span class="sxs-lookup"><span data-stu-id="37f38-136">Type</span></span>|<span data-ttu-id="37f38-137">Описание</span><span class="sxs-lookup"><span data-stu-id="37f38-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37f38-138">id</span><span class="sxs-lookup"><span data-stu-id="37f38-138">id</span></span>|<span data-ttu-id="37f38-139">Строка</span><span class="sxs-lookup"><span data-stu-id="37f38-139">String</span></span>|<span data-ttu-id="37f38-140">Идентификатор языка.</span><span class="sxs-lookup"><span data-stu-id="37f38-140">The identifier of the language.</span></span> <span data-ttu-id="37f38-141">Это поле — тег языкового [ID RFC 5646,](https://tools.ietf.org/html/rfc5646) который должен быть документированным языковым ИД.</span><span class="sxs-lookup"><span data-stu-id="37f38-141">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span> <span data-ttu-id="37f38-142">Если оно предоставлено в теле запроса, оно должно соответствовать identifer, предоставленного в URL-адресе запроса.</span><span class="sxs-lookup"><span data-stu-id="37f38-142">If provided in the request body, it must match the identifer provided in the request URL.</span></span>|
|<span data-ttu-id="37f38-143">isEnabled</span><span class="sxs-lookup"><span data-stu-id="37f38-143">isEnabled</span></span>|<span data-ttu-id="37f38-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="37f38-144">Boolean</span></span>|<span data-ttu-id="37f38-145">Указывает, включен ли язык в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="37f38-145">Indicates whether the language is enabled within the user flow.</span></span> <span data-ttu-id="37f38-146">Если это не предусмотрено в запросе, для isEnabled будет установлено "true".</span><span class="sxs-lookup"><span data-stu-id="37f38-146">If this is not provided in the request, isEnabled will be set to 'true'.</span></span>|

## <a name="response"></a><span data-ttu-id="37f38-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="37f38-147">Response</span></span>

<span data-ttu-id="37f38-148">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="37f38-148">If successful, this method returns a `201 Created` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37f38-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="37f38-149">Examples</span></span>

### <a name="example-1-create-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="37f38-150">Пример 1. Создание настраиваемого языка в потоке пользователей Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="37f38-150">Example 1: Create a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="37f38-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="37f38-151">Request</span></span>

<span data-ttu-id="37f38-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37f38-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="37f38-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="37f38-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_userflowlanguageconfiguration_from__1"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES
Content-Type: application/json

{
  "id": "es-ES",
  "isEnabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="37f38-154">C#</span><span class="sxs-lookup"><span data-stu-id="37f38-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowlanguageconfiguration-from--1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37f38-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37f38-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowlanguageconfiguration-from--1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37f38-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37f38-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowlanguageconfiguration-from--1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37f38-157">Java</span><span class="sxs-lookup"><span data-stu-id="37f38-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowlanguageconfiguration-from--1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37f38-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="37f38-158">Response</span></span>

<span data-ttu-id="37f38-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="37f38-159">The following is an example of the response.</span></span>

<span data-ttu-id="37f38-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="37f38-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowLanguageConfiguration"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('B2C_1_CustomerSignUp')/languages/$entity",
  "id": "es-ES",
  "isEnabled": true,
  "displayName": "Spanish (Spain)"
}
```

### <a name="example-2-update-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="37f38-161">Пример 2. Обновление настраиваемого языка в потоке пользователей Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="37f38-161">Example 2: Update a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="37f38-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="37f38-162">Request</span></span>

<span data-ttu-id="37f38-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="37f38-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="37f38-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="37f38-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_userflowlanguageconfiguration_from__2"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES
Content-Type: application/json

{
  "isEnabled": false
}
```
# <a name="c"></a>[<span data-ttu-id="37f38-165">C#</span><span class="sxs-lookup"><span data-stu-id="37f38-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowlanguageconfiguration-from--2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37f38-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37f38-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowlanguageconfiguration-from--2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37f38-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37f38-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowlanguageconfiguration-from--2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37f38-168">Java</span><span class="sxs-lookup"><span data-stu-id="37f38-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowlanguageconfiguration-from--2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37f38-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="37f38-169">Response</span></span>

<span data-ttu-id="37f38-170">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="37f38-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
