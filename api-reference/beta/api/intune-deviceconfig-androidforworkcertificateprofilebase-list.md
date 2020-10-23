---
title: Список Андроидфорворкцертификатепрофилебасес
description: Список свойств и связей объектов Андроидфорворкцертификатепрофилебасе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba066ab8fc3cbf8d7d0088b888dc9743b2f84fe1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733100"
---
# <a name="list-androidforworkcertificateprofilebases"></a><span data-ttu-id="af958-103">Список Андроидфорворкцертификатепрофилебасес</span><span class="sxs-lookup"><span data-stu-id="af958-103">List androidForWorkCertificateProfileBases</span></span>

<span data-ttu-id="af958-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af958-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af958-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af958-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af958-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af958-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af958-107">Список свойств и связей объектов [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="af958-107">List properties and relationships of the [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af958-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="af958-108">Prerequisites</span></span>
<span data-ttu-id="af958-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af958-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af958-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af958-111">Permission type</span></span>|<span data-ttu-id="af958-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af958-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af958-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af958-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af958-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="af958-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="af958-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af958-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af958-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af958-116">Not supported.</span></span>|
|<span data-ttu-id="af958-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af958-117">Application</span></span>|<span data-ttu-id="af958-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="af958-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af958-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af958-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="af958-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="af958-120">Request headers</span></span>
|<span data-ttu-id="af958-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af958-121">Header</span></span>|<span data-ttu-id="af958-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af958-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af958-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af958-123">Authorization</span></span>|<span data-ttu-id="af958-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af958-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af958-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af958-125">Accept</span></span>|<span data-ttu-id="af958-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af958-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af958-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af958-127">Request body</span></span>
<span data-ttu-id="af958-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af958-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af958-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="af958-129">Response</span></span>
<span data-ttu-id="af958-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидфорворкцертификатепрофилебасе](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af958-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af958-131">Пример</span><span class="sxs-lookup"><span data-stu-id="af958-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="af958-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="af958-132">Request</span></span>
<span data-ttu-id="af958-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af958-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="af958-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="af958-134">Response</span></span>
<span data-ttu-id="af958-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af958-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1832

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkCertificateProfileBase",
      "id": "87f1d53b-d53b-87f1-3bd5-f1873bd5f187",
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
      "subjectAlternativeNameType": "emailAddress"
    }
  ]
}
```





