---
title: Список userPFXCertificates
description: Свойства списка и связей объектов userPFXCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b63332f8f84378347f48402af7ec5870e242cd1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411486"
---
# <a name="list-userpfxcertificates"></a><span data-ttu-id="ef7ed-103">Список userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="ef7ed-103">List userPFXCertificates</span></span>

> <span data-ttu-id="ef7ed-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef7ed-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ef7ed-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef7ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef7ed-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef7ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef7ed-107">Свойства списка и связей объектов [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="ef7ed-107">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef7ed-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="ef7ed-108">Prerequisites</span></span>
<span data-ttu-id="ef7ed-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ef7ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ef7ed-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef7ed-111">Permission type</span></span>|<span data-ttu-id="ef7ed-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef7ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef7ed-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef7ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef7ed-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef7ed-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ef7ed-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef7ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef7ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef7ed-116">Not supported.</span></span>|
|<span data-ttu-id="ef7ed-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef7ed-117">Application</span></span>|<span data-ttu-id="ef7ed-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef7ed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef7ed-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef7ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="ef7ed-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef7ed-120">Request headers</span></span>
|<span data-ttu-id="ef7ed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef7ed-121">Header</span></span>|<span data-ttu-id="ef7ed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ef7ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef7ed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef7ed-123">Authorization</span></span>|<span data-ttu-id="ef7ed-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ef7ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef7ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef7ed-125">Accept</span></span>|<span data-ttu-id="ef7ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef7ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef7ed-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef7ed-127">Request body</span></span>
<span data-ttu-id="ef7ed-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ef7ed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef7ed-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef7ed-129">Response</span></span>
<span data-ttu-id="ef7ed-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ef7ed-130">If successful, this method returns a `200 OK` response code and a collection of [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef7ed-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ef7ed-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef7ed-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef7ed-132">Request</span></span>
<span data-ttu-id="ef7ed-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef7ed-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
```

### <a name="response"></a><span data-ttu-id="ef7ed-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef7ed-134">Response</span></span>
<span data-ttu-id="ef7ed-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ef7ed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




