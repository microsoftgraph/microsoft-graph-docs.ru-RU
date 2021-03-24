---
title: Get windows10EasEmailProfileConfiguration
description: Чтение свойств и связей объекта windows10EasEmailProfileConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2293c166f266e400c948010432bca36aa02fdcd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129456"
---
# <a name="get-windows10easemailprofileconfiguration"></a><span data-ttu-id="daf98-103">Get windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="daf98-103">Get windows10EasEmailProfileConfiguration</span></span>

<span data-ttu-id="daf98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daf98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="daf98-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daf98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daf98-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="daf98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daf98-107">Чтение свойств и связей [объекта windows10EasEmailProfileConfiguration.](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="daf98-107">Read properties and relationships of the [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="daf98-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="daf98-108">Prerequisites</span></span>
<span data-ttu-id="daf98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daf98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="daf98-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="daf98-111">Permission type</span></span>|<span data-ttu-id="daf98-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="daf98-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daf98-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="daf98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="daf98-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daf98-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="daf98-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="daf98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daf98-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daf98-116">Not supported.</span></span>|
|<span data-ttu-id="daf98-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="daf98-117">Application</span></span>|<span data-ttu-id="daf98-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daf98-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="daf98-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="daf98-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="daf98-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="daf98-120">Optional query parameters</span></span>
<span data-ttu-id="daf98-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="daf98-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="daf98-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="daf98-122">Request headers</span></span>
|<span data-ttu-id="daf98-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="daf98-123">Header</span></span>|<span data-ttu-id="daf98-124">Значение</span><span class="sxs-lookup"><span data-stu-id="daf98-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="daf98-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="daf98-125">Authorization</span></span>|<span data-ttu-id="daf98-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="daf98-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="daf98-127">Accept</span><span class="sxs-lookup"><span data-stu-id="daf98-127">Accept</span></span>|<span data-ttu-id="daf98-128">application/json</span><span class="sxs-lookup"><span data-stu-id="daf98-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="daf98-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="daf98-129">Request body</span></span>
<span data-ttu-id="daf98-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="daf98-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daf98-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="daf98-131">Response</span></span>
<span data-ttu-id="daf98-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект Windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="daf98-132">If successful, this method returns a `200 OK` response code and [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daf98-133">Пример</span><span class="sxs-lookup"><span data-stu-id="daf98-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="daf98-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="daf98-134">Request</span></span>
<span data-ttu-id="daf98-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="daf98-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="daf98-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="daf98-136">Response</span></span>
<span data-ttu-id="daf98-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="daf98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1807

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EasEmailProfileConfiguration",
    "id": "9dc6f073-f073-9dc6-73f0-c69d73f0c69d",
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
    "usernameSource": "primarySmtpAddress",
    "usernameAADSource": "primarySmtpAddress",
    "userDomainNameSource": "netBiosDomainName",
    "customDomainName": "Custom Domain Name value",
    "accountName": "Account Name value",
    "syncCalendar": true,
    "syncContacts": true,
    "syncTasks": true,
    "durationOfEmailToSync": "oneDay",
    "emailAddressSource": "primarySmtpAddress",
    "emailSyncSchedule": "asMessagesArrive",
    "hostName": "Host Name value",
    "requireSsl": true
  }
}
```




