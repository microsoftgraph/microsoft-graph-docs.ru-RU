---
title: Список deviceManagementConfigurationSettingDefinitions
description: Список свойств и связей объектов deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 40ff3b97957a07045e29bf9c4669bea96106064e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665191"
---
# <a name="list-devicemanagementconfigurationsettingdefinitions"></a><span data-ttu-id="ca561-103">Список deviceManagementConfigurationSettingDefinitions</span><span class="sxs-lookup"><span data-stu-id="ca561-103">List deviceManagementConfigurationSettingDefinitions</span></span>

<span data-ttu-id="ca561-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca561-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca561-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca561-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca561-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca561-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca561-107">Список свойств и связей [объектов deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="ca561-107">List properties and relationships of the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca561-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ca561-108">Prerequisites</span></span>
<span data-ttu-id="ca561-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca561-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca561-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca561-111">Permission type</span></span>|<span data-ttu-id="ca561-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca561-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca561-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca561-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca561-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca561-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca561-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca561-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca561-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca561-116">Not supported.</span></span>|
|<span data-ttu-id="ca561-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ca561-117">Application</span></span>|<span data-ttu-id="ca561-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca561-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca561-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca561-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reusableSettings
GET /deviceManagement/configurationSettings
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
GET /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ca561-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ca561-120">Request headers</span></span>
|<span data-ttu-id="ca561-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca561-121">Header</span></span>|<span data-ttu-id="ca561-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ca561-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca561-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca561-123">Authorization</span></span>|<span data-ttu-id="ca561-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ca561-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca561-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ca561-125">Accept</span></span>|<span data-ttu-id="ca561-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca561-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca561-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca561-127">Request body</span></span>
<span data-ttu-id="ca561-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ca561-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca561-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca561-129">Response</span></span>
<span data-ttu-id="ca561-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ca561-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca561-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ca561-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca561-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca561-132">Request</span></span>
<span data-ttu-id="ca561-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca561-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusableSettings
```

### <a name="response"></a><span data-ttu-id="ca561-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca561-134">Response</span></span>
<span data-ttu-id="ca561-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ca561-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1496

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDefinition",
      "applicability": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingApplicability",
        "description": "Description value",
        "platform": "macOS",
        "deviceMode": "kiosk",
        "technologies": "mdm"
      },
      "accessTypes": "add",
      "keywords": [
        "Keywords value"
      ],
      "infoUrls": [
        "Info Urls value"
      ],
      "occurrence": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingOccurrence",
        "minDeviceOccurrence": 3,
        "maxDeviceOccurrence": 3
      },
      "baseUri": "Base Uri value",
      "offsetUri": "Offset Uri value",
      "rootDefinitionId": "Root Definition Id value",
      "categoryId": "Category Id value",
      "settingUsage": "configuration",
      "uxBehavior": "dropdown",
      "visibility": "settingsCatalog",
      "referredSettingInformationList": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
          "settingDefinitionId": "Setting Definition Id value"
        }
      ],
      "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value",
      "version": "Version value"
    }
  ]
}
```




