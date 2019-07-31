---
title: Список Андроидцертификатепрофилебасес
description: Список свойств и связей объектов Андроидцертификатепрофилебасе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e2560c0399fd35a99b598cb1a816aba5818e766
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958321"
---
# <a name="list-androidcertificateprofilebases"></a><span data-ttu-id="88c81-103">Список Андроидцертификатепрофилебасес</span><span class="sxs-lookup"><span data-stu-id="88c81-103">List androidCertificateProfileBases</span></span>

> <span data-ttu-id="88c81-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88c81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88c81-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88c81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88c81-106">Список свойств и связей объектов [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="88c81-106">List properties and relationships of the [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88c81-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="88c81-107">Prerequisites</span></span>
<span data-ttu-id="88c81-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="88c81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88c81-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="88c81-110">Permission type</span></span>|<span data-ttu-id="88c81-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="88c81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88c81-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="88c81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88c81-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88c81-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="88c81-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="88c81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88c81-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88c81-115">Not supported.</span></span>|
|<span data-ttu-id="88c81-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="88c81-116">Application</span></span>|<span data-ttu-id="88c81-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88c81-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88c81-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="88c81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="88c81-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="88c81-119">Request headers</span></span>
|<span data-ttu-id="88c81-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="88c81-120">Header</span></span>|<span data-ttu-id="88c81-121">Значение</span><span class="sxs-lookup"><span data-stu-id="88c81-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88c81-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="88c81-122">Authorization</span></span>|<span data-ttu-id="88c81-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="88c81-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88c81-124">Accept</span><span class="sxs-lookup"><span data-stu-id="88c81-124">Accept</span></span>|<span data-ttu-id="88c81-125">application/json</span><span class="sxs-lookup"><span data-stu-id="88c81-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88c81-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="88c81-126">Request body</span></span>
<span data-ttu-id="88c81-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="88c81-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88c81-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="88c81-128">Response</span></span>
<span data-ttu-id="88c81-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидцертификатепрофилебасе](../resources/intune-deviceconfig-androidcertificateprofilebase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="88c81-129">If successful, this method returns a `200 OK` response code and a collection of [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88c81-130">Пример</span><span class="sxs-lookup"><span data-stu-id="88c81-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="88c81-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="88c81-131">Request</span></span>
<span data-ttu-id="88c81-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="88c81-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="88c81-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="88c81-133">Response</span></span>
<span data-ttu-id="88c81-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="88c81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1825

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidCertificateProfileBase",
      "id": "76cf241d-241d-76cf-1d24-cf761d24cf76",
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
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ]
    }
  ]
}
```





