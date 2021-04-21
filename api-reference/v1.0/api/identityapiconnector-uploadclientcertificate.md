---
title: 'identityApiConnector: uploadClientCertificate'
description: Загрузите ключ формата PKCS 12 (PFX) в конфигурацию проверки подлинности соединителями API.
localization_priority: Normal
author: nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 84cf8a767a4cf944a143342c1b3a0678252a4e8b
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921185"
---
# <a name="identityapiconnector-uploadclientcertificate"></a><span data-ttu-id="89cff-103">identityApiConnector: uploadClientCertificate</span><span class="sxs-lookup"><span data-stu-id="89cff-103">identityApiConnector: uploadClientCertificate</span></span>

<span data-ttu-id="89cff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89cff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89cff-105">Загрузите ключ формата PKCS 12 (.pfx) в конфигурацию проверки подлинности соединителя API.</span><span class="sxs-lookup"><span data-stu-id="89cff-105">Upload a PKCS 12 format key (.pfx) to an API connector's authentication configuration.</span></span> <span data-ttu-id="89cff-106">Вход — это закодированное значение базового 64 содержимого сертификата PKCS 12.</span><span class="sxs-lookup"><span data-stu-id="89cff-106">The input is a base-64 encoded value of the PKCS 12 certificate contents.</span></span> <span data-ttu-id="89cff-107">Этот метод возвращает [apiConnector](../resources/identityApiConnector.md).</span><span class="sxs-lookup"><span data-stu-id="89cff-107">This method returns an [apiConnector](../resources/identityApiConnector.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="89cff-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89cff-108">Permissions</span></span>

<span data-ttu-id="89cff-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89cff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89cff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89cff-111">Permission type</span></span>                        | <span data-ttu-id="89cff-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89cff-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="89cff-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89cff-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="89cff-114">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89cff-114">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="89cff-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89cff-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89cff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89cff-116">Not supported.</span></span>  |
| <span data-ttu-id="89cff-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89cff-117">Application</span></span>                            | <span data-ttu-id="89cff-118">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89cff-118">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="89cff-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="89cff-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="89cff-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="89cff-120">Global administrator</span></span>
* <span data-ttu-id="89cff-121">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="89cff-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="89cff-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89cff-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/apiconnectors/{id}/uploadClientCertificate
```

## <a name="request-headers"></a><span data-ttu-id="89cff-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89cff-123">Request headers</span></span>

| <span data-ttu-id="89cff-124">Имя</span><span class="sxs-lookup"><span data-stu-id="89cff-124">Name</span></span>          | <span data-ttu-id="89cff-125">Описание</span><span class="sxs-lookup"><span data-stu-id="89cff-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="89cff-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89cff-126">Authorization</span></span> | <span data-ttu-id="89cff-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89cff-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="89cff-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89cff-129">Content-type</span></span>  | <span data-ttu-id="89cff-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89cff-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89cff-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89cff-132">Request body</span></span>

<span data-ttu-id="89cff-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="89cff-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="89cff-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="89cff-134">Property</span></span>|<span data-ttu-id="89cff-135">Тип</span><span class="sxs-lookup"><span data-stu-id="89cff-135">Type</span></span>|<span data-ttu-id="89cff-136">Описание</span><span class="sxs-lookup"><span data-stu-id="89cff-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89cff-137">pkcs12Value</span><span class="sxs-lookup"><span data-stu-id="89cff-137">pkcs12Value</span></span>|<span data-ttu-id="89cff-138">Строка</span><span class="sxs-lookup"><span data-stu-id="89cff-138">String</span></span>| <span data-ttu-id="89cff-139">Это поле для отправки контента pfx.</span><span class="sxs-lookup"><span data-stu-id="89cff-139">This is the field for sending the pfx content.</span></span> <span data-ttu-id="89cff-140">Значение должно быть кодированной версией базового-64 фактического контента сертификата.</span><span class="sxs-lookup"><span data-stu-id="89cff-140">The value should be a base-64 encoded version of the actual certificate content.</span></span> <span data-ttu-id="89cff-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89cff-141">Required.</span></span>|
|<span data-ttu-id="89cff-142">password</span><span class="sxs-lookup"><span data-stu-id="89cff-142">password</span></span>|<span data-ttu-id="89cff-143">Строка</span><span class="sxs-lookup"><span data-stu-id="89cff-143">String</span></span>| <span data-ttu-id="89cff-144">Это пароль для файла pfx.</span><span class="sxs-lookup"><span data-stu-id="89cff-144">This is the password for the pfx file.</span></span> <span data-ttu-id="89cff-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89cff-145">Required.</span></span> <span data-ttu-id="89cff-146">Если пароль не используется, необходимо по-прежнему предоставлять значение `""` .</span><span class="sxs-lookup"><span data-stu-id="89cff-146">If no password is used, must still provide a value of `""`.</span></span>|

## <a name="response"></a><span data-ttu-id="89cff-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="89cff-147">Response</span></span>

<span data-ttu-id="89cff-148">В случае успешной работы этот метод возвращает код ответа и `200 OK` [apiConnector,](../resources/identityApiConnector.md) содержащий общедоступные сведения `authenticationConfiguration` клиентского сертификата.</span><span class="sxs-lookup"><span data-stu-id="89cff-148">If successful, this method returns a `200 OK` response code and the [apiConnector](../resources/identityApiConnector.md) whose `authenticationConfiguration` contains the public information of the client certificate.</span></span>

## <a name="examples"></a><span data-ttu-id="89cff-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="89cff-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89cff-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="89cff-150">Request</span></span>

<span data-ttu-id="89cff-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89cff-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="89cff-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="89cff-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "identityapiconnector_uploadclientcertificate"
}-->

```http
POST https://graph.microsoft.com/v1.0/identity/apiconnectors/{id}/uploadClientCertificate
Content-type: application/json

{
    "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
    "password": "<password>"
}
```
# <a name="c"></a>[<span data-ttu-id="89cff-153">C#</span><span class="sxs-lookup"><span data-stu-id="89cff-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/identityapiconnector-uploadclientcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89cff-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89cff-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/identityapiconnector-uploadclientcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89cff-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89cff-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/identityapiconnector-uploadclientcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89cff-156">Java</span><span class="sxs-lookup"><span data-stu-id="89cff-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/identityapiconnector-uploadclientcertificate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89cff-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="89cff-157">Response</span></span>

<span data-ttu-id="89cff-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89cff-158">The following is an example of the response.</span></span>

> <span data-ttu-id="89cff-159">**Примечание:** `authenticationConfiguration` в ответе — тип [microsoft.graph.clientCertificateAuthentication,](../resources/clientcertificateauthentication.md) так как это представляет общедоступные сведения о загруженных сертификатах.</span><span class="sxs-lookup"><span data-stu-id="89cff-159">**Note:** `authenticationConfiguration` in the response is of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md) because this represents the public information of uploaded certificates.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/apiConnectors/$entity",
    "id": "guid",
    "displayName": "My API connector",
    "targetUrl": "https://api.contoso.com/endpoint",
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed982019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "identityApiConnector: uploadClientCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
