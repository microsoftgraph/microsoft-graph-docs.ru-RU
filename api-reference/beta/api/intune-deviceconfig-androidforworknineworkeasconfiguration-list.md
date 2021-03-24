---
title: Список androidForWorkNineWorkEasConfigurations
description: Список свойств и связей объектов AndroidForWorkNineWorkEasConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b837e58091b0100541097809b28956e55dfd2cf6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128378"
---
# <a name="list-androidforworknineworkeasconfigurations"></a><span data-ttu-id="12871-103">Список androidForWorkNineWorkEasConfigurations</span><span class="sxs-lookup"><span data-stu-id="12871-103">List androidForWorkNineWorkEasConfigurations</span></span>

<span data-ttu-id="12871-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12871-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12871-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12871-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12871-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12871-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12871-107">Список свойств и связей объектов [AndroidForWorkNineWorkEasConfiguration.](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="12871-107">List properties and relationships of the [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12871-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="12871-108">Prerequisites</span></span>
<span data-ttu-id="12871-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12871-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12871-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12871-111">Permission type</span></span>|<span data-ttu-id="12871-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12871-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12871-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12871-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12871-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12871-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12871-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12871-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12871-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12871-116">Not supported.</span></span>|
|<span data-ttu-id="12871-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="12871-117">Application</span></span>|<span data-ttu-id="12871-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12871-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12871-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12871-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="12871-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="12871-120">Request headers</span></span>
|<span data-ttu-id="12871-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12871-121">Header</span></span>|<span data-ttu-id="12871-122">Значение</span><span class="sxs-lookup"><span data-stu-id="12871-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12871-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="12871-123">Authorization</span></span>|<span data-ttu-id="12871-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12871-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12871-125">Accept</span><span class="sxs-lookup"><span data-stu-id="12871-125">Accept</span></span>|<span data-ttu-id="12871-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12871-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12871-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12871-127">Request body</span></span>
<span data-ttu-id="12871-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12871-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12871-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="12871-129">Response</span></span>
<span data-ttu-id="12871-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="12871-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkNineWorkEasConfiguration](../resources/intune-deviceconfig-androidforworknineworkeasconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12871-131">Пример</span><span class="sxs-lookup"><span data-stu-id="12871-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="12871-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="12871-132">Request</span></span>
<span data-ttu-id="12871-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12871-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="12871-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="12871-134">Response</span></span>
<span data-ttu-id="12871-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12871-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1708

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkNineWorkEasConfiguration",
      "id": "f8ef19e0-19e0-f8ef-e019-eff8e019eff8",
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
      "authenticationMethod": "certificate",
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "hostName": "Host Name value",
      "requireSsl": true,
      "usernameSource": "userPrincipalName",
      "syncCalendar": true,
      "syncContacts": true,
      "syncTasks": true
    }
  ]
}
```




