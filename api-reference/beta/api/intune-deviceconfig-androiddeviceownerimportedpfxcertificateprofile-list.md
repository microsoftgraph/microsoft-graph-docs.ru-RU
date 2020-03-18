---
title: Список Андроиддевицеовнеримпортедпфксцертификатепрофилес
description: Список свойств и связей объектов Андроиддевицеовнеримпортедпфксцертификатепрофиле.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b6c1d06336838e1c81a87a0247d1a4c23295e8c2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759768"
---
# <a name="list-androiddeviceownerimportedpfxcertificateprofiles"></a><span data-ttu-id="6c679-103">Список Андроиддевицеовнеримпортедпфксцертификатепрофилес</span><span class="sxs-lookup"><span data-stu-id="6c679-103">List androidDeviceOwnerImportedPFXCertificateProfiles</span></span>

> <span data-ttu-id="6c679-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c679-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c679-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c679-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c679-106">Список свойств и связей объектов [андроиддевицеовнеримпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6c679-106">List properties and relationships of the [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c679-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6c679-107">Prerequisites</span></span>
<span data-ttu-id="6c679-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c679-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c679-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6c679-110">Permission type</span></span>|<span data-ttu-id="6c679-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6c679-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c679-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6c679-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c679-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c679-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6c679-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6c679-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c679-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c679-115">Not supported.</span></span>|
|<span data-ttu-id="6c679-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="6c679-116">Application</span></span>|<span data-ttu-id="6c679-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c679-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c679-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6c679-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6c679-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6c679-119">Request headers</span></span>
|<span data-ttu-id="6c679-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6c679-120">Header</span></span>|<span data-ttu-id="6c679-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6c679-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c679-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c679-122">Authorization</span></span>|<span data-ttu-id="6c679-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6c679-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c679-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6c679-124">Accept</span></span>|<span data-ttu-id="6c679-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c679-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c679-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6c679-126">Request body</span></span>
<span data-ttu-id="6c679-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6c679-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c679-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="6c679-128">Response</span></span>
<span data-ttu-id="6c679-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроиддевицеовнеримпортедпфксцертификатепрофиле](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6c679-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerImportedPFXCertificateProfile](../resources/intune-deviceconfig-androiddeviceownerimportedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c679-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6c679-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c679-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6c679-131">Request</span></span>
<span data-ttu-id="6c679-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6c679-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="6c679-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6c679-133">Response</span></span>
<span data-ttu-id="6c679-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6c679-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1888

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerImportedPFXCertificateProfile",
      "id": "8d46d3c7-d3c7-8d46-c7d3-468dc7d3468d",
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
      "subjectNameFormat": "commonNameIncludingEmail",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "subjectAlternativeNameType": "emailAddress",
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```




