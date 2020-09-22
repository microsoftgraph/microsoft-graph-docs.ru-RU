---
title: Список Усерпфксцертификатес
description: Список свойств и связей объектов Усерпфксцертификате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1c9d884e3833e4934c4a8348d81a8b51ceee9926
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010908"
---
# <a name="list-userpfxcertificates"></a><span data-ttu-id="1fa5b-103">Список Усерпфксцертификатес</span><span class="sxs-lookup"><span data-stu-id="1fa5b-103">List userPFXCertificates</span></span>

<span data-ttu-id="1fa5b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fa5b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fa5b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fa5b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fa5b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1fa5b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fa5b-107">Список свойств и связей объектов [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="1fa5b-107">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1fa5b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1fa5b-108">Prerequisites</span></span>
<span data-ttu-id="1fa5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fa5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fa5b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fa5b-111">Permission type</span></span>|<span data-ttu-id="1fa5b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fa5b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fa5b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fa5b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fa5b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fa5b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1fa5b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fa5b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fa5b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1fa5b-116">Not supported.</span></span>|
|<span data-ttu-id="1fa5b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fa5b-117">Application</span></span>|<span data-ttu-id="1fa5b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fa5b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fa5b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fa5b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="1fa5b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1fa5b-120">Request headers</span></span>
|<span data-ttu-id="1fa5b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1fa5b-121">Header</span></span>|<span data-ttu-id="1fa5b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1fa5b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fa5b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1fa5b-123">Authorization</span></span>|<span data-ttu-id="1fa5b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fa5b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fa5b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1fa5b-125">Accept</span></span>|<span data-ttu-id="1fa5b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fa5b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fa5b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1fa5b-127">Request body</span></span>
<span data-ttu-id="1fa5b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1fa5b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fa5b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fa5b-129">Response</span></span>
<span data-ttu-id="1fa5b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1fa5b-130">If successful, this method returns a `200 OK` response code and a collection of [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fa5b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1fa5b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1fa5b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fa5b-132">Request</span></span>
<span data-ttu-id="1fa5b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fa5b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
```

### <a name="response"></a><span data-ttu-id="1fa5b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fa5b-134">Response</span></span>
<span data-ttu-id="1fa5b-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1fa5b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






