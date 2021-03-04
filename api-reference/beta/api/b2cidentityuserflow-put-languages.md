---
title: Создание языков
description: Создание настраиваемого языка в потоке пользователей Azure AD B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e24841cebf0385563a1445a576cda8e8609f40c7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438192"
---
# <a name="create-languages"></a><span data-ttu-id="43b1a-103">Создание языков</span><span class="sxs-lookup"><span data-stu-id="43b1a-103">Create languages</span></span>

<span data-ttu-id="43b1a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43b1a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="43b1a-105">Этот метод используется для создания или обновления настраиваемого языка в потоке пользователей Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="43b1a-105">This method is used to create or update a custom language in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="43b1a-106">**Примечание:** Прежде чем создать настраиваемый язык, необходимо включить настройку языка в потоке пользователей Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="43b1a-106">**Note:** You must enable language customization in the Azure AD B2C user flow before you can create a custom language.</span></span> <span data-ttu-id="43b1a-107">Дополнительные сведения см. [в обновлении b2cIdentityUserFlow.](../api/b2cidentityuserflow-update.md)</span><span class="sxs-lookup"><span data-stu-id="43b1a-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="43b1a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43b1a-108">Permissions</span></span>

<span data-ttu-id="43b1a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43b1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43b1a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43b1a-111">Permission type</span></span>      | <span data-ttu-id="43b1a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43b1a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43b1a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43b1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="43b1a-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43b1a-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="43b1a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43b1a-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="43b1a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43b1a-116">Not supported.</span></span>|
|<span data-ttu-id="43b1a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="43b1a-117">Application</span></span>|<span data-ttu-id="43b1a-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43b1a-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="43b1a-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="43b1a-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="43b1a-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="43b1a-120">Global administrator</span></span>
* <span data-ttu-id="43b1a-121">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="43b1a-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="43b1a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43b1a-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="43b1a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43b1a-123">Request headers</span></span>

|<span data-ttu-id="43b1a-124">Имя</span><span class="sxs-lookup"><span data-stu-id="43b1a-124">Name</span></span>|<span data-ttu-id="43b1a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="43b1a-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="43b1a-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43b1a-126">Authorization</span></span>|<span data-ttu-id="43b1a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43b1a-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="43b1a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43b1a-129">Content-Type</span></span>|<span data-ttu-id="43b1a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43b1a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="43b1a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43b1a-132">Request body</span></span>

<span data-ttu-id="43b1a-133">В теле запроса предоставляем представление JSON объекта [userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43b1a-133">In the request body, supply a JSON representation of the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span>

<span data-ttu-id="43b1a-134">В следующей таблице показаны свойства, которые можно дополнительно предоставлять при создании [userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="43b1a-134">The following table shows the properties that can be optionally provided when you create the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md).</span></span>

|<span data-ttu-id="43b1a-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="43b1a-135">Property</span></span>|<span data-ttu-id="43b1a-136">Тип</span><span class="sxs-lookup"><span data-stu-id="43b1a-136">Type</span></span>|<span data-ttu-id="43b1a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="43b1a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43b1a-138">id</span><span class="sxs-lookup"><span data-stu-id="43b1a-138">id</span></span>|<span data-ttu-id="43b1a-139">String</span><span class="sxs-lookup"><span data-stu-id="43b1a-139">String</span></span>|<span data-ttu-id="43b1a-140">Идентификатор языка.</span><span class="sxs-lookup"><span data-stu-id="43b1a-140">The identifier of the language.</span></span> <span data-ttu-id="43b1a-141">Это поле — тег языкового [ID RFC 5646,](https://tools.ietf.org/html/rfc5646) который должен быть документированным языковым ИД.</span><span class="sxs-lookup"><span data-stu-id="43b1a-141">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span> <span data-ttu-id="43b1a-142">Если оно предоставлено в теле запроса, оно должно соответствовать identifer, предоставленного в URL-адресе запроса.</span><span class="sxs-lookup"><span data-stu-id="43b1a-142">If provided in the request body, it must match the identifer provided in the request URL.</span></span>|
|<span data-ttu-id="43b1a-143">isEnabled</span><span class="sxs-lookup"><span data-stu-id="43b1a-143">isEnabled</span></span>|<span data-ttu-id="43b1a-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="43b1a-144">Boolean</span></span>|<span data-ttu-id="43b1a-145">Указывает, включен ли язык в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="43b1a-145">Indicates whether the language is enabled within the user flow.</span></span> <span data-ttu-id="43b1a-146">Если это не предусмотрено в запросе, для isEnabled будет установлено "true".</span><span class="sxs-lookup"><span data-stu-id="43b1a-146">If this is not provided in the request, isEnabled will be set to 'true'.</span></span>|

## <a name="response"></a><span data-ttu-id="43b1a-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="43b1a-147">Response</span></span>

<span data-ttu-id="43b1a-148">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="43b1a-148">If successful, this method returns a `201 Created` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43b1a-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="43b1a-149">Examples</span></span>

### <a name="example-1-create-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="43b1a-150">Пример 1. Создание настраиваемого языка в потоке пользователей Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="43b1a-150">Example 1: Create a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="43b1a-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="43b1a-151">Request</span></span>

<span data-ttu-id="43b1a-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43b1a-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="43b1a-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="43b1a-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_userflowlanguageconfiguration_from_"
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
# <a name="c"></a>[<span data-ttu-id="43b1a-154">C#</span><span class="sxs-lookup"><span data-stu-id="43b1a-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowlanguageconfiguration-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43b1a-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43b1a-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowlanguageconfiguration-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43b1a-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43b1a-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowlanguageconfiguration-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43b1a-157">Java</span><span class="sxs-lookup"><span data-stu-id="43b1a-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowlanguageconfiguration-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="43b1a-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="43b1a-158">Response</span></span>

<span data-ttu-id="43b1a-159">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="43b1a-159">The following is an example of the response.</span></span>

<span data-ttu-id="43b1a-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="43b1a-160">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-update-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="43b1a-161">Пример 2. Обновление настраиваемого языка в потоке пользователей Azure AD B2C</span><span class="sxs-lookup"><span data-stu-id="43b1a-161">Example 2: Update a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="43b1a-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="43b1a-162">Request</span></span>

<span data-ttu-id="43b1a-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43b1a-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_userflowlanguageconfiguration_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages/es-ES
Content-Type: application/json

{
  "isEnabled": false
}
```

#### <a name="response"></a><span data-ttu-id="43b1a-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="43b1a-164">Response</span></span>

<span data-ttu-id="43b1a-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="43b1a-165">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
