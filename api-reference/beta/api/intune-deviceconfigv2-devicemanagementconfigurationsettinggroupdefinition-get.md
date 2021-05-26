---
title: Get deviceManagementConfigurationSettingGroupDefinition
description: Чтение свойств и связей объекта deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2bba86cf0c575b34377a7db46bca44902e410aa6
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665457"
---
# <a name="get-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="4f0a5-103">Get deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="4f0a5-103">Get deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="4f0a5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f0a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f0a5-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f0a5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f0a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f0a5-107">Чтение свойств и связей [объекта deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="4f0a5-107">Read properties and relationships of the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f0a5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4f0a5-108">Prerequisites</span></span>
<span data-ttu-id="4f0a5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f0a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f0a5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f0a5-111">Permission type</span></span>|<span data-ttu-id="4f0a5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f0a5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f0a5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f0a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f0a5-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f0a5-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f0a5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f0a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f0a5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f0a5-116">Not supported.</span></span>|
|<span data-ttu-id="4f0a5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4f0a5-117">Application</span></span>|<span data-ttu-id="4f0a5-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f0a5-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f0a5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f0a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f0a5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f0a5-120">Optional query parameters</span></span>
<span data-ttu-id="4f0a5-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4f0a5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f0a5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f0a5-122">Request headers</span></span>
|<span data-ttu-id="4f0a5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f0a5-123">Header</span></span>|<span data-ttu-id="4f0a5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="4f0a5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f0a5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f0a5-125">Authorization</span></span>|<span data-ttu-id="4f0a5-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f0a5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f0a5-127">Accept</span><span class="sxs-lookup"><span data-stu-id="4f0a5-127">Accept</span></span>|<span data-ttu-id="4f0a5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4f0a5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f0a5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f0a5-129">Request body</span></span>
<span data-ttu-id="4f0a5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f0a5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f0a5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f0a5-131">Response</span></span>
<span data-ttu-id="4f0a5-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4f0a5-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f0a5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4f0a5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f0a5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f0a5-134">Request</span></span>
<span data-ttu-id="4f0a5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f0a5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="4f0a5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f0a5-136">Response</span></span>
<span data-ttu-id="4f0a5-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f0a5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1909

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupDefinition",
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
    "id": "95dc9604-9604-95dc-0496-dc950496dc95",
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
    ]
  }
}
```




