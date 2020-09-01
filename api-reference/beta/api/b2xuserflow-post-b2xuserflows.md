---
title: Создание b2xUserFlow
description: Создание нового объекта b2xUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2a7b73aae6c918557ef4d2c7dc0357e138333eda
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319806"
---
# <a name="create-b2xuserflow"></a><span data-ttu-id="b640f-103">Создание b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="b640f-103">Create b2xUserFlow</span></span>

<span data-ttu-id="b640f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b640f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b640f-105">Создание нового объекта [b2xUserFlow](../resources/b2xuserflows.md) .</span><span class="sxs-lookup"><span data-stu-id="b640f-105">Create a new [b2xUserFlow](../resources/b2xuserflows.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b640f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b640f-106">Permissions</span></span>

<span data-ttu-id="b640f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b640f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b640f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b640f-109">Permission type</span></span>      | <span data-ttu-id="b640f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b640f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b640f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b640f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b640f-112">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b640f-112">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="b640f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b640f-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b640f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b640f-114">Not supported.</span></span>|
|<span data-ttu-id="b640f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b640f-115">Application</span></span>|<span data-ttu-id="b640f-116">Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b640f-116">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="b640f-117">Рабочая или учебная учетная запись должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="b640f-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="b640f-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="b640f-118">Global administrator</span></span>
* <span data-ttu-id="b640f-119">Администратор внешнего пользовательского процесса идентификации</span><span class="sxs-lookup"><span data-stu-id="b640f-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="b640f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b640f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/b2xUserFlow
```

## <a name="request-headers"></a><span data-ttu-id="b640f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b640f-121">Request headers</span></span>

|<span data-ttu-id="b640f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b640f-122">Name</span></span>|<span data-ttu-id="b640f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="b640f-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b640f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b640f-124">Authorization</span></span>|<span data-ttu-id="b640f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b640f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b640f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b640f-127">Content-Type</span></span>|<span data-ttu-id="b640f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b640f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b640f-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b640f-130">Request body</span></span>

<span data-ttu-id="b640f-131">В тексте запроса предоставьте представление объекта [b2xUserFlow](../resources/b2xuserflows.md)в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b640f-131">In the request body, provide a JSON representation of a [b2xUserFlow](../resources/b2xuserflows.md).</span></span>

|<span data-ttu-id="b640f-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="b640f-132">Property</span></span>|<span data-ttu-id="b640f-133">Тип</span><span class="sxs-lookup"><span data-stu-id="b640f-133">Type</span></span>|<span data-ttu-id="b640f-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b640f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b640f-135">id</span><span class="sxs-lookup"><span data-stu-id="b640f-135">id</span></span>|<span data-ttu-id="b640f-136">String</span><span class="sxs-lookup"><span data-stu-id="b640f-136">String</span></span>|<span data-ttu-id="b640f-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b640f-137">Required.</span></span> <span data-ttu-id="b640f-138">Имя пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="b640f-138">The name of the user flow.</span></span> <span data-ttu-id="b640f-139">Имя будет предваряться `B2X_1` после создания.</span><span class="sxs-lookup"><span data-stu-id="b640f-139">The name will be pre-pended with `B2X_1` after creation.</span></span>|
|<span data-ttu-id="b640f-140">усерфловтипе</span><span class="sxs-lookup"><span data-stu-id="b640f-140">userFlowType</span></span>|<span data-ttu-id="b640f-141">String</span><span class="sxs-lookup"><span data-stu-id="b640f-141">String</span></span>|<span data-ttu-id="b640f-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b640f-142">Required.</span></span> <span data-ttu-id="b640f-143">Тип создаваемого пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="b640f-143">The type of user flow you are creating.</span></span> <span data-ttu-id="b640f-144">Это значение всегда будет равно `signUpOrSignIn` .</span><span class="sxs-lookup"><span data-stu-id="b640f-144">This value will always be `signUpOrSignIn`.</span></span>|
|<span data-ttu-id="b640f-145">усерфловтипеверсион</span><span class="sxs-lookup"><span data-stu-id="b640f-145">userFlowTypeVersion</span></span>|<span data-ttu-id="b640f-146">С плавающей запятой</span><span class="sxs-lookup"><span data-stu-id="b640f-146">Float</span></span>|<span data-ttu-id="b640f-147">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b640f-147">Required.</span></span> <span data-ttu-id="b640f-148">Версия пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="b640f-148">The version of the user flow.</span></span> <span data-ttu-id="b640f-149">Это значение всегда равно 1.</span><span class="sxs-lookup"><span data-stu-id="b640f-149">This value will always be 1.</span></span>|
|<span data-ttu-id="b640f-150">идентитипровидерс</span><span class="sxs-lookup"><span data-stu-id="b640f-150">identityProviders</span></span>|<span data-ttu-id="b640f-151">Коллекция [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="b640f-151">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="b640f-152">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b640f-152">Optional.</span></span> <span data-ttu-id="b640f-153">Поставщики удостоверений, которые необходимо включить в пользовательский блок.</span><span class="sxs-lookup"><span data-stu-id="b640f-153">The identity providers you want to include in the user flow.</span></span>|

## <a name="response"></a><span data-ttu-id="b640f-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="b640f-154">Response</span></span>

<span data-ttu-id="b640f-155">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и заголовок Location с URI для объекта [b2xUserFlow](../resources/b2xuserflows.md) , созданного для этого запроса, с `B2X_1` префиксом, добавленным к имени.</span><span class="sxs-lookup"><span data-stu-id="b640f-155">If successful, this method returns a `201 Created` response code and a Location header with a URI to the [b2xUserFlow](../resources/b2xuserflows.md) object created for this request, with the `B2X_1` prefix added to the name.</span></span> <span data-ttu-id="b640f-156">В случае неудачи возвращается ошибка `4xx` с подробностями.</span><span class="sxs-lookup"><span data-stu-id="b640f-156">If unsuccessful, a `4xx` error will be returned with specific details.</span></span>

## <a name="examples"></a><span data-ttu-id="b640f-157">Примеры</span><span class="sxs-lookup"><span data-stu-id="b640f-157">Examples</span></span>

### <a name="example-1-create-a-user-flow-with-the-default-values"></a><span data-ttu-id="b640f-158">Пример 1: создание пользовательского процесса со значениями по умолчанию</span><span class="sxs-lookup"><span data-stu-id="b640f-158">Example 1: Create a user flow with the default values</span></span>

#### <a name="request"></a><span data-ttu-id="b640f-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b640f-159">Request</span></span>

<span data-ttu-id="b640f-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b640f-160">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows
Content-type: application/json
Content-length: 154

{
    "id": "Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

#### <a name="response"></a><span data-ttu-id="b640f-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="b640f-161">Response</span></span>

<span data-ttu-id="b640f-162">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b640f-162">The following is an example of the response.</span></span>

<span data-ttu-id="b640f-163">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b640f-163">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

### <a name="example-2-create-a-user-flow-with-the-default-values-and-an-identity-provider"></a><span data-ttu-id="b640f-164">Пример 2: создание пользовательского процесса со значениями по умолчанию и поставщиком удостоверений</span><span class="sxs-lookup"><span data-stu-id="b640f-164">Example 2: Create a user flow with the default values and an identity provider</span></span>

#### <a name="request"></a><span data-ttu-id="b640f-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="b640f-165">Request</span></span>

<span data-ttu-id="b640f-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b640f-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_b2xuserflow_from_b2xuserflows_identityProviders"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/b2xUserFlows
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

#### <a name="response"></a><span data-ttu-id="b640f-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="b640f-167">Response</span></span>

<span data-ttu-id="b640f-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b640f-168">The following is an example of the response.</span></span>

<span data-ttu-id="b640f-169">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b640f-169">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/identity/b2xUserFlows/B2X_1_Partner
Content-type: application/json

{
    "id": "B2X_1_Partner",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
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
    "Error: create_b2xUserFlow_from_b2xUserFlows_identityProviders/userFlowTypeVersion:\r\n    Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
