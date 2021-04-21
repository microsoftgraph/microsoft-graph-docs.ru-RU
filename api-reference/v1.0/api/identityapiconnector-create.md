---
title: Создание identityApiConnector
description: Создание нового объекта identityApiConnector.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8cdebdaa8ed86e6d6d60ad07c987b2152baf6737
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920366"
---
# <a name="create-identityapiconnector"></a><span data-ttu-id="1b330-103">Создание identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="1b330-103">Create identityApiConnector</span></span>

<span data-ttu-id="1b330-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b330-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b330-105">Создание нового [объекта identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="1b330-105">Create a new [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b330-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b330-106">Permissions</span></span>

<span data-ttu-id="1b330-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b330-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b330-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b330-109">Permission type</span></span>                        | <span data-ttu-id="1b330-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b330-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="1b330-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b330-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b330-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b330-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="1b330-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b330-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b330-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b330-114">Not supported.</span></span>  |
| <span data-ttu-id="1b330-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b330-115">Application</span></span>                            | <span data-ttu-id="1b330-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b330-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="1b330-117">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="1b330-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="1b330-118">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="1b330-118">Global administrator</span></span>
* <span data-ttu-id="1b330-119">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="1b330-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="1b330-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b330-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
POST /identity/apiConnectors
```

## <a name="request-headers"></a><span data-ttu-id="1b330-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b330-121">Request headers</span></span>

| <span data-ttu-id="1b330-122">Имя</span><span class="sxs-lookup"><span data-stu-id="1b330-122">Name</span></span>          | <span data-ttu-id="1b330-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1b330-123">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="1b330-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b330-124">Authorization</span></span> | <span data-ttu-id="1b330-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b330-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="1b330-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1b330-127">Content-Type</span></span>  | <span data-ttu-id="1b330-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b330-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b330-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b330-130">Request body</span></span>

<span data-ttu-id="1b330-131">В теле запроса поставляем представление JSON объекта [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="1b330-131">In the request body, supply a JSON representation of the [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

<span data-ttu-id="1b330-132">В следующей таблице показаны свойства, необходимые при создании [identityApiConnector.](../resources/identityapiconnector.md)</span><span class="sxs-lookup"><span data-stu-id="1b330-132">The following table shows the properties that are required when you create the [identityApiConnector](../resources/identityapiconnector.md).</span></span>

|<span data-ttu-id="1b330-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b330-133">Property</span></span>|<span data-ttu-id="1b330-134">Тип</span><span class="sxs-lookup"><span data-stu-id="1b330-134">Type</span></span>|<span data-ttu-id="1b330-135">Описание</span><span class="sxs-lookup"><span data-stu-id="1b330-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b330-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1b330-136">displayName</span></span>|<span data-ttu-id="1b330-137">Строка</span><span class="sxs-lookup"><span data-stu-id="1b330-137">String</span></span>| <span data-ttu-id="1b330-138">Имя соединитетеля API.</span><span class="sxs-lookup"><span data-stu-id="1b330-138">The name of the API connector.</span></span> |
|<span data-ttu-id="1b330-139">targetUrl</span><span class="sxs-lookup"><span data-stu-id="1b330-139">targetUrl</span></span>|<span data-ttu-id="1b330-140">Строка</span><span class="sxs-lookup"><span data-stu-id="1b330-140">String</span></span>| <span data-ttu-id="1b330-141">URL-адрес конечной точки API для вызова.</span><span class="sxs-lookup"><span data-stu-id="1b330-141">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="1b330-142">проверка подлинностиКонфигурация</span><span class="sxs-lookup"><span data-stu-id="1b330-142">authenticationConfiguration</span></span>|[<span data-ttu-id="1b330-143">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="1b330-143">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="1b330-144">Объект, описывая сведения о конфигурации проверки подлинности для вызова API.</span><span class="sxs-lookup"><span data-stu-id="1b330-144">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="1b330-145">[Поддерживается базовая](../resources/basicauthentication.md) проверка подлинности и [клиентский сертификат PKCS 12.](../resources/pkcs12certificate.md)</span><span class="sxs-lookup"><span data-stu-id="1b330-145">[Basic authentication](../resources/basicauthentication.md) and [PKCS 12 client certificate](../resources/pkcs12certificate.md) are supported.</span></span>|

## <a name="response"></a><span data-ttu-id="1b330-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b330-146">Response</span></span>

<span data-ttu-id="1b330-147">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект identityApiConnector](../resources/identityapiconnector.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1b330-147">If successful, this method returns a `201 Created` response code and an [identityApiConnector](../resources/identityapiconnector.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b330-148">Примеры</span><span class="sxs-lookup"><span data-stu-id="1b330-148">Examples</span></span>

### <a name="example-1-create-an-api-connector-with-basic-authentication"></a><span data-ttu-id="1b330-149">Пример 1. Создание соединителя API с базовой проверкой подлинности</span><span class="sxs-lookup"><span data-stu-id="1b330-149">Example 1: Create an API connector with basic authentication</span></span>

#### <a name="request"></a><span data-ttu-id="1b330-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b330-150">Request</span></span>

<span data-ttu-id="1b330-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b330-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1b330-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b330-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/v1.0/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someapi.com/api",
    "authenticationConfiguration": {
      "@odata.type":"#microsoft.graph.basicAuthentication",
      "username": "MyUsername",
      "password": "MyPassword"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="1b330-153">C#</span><span class="sxs-lookup"><span data-stu-id="1b330-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityapiconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b330-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b330-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityapiconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b330-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b330-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityapiconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b330-156">Java</span><span class="sxs-lookup"><span data-stu-id="1b330-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityapiconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1b330-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b330-157">Response</span></span>

<span data-ttu-id="1b330-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1b330-158">The following is an example of the response.</span></span>

><span data-ttu-id="1b330-159">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1b330-159">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.basicAuthentication",
        "username": "MyUsername",
        "password": "******"
    }
}
```

### <a name="example-2-create-an-api-connector-with-client-certificate-authentication"></a><span data-ttu-id="1b330-160">Пример 2. Создание соединителя API с проверкой подлинности сертификата клиента</span><span class="sxs-lookup"><span data-stu-id="1b330-160">Example 2: Create an API connector with client certificate authentication</span></span>

#### <a name="request"></a><span data-ttu-id="1b330-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b330-161">Request</span></span>

<span data-ttu-id="1b330-162">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b330-162">The following is an example of the request.</span></span>

> <span data-ttu-id="1b330-163">**Примечание:** `authenticationConfiguration` в запросе имеется тип [microsoft.graph.pkcs12certificate,](../resources/pkcs12certificate.md)который представляет конфигурацию сертификата, необходимого для загрузки или создания.</span><span class="sxs-lookup"><span data-stu-id="1b330-163">**Note:** `authenticationConfiguration` in the request is of type [microsoft.graph.pkcs12certificate](../resources/pkcs12certificate.md), which represents the configuration of a certificate needed on upload or create.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_identityapiconnector"
}
-->

```http
POST https://graph.microsoft.com/v1.0/identity/apiConnectors
Content-Type: application/json

{
    "displayName":"Test API",
    "targetUrl":"https://someotherapi.com/api",
    "authenticationConfiguration": {
        "@odata.type":"#microsoft.graph.pkcs12Certificate",
        "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
        "password": "CertificatePassword"
    }
}
```

#### <a name="response"></a><span data-ttu-id="1b330-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b330-164">Response</span></span>

<span data-ttu-id="1b330-165">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1b330-165">The following is an example of the response.</span></span>

> <span data-ttu-id="1b330-166">**Примечание:** `authenticationConfiguration` в ответе — тип [microsoft.graph.clientCertificateAuthentication,](../resources/clientcertificateauthentication.md) так как это представляет общедоступные сведения о загруженных сертификатах.</span><span class="sxs-lookup"><span data-stu-id="1b330-166">**Note:** `authenticationConfiguration` in the response is of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md) because this represents the public information of uploaded certificates.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors/$entity",
    "id":"guid",
    "displayName": "Test API",
    "targetUrl": "https://someotherapi.com/api",
    "authenticationConfiguration": {
        "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
        "certificateList": [
            {
                "thumbprint": "0EB255CC895477798BA418B378255204304897AD",
                "notAfter": 1666350522,
                "notBefore": 1508670522,
                "isActive": true
            }
        ]
    }
}
```
