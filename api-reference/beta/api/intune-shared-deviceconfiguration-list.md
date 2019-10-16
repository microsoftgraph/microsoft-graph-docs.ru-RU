---
title: Перечисление объектов deviceConfiguration
description: Список свойств и связей объектов deviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b394d5cdfc12038ab02cd73981e6fea157e1f87
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537045"
---
# <a name="list-deviceconfigurations"></a><span data-ttu-id="2aa25-103">Перечисление объектов deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2aa25-103">List deviceConfigurations</span></span>

> <span data-ttu-id="2aa25-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2aa25-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2aa25-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2aa25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2aa25-106">Список свойств и связей объектов [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2aa25-106">List properties and relationships of the [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2aa25-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2aa25-107">Prerequisites</span></span>
<span data-ttu-id="2aa25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2aa25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2aa25-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2aa25-110">Permission type</span></span>|<span data-ttu-id="2aa25-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2aa25-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2aa25-112">Делегированная (Рабочая или учебная учетная запись</span><span class="sxs-lookup"><span data-stu-id="2aa25-112">Delegated (work or school account</span></span>||
| <span data-ttu-id="2aa25-113">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="2aa25-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="2aa25-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2aa25-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="2aa25-115">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2aa25-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2aa25-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2aa25-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2aa25-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2aa25-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2aa25-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2aa25-118">Not supported.</span></span>|
|<span data-ttu-id="2aa25-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="2aa25-119">Application</span></span>||
| <span data-ttu-id="2aa25-120">&nbsp; &nbsp; **Конфигурация устройств**</span><span class="sxs-lookup"><span data-stu-id="2aa25-120">&nbsp; &nbsp; **Device configuration**</span></span> |<span data-ttu-id="2aa25-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2aa25-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="2aa25-122">&nbsp;&nbsp; **Набор политик**</span><span class="sxs-lookup"><span data-stu-id="2aa25-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2aa25-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2aa25-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2aa25-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2aa25-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2aa25-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2aa25-125">Request headers</span></span>
|<span data-ttu-id="2aa25-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2aa25-126">Header</span></span>|<span data-ttu-id="2aa25-127">Значение</span><span class="sxs-lookup"><span data-stu-id="2aa25-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2aa25-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2aa25-128">Authorization</span></span>|<span data-ttu-id="2aa25-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2aa25-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2aa25-130">Accept</span><span class="sxs-lookup"><span data-stu-id="2aa25-130">Accept</span></span>|<span data-ttu-id="2aa25-131">application/json</span><span class="sxs-lookup"><span data-stu-id="2aa25-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2aa25-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2aa25-132">Request body</span></span>
<span data-ttu-id="2aa25-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2aa25-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2aa25-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2aa25-134">Response</span></span>
<span data-ttu-id="2aa25-135">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2aa25-135">If successful, this method returns a `200 OK` response code and a collection of [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2aa25-136">Пример</span><span class="sxs-lookup"><span data-stu-id="2aa25-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="2aa25-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="2aa25-137">Request</span></span>
<span data-ttu-id="2aa25-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2aa25-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="2aa25-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2aa25-139">Response</span></span>
<span data-ttu-id="2aa25-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2aa25-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1355

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfiguration",
      "id": "34977265-7265-3497-6572-973465729734",
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
      "version": 7
    }
  ]
}
```






