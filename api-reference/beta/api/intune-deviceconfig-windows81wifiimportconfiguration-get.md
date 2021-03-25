---
title: Get windows81WifiImportConfiguration
description: Чтение свойств и связей объекта Windows81WifiImportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f69d078269ae32c7f94e5169bc25503d51dfe6d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151048"
---
# <a name="get-windows81wifiimportconfiguration"></a><span data-ttu-id="d2c11-103">Get windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2c11-103">Get windows81WifiImportConfiguration</span></span>

<span data-ttu-id="d2c11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2c11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2c11-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2c11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2c11-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2c11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2c11-107">Чтение свойств и связей [объекта Windows81WifiImportConfiguration.](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2c11-107">Read properties and relationships of the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2c11-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d2c11-108">Prerequisites</span></span>
<span data-ttu-id="d2c11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2c11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2c11-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2c11-111">Permission type</span></span>|<span data-ttu-id="d2c11-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2c11-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2c11-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2c11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2c11-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2c11-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d2c11-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2c11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2c11-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2c11-116">Not supported.</span></span>|
|<span data-ttu-id="d2c11-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="d2c11-117">Application</span></span>|<span data-ttu-id="d2c11-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2c11-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2c11-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2c11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2c11-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2c11-120">Optional query parameters</span></span>
<span data-ttu-id="d2c11-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d2c11-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2c11-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2c11-122">Request headers</span></span>
|<span data-ttu-id="d2c11-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2c11-123">Header</span></span>|<span data-ttu-id="d2c11-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d2c11-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2c11-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2c11-125">Authorization</span></span>|<span data-ttu-id="d2c11-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2c11-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2c11-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d2c11-127">Accept</span></span>|<span data-ttu-id="d2c11-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d2c11-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2c11-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2c11-129">Request body</span></span>
<span data-ttu-id="d2c11-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2c11-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2c11-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2c11-131">Response</span></span>
<span data-ttu-id="d2c11-132">В случае успеха этот метод возвращает код отклика и `200 OK` [объект Windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d2c11-132">If successful, this method returns a `200 OK` response code and [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2c11-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d2c11-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2c11-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2c11-134">Request</span></span>
<span data-ttu-id="d2c11-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d2c11-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d2c11-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2c11-136">Response</span></span>
<span data-ttu-id="d2c11-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2c11-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1415

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
    "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
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
    "payloadFileName": "Payload File Name value",
    "profileName": "Profile Name value",
    "payload": "cGF5bG9hZA=="
  }
}
```




