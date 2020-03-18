---
title: Список windowsPhone81ImportedPFXCertificateProfiles
description: Список свойств и связей объектов windowsPhone81ImportedPFXCertificateProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6d3ef00ab0d69ee5aa49e70659b023d84b20743c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42733884"
---
# <a name="list-windowsphone81importedpfxcertificateprofiles"></a><span data-ttu-id="5db6e-103">Список windowsPhone81ImportedPFXCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="5db6e-103">List windowsPhone81ImportedPFXCertificateProfiles</span></span>

> <span data-ttu-id="5db6e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5db6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5db6e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5db6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5db6e-106">Список свойств и связей объектов [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="5db6e-106">List properties and relationships of the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5db6e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5db6e-107">Prerequisites</span></span>
<span data-ttu-id="5db6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5db6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5db6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5db6e-110">Permission type</span></span>|<span data-ttu-id="5db6e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5db6e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5db6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5db6e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5db6e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5db6e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5db6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5db6e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5db6e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5db6e-115">Not supported.</span></span>|
|<span data-ttu-id="5db6e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5db6e-116">Application</span></span>|<span data-ttu-id="5db6e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5db6e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5db6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5db6e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5db6e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5db6e-119">Request headers</span></span>
|<span data-ttu-id="5db6e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5db6e-120">Header</span></span>|<span data-ttu-id="5db6e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5db6e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5db6e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5db6e-122">Authorization</span></span>|<span data-ttu-id="5db6e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5db6e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5db6e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5db6e-124">Accept</span></span>|<span data-ttu-id="5db6e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5db6e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5db6e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5db6e-126">Request body</span></span>
<span data-ttu-id="5db6e-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5db6e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5db6e-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="5db6e-128">Response</span></span>
<span data-ttu-id="5db6e-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5db6e-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5db6e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5db6e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="5db6e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5db6e-131">Request</span></span>
<span data-ttu-id="5db6e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5db6e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="5db6e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="5db6e-133">Response</span></span>
<span data-ttu-id="5db6e-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5db6e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1725

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
      "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
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
      "version": 7,
      "renewalThresholdPercentage": 10,
      "keyStorageProvider": "useTpmKspOtherwiseFail",
      "subjectNameFormat": "commonNameIncludingEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```




