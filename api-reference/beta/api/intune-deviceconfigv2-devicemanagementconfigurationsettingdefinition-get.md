---
title: Get deviceManagementConfigurationSettingDefinition
description: Чтение свойств и связей объекта deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 93b1726861e6a77f64661d8ef8d252cd4c9bcf30
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51862836"
---
# <a name="get-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="f2d3c-103">Get deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="f2d3c-103">Get deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="f2d3c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2d3c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2d3c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2d3c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2d3c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2d3c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2d3c-107">Чтение свойств и связей [объекта deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f2d3c-107">Read properties and relationships of the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2d3c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f2d3c-108">Prerequisites</span></span>
<span data-ttu-id="f2d3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2d3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2d3c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2d3c-111">Permission type</span></span>|<span data-ttu-id="f2d3c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2d3c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2d3c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2d3c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2d3c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2d3c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2d3c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2d3c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2d3c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2d3c-116">Not supported.</span></span>|
|<span data-ttu-id="f2d3c-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="f2d3c-117">Application</span></span>|<span data-ttu-id="f2d3c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2d3c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2d3c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2d3c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f2d3c-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f2d3c-120">Optional query parameters</span></span>
<span data-ttu-id="f2d3c-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f2d3c-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2d3c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2d3c-122">Request headers</span></span>
|<span data-ttu-id="f2d3c-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2d3c-123">Header</span></span>|<span data-ttu-id="f2d3c-124">Значение</span><span class="sxs-lookup"><span data-stu-id="f2d3c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2d3c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2d3c-125">Authorization</span></span>|<span data-ttu-id="f2d3c-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2d3c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2d3c-127">Accept</span><span class="sxs-lookup"><span data-stu-id="f2d3c-127">Accept</span></span>|<span data-ttu-id="f2d3c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f2d3c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2d3c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2d3c-129">Request body</span></span>
<span data-ttu-id="f2d3c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2d3c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2d3c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2d3c-131">Response</span></span>
<span data-ttu-id="f2d3c-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f2d3c-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2d3c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f2d3c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2d3c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2d3c-134">Request</span></span>
<span data-ttu-id="f2d3c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2d3c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reusableSettings/{deviceManagementConfigurationSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="f2d3c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2d3c-136">Response</span></span>
<span data-ttu-id="f2d3c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2d3c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1404

{
  "value": {
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
}
```




