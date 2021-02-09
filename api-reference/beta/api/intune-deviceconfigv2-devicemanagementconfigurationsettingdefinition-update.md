---
title: Обновление deviceManagementConfigurationSettingDefinition
description: Обновление свойств объекта deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1370c49932bb32e3fb96d0a1111b496094f69000
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160055"
---
# <a name="update-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="3d2d7-103">Обновление deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="3d2d7-103">Update deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="3d2d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d2d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d2d7-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d2d7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d2d7-107">Обновление свойств объекта [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3d2d7-107">Update the properties of a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d2d7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3d2d7-108">Prerequisites</span></span>
<span data-ttu-id="3d2d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d2d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d2d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d2d7-111">Permission type</span></span>|<span data-ttu-id="3d2d7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d2d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d2d7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d2d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d2d7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d2d7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3d2d7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d2d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d2d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-116">Not supported.</span></span>|
|<span data-ttu-id="3d2d7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d2d7-117">Application</span></span>|<span data-ttu-id="3d2d7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d2d7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d2d7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d2d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="3d2d7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3d2d7-120">Request headers</span></span>
|<span data-ttu-id="3d2d7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3d2d7-121">Header</span></span>|<span data-ttu-id="3d2d7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3d2d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d2d7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d2d7-123">Authorization</span></span>|<span data-ttu-id="3d2d7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d2d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3d2d7-125">Accept</span></span>|<span data-ttu-id="3d2d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d2d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d2d7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d2d7-127">Request body</span></span>
<span data-ttu-id="3d2d7-128">В теле запроса предопределение представления объекта [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

<span data-ttu-id="3d2d7-129">В следующей таблице показаны свойства, необходимые при создании [объекта deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="3d2d7-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span>

|<span data-ttu-id="3d2d7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3d2d7-130">Property</span></span>|<span data-ttu-id="3d2d7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3d2d7-131">Type</span></span>|<span data-ttu-id="3d2d7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3d2d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d2d7-133">применимость</span><span class="sxs-lookup"><span data-stu-id="3d2d7-133">applicability</span></span>|[<span data-ttu-id="3d2d7-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="3d2d7-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="3d2d7-135">Сведения о том, какой параметр устройства применим к</span><span class="sxs-lookup"><span data-stu-id="3d2d7-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="3d2d7-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="3d2d7-136">accessTypes</span></span>|[<span data-ttu-id="3d2d7-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="3d2d7-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="3d2d7-138">Режим доступа для чтения и записи параметра.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="3d2d7-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="3d2d7-140">keywords</span><span class="sxs-lookup"><span data-stu-id="3d2d7-140">keywords</span></span>|<span data-ttu-id="3d2d7-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3d2d7-141">String collection</span></span>|<span data-ttu-id="3d2d7-142">Маркеры, в которых необходимо искать параметры</span><span class="sxs-lookup"><span data-stu-id="3d2d7-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="3d2d7-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="3d2d7-143">infoUrls</span></span>|<span data-ttu-id="3d2d7-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3d2d7-144">String collection</span></span>|<span data-ttu-id="3d2d7-145">Список ссылок на дополнительные сведения о параметре можно найти по адресу</span><span class="sxs-lookup"><span data-stu-id="3d2d7-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="3d2d7-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="3d2d7-146">occurrence</span></span>|[<span data-ttu-id="3d2d7-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="3d2d7-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="3d2d7-148">Указывает, является ли параметр требуемой</span><span class="sxs-lookup"><span data-stu-id="3d2d7-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="3d2d7-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="3d2d7-149">baseUri</span></span>|<span data-ttu-id="3d2d7-150">String</span><span class="sxs-lookup"><span data-stu-id="3d2d7-150">String</span></span>|<span data-ttu-id="3d2d7-151">Базовый путь CSP</span><span class="sxs-lookup"><span data-stu-id="3d2d7-151">Base CSP Path</span></span>|
|<span data-ttu-id="3d2d7-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="3d2d7-152">offsetUri</span></span>|<span data-ttu-id="3d2d7-153">String</span><span class="sxs-lookup"><span data-stu-id="3d2d7-153">String</span></span>|<span data-ttu-id="3d2d7-154">Смещение пути CSP от базового</span><span class="sxs-lookup"><span data-stu-id="3d2d7-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="3d2d7-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="3d2d7-155">rootDefinitionId</span></span>|<span data-ttu-id="3d2d7-156">String</span><span class="sxs-lookup"><span data-stu-id="3d2d7-156">String</span></span>|<span data-ttu-id="3d2d7-157">Определение корневого параметра, если этот параметр является параметром-дитя.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="3d2d7-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="3d2d7-158">categoryId</span></span>|<span data-ttu-id="3d2d7-159">String</span><span class="sxs-lookup"><span data-stu-id="3d2d7-159">String</span></span>|<span data-ttu-id="3d2d7-160">Указывает группу области, в которой этот параметр настроен в указанном поставщике служб конфигурации (CSP)</span><span class="sxs-lookup"><span data-stu-id="3d2d7-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="3d2d7-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="3d2d7-161">settingUsage</span></span>|[<span data-ttu-id="3d2d7-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="3d2d7-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="3d2d7-163">Тип параметра, например конфигурация и соответствие требованиям.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="3d2d7-164">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="3d2d7-165">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="3d2d7-165">uxBehavior</span></span>|[<span data-ttu-id="3d2d7-166">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="3d2d7-166">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="3d2d7-167">Представление типа управления параметром в UX.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-167">Setting control type representation in the UX.</span></span> <span data-ttu-id="3d2d7-168">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-168">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="3d2d7-169">id</span><span class="sxs-lookup"><span data-stu-id="3d2d7-169">id</span></span>|<span data-ttu-id="3d2d7-170">String</span><span class="sxs-lookup"><span data-stu-id="3d2d7-170">String</span></span>|<span data-ttu-id="3d2d7-171">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="3d2d7-171">Identifier for item</span></span>|
|<span data-ttu-id="3d2d7-172">description</span><span class="sxs-lookup"><span data-stu-id="3d2d7-172">description</span></span>|<span data-ttu-id="3d2d7-173">String</span><span class="sxs-lookup"><span data-stu-id="3d2d7-173">String</span></span>|<span data-ttu-id="3d2d7-174">Описание элемента</span><span class="sxs-lookup"><span data-stu-id="3d2d7-174">Description of the item</span></span>|
|<span data-ttu-id="3d2d7-175">helpText</span><span class="sxs-lookup"><span data-stu-id="3d2d7-175">helpText</span></span>|<span data-ttu-id="3d2d7-176">String</span><span class="sxs-lookup"><span data-stu-id="3d2d7-176">String</span></span>|<span data-ttu-id="3d2d7-177">Текст справки для элемента</span><span class="sxs-lookup"><span data-stu-id="3d2d7-177">Help text of the item</span></span>|
|<span data-ttu-id="3d2d7-178">name</span><span class="sxs-lookup"><span data-stu-id="3d2d7-178">name</span></span>|<span data-ttu-id="3d2d7-179">String</span><span class="sxs-lookup"><span data-stu-id="3d2d7-179">String</span></span>|<span data-ttu-id="3d2d7-180">Имя элемента</span><span class="sxs-lookup"><span data-stu-id="3d2d7-180">Name of the item</span></span>|
|<span data-ttu-id="3d2d7-181">displayName</span><span class="sxs-lookup"><span data-stu-id="3d2d7-181">displayName</span></span>|<span data-ttu-id="3d2d7-182">String</span><span class="sxs-lookup"><span data-stu-id="3d2d7-182">String</span></span>|<span data-ttu-id="3d2d7-183">Отображаемого имени элемента</span><span class="sxs-lookup"><span data-stu-id="3d2d7-183">Display name of the item</span></span>|
|<span data-ttu-id="3d2d7-184">version</span><span class="sxs-lookup"><span data-stu-id="3d2d7-184">version</span></span>|<span data-ttu-id="3d2d7-185">String</span><span class="sxs-lookup"><span data-stu-id="3d2d7-185">String</span></span>|<span data-ttu-id="3d2d7-186">Версия элемента</span><span class="sxs-lookup"><span data-stu-id="3d2d7-186">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="3d2d7-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d2d7-187">Response</span></span>
<span data-ttu-id="3d2d7-188">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-188">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d2d7-189">Пример</span><span class="sxs-lookup"><span data-stu-id="3d2d7-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d2d7-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d2d7-190">Request</span></span>
<span data-ttu-id="3d2d7-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-191">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1006

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
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="3d2d7-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d2d7-192">Response</span></span>
<span data-ttu-id="3d2d7-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d2d7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1055

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
  "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```




