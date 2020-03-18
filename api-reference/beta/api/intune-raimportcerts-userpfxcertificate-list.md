---
title: Список Усерпфксцертификатес
description: Список свойств и связей объектов Усерпфксцертификате.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dad8fa4538d907df5a0ac86a4b5aca1a4daa47d2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801826"
---
# <a name="list-userpfxcertificates"></a><span data-ttu-id="6a357-103">Список Усерпфксцертификатес</span><span class="sxs-lookup"><span data-stu-id="6a357-103">List userPFXCertificates</span></span>

> <span data-ttu-id="6a357-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a357-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a357-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a357-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a357-106">Список свойств и связей объектов [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="6a357-106">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a357-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6a357-107">Prerequisites</span></span>
<span data-ttu-id="6a357-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a357-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a357-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a357-110">Permission type</span></span>|<span data-ttu-id="6a357-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a357-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a357-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a357-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a357-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a357-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6a357-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a357-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a357-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a357-115">Not supported.</span></span>|
|<span data-ttu-id="6a357-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6a357-116">Application</span></span>|<span data-ttu-id="6a357-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a357-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a357-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a357-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="6a357-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6a357-119">Request headers</span></span>
|<span data-ttu-id="6a357-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a357-120">Header</span></span>|<span data-ttu-id="6a357-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6a357-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a357-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a357-122">Authorization</span></span>|<span data-ttu-id="6a357-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a357-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a357-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6a357-124">Accept</span></span>|<span data-ttu-id="6a357-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a357-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a357-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a357-126">Request body</span></span>
<span data-ttu-id="6a357-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a357-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a357-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a357-128">Response</span></span>
<span data-ttu-id="6a357-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [усерпфксцертификате](../resources/intune-raimportcerts-userpfxcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a357-129">If successful, this method returns a `200 OK` response code and a collection of [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a357-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6a357-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a357-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a357-131">Request</span></span>
<span data-ttu-id="6a357-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a357-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
```

### <a name="response"></a><span data-ttu-id="6a357-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a357-133">Response</span></span>
<span data-ttu-id="6a357-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a357-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




