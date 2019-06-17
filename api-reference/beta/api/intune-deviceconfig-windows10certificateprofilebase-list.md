---
title: Список windows10CertificateProfileBases
description: Список свойств и связей объектов windows10CertificateProfileBase.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a792369fb7d8ad21b897e57266407bae91bf0040
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976206"
---
# <a name="list-windows10certificateprofilebases"></a><span data-ttu-id="edce7-103">Список windows10CertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="edce7-103">List windows10CertificateProfileBases</span></span>

> <span data-ttu-id="edce7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edce7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="edce7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edce7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edce7-106">Список свойств и связей объектов [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="edce7-106">List properties and relationships of the [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edce7-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="edce7-107">Prerequisites</span></span>
<span data-ttu-id="edce7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edce7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edce7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edce7-110">Permission type</span></span>|<span data-ttu-id="edce7-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="edce7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edce7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edce7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="edce7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="edce7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="edce7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edce7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edce7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edce7-115">Not supported.</span></span>|
|<span data-ttu-id="edce7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edce7-116">Application</span></span>|<span data-ttu-id="edce7-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edce7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="edce7-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edce7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="edce7-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edce7-119">Request headers</span></span>
|<span data-ttu-id="edce7-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="edce7-120">Header</span></span>|<span data-ttu-id="edce7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="edce7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edce7-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edce7-122">Authorization</span></span>|<span data-ttu-id="edce7-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edce7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edce7-124">Accept</span><span class="sxs-lookup"><span data-stu-id="edce7-124">Accept</span></span>|<span data-ttu-id="edce7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="edce7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edce7-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="edce7-126">Request body</span></span>
<span data-ttu-id="edce7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="edce7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edce7-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="edce7-128">Response</span></span>
<span data-ttu-id="edce7-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="edce7-129">If successful, this method returns a `200 OK` response code and a collection of [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edce7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="edce7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="edce7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="edce7-131">Request</span></span>
<span data-ttu-id="edce7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edce7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="edce7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="edce7-133">Response</span></span>
<span data-ttu-id="edce7-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="edce7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1668

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CertificateProfileBase",
      "id": "1f01ffc6-ffc6-1f01-c6ff-011fc6ff011f",
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
      "certificateValidityPeriodScale": "months"
    }
  ]
}
```





