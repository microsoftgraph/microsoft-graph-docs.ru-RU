---
title: Список Усерпфксцертификатес
description: Список свойств и связей объектов Усерпфксцертификате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a52a98e7dcde9f4cb2e75fd7e23db697a1679d92
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37189678"
---
# <a name="list-userpfxcertificates"></a><span data-ttu-id="1f535-103">Список Усерпфксцертификатес</span><span class="sxs-lookup"><span data-stu-id="1f535-103">List userPFXCertificates</span></span>

> <span data-ttu-id="1f535-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f535-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f535-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f535-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f535-106">Список свойств и связей объектов [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="1f535-106">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f535-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1f535-107">Prerequisites</span></span>
<span data-ttu-id="1f535-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f535-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f535-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f535-110">Permission type</span></span>|<span data-ttu-id="1f535-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f535-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f535-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f535-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f535-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f535-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1f535-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f535-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f535-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f535-115">Not supported.</span></span>|
|<span data-ttu-id="1f535-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f535-116">Application</span></span>|<span data-ttu-id="1f535-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f535-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f535-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f535-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="1f535-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f535-119">Request headers</span></span>
|<span data-ttu-id="1f535-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f535-120">Header</span></span>|<span data-ttu-id="1f535-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1f535-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f535-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1f535-122">Authorization</span></span>|<span data-ttu-id="1f535-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f535-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f535-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1f535-124">Accept</span></span>|<span data-ttu-id="1f535-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f535-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f535-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f535-126">Request body</span></span>
<span data-ttu-id="1f535-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1f535-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f535-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f535-128">Response</span></span>
<span data-ttu-id="1f535-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1f535-129">If successful, this method returns a `200 OK` response code and a collection of [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f535-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1f535-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f535-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f535-131">Request</span></span>
<span data-ttu-id="1f535-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f535-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
```

### <a name="response"></a><span data-ttu-id="1f535-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f535-133">Response</span></span>
<span data-ttu-id="1f535-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f535-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 784

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userPFXCertificate",
      "id": "045c159b-159b-045c-9b15-5c049b155c04",
      "thumbprint": "Thumbprint value",
      "intendedPurpose": "smimeEncryption",
      "userPrincipalName": "User Principal Name value",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "providerName": "Provider Name value",
      "keyName": "Key Name value",
      "paddingScheme": "pkcs1",
      "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
      "encryptedPfxPassword": "Encrypted Pfx Password value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




