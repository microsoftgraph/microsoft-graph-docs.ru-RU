---
title: Создание b2xIdentityUserFlow
description: Создайте новый объект b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: b5f5d702a7707e942db6bbd6dd85eca02e26eb49
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883342"
---
# <a name="create-b2xidentityuserflow"></a><span data-ttu-id="6ab56-103">Создание b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="6ab56-103">Create b2xIdentityUserFlow</span></span>

<span data-ttu-id="6ab56-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ab56-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6ab56-105">Создайте [новый объект b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="6ab56-105">Create a new [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ab56-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ab56-106">Permissions</span></span>

<span data-ttu-id="6ab56-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ab56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ab56-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ab56-109">Permission type</span></span>      | <span data-ttu-id="6ab56-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ab56-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ab56-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ab56-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6ab56-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ab56-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="6ab56-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ab56-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6ab56-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ab56-114">Not supported.</span></span>|
|<span data-ttu-id="6ab56-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ab56-115">Application</span></span>|<span data-ttu-id="6ab56-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ab56-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="6ab56-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="6ab56-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="6ab56-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="6ab56-118">Global administrator</span></span>
* <span data-ttu-id="6ab56-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="6ab56-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="6ab56-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ab56-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlows
```

## <a name="request-headers"></a><span data-ttu-id="6ab56-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ab56-121">Request headers</span></span>

|<span data-ttu-id="6ab56-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6ab56-122">Name</span></span>|<span data-ttu-id="6ab56-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6ab56-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="6ab56-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6ab56-124">Authorization</span></span>|<span data-ttu-id="6ab56-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ab56-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6ab56-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6ab56-127">Content-Type</span></span>|<span data-ttu-id="6ab56-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ab56-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ab56-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ab56-130">Request body</span></span>

<span data-ttu-id="6ab56-131">В теле запроса предостерегать представление [JSON b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="6ab56-131">In the request body, provide a JSON representation of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md).</span></span>

|<span data-ttu-id="6ab56-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ab56-132">Property</span></span>|<span data-ttu-id="6ab56-133">Тип</span><span class="sxs-lookup"><span data-stu-id="6ab56-133">Type</span></span>|<span data-ttu-id="6ab56-134">Описание</span><span class="sxs-lookup"><span data-stu-id="6ab56-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ab56-135">id</span><span class="sxs-lookup"><span data-stu-id="6ab56-135">id</span></span>|<span data-ttu-id="6ab56-136">String</span><span class="sxs-lookup"><span data-stu-id="6ab56-136">String</span></span>|<span data-ttu-id="6ab56-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ab56-137">Required.</span></span> <span data-ttu-id="6ab56-138">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="6ab56-138">The name of the user flow.</span></span> <span data-ttu-id="6ab56-139">После создания имя будет предварительно заранее. `B2X_1`</span><span class="sxs-lookup"><span data-stu-id="6ab56-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="6ab56-140">userFlowType</span><span class="sxs-lookup"><span data-stu-id="6ab56-140">userFlowType</span></span>|<span data-ttu-id="6ab56-141">Строка</span><span class="sxs-lookup"><span data-stu-id="6ab56-141">String</span></span>|<span data-ttu-id="6ab56-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ab56-142">Required.</span></span> <span data-ttu-id="6ab56-143">Тип пользовательского потока, который вы создаете.</span><span class="sxs-lookup"><span data-stu-id="6ab56-143">The type of user flow you are creating.</span></span> <span data-ttu-id="6ab56-144">Это значение всегда будет `signUpOrSignIn` .</span><span class="sxs-lookup"><span data-stu-id="6ab56-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="6ab56-145">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="6ab56-145">userFlowTypeVersion</span></span>|<span data-ttu-id="6ab56-146">С плавающей запятой</span><span class="sxs-lookup"><span data-stu-id="6ab56-146">Float</span></span>|<span data-ttu-id="6ab56-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="6ab56-147">Required.</span></span> <span data-ttu-id="6ab56-148">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="6ab56-148">The version of the user flow.</span></span> <span data-ttu-id="6ab56-149">Это значение всегда будет 1.</span><span class="sxs-lookup"><span data-stu-id="6ab56-149">This value will always be 1.</span></span>|
|<span data-ttu-id="6ab56-150">apiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ab56-150">apiConnectorConfiguration</span></span>|[<span data-ttu-id="6ab56-151">userFlowApiConnectorConfiguration</span><span class="sxs-lookup"><span data-stu-id="6ab56-151">userFlowApiConnectorConfiguration</span></span>](../resources/userflowapiconnectorconfiguration.md)|<span data-ttu-id="6ab56-152">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="6ab56-152">Optional.</span></span> <span data-ttu-id="6ab56-153">Настройка для включения соединителя API с целью использования в составе пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="6ab56-153">Configuration for enabling an API connector for use as part of the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="6ab56-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ab56-154">Response</span></span>

<span data-ttu-id="6ab56-155">В случае успеха этот метод возвращает код отклика и заголовку Location с URI на объект `201 Created` [b2xIdentityUserFlow,](../resources/b2xidentityuserflow.md) созданный для этого запроса, с префиксом, добавленным в `B2X_1` имя.</span><span class="sxs-lookup"><span data-stu-id="6ab56-155">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="6ab56-156">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="6ab56-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="6ab56-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="6ab56-157">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="6ab56-158">Пример 1. Создание пользовательского потока со значениями по умолчанию</span><span class="sxs-lookup"><span data-stu-id="6ab56-158">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="6ab56-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ab56-159">Request</span></span>

<span data-ttu-id="6ab56-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ab56-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

#### <a name="response"></a><span data-ttu-id="6ab56-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ab56-161">Response</span></span>

<span data-ttu-id="6ab56-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ab56-162">The following is an example of the response.</span></span>

<span data-ttu-id="6ab56-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6ab56-163">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="6ab56-164">Пример 2. Создание пользовательского потока со значениями по умолчанию и поставщиком удостоверений</span><span class="sxs-lookup"><span data-stu-id="6ab56-164">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="6ab56-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ab56-165">Request</span></span>

<span data-ttu-id="6ab56-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ab56-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_identityProviders"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "identityProviders": [
        {
            "id": "Facebook-OAuth",
            "type": "Facebook",
            "name": "Facebook"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="6ab56-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ab56-167">Response</span></span>

<span data-ttu-id="6ab56-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ab56-168">The following is an example of the response.</span></span>

<span data-ttu-id="6ab56-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6ab56-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-3-create-a-user-flow-with-the-default-values-and-configuration-for-api-connectors"></a><span data-ttu-id="6ab56-170">Пример 3. Создание пользовательского потока с значениями по умолчанию и конфигурацией для соединителов API</span><span class="sxs-lookup"><span data-stu-id="6ab56-170">Example 3: Create a user flow with the default values and configuration for API connectors</span></span>

#### <a name="request"></a><span data-ttu-id="6ab56-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ab56-171">Request</span></span>

<span data-ttu-id="6ab56-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ab56-172">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_apiconnectors"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration":{
        "postFederationSignup":{
            "@odata.id": "https://graph.microsoft.com/v1/identity/apiConnectors/{id}"
        },
        "postAttributeCollection":{
            "@odata.id": "https://graph.microsoft.com/v1/identity/apiConnectors/{id}"
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="6ab56-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ab56-173">Response</span></span>

<span data-ttu-id="6ab56-174">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ab56-174">The following is an example of the response.</span></span>

<span data-ttu-id="6ab56-175">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6ab56-175">**Note:** The response object shown here might be shortened for readability.</span></span>

<span data-ttu-id="6ab56-176">**Примечание:** Свойство `apiConnectorConfiguration` всегда возвращает значение {} '.</span><span class="sxs-lookup"><span data-stu-id="6ab56-176">**Note:** The `apiConnectorConfiguration` property always returns a '{}' value.</span></span> <span data-ttu-id="6ab56-177">Чтобы увидеть полное значение свойств навигации, используйте [этот](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span><span class="sxs-lookup"><span data-stu-id="6ab56-177">To see full value with the navigation properties, use [this](../api/b2xidentityuserflow-get-apiConnectorConfiguration.md) API.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows/$entity",
    "id": "B2X_1_UserFlowWithAPIConnector",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "apiConnectorConfiguration": {}
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Create b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_b2xUserFlow_from_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2xUserFlow_from_b2xUserFlows_identityProviders/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: create_b2xUserFlow_from_b2xuserflows_apiconnectors/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
