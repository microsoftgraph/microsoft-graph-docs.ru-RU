---
title: Список Виндовсфониасемаилпрофилеконфигуратионс
description: Список свойств и связей объектов Виндовсфониасемаилпрофилеконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 68975a5ebac8fd2ad0b16e58ce6d4346f91e9709
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42473999"
---
# <a name="list-windowsphoneeasemailprofileconfigurations"></a><span data-ttu-id="a8731-103">Список Виндовсфониасемаилпрофилеконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="a8731-103">List windowsPhoneEASEmailProfileConfigurations</span></span>

<span data-ttu-id="a8731-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a8731-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a8731-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8731-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8731-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8731-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8731-107">Список свойств и связей объектов [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a8731-107">List properties and relationships of the [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8731-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a8731-108">Prerequisites</span></span>
<span data-ttu-id="a8731-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8731-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8731-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8731-111">Permission type</span></span>|<span data-ttu-id="a8731-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8731-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8731-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8731-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a8731-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8731-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a8731-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8731-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8731-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8731-116">Not supported.</span></span>|
|<span data-ttu-id="a8731-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8731-117">Application</span></span>|<span data-ttu-id="a8731-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8731-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8731-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8731-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a8731-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a8731-120">Request headers</span></span>
|<span data-ttu-id="a8731-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8731-121">Header</span></span>|<span data-ttu-id="a8731-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a8731-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8731-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8731-123">Authorization</span></span>|<span data-ttu-id="a8731-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8731-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8731-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a8731-125">Accept</span></span>|<span data-ttu-id="a8731-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a8731-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8731-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8731-127">Request body</span></span>
<span data-ttu-id="a8731-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8731-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8731-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8731-129">Response</span></span>
<span data-ttu-id="a8731-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсфониасемаилпрофилеконфигуратион](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a8731-130">If successful, this method returns a `200 OK` response code and a collection of [windowsPhoneEASEmailProfileConfiguration](../resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8731-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a8731-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8731-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8731-132">Request</span></span>
<span data-ttu-id="a8731-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8731-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a8731-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8731-134">Response</span></span>
<span data-ttu-id="a8731-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a8731-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1956

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhoneEASEmailProfileConfiguration",
      "id": "554f402a-402a-554f-2a40-4f552a404f55",
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
      "applyOnlyToWindowsPhone81": true,
      "syncCalendar": true,
      "syncContacts": true,
      "syncTasks": true,
      "durationOfEmailToSync": "oneDay",
      "emailAddressSource": "primarySmtpAddress",
      "emailSyncSchedule": "asMessagesArrive",
      "hostName": "Host Name value",
      "requireSsl": true
    }
  ]
}
```





