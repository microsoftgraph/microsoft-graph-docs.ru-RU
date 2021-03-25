---
title: Get iosCertificateProfile
description: Чтение свойств и связей объекта iosCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4dcc0772561e7c58462d332bd86058aa1f7a0a4c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155360"
---
# <a name="get-ioscertificateprofile"></a><span data-ttu-id="ff239-103">Get iosCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="ff239-103">Get iosCertificateProfile</span></span>

<span data-ttu-id="ff239-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff239-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff239-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff239-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff239-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff239-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff239-107">Чтение свойств и связей объекта [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ff239-107">Read properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff239-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ff239-108">Prerequisites</span></span>
<span data-ttu-id="ff239-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff239-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff239-111">Permission type</span></span>|<span data-ttu-id="ff239-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff239-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff239-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff239-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff239-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff239-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff239-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff239-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff239-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff239-116">Not supported.</span></span>|
|<span data-ttu-id="ff239-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ff239-117">Application</span></span>|<span data-ttu-id="ff239-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff239-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff239-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff239-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeSigningCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeEncryptionCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff239-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ff239-120">Optional query parameters</span></span>
<span data-ttu-id="ff239-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ff239-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff239-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff239-122">Request headers</span></span>
|<span data-ttu-id="ff239-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff239-123">Header</span></span>|<span data-ttu-id="ff239-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ff239-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff239-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff239-125">Authorization</span></span>|<span data-ttu-id="ff239-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ff239-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff239-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ff239-127">Accept</span></span>|<span data-ttu-id="ff239-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ff239-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff239-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff239-129">Request body</span></span>
<span data-ttu-id="ff239-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ff239-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff239-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff239-131">Response</span></span>
<span data-ttu-id="ff239-132">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ff239-132">If successful, this method returns a `200 OK` response code and [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff239-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ff239-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff239-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff239-134">Request</span></span>
<span data-ttu-id="ff239-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff239-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/smimeSigningCertificate
```

### <a name="response"></a><span data-ttu-id="ff239-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff239-136">Response</span></span>
<span data-ttu-id="ff239-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ff239-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1279

{
  "value": {
    "@odata.type": "#microsoft.graph.iosCertificateProfile",
    "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "deviceManagementApplicabilityRuleOsEdition": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
      "osEditionTypes": [
        "windows10EnterpriseN"
      ],
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleOsVersion": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
      "minOSVersion": "Min OSVersion value",
      "maxOSVersion": "Max OSVersion value",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "deviceManagementApplicabilityRuleDeviceMode": {
      "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
      "deviceMode": "sModeConfiguration",
      "name": "Name value",
      "ruleType": "exclude"
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```




