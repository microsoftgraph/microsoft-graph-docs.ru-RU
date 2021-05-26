---
title: Список deviceManagementConfigurationSettingGroupCollectionDefinitions
description: Список свойств и связей объектов deviceManagementConfigurationSettingGroupCollectionDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d3f54b474b8152449e8c1e3b7c06e5788d91c661
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665156"
---
# <a name="list-devicemanagementconfigurationsettinggroupcollectiondefinitions"></a><span data-ttu-id="5b381-103">Список deviceManagementConfigurationSettingGroupCollectionDefinitions</span><span class="sxs-lookup"><span data-stu-id="5b381-103">List deviceManagementConfigurationSettingGroupCollectionDefinitions</span></span>

<span data-ttu-id="5b381-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b381-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b381-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b381-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b381-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b381-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b381-107">Список свойств и связей объектов [deviceManagementConfigurationSettingGroupCollectionDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md)</span><span class="sxs-lookup"><span data-stu-id="5b381-107">List properties and relationships of the [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b381-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5b381-108">Prerequisites</span></span>
<span data-ttu-id="5b381-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b381-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b381-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b381-111">Permission type</span></span>|<span data-ttu-id="5b381-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b381-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b381-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b381-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b381-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b381-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b381-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b381-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b381-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b381-116">Not supported.</span></span>|
|<span data-ttu-id="5b381-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="5b381-117">Application</span></span>|<span data-ttu-id="5b381-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b381-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b381-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b381-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5b381-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5b381-120">Request headers</span></span>
|<span data-ttu-id="5b381-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b381-121">Header</span></span>|<span data-ttu-id="5b381-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5b381-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b381-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b381-123">Authorization</span></span>|<span data-ttu-id="5b381-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b381-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b381-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b381-125">Accept</span></span>|<span data-ttu-id="5b381-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b381-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b381-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b381-127">Request body</span></span>
<span data-ttu-id="5b381-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5b381-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b381-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b381-129">Response</span></span>
<span data-ttu-id="5b381-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5b381-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementConfigurationSettingGroupCollectionDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupcollectiondefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b381-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5b381-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b381-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b381-132">Request</span></span>
<span data-ttu-id="5b381-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b381-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusableSettings
```

### <a name="response"></a><span data-ttu-id="5b381-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b381-134">Response</span></span>
<span data-ttu-id="5b381-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b381-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2099

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionDefinition",
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
      "id": "739da194-a194-739d-94a1-9d7394a19d73",
      "description": "Description value",
      "helpText": "Help Text value",
      "name": "Name value",
      "displayName": "Display Name value",
      "version": "Version value",
      "childIds": [
        "Child Ids value"
      ],
      "dependentOn": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn",
          "dependentOn": "Dependent On value",
          "parentSettingId": "Parent Setting Id value"
        }
      ],
      "dependedOnBy": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
          "dependedOnBy": "Depended On By value",
          "required": true
        }
      ],
      "maximumCount": 12,
      "minimumCount": 12
    }
  ]
}
```




