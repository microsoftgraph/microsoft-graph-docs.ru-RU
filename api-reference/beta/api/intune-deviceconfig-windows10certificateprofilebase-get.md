---
title: Получение windows10CertificateProfileBase
description: Чтение свойств и связей объекта windows10CertificateProfileBase.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f20311d3a4a45a52bf4b51b31a12552c827cbda
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42482155"
---
# <a name="get-windows10certificateprofilebase"></a><span data-ttu-id="a475a-103">Получение windows10CertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="a475a-103">Get windows10CertificateProfileBase</span></span>

<span data-ttu-id="a475a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a475a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a475a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a475a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a475a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a475a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a475a-107">Чтение свойств и связей объекта [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="a475a-107">Read properties and relationships of the [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a475a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a475a-108">Prerequisites</span></span>
<span data-ttu-id="a475a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a475a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a475a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a475a-111">Permission type</span></span>|<span data-ttu-id="a475a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a475a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a475a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a475a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a475a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a475a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a475a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a475a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a475a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a475a-116">Not supported.</span></span>|
|<span data-ttu-id="a475a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a475a-117">Application</span></span>|<span data-ttu-id="a475a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a475a-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a475a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a475a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a475a-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a475a-120">Optional query parameters</span></span>
<span data-ttu-id="a475a-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a475a-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a475a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a475a-122">Request headers</span></span>
|<span data-ttu-id="a475a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a475a-123">Header</span></span>|<span data-ttu-id="a475a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a475a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a475a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a475a-125">Authorization</span></span>|<span data-ttu-id="a475a-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a475a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a475a-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a475a-127">Accept</span></span>|<span data-ttu-id="a475a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a475a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a475a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a475a-129">Request body</span></span>
<span data-ttu-id="a475a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a475a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a475a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="a475a-131">Response</span></span>
<span data-ttu-id="a475a-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a475a-132">If successful, this method returns a `200 OK` response code and [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a475a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="a475a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a475a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a475a-134">Request</span></span>
<span data-ttu-id="a475a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a475a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a475a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a475a-136">Response</span></span>
<span data-ttu-id="a475a-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a475a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1578

{
  "value": {
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
}
```





