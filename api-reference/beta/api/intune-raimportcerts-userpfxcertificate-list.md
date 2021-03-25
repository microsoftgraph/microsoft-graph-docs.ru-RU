---
title: Список пользователейPFXCertificates
description: Список свойств и связей объектов userPFXCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f9d59b67a3deffb052ea2ed25a1f567b74800478
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152210"
---
# <a name="list-userpfxcertificates"></a><span data-ttu-id="07ac4-103">Список пользователейPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="07ac4-103">List userPFXCertificates</span></span>

<span data-ttu-id="07ac4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07ac4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07ac4-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07ac4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07ac4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07ac4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07ac4-107">Список свойств и связей [объектов userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="07ac4-107">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07ac4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="07ac4-108">Prerequisites</span></span>
<span data-ttu-id="07ac4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07ac4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07ac4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07ac4-111">Permission type</span></span>|<span data-ttu-id="07ac4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07ac4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07ac4-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07ac4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07ac4-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07ac4-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07ac4-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07ac4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07ac4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07ac4-116">Not supported.</span></span>|
|<span data-ttu-id="07ac4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="07ac4-117">Application</span></span>|<span data-ttu-id="07ac4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07ac4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07ac4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07ac4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="07ac4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="07ac4-120">Request headers</span></span>
|<span data-ttu-id="07ac4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07ac4-121">Header</span></span>|<span data-ttu-id="07ac4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="07ac4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07ac4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07ac4-123">Authorization</span></span>|<span data-ttu-id="07ac4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07ac4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07ac4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="07ac4-125">Accept</span></span>|<span data-ttu-id="07ac4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07ac4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07ac4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07ac4-127">Request body</span></span>
<span data-ttu-id="07ac4-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="07ac4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07ac4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="07ac4-129">Response</span></span>
<span data-ttu-id="07ac4-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="07ac4-130">If successful, this method returns a `200 OK` response code and a collection of [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07ac4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="07ac4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="07ac4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="07ac4-132">Request</span></span>
<span data-ttu-id="07ac4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07ac4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
```

### <a name="response"></a><span data-ttu-id="07ac4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="07ac4-134">Response</span></span>
<span data-ttu-id="07ac4-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07ac4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




