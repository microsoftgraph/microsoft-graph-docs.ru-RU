---
title: 'identityApiConnector: uploadClientCertificate'
description: Загрузите ключ формата PKCS 12 (PFX) в конфигурацию проверки подлинности соединителями API.
localization_priority: Normal
author: nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 779b4e6d7800ad9284c77295145ea1c5f27d82a3
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509395"
---
# <a name="identityapiconnector-uploadclientcertificate"></a><span data-ttu-id="f31ba-103">identityApiConnector: uploadClientCertificate</span><span class="sxs-lookup"><span data-stu-id="f31ba-103">identityApiConnector: uploadClientCertificate</span></span>

<span data-ttu-id="f31ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f31ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f31ba-105">Загрузите ключ формата PKCS 12 (.pfx) в конфигурацию проверки подлинности соединителя API.</span><span class="sxs-lookup"><span data-stu-id="f31ba-105">Upload a PKCS 12 format key (.pfx) to an API connector's authentication configuration.</span></span> <span data-ttu-id="f31ba-106">Вход — это закодированное значение базового 64 содержимого сертификата PKCS 12.</span><span class="sxs-lookup"><span data-stu-id="f31ba-106">The input is a base-64 encoded value of the PKCS 12 certificate contents.</span></span> <span data-ttu-id="f31ba-107">Этот метод возвращает [apiConnector](../resources/identityApiConnector.md).</span><span class="sxs-lookup"><span data-stu-id="f31ba-107">This method returns an [apiConnector](../resources/identityApiConnector.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f31ba-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f31ba-108">Permissions</span></span>

<span data-ttu-id="f31ba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f31ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f31ba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f31ba-111">Permission type</span></span>                        | <span data-ttu-id="f31ba-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f31ba-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f31ba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f31ba-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="f31ba-114">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f31ba-114">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="f31ba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f31ba-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f31ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f31ba-116">Not supported.</span></span>  |
| <span data-ttu-id="f31ba-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f31ba-117">Application</span></span>                            | <span data-ttu-id="f31ba-118">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f31ba-118">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="f31ba-119">Учетная запись для работы или школы должна принадлежать к одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="f31ba-119">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f31ba-120">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="f31ba-120">Global administrator</span></span>
* <span data-ttu-id="f31ba-121">Администратор потока внешних пользователей удостоверений</span><span class="sxs-lookup"><span data-stu-id="f31ba-121">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f31ba-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f31ba-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/apiconnectors/{id}/uploadClientCertificate
```

## <a name="request-headers"></a><span data-ttu-id="f31ba-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f31ba-123">Request headers</span></span>

| <span data-ttu-id="f31ba-124">Имя</span><span class="sxs-lookup"><span data-stu-id="f31ba-124">Name</span></span>          | <span data-ttu-id="f31ba-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f31ba-125">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f31ba-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f31ba-126">Authorization</span></span> | <span data-ttu-id="f31ba-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f31ba-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f31ba-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f31ba-129">Content-type</span></span>  | <span data-ttu-id="f31ba-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f31ba-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f31ba-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f31ba-132">Request body</span></span>

<span data-ttu-id="f31ba-133">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f31ba-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="f31ba-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="f31ba-134">Property</span></span>|<span data-ttu-id="f31ba-135">Тип</span><span class="sxs-lookup"><span data-stu-id="f31ba-135">Type</span></span>|<span data-ttu-id="f31ba-136">Описание</span><span class="sxs-lookup"><span data-stu-id="f31ba-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f31ba-137">pkcs12Value</span><span class="sxs-lookup"><span data-stu-id="f31ba-137">pkcs12Value</span></span>|<span data-ttu-id="f31ba-138">String</span><span class="sxs-lookup"><span data-stu-id="f31ba-138">String</span></span>| <span data-ttu-id="f31ba-139">Это поле для отправки контента pfx.</span><span class="sxs-lookup"><span data-stu-id="f31ba-139">This is the field for sending the pfx content.</span></span> <span data-ttu-id="f31ba-140">Значение должно быть кодированной версией базового-64 фактического контента сертификата.</span><span class="sxs-lookup"><span data-stu-id="f31ba-140">The value should be a base-64 encoded version of the actual certificate content.</span></span> <span data-ttu-id="f31ba-141">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f31ba-141">Required.</span></span>|
|<span data-ttu-id="f31ba-142">password</span><span class="sxs-lookup"><span data-stu-id="f31ba-142">password</span></span>|<span data-ttu-id="f31ba-143">Строка</span><span class="sxs-lookup"><span data-stu-id="f31ba-143">String</span></span>| <span data-ttu-id="f31ba-144">Это пароль для файла pfx.</span><span class="sxs-lookup"><span data-stu-id="f31ba-144">This is the password for the pfx file.</span></span> <span data-ttu-id="f31ba-145">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f31ba-145">Required.</span></span> <span data-ttu-id="f31ba-146">Если пароль не используется, необходимо по-прежнему предоставлять значение `""` .</span><span class="sxs-lookup"><span data-stu-id="f31ba-146">If no password is used, must still provide a value of `""`.</span></span>|

## <a name="response"></a><span data-ttu-id="f31ba-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="f31ba-147">Response</span></span>

<span data-ttu-id="f31ba-148">В случае успешной работы этот метод возвращает код ответа и `200 OK` [apiConnector,](../resources/identityApiConnector.md) содержащий общедоступные сведения `authenticationConfiguration` клиентского сертификата.</span><span class="sxs-lookup"><span data-stu-id="f31ba-148">If successful, this method returns a `200 OK` response code and the [apiConnector](../resources/identityApiConnector.md) whose `authenticationConfiguration` contains the public information of the client certificate.</span></span>

## <a name="examples"></a><span data-ttu-id="f31ba-149">Примеры</span><span class="sxs-lookup"><span data-stu-id="f31ba-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f31ba-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="f31ba-150">Request</span></span>

<span data-ttu-id="f31ba-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f31ba-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "identityapiconnector_uploadclientcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/identity/apiconnectors/{id}/uploadClientCertificate
Content-type: application/json

{
    "pkcs12Value": "eyJhbGciOiJSU0EtT0FFUCIsImVuYyI6IkEyNTZHQ00ifQ...kDJ04sJShkkgjL9Bm49plA",
    "password": "<password>"
}
```

### <a name="response"></a><span data-ttu-id="f31ba-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="f31ba-152">Response</span></span>

<span data-ttu-id="f31ba-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f31ba-153">The following is an example of the response.</span></span>

> <span data-ttu-id="f31ba-154">**Примечание:** `authenticationConfiguration` в ответе — тип [microsoft.graph.clientCertificateAuthentication,](../resources/clientcertificateauthentication.md) так как это представляет общедоступные сведения о загруженных сертификатах.</span><span class="sxs-lookup"><span data-stu-id="f31ba-154">**Note:** `authenticationConfiguration` in the response is of type [microsoft.graph.clientCertificateAuthentication](../resources/clientcertificateauthentication.md) because this represents the public information of uploaded certificates.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors/$entity",
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
            },
            {
                "thumbprint": "1AB255CC895477798BA418B378255204304897BC",
                "notAfter": 1766350522,
                "notBefore": 1608670522,
                "isActive": false
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
