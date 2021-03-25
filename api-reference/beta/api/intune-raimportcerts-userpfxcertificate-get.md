---
title: Get userPFXCertificate
description: Чтение свойств и связей объекта userPFXCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 71af940118bc256f9212ab9e19442802f672d1a2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152238"
---
# <a name="get-userpfxcertificate"></a><span data-ttu-id="f0b7c-103">Get userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="f0b7c-103">Get userPFXCertificate</span></span>

<span data-ttu-id="f0b7c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0b7c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0b7c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0b7c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0b7c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0b7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0b7c-107">Чтение свойств и связей [объекта userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="f0b7c-107">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0b7c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f0b7c-108">Prerequisites</span></span>
<span data-ttu-id="f0b7c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0b7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0b7c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0b7c-111">Permission type</span></span>|<span data-ttu-id="f0b7c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0b7c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0b7c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0b7c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0b7c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0b7c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0b7c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0b7c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0b7c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0b7c-116">Not supported.</span></span>|
|<span data-ttu-id="f0b7c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f0b7c-117">Application</span></span>|<span data-ttu-id="f0b7c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0b7c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0b7c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0b7c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0b7c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f0b7c-120">Optional query parameters</span></span>
<span data-ttu-id="f0b7c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f0b7c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0b7c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0b7c-122">Request headers</span></span>
|<span data-ttu-id="f0b7c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0b7c-123">Header</span></span>|<span data-ttu-id="f0b7c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f0b7c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0b7c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0b7c-125">Authorization</span></span>|<span data-ttu-id="f0b7c-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0b7c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0b7c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f0b7c-127">Accept</span></span>|<span data-ttu-id="f0b7c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f0b7c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0b7c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0b7c-129">Request body</span></span>
<span data-ttu-id="f0b7c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f0b7c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0b7c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0b7c-131">Response</span></span>
<span data-ttu-id="f0b7c-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f0b7c-132">If successful, this method returns a `200 OK` response code and [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0b7c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f0b7c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0b7c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0b7c-134">Request</span></span>
<span data-ttu-id="f0b7c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0b7c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

### <a name="response"></a><span data-ttu-id="f0b7c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0b7c-136">Response</span></span>
<span data-ttu-id="f0b7c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0b7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 742

{
  "value": {
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
}
```




