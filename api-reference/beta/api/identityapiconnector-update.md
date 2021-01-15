---
title: Обновление identityApiConnector
description: Обновление свойств объекта identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9037a6bfcd53af0ee009f232909a964a8b0e6a86
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873670"
---
# <a name="update-identityapiconnector"></a><span data-ttu-id="a8887-103">Обновление identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="a8887-103">Update identityApiConnector</span></span>

<span data-ttu-id="a8887-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8887-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8887-105">Обновление свойств объекта [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="a8887-105">Update the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8887-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8887-106">Permissions</span></span>

<span data-ttu-id="a8887-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8887-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8887-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8887-109">Permission type</span></span>                        | <span data-ttu-id="a8887-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8887-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a8887-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8887-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8887-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8887-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="a8887-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8887-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8887-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8887-114">Not supported.</span></span>  |
| <span data-ttu-id="a8887-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a8887-115">Application</span></span>                            | <span data-ttu-id="a8887-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8887-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="a8887-117">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="a8887-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a8887-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a8887-118">Global administrator</span></span>
* <span data-ttu-id="a8887-119">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="a8887-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a8887-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8887-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="a8887-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8887-121">Request headers</span></span>
|<span data-ttu-id="a8887-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a8887-122">Name</span></span>|<span data-ttu-id="a8887-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a8887-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a8887-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8887-124">Authorization</span></span>|<span data-ttu-id="a8887-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8887-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a8887-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8887-127">Content-Type</span></span>|<span data-ttu-id="a8887-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8887-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8887-130">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8887-130">Request body</span></span>
<span data-ttu-id="a8887-131">В теле запроса укажу представление объекта [identityApiConnector](../resources/identityapiconnector.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="a8887-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="a8887-132">В следующей таблице показаны свойства [identityApiConnector,](../resources/identityapiconnector.md) которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="a8887-132">The following table shows the properties of the [identityApiConnector](../resources/identityapiconnector.md) that can be updated.</span></span>


|<span data-ttu-id="a8887-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8887-133">Property</span></span>|<span data-ttu-id="a8887-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a8887-134">Type</span></span>|<span data-ttu-id="a8887-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a8887-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8887-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a8887-136">displayName</span></span>|<span data-ttu-id="a8887-137">String</span><span class="sxs-lookup"><span data-stu-id="a8887-137">String</span></span>| <span data-ttu-id="a8887-138">Имя соединители API.</span><span class="sxs-lookup"><span data-stu-id="a8887-138">The name of the API connector.</span></span> |
|<span data-ttu-id="a8887-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="a8887-139">targetUrl</span></span>|<span data-ttu-id="a8887-140">String</span><span class="sxs-lookup"><span data-stu-id="a8887-140">String</span></span>| <span data-ttu-id="a8887-141">URL-адрес конечной точки API для вызова.</span><span class="sxs-lookup"><span data-stu-id="a8887-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="a8887-142">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8887-142">authenticationConfiguration</span></span>|[<span data-ttu-id="a8887-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="a8887-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="a8887-144">Объект, который описывает сведения о конфигурации проверки подлинности для вызова API.</span><span class="sxs-lookup"><span data-stu-id="a8887-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="a8887-145">В [настоящее время поддерживается](../resources/basicauthentication.md) только базовая проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="a8887-145">Only [Basic authentication](../resources/basicauthentication.md) is supported at this time.</span></span> <span data-ttu-id="a8887-146">Все свойства apiAuthenticationConfigurationBase должны быть установлены одновременно, например имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="a8887-146">All properties of the apiAuthenticationConfigurationBase must be set at the same time, like both username and password.</span></span>|

## <a name="response"></a><span data-ttu-id="a8887-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8887-147">Response</span></span>

<span data-ttu-id="a8887-148">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a8887-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a8887-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="a8887-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a8887-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8887-150">Request</span></span>

<span data-ttu-id="a8887-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8887-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a8887-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8887-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/apiConnectors/{identityApiConnectorId}
Content-Type: application/json

{
  "displayName": "New Test API",
  "targetUrl": "https://otherapi.com/api/endpoint",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.basicAuthentication",
    "username":"<NEW_USERNAME>", 
    "password":"<NEW_PASSWORD>"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="a8887-153">C#</span><span class="sxs-lookup"><span data-stu-id="a8887-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a8887-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8887-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a8887-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8887-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a8887-156">Java</span><span class="sxs-lookup"><span data-stu-id="a8887-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a8887-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8887-157">Response</span></span>

<span data-ttu-id="a8887-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a8887-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
