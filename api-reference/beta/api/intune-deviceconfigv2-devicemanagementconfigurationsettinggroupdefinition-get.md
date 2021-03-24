---
title: Get deviceManagementConfigurationSettingGroupDefinition
description: Чтение свойств и связей объекта deviceManagementConfigurationSettingGroupDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03c9d864f63e703d6868cf194ca139d97b66d804
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129218"
---
# <a name="get-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="bc0fe-103">Get deviceManagementConfigurationSettingGroupDefinition</span><span class="sxs-lookup"><span data-stu-id="bc0fe-103">Get deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="bc0fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc0fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc0fe-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc0fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc0fe-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc0fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc0fe-107">Чтение свойств и связей [объекта deviceManagementConfigurationSettingGroupDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="bc0fe-107">Read properties and relationships of the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc0fe-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bc0fe-108">Prerequisites</span></span>
<span data-ttu-id="bc0fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc0fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc0fe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc0fe-111">Permission type</span></span>|<span data-ttu-id="bc0fe-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc0fe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc0fe-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc0fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc0fe-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fe-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bc0fe-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc0fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc0fe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc0fe-116">Not supported.</span></span>|
|<span data-ttu-id="bc0fe-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bc0fe-117">Application</span></span>|<span data-ttu-id="bc0fe-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fe-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc0fe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc0fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc0fe-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bc0fe-120">Optional query parameters</span></span>
<span data-ttu-id="bc0fe-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bc0fe-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc0fe-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc0fe-122">Request headers</span></span>
|<span data-ttu-id="bc0fe-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc0fe-123">Header</span></span>|<span data-ttu-id="bc0fe-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bc0fe-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc0fe-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc0fe-125">Authorization</span></span>|<span data-ttu-id="bc0fe-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc0fe-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc0fe-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bc0fe-127">Accept</span></span>|<span data-ttu-id="bc0fe-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bc0fe-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc0fe-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc0fe-129">Request body</span></span>
<span data-ttu-id="bc0fe-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc0fe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc0fe-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc0fe-131">Response</span></span>
<span data-ttu-id="bc0fe-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="bc0fe-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc0fe-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bc0fe-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc0fe-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc0fe-134">Request</span></span>
<span data-ttu-id="bc0fe-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc0fe-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="bc0fe-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc0fe-136">Response</span></span>
<span data-ttu-id="bc0fe-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc0fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1681

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




