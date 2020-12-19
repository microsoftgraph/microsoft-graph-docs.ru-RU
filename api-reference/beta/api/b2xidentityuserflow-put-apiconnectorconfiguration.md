---
title: Настройка соединители API в пользовательском потоке
description: Включив или отключив соединители API для определенного шага в пользовательском потоке, обновив свойство apiConnectorConfiguration.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6291c0205f69090a22d33cec847087731af75304
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720359"
---
# <a name="configure-userflowapiconnectorconfiguration"></a><span data-ttu-id="5529b-103">Настройка userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="5529b-103">Configure userFlowApiConnectorConfiguration</span></span>

<span data-ttu-id="5529b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5529b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5529b-105">Обновите свойство [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) в [потоке b2xIdentityUserFlow,](../resources/b2xidentityuserflow.md) чтобы включить или отключить соединители API в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="5529b-105">Update the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) to enable or disable an API connector in a user flow.</span></span> <span data-ttu-id="5529b-106">Каждая связь [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) соответствует определенному шагу в пользовательском потоке, который можно настроить для вызова соединителя API.</span><span class="sxs-lookup"><span data-stu-id="5529b-106">Each relationship of the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span> <span data-ttu-id="5529b-107">Соединители API настраиваются для определенного шага по одному, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="5529b-107">You configure an API connector for a particular step one at a time as shown below.</span></span>

## <a name="permissions"></a><span data-ttu-id="5529b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5529b-108">Permissions</span></span>

<span data-ttu-id="5529b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5529b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5529b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5529b-111">Permission type</span></span>|<span data-ttu-id="5529b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5529b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5529b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5529b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5529b-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5529b-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="5529b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5529b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5529b-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="5529b-116">Not supported</span></span>|
|<span data-ttu-id="5529b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5529b-117">Application</span></span>|<span data-ttu-id="5529b-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5529b-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="5529b-119">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="5529b-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="5529b-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="5529b-120">Global administrator</span></span>
* <span data-ttu-id="5529b-121">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="5529b-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="5529b-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5529b-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2xUserFlows/{b2xUserFlowId}/apiConnectorConfiguration/{step}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5529b-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5529b-123">Request headers</span></span>

|<span data-ttu-id="5529b-124">Имя</span><span class="sxs-lookup"><span data-stu-id="5529b-124">Name</span></span>|<span data-ttu-id="5529b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="5529b-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5529b-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5529b-126">Authorization</span></span>|<span data-ttu-id="5529b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5529b-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5529b-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5529b-129">Content-Type</span></span>|<span data-ttu-id="5529b-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5529b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5529b-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5529b-132">Request body</span></span>

<span data-ttu-id="5529b-133">В теле запроса укажите представление идентификатора `id` [IdentityApiConnector](../resources/identityapiconnector.md) в JSON, который вы хотите использовать для конкретного шага.</span><span class="sxs-lookup"><span data-stu-id="5529b-133">In the request body, provide a JSON representation of the `id` of the [identityApiConnector](../resources/identityapiconnector.md) you want to use the particular step.</span></span> <span data-ttu-id="5529b-134">Чтобы отключить соединители API, можно использовать значение {} .</span><span class="sxs-lookup"><span data-stu-id="5529b-134">To disable an API connector, the value can be {}.</span></span>

## <a name="response"></a><span data-ttu-id="5529b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5529b-135">Response</span></span>

<span data-ttu-id="5529b-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="5529b-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5529b-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="5529b-137">Examples</span></span>

### <a name="example-1-enable-api-connector-for-post-idp-federation-on-sign-up"></a><span data-ttu-id="5529b-138">Пример 1. Enable API connector for Post IDP Federation on sign up</span><span class="sxs-lookup"><span data-stu-id="5529b-138">Example 1: Enable API connector for Post IDP Federation on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="5529b-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="5529b-139">Request</span></span>

<span data-ttu-id="5529b-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5529b-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postFederationSignup"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
}
```

---

#### <a name="response"></a><span data-ttu-id="5529b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5529b-141">Response</span></span> 

<span data-ttu-id="5529b-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5529b-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="5529b-143">Пример 2. Enable API connector for Post Attribute Collection on sign up</span><span class="sxs-lookup"><span data-stu-id="5529b-143">Example 2: Enable API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="5529b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="5529b-144">Request</span></span> 

<span data-ttu-id="5529b-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5529b-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identity/apiConnectors/{id}"   
}
```

#### <a name="response"></a><span data-ttu-id="5529b-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5529b-146">Response</span></span>

<span data-ttu-id="5529b-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5529b-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-an-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="5529b-148">Пример 3. Отключение соединители API для коллекции атрибутов Post при регистрации</span><span class="sxs-lookup"><span data-stu-id="5529b-148">Example 3: Disable an API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="5529b-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="5529b-149">Request</span></span> 

<span data-ttu-id="5529b-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5529b-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_disable-postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{ }
```

#### <a name="response"></a><span data-ttu-id="5529b-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="5529b-151">Response</span></span>

<span data-ttu-id="5529b-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5529b-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
