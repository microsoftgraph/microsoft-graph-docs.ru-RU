---
title: Обновление identityApiConnector
description: Обновление свойств объекта identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 09733c849f99c2928ba7c2cc3b1702f411952cd7
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921619"
---
# <a name="update-identityapiconnector"></a><span data-ttu-id="2fb21-103">Обновление identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="2fb21-103">Update identityApiConnector</span></span>

<span data-ttu-id="2fb21-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fb21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2fb21-105">Обновление свойств объекта [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="2fb21-105">Update the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fb21-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2fb21-106">Permissions</span></span>

<span data-ttu-id="2fb21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fb21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2fb21-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2fb21-109">Permission type</span></span>                        | <span data-ttu-id="2fb21-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2fb21-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2fb21-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2fb21-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2fb21-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fb21-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="2fb21-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2fb21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fb21-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fb21-114">Not supported.</span></span>  |
| <span data-ttu-id="2fb21-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2fb21-115">Application</span></span>                            | <span data-ttu-id="2fb21-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fb21-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="2fb21-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="2fb21-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="2fb21-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="2fb21-118">Global administrator</span></span>
* <span data-ttu-id="2fb21-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="2fb21-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="2fb21-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fb21-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="2fb21-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2fb21-121">Request headers</span></span>
|<span data-ttu-id="2fb21-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2fb21-122">Name</span></span>|<span data-ttu-id="2fb21-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2fb21-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2fb21-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2fb21-124">Authorization</span></span>|<span data-ttu-id="2fb21-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2fb21-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2fb21-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2fb21-127">Content-Type</span></span>|<span data-ttu-id="2fb21-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2fb21-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fb21-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2fb21-130">Request body</span></span>
<span data-ttu-id="2fb21-131">В теле запроса поставляем представление JSON объекта [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="2fb21-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="2fb21-132">В следующей таблице показаны свойства [удостоверенияApiConnector,](../resources/identityapiconnector.md) который можно обновить.</span><span class="sxs-lookup"><span data-stu-id="2fb21-132">The following table shows the properties of the [identityApiConnector](../resources/identityapiconnector.md) that can be updated.</span></span>


|<span data-ttu-id="2fb21-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fb21-133">Property</span></span>|<span data-ttu-id="2fb21-134">Тип</span><span class="sxs-lookup"><span data-stu-id="2fb21-134">Type</span></span>|<span data-ttu-id="2fb21-135">Описание</span><span class="sxs-lookup"><span data-stu-id="2fb21-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fb21-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2fb21-136">displayName</span></span>|<span data-ttu-id="2fb21-137">Строка</span><span class="sxs-lookup"><span data-stu-id="2fb21-137">String</span></span>| <span data-ttu-id="2fb21-138">Имя соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="2fb21-138">The name of the API connector.</span></span> |
|<span data-ttu-id="2fb21-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="2fb21-139">targetUrl</span></span>|<span data-ttu-id="2fb21-140">Строка</span><span class="sxs-lookup"><span data-stu-id="2fb21-140">String</span></span>| <span data-ttu-id="2fb21-141">URL-адрес конечной точки API для вызова.</span><span class="sxs-lookup"><span data-stu-id="2fb21-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="2fb21-142">проверка подлинностиКонфигурация</span><span class="sxs-lookup"><span data-stu-id="2fb21-142">authenticationConfiguration</span></span>|[<span data-ttu-id="2fb21-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="2fb21-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="2fb21-144">Объект, описывая сведения о конфигурации проверки подлинности для вызова API.</span><span class="sxs-lookup"><span data-stu-id="2fb21-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="2fb21-145">Поддерживается [только базовая](../resources/basicauthentication.md) проверка подлинности и клиентский [сертификат PKCS 12.](../resources/pkcs12certificate.md)</span><span class="sxs-lookup"><span data-stu-id="2fb21-145">Only [Basic authentication](../resources/basicauthentication.md) and [PKCS 12 client certificate](../resources/pkcs12certificate.md) are supported.</span></span>|

## <a name="response"></a><span data-ttu-id="2fb21-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fb21-146">Response</span></span>

<span data-ttu-id="2fb21-147">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2fb21-147">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2fb21-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="2fb21-148">Examples</span></span>

### <a name="example-1-changing-display-name-targeturl-and-username--password-used-for-basic-authentication"></a><span data-ttu-id="2fb21-149">Пример 1. Изменение имени отображения, targetUrl и & пароля, используемой для базовой проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="2fb21-149">Example 1: Changing display name, targetUrl, and username & password used for basic authentication</span></span>

#### <a name="request"></a><span data-ttu-id="2fb21-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fb21-150">Request</span></span>

<span data-ttu-id="2fb21-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fb21-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2fb21-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fb21-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/apiConnectors/{identityApiConnectorId}
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
# <a name="c"></a>[<span data-ttu-id="2fb21-153">C#</span><span class="sxs-lookup"><span data-stu-id="2fb21-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fb21-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fb21-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fb21-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fb21-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2fb21-156">Java</span><span class="sxs-lookup"><span data-stu-id="2fb21-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2fb21-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fb21-157">Response</span></span>

<span data-ttu-id="2fb21-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2fb21-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-changing-api-connector-to-use-client-certificate-authentication"></a><span data-ttu-id="2fb21-159">Пример 2. Изменение соединителя API для использования проверки подлинности сертификата клиента</span><span class="sxs-lookup"><span data-stu-id="2fb21-159">Example 2: Changing API connector to use client certificate authentication</span></span>

<span data-ttu-id="2fb21-160">Это переоценит все предыдущие параметры проверки подлинностиConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2fb21-160">This will overwrite any previous authenticationConfiguration settings.</span></span> <span data-ttu-id="2fb21-161">Чтобы изменению с базовой проверки подлинности на проверку подлинности сертификатов, используйте эту функцию.</span><span class="sxs-lookup"><span data-stu-id="2fb21-161">To change from Basic authentication to certificate authentication, use this.</span></span> <span data-ttu-id="2fb21-162">Чтобы добавить дополнительные сертификаты в список сертификатов, используйте метод [Upload client certificate.](../api/identityapiconnector-uploadclientcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="2fb21-162">To add additional certificates to list of certificates, use the [Upload client certificate](../api/identityapiconnector-uploadclientcertificate.md) method.</span></span> <span data-ttu-id="2fb21-163">При использовании этого метода последующие операции соединителя API "Get" или "List" будут иметь тип `authenticationConfiguration` [microsoft.graph.clientCertificateAuthentication.](../resources/clientcertificateauthentication.md)</span><span class="sxs-lookup"><span data-stu-id="2fb21-163">When using this method, consequent "Get" or "List" operations of API connectors, `authenticationConfiguration` will be of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md).</span></span>

#### <a name="request"></a><span data-ttu-id="2fb21-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fb21-164">Request</span></span>

<span data-ttu-id="2fb21-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fb21-165">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2fb21-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fb21-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_identityapiconnector"
}
-->

``` http
PATCH https://graph.microsoft.com/v1.0/identity/apiConnectors/be1f769b-9b13-437e-b540-79a905c4932c
Content-Type: application/json

{
  "authenticationConfiguration": {
    "@odata.type": "#microsoft.graph.pkcs12Certificate",
    "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
    "password": "secret"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="2fb21-167">C#</span><span class="sxs-lookup"><span data-stu-id="2fb21-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2fb21-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fb21-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2fb21-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2fb21-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2fb21-170">Java</span><span class="sxs-lookup"><span data-stu-id="2fb21-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2fb21-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="2fb21-171">Response</span></span>

<span data-ttu-id="2fb21-172">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2fb21-172">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
