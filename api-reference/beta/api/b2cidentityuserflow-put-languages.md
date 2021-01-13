---
title: Создание языков
description: Создайте пользовательский язык в пользовательском потоке Azure AD B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1edc89a4de37805bc150e2d0fc9f0a2c74b262da
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843929"
---
# <a name="create-languages"></a><span data-ttu-id="c1a35-103">Создание языков</span><span class="sxs-lookup"><span data-stu-id="c1a35-103">Create languages</span></span>

<span data-ttu-id="c1a35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1a35-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c1a35-105">Этот метод используется для создания или обновления пользовательского языка в пользовательском потоке Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="c1a35-105">This method is used to create or update a custom language in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="c1a35-106">**Примечание.** Перед созданием настраиваемого языка необходимо включить настройку языка в пользовательском потоке Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="c1a35-106">**Note:** You must enable language customization in the Azure AD B2C user flow before you can create a custom language.</span></span> <span data-ttu-id="c1a35-107">Дополнительные сведения [см. в обновлении b2cIdentityUserFlow.](../api/b2cidentityuserflow-update.md)</span><span class="sxs-lookup"><span data-stu-id="c1a35-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1a35-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1a35-108">Permissions</span></span>

<span data-ttu-id="c1a35-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1a35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1a35-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1a35-111">Permission type</span></span>      | <span data-ttu-id="c1a35-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1a35-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1a35-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1a35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1a35-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1a35-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="c1a35-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1a35-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="c1a35-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1a35-116">Not supported.</span></span>|
|<span data-ttu-id="c1a35-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c1a35-117">Application</span></span>|<span data-ttu-id="c1a35-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1a35-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="c1a35-119">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="c1a35-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="c1a35-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="c1a35-120">Global administrator</span></span>
* <span data-ttu-id="c1a35-121">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="c1a35-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="c1a35-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1a35-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c1a35-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1a35-123">Request headers</span></span>

|<span data-ttu-id="c1a35-124">Имя</span><span class="sxs-lookup"><span data-stu-id="c1a35-124">Name</span></span>|<span data-ttu-id="c1a35-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c1a35-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c1a35-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1a35-126">Authorization</span></span>|<span data-ttu-id="c1a35-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1a35-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c1a35-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1a35-129">Content-Type</span></span>|<span data-ttu-id="c1a35-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1a35-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1a35-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1a35-132">Request body</span></span>

<span data-ttu-id="c1a35-133">В теле запроса предоставляем представление объекта [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="c1a35-133">In the request body, supply a JSON representation of the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span>

<span data-ttu-id="c1a35-134">В следующей таблице показаны свойства, которые можно предоставлять при создании [объекта userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c1a35-134">The following table shows the properties that can be optionally provided when you create the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md).</span></span>

|<span data-ttu-id="c1a35-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1a35-135">Property</span></span>|<span data-ttu-id="c1a35-136">Тип</span><span class="sxs-lookup"><span data-stu-id="c1a35-136">Type</span></span>|<span data-ttu-id="c1a35-137">Описание</span><span class="sxs-lookup"><span data-stu-id="c1a35-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1a35-138">id</span><span class="sxs-lookup"><span data-stu-id="c1a35-138">id</span></span>|<span data-ttu-id="c1a35-139">String</span><span class="sxs-lookup"><span data-stu-id="c1a35-139">String</span></span>|<span data-ttu-id="c1a35-140">Идентификатор языка.</span><span class="sxs-lookup"><span data-stu-id="c1a35-140">The identifier of the language.</span></span> <span data-ttu-id="c1a35-141">Это поле является тегом языка, совместимым с [RFC 5646,](https://tools.ietf.org/html/rfc5646) и должно быть документированным ИД языка.</span><span class="sxs-lookup"><span data-stu-id="c1a35-141">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span> <span data-ttu-id="c1a35-142">Если он указан в теле запроса, он должен соответствовать отступу, предоставленного в URL-адресе запроса.</span><span class="sxs-lookup"><span data-stu-id="c1a35-142">If provided in the request body, it must match the identifer provided in the request URL.</span></span>|
|<span data-ttu-id="c1a35-143">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c1a35-143">isEnabled</span></span>|<span data-ttu-id="c1a35-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1a35-144">Boolean</span></span>|<span data-ttu-id="c1a35-145">Указывает, включен ли язык в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="c1a35-145">Indicates whether the language is enabled within the user flow.</span></span> <span data-ttu-id="c1a35-146">Если это не предоставлено в запросе, для isEnabled будет установлено "true".</span><span class="sxs-lookup"><span data-stu-id="c1a35-146">If this is not provided in the request, isEnabled will be set to 'true'.</span></span>|

## <a name="response"></a><span data-ttu-id="c1a35-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a35-147">Response</span></span>

<span data-ttu-id="c1a35-148">В случае успеха этот метод возвращает код отклика и объект `201 Created` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c1a35-148">If successful, this method returns a `201 Created` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1a35-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="c1a35-149">Examples</span></span>

### <a name="example-1-create-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="c1a35-150">Пример 1. Создание настраиваемого языка в пользовательском потоке B2C Azure AD</span><span class="sxs-lookup"><span data-stu-id="c1a35-150">Example 1: Create a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="c1a35-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1a35-151">Request</span></span>

<span data-ttu-id="c1a35-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1a35-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c1a35-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a35-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c1a35-154">C#</span><span class="sxs-lookup"><span data-stu-id="c1a35-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-userflowlanguageconfiguration-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1a35-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1a35-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-userflowlanguageconfiguration-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1a35-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1a35-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-userflowlanguageconfiguration-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1a35-157">Java</span><span class="sxs-lookup"><span data-stu-id="c1a35-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-userflowlanguageconfiguration-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1a35-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a35-158">Response</span></span>

<span data-ttu-id="c1a35-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c1a35-159">The following is an example of the response.</span></span>

<span data-ttu-id="c1a35-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c1a35-160">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-update-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="c1a35-161">Пример 2. Обновление настраиваемого языка в пользовательском потоке B2C Azure AD</span><span class="sxs-lookup"><span data-stu-id="c1a35-161">Example 2: Update a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="c1a35-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1a35-162">Request</span></span>

<span data-ttu-id="c1a35-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1a35-163">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c1a35-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1a35-164">Response</span></span>

<span data-ttu-id="c1a35-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c1a35-165">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
