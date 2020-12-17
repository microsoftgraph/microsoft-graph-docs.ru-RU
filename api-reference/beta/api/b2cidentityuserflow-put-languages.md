---
title: Создание языков
description: Создайте пользовательский язык в пользовательском потоке Azure AD B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a45e19b056b040d700bdb246e07eefee471342b2
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706332"
---
# <a name="create-languages"></a><span data-ttu-id="3d4ed-103">Создание языков</span><span class="sxs-lookup"><span data-stu-id="3d4ed-103">Create languages</span></span>

<span data-ttu-id="3d4ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d4ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3d4ed-105">Этот метод используется для создания или обновления пользовательского языка в пользовательском потоке Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-105">This method is used to create or update a custom language in an Azure AD B2C user flow.</span></span>

<span data-ttu-id="3d4ed-106">**Примечание.** Перед созданием настраиваемого языка необходимо включить настройку языка в пользовательском потоке Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-106">**Note:** You must enable language customization in the Azure AD B2C user flow before you can create a custom language.</span></span> <span data-ttu-id="3d4ed-107">Дополнительные сведения [см. в обновлении b2cIdentityUserFlow.](../api/b2cidentityuserflow-update.md)</span><span class="sxs-lookup"><span data-stu-id="3d4ed-107">For more information, see [Update b2cIdentityUserFlow](../api/b2cidentityuserflow-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3d4ed-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d4ed-108">Permissions</span></span>

<span data-ttu-id="3d4ed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d4ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d4ed-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d4ed-111">Permission type</span></span>      | <span data-ttu-id="3d4ed-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d4ed-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d4ed-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d4ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d4ed-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d4ed-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="3d4ed-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d4ed-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3d4ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-116">Not supported.</span></span>|
|<span data-ttu-id="3d4ed-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3d4ed-117">Application</span></span>|<span data-ttu-id="3d4ed-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d4ed-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="3d4ed-119">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="3d4ed-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="3d4ed-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="3d4ed-120">Global administrator</span></span>
* <span data-ttu-id="3d4ed-121">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="3d4ed-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3d4ed-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d4ed-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3d4ed-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d4ed-123">Request headers</span></span>

|<span data-ttu-id="3d4ed-124">Имя</span><span class="sxs-lookup"><span data-stu-id="3d4ed-124">Name</span></span>|<span data-ttu-id="3d4ed-125">Описание</span><span class="sxs-lookup"><span data-stu-id="3d4ed-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3d4ed-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d4ed-126">Authorization</span></span>|<span data-ttu-id="3d4ed-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3d4ed-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3d4ed-129">Content-Type</span></span>|<span data-ttu-id="3d4ed-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d4ed-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d4ed-132">Request body</span></span>

<span data-ttu-id="3d4ed-133">В теле запроса предоставляем представление объекта [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-133">In the request body, supply a JSON representation of the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object.</span></span>

<span data-ttu-id="3d4ed-134">В следующей таблице показаны свойства, которые можно предоставлять при создании [объекта userFlowLanguageConfiguration.](../resources/userflowlanguageconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3d4ed-134">The following table shows the properties that can be optionally provided when you create the [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md).</span></span>

|<span data-ttu-id="3d4ed-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d4ed-135">Property</span></span>|<span data-ttu-id="3d4ed-136">Тип</span><span class="sxs-lookup"><span data-stu-id="3d4ed-136">Type</span></span>|<span data-ttu-id="3d4ed-137">Описание</span><span class="sxs-lookup"><span data-stu-id="3d4ed-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d4ed-138">id</span><span class="sxs-lookup"><span data-stu-id="3d4ed-138">id</span></span>|<span data-ttu-id="3d4ed-139">String</span><span class="sxs-lookup"><span data-stu-id="3d4ed-139">String</span></span>|<span data-ttu-id="3d4ed-140">Идентификатор языка.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-140">The identifier of the language.</span></span> <span data-ttu-id="3d4ed-141">Это поле является тегом языка, совместимым с [RFC 5646,](https://tools.ietf.org/html/rfc5646) и должно быть документированным ИД языка.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-141">This field is Language ID tag [RFC 5646](https://tools.ietf.org/html/rfc5646) compliant and must be a documented Language ID.</span></span> <span data-ttu-id="3d4ed-142">Если он указан в теле запроса, он должен соответствовать отступу, предоставленного в URL-адресе запроса.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-142">If provided in the request body, it must match the identifer provided in the request URL.</span></span>|
|<span data-ttu-id="3d4ed-143">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3d4ed-143">isEnabled</span></span>|<span data-ttu-id="3d4ed-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d4ed-144">Boolean</span></span>|<span data-ttu-id="3d4ed-145">Указывает, включен ли язык в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-145">Indicates whether the language is enabled within the user flow.</span></span> <span data-ttu-id="3d4ed-146">Если это не предоставлено в запросе, для isEnabled будет установлено "true".</span><span class="sxs-lookup"><span data-stu-id="3d4ed-146">If this is not provided in the request, isEnabled will be set to 'true'.</span></span>|

## <a name="response"></a><span data-ttu-id="3d4ed-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d4ed-147">Response</span></span>

<span data-ttu-id="3d4ed-148">В случае успеха этот метод возвращает код отклика и объект `201 Created` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-148">If successful, this method returns a `201 Created` response code and a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3d4ed-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="3d4ed-149">Examples</span></span>

### <a name="example-1-create-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="3d4ed-150">Пример 1. Создание настраиваемого языка в пользовательском потоке B2C Azure AD</span><span class="sxs-lookup"><span data-stu-id="3d4ed-150">Example 1: Create a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="3d4ed-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d4ed-151">Request</span></span>

<span data-ttu-id="3d4ed-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-152">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="3d4ed-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d4ed-153">Response</span></span>

<span data-ttu-id="3d4ed-154">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-154">The following is an example of the response.</span></span>

<span data-ttu-id="3d4ed-155">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-155">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-update-a-custom-language-in-an-azure-ad-b2c-user-flow"></a><span data-ttu-id="3d4ed-156">Пример 2. Обновление настраиваемого языка в пользовательском потоке B2C Azure AD</span><span class="sxs-lookup"><span data-stu-id="3d4ed-156">Example 2: Update a custom language in an Azure AD B2C user flow</span></span>

#### <a name="request"></a><span data-ttu-id="3d4ed-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d4ed-157">Request</span></span>

<span data-ttu-id="3d4ed-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-158">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="3d4ed-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d4ed-159">Response</span></span>

<span data-ttu-id="3d4ed-160">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3d4ed-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
