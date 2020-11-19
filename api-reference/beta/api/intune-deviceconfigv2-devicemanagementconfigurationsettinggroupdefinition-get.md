---
title: Получение Девицеманажементконфигуратионсеттингграупдефинитион
description: Чтение свойств и связей объекта Девицеманажементконфигуратионсеттингграупдефинитион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c935a41db0da46d782e3d92c637a0a440200eca
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242494"
---
# <a name="get-devicemanagementconfigurationsettinggroupdefinition"></a><span data-ttu-id="e4919-103">Получение Девицеманажементконфигуратионсеттингграупдефинитион</span><span class="sxs-lookup"><span data-stu-id="e4919-103">Get deviceManagementConfigurationSettingGroupDefinition</span></span>

<span data-ttu-id="e4919-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4919-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4919-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4919-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4919-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4919-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4919-107">Чтение свойств и связей объекта [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="e4919-107">Read properties and relationships of the [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4919-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e4919-108">Prerequisites</span></span>
<span data-ttu-id="e4919-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4919-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4919-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4919-111">Permission type</span></span>|<span data-ttu-id="e4919-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4919-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4919-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4919-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4919-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4919-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e4919-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4919-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4919-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4919-116">Not supported.</span></span>|
|<span data-ttu-id="e4919-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e4919-117">Application</span></span>|<span data-ttu-id="e4919-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4919-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4919-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4919-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
GET /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4919-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e4919-120">Optional query parameters</span></span>
<span data-ttu-id="e4919-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e4919-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4919-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4919-122">Request headers</span></span>
|<span data-ttu-id="e4919-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4919-123">Header</span></span>|<span data-ttu-id="e4919-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e4919-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4919-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4919-125">Authorization</span></span>|<span data-ttu-id="e4919-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4919-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4919-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e4919-127">Accept</span></span>|<span data-ttu-id="e4919-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e4919-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4919-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4919-129">Request body</span></span>
<span data-ttu-id="e4919-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4919-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4919-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4919-131">Response</span></span>
<span data-ttu-id="e4919-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементконфигуратионсеттингграупдефинитион](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4919-132">If successful, this method returns a `200 OK` response code and [deviceManagementConfigurationSettingGroupDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinggroupdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4919-133">Пример</span><span class="sxs-lookup"><span data-stu-id="e4919-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4919-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4919-134">Request</span></span>
<span data-ttu-id="e4919-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4919-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
```

### <a name="response"></a><span data-ttu-id="e4919-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4919-136">Response</span></span>
<span data-ttu-id="e4919-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4919-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1612

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




