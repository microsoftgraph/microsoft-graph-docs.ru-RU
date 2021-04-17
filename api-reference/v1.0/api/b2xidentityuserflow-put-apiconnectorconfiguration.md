---
title: Обновление apiConnectorConfiguration
description: Включить или отключить соединители API для определенного шага в потоке пользователей, обновив свойство apiConnectorConfiguration.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8c4b7cff6c1e6221bbece4e369c928b72eae705f
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883074"
---
# <a name="update-apiconnectorconfiguration"></a><span data-ttu-id="2d1d7-103">Обновление apiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="2d1d7-103">Update apiConnectorConfiguration</span></span>

<span data-ttu-id="2d1d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d1d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d1d7-105">[Обнови свойство apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) в [потоке b2xIdentityUserFlow,](../resources/b2xidentityuserflow.md) чтобы включить или отключить соединители API в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-105">Update the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) property in a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) to enable or disable an API connector in a user flow.</span></span> <span data-ttu-id="2d1d7-106">Каждое отношение [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) соответствует определенному шагу в потоке пользователей, который можно настроить для вызова соединителя API.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-106">Each relationship of the [apiConnectorConfiguration](../resources/userflowapiconnectorconfiguration.md) corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span> <span data-ttu-id="2d1d7-107">Вы настраивает соединители API для определенного шага одновременно, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-107">You configure an API connector for a particular step one at a time as shown below.</span></span>

## <a name="permissions"></a><span data-ttu-id="2d1d7-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d1d7-108">Permissions</span></span>

<span data-ttu-id="2d1d7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d1d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d1d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d1d7-111">Permission type</span></span>|<span data-ttu-id="2d1d7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d1d7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d1d7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d1d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2d1d7-114">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d1d7-114">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="2d1d7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d1d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d1d7-116">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="2d1d7-116">Not supported</span></span>|
|<span data-ttu-id="2d1d7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d1d7-117">Application</span></span>|<span data-ttu-id="2d1d7-118">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d1d7-118">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="2d1d7-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="2d1d7-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="2d1d7-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2d1d7-120">Global administrator</span></span>
* <span data-ttu-id="2d1d7-121">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="2d1d7-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="2d1d7-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d1d7-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PUT /identity/b2xUserFlows/{b2xUserFlowId}/apiConnectorConfiguration/{step}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2d1d7-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d1d7-123">Request headers</span></span>

|<span data-ttu-id="2d1d7-124">Имя</span><span class="sxs-lookup"><span data-stu-id="2d1d7-124">Name</span></span>|<span data-ttu-id="2d1d7-125">Описание</span><span class="sxs-lookup"><span data-stu-id="2d1d7-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2d1d7-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d1d7-126">Authorization</span></span>|<span data-ttu-id="2d1d7-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2d1d7-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2d1d7-129">Content-Type</span></span>|<span data-ttu-id="2d1d7-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d1d7-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d1d7-132">Request body</span></span>

<span data-ttu-id="2d1d7-133">В теле запроса уделяем JSON представление `id` [удостоверенияApiConnector,](../resources/identityapiconnector.md) который необходимо использовать для определенного шага.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-133">In the request body, provide a JSON representation of the `id` of the [identityApiConnector](../resources/identityapiconnector.md) you want to use the particular step.</span></span> <span data-ttu-id="2d1d7-134">Чтобы отключить соединители API, значение может быть {} .</span><span class="sxs-lookup"><span data-stu-id="2d1d7-134">To disable an API connector, the value can be {}.</span></span>

## <a name="response"></a><span data-ttu-id="2d1d7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d1d7-135">Response</span></span>

<span data-ttu-id="2d1d7-136">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2d1d7-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="2d1d7-137">Examples</span></span>

### <a name="example-1-enable-api-connector-for-post-idp-federation-on-sign-up"></a><span data-ttu-id="2d1d7-138">Пример 1. Включить соединители API для Федерации почтовых IDP при регистрации</span><span class="sxs-lookup"><span data-stu-id="2d1d7-138">Example 1: Enable API connector for Post IDP Federation on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="2d1d7-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d1d7-139">Request</span></span>

<span data-ttu-id="2d1d7-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postFederationSignup"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/v1.0/identity/apiConnectors/{id}"   
}
```

#### <a name="response"></a><span data-ttu-id="2d1d7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d1d7-141">Response</span></span> 

<span data-ttu-id="2d1d7-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-enable-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="2d1d7-143">Пример 2. Включить соединители API для коллекции атрибутов post при регистрации</span><span class="sxs-lookup"><span data-stu-id="2d1d7-143">Example 2: Enable API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="2d1d7-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d1d7-144">Request</span></span> 

<span data-ttu-id="2d1d7-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-145">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{
    "@odata.id": "https://graph.microsoft.com/v1.0/identity/apiConnectors/{id}"   
}
```

#### <a name="response"></a><span data-ttu-id="2d1d7-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d1d7-146">Response</span></span>

<span data-ttu-id="2d1d7-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-disable-an-api-connector-for-post-attribute-collection-on-sign-up"></a><span data-ttu-id="2d1d7-148">Пример 3. Отключение соединители API для коллекции атрибутов post при регистрации</span><span class="sxs-lookup"><span data-stu-id="2d1d7-148">Example 3: Disable an API connector for Post Attribute Collection on sign up</span></span>

#### <a name="request"></a><span data-ttu-id="2d1d7-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d1d7-149">Request</span></span> 

<span data-ttu-id="2d1d7-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-150">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "put_b2xuserflows-apiconnectorconfiguration_disable-postAttributeCollection"
}
-->

``` http
PUT https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postAttributeCollection/$ref
Content-Type: application/json

{ }
```

#### <a name="response"></a><span data-ttu-id="2d1d7-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d1d7-151">Response</span></span>

<span data-ttu-id="2d1d7-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2d1d7-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
