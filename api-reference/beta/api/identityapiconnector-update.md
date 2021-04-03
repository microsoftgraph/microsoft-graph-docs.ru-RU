---
title: Обновление identityApiConnector
description: Обновление свойств объекта identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b7383d82f30f76bc97fc9e66dd57c21044a963ca
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508731"
---
# <a name="update-identityapiconnector"></a><span data-ttu-id="a9038-103">Обновление identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="a9038-103">Update identityApiConnector</span></span>

<span data-ttu-id="a9038-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9038-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9038-105">Обновление свойств объекта [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="a9038-105">Update the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9038-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9038-106">Permissions</span></span>

<span data-ttu-id="a9038-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9038-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9038-109">Permission type</span></span>                        | <span data-ttu-id="a9038-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9038-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="a9038-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9038-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9038-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9038-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="a9038-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9038-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9038-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9038-114">Not supported.</span></span>  |
| <span data-ttu-id="a9038-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a9038-115">Application</span></span>                            | <span data-ttu-id="a9038-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9038-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="a9038-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="a9038-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="a9038-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="a9038-118">Global administrator</span></span>
* <span data-ttu-id="a9038-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="a9038-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="a9038-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9038-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="a9038-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9038-121">Request headers</span></span>
|<span data-ttu-id="a9038-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a9038-122">Name</span></span>|<span data-ttu-id="a9038-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a9038-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a9038-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9038-124">Authorization</span></span>|<span data-ttu-id="a9038-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9038-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a9038-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a9038-127">Content-Type</span></span>|<span data-ttu-id="a9038-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9038-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9038-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9038-130">Request body</span></span>
<span data-ttu-id="a9038-131">В теле запроса поставляем представление JSON объекта [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="a9038-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="a9038-132">В следующей таблице показаны свойства [удостоверенияApiConnector,](../resources/identityapiconnector.md) который можно обновить.</span><span class="sxs-lookup"><span data-stu-id="a9038-132">The following table shows the properties of the [identityApiConnector](../resources/identityapiconnector.md) that can be updated.</span></span>


|<span data-ttu-id="a9038-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9038-133">Property</span></span>|<span data-ttu-id="a9038-134">Тип</span><span class="sxs-lookup"><span data-stu-id="a9038-134">Type</span></span>|<span data-ttu-id="a9038-135">Описание</span><span class="sxs-lookup"><span data-stu-id="a9038-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9038-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a9038-136">displayName</span></span>|<span data-ttu-id="a9038-137">String</span><span class="sxs-lookup"><span data-stu-id="a9038-137">String</span></span>| <span data-ttu-id="a9038-138">Имя соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="a9038-138">The name of the API connector.</span></span> |
|<span data-ttu-id="a9038-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="a9038-139">targetUrl</span></span>|<span data-ttu-id="a9038-140">String</span><span class="sxs-lookup"><span data-stu-id="a9038-140">String</span></span>| <span data-ttu-id="a9038-141">URL-адрес конечной точки API для вызова.</span><span class="sxs-lookup"><span data-stu-id="a9038-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="a9038-142">проверка подлинностиКонфигурация</span><span class="sxs-lookup"><span data-stu-id="a9038-142">authenticationConfiguration</span></span>|[<span data-ttu-id="a9038-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="a9038-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="a9038-144">Объект, описывая сведения о конфигурации проверки подлинности для вызова API.</span><span class="sxs-lookup"><span data-stu-id="a9038-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="a9038-145">Поддерживается [только базовая](../resources/basicauthentication.md) проверка подлинности и клиентский [сертификат PKCS 12.](../resources/pkcs12certificate.md)</span><span class="sxs-lookup"><span data-stu-id="a9038-145">Only [Basic authentication](../resources/basicauthentication.md) and [PKCS 12 client certificate](../resources/pkcs12certificate.md) are supported.</span></span>|

## <a name="response"></a><span data-ttu-id="a9038-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9038-146">Response</span></span>

<span data-ttu-id="a9038-147">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a9038-147">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a9038-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="a9038-148">Examples</span></span>

### <a name="example-1-changing-display-name-targeturl-and-username--password-used-for-basic-authentication"></a><span data-ttu-id="a9038-149">Пример 1. Изменение имени отображения, targetUrl и & пароля, используемой для базовой проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="a9038-149">Example 1: Changing display name, targetUrl, and username & password used for basic authentication</span></span>

#### <a name="request"></a><span data-ttu-id="a9038-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9038-150">Request</span></span>

<span data-ttu-id="a9038-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9038-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9038-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9038-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a9038-153">C#</span><span class="sxs-lookup"><span data-stu-id="a9038-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9038-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9038-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9038-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9038-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a9038-156">Java</span><span class="sxs-lookup"><span data-stu-id="a9038-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a9038-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9038-157">Response</span></span>

<span data-ttu-id="a9038-158">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a9038-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-changing-api-connector-to-use-client-certificate-authentication"></a><span data-ttu-id="a9038-159">Пример 2. Изменение соединителя API для использования проверки подлинности сертификата клиента</span><span class="sxs-lookup"><span data-stu-id="a9038-159">Example 2: Changing API connector to use client certificate authentication</span></span>

> <span data-ttu-id="a9038-160">**Примечание:** Это переоценит все предыдущие параметры проверки подлинностиConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a9038-160">**Note:** This will overwrite any previous authenticationConfiguration settings.</span></span> <span data-ttu-id="a9038-161">Чтобы изменению с базовой проверки подлинности на проверку подлинности сертификатов, используйте эту функцию.</span><span class="sxs-lookup"><span data-stu-id="a9038-161">To change from Basic authentication to certificate authentication, use this.</span></span> <span data-ttu-id="a9038-162">Чтобы добавить дополнительные сертификаты в список сертификатов, используйте метод [Upload client certificate.](../api/identityapiconnector-uploadclientcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="a9038-162">To add additional certificates to list of certificates, use the [Upload client certificate](../api/identityapiconnector-uploadclientcertificate.md) method.</span></span> <span data-ttu-id="a9038-163">При использовании этого метода последующие операции соединителя API "Get" или "List" будут иметь тип `authenticationConfiguration` [microsoft.graph.clientCertificateAuthentication.](../resources/clientcertificateauthentication.md)</span><span class="sxs-lookup"><span data-stu-id="a9038-163">When using this method, consequent "Get" or "List" operations of API connectors, `authenticationConfiguration` will be of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md).</span></span>

#### <a name="request"></a><span data-ttu-id="a9038-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9038-164">Request</span></span>

<span data-ttu-id="a9038-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9038-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/apiConnectors/{identityApiConnectorId}
Content-Type: application/json

{
  "authenticationConfiguration": {
    "@odata.type": "#microsoft.graph.pkcs12Certificate",
    "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
    "password": "secret"
  }
}
```

#### <a name="response"></a><span data-ttu-id="a9038-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9038-166">Response</span></span>

<span data-ttu-id="a9038-167">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a9038-167">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
