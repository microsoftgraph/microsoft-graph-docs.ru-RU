---
title: Создание deviceManagementConfigurationSettingDefinition
description: Создание объекта deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8948ad0f1c4224a1febc0bbd84433c26674065b3
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161097"
---
# <a name="create-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="272a6-103">Создание deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="272a6-103">Create deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="272a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="272a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="272a6-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="272a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="272a6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="272a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="272a6-107">Создание объекта [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="272a6-107">Create a new [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="272a6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="272a6-108">Prerequisites</span></span>
<span data-ttu-id="272a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="272a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="272a6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="272a6-111">Permission type</span></span>|<span data-ttu-id="272a6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="272a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="272a6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="272a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="272a6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="272a6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="272a6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="272a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="272a6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="272a6-116">Not supported.</span></span>|
|<span data-ttu-id="272a6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="272a6-117">Application</span></span>|<span data-ttu-id="272a6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="272a6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="272a6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="272a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="272a6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="272a6-120">Request headers</span></span>
|<span data-ttu-id="272a6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="272a6-121">Header</span></span>|<span data-ttu-id="272a6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="272a6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="272a6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="272a6-123">Authorization</span></span>|<span data-ttu-id="272a6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="272a6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="272a6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="272a6-125">Accept</span></span>|<span data-ttu-id="272a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="272a6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="272a6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="272a6-127">Request body</span></span>
<span data-ttu-id="272a6-128">В теле запроса предопределение представления объекта deviceManagementConfigurationSettingDefinition в JSON.</span><span class="sxs-lookup"><span data-stu-id="272a6-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingDefinition object.</span></span>

<span data-ttu-id="272a6-129">В следующей таблице показаны свойства, необходимые при создании объекта deviceManagementConfigurationSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="272a6-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingDefinition.</span></span>

|<span data-ttu-id="272a6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="272a6-130">Property</span></span>|<span data-ttu-id="272a6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="272a6-131">Type</span></span>|<span data-ttu-id="272a6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="272a6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="272a6-133">применимость</span><span class="sxs-lookup"><span data-stu-id="272a6-133">applicability</span></span>|[<span data-ttu-id="272a6-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="272a6-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="272a6-135">Сведения о том, какой параметр устройства применим к</span><span class="sxs-lookup"><span data-stu-id="272a6-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="272a6-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="272a6-136">accessTypes</span></span>|[<span data-ttu-id="272a6-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="272a6-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="272a6-138">Режим доступа для чтения и записи параметра.</span><span class="sxs-lookup"><span data-stu-id="272a6-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="272a6-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="272a6-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="272a6-140">keywords</span><span class="sxs-lookup"><span data-stu-id="272a6-140">keywords</span></span>|<span data-ttu-id="272a6-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="272a6-141">String collection</span></span>|<span data-ttu-id="272a6-142">Маркеры, в которых необходимо искать параметры</span><span class="sxs-lookup"><span data-stu-id="272a6-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="272a6-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="272a6-143">infoUrls</span></span>|<span data-ttu-id="272a6-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="272a6-144">String collection</span></span>|<span data-ttu-id="272a6-145">Список ссылок на дополнительные сведения о параметре можно найти по адресу</span><span class="sxs-lookup"><span data-stu-id="272a6-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="272a6-146">occurrence</span><span class="sxs-lookup"><span data-stu-id="272a6-146">occurrence</span></span>|[<span data-ttu-id="272a6-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="272a6-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="272a6-148">Указывает, является ли параметр требуемой</span><span class="sxs-lookup"><span data-stu-id="272a6-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="272a6-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="272a6-149">baseUri</span></span>|<span data-ttu-id="272a6-150">String</span><span class="sxs-lookup"><span data-stu-id="272a6-150">String</span></span>|<span data-ttu-id="272a6-151">Базовый путь CSP</span><span class="sxs-lookup"><span data-stu-id="272a6-151">Base CSP Path</span></span>|
|<span data-ttu-id="272a6-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="272a6-152">offsetUri</span></span>|<span data-ttu-id="272a6-153">String</span><span class="sxs-lookup"><span data-stu-id="272a6-153">String</span></span>|<span data-ttu-id="272a6-154">Смещение пути CSP от базового</span><span class="sxs-lookup"><span data-stu-id="272a6-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="272a6-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="272a6-155">rootDefinitionId</span></span>|<span data-ttu-id="272a6-156">String</span><span class="sxs-lookup"><span data-stu-id="272a6-156">String</span></span>|<span data-ttu-id="272a6-157">Определение корневого параметра, если этот параметр является параметром-child.</span><span class="sxs-lookup"><span data-stu-id="272a6-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="272a6-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="272a6-158">categoryId</span></span>|<span data-ttu-id="272a6-159">String</span><span class="sxs-lookup"><span data-stu-id="272a6-159">String</span></span>|<span data-ttu-id="272a6-160">Указывает группу области, в которой этот параметр настроен в указанном поставщике служб конфигурации (CSP)</span><span class="sxs-lookup"><span data-stu-id="272a6-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="272a6-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="272a6-161">settingUsage</span></span>|[<span data-ttu-id="272a6-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="272a6-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="272a6-163">Тип параметра, например конфигурация и соответствие требованиям.</span><span class="sxs-lookup"><span data-stu-id="272a6-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="272a6-164">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="272a6-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="272a6-165">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="272a6-165">uxBehavior</span></span>|[<span data-ttu-id="272a6-166">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="272a6-166">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="272a6-167">Представление типа управления параметром в UX.</span><span class="sxs-lookup"><span data-stu-id="272a6-167">Setting control type representation in the UX.</span></span> <span data-ttu-id="272a6-168">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="272a6-168">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="272a6-169">id</span><span class="sxs-lookup"><span data-stu-id="272a6-169">id</span></span>|<span data-ttu-id="272a6-170">String</span><span class="sxs-lookup"><span data-stu-id="272a6-170">String</span></span>|<span data-ttu-id="272a6-171">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="272a6-171">Identifier for item</span></span>|
|<span data-ttu-id="272a6-172">description</span><span class="sxs-lookup"><span data-stu-id="272a6-172">description</span></span>|<span data-ttu-id="272a6-173">String</span><span class="sxs-lookup"><span data-stu-id="272a6-173">String</span></span>|<span data-ttu-id="272a6-174">Описание элемента</span><span class="sxs-lookup"><span data-stu-id="272a6-174">Description of the item</span></span>|
|<span data-ttu-id="272a6-175">helpText</span><span class="sxs-lookup"><span data-stu-id="272a6-175">helpText</span></span>|<span data-ttu-id="272a6-176">String</span><span class="sxs-lookup"><span data-stu-id="272a6-176">String</span></span>|<span data-ttu-id="272a6-177">Текст справки для элемента</span><span class="sxs-lookup"><span data-stu-id="272a6-177">Help text of the item</span></span>|
|<span data-ttu-id="272a6-178">name</span><span class="sxs-lookup"><span data-stu-id="272a6-178">name</span></span>|<span data-ttu-id="272a6-179">String</span><span class="sxs-lookup"><span data-stu-id="272a6-179">String</span></span>|<span data-ttu-id="272a6-180">Имя элемента</span><span class="sxs-lookup"><span data-stu-id="272a6-180">Name of the item</span></span>|
|<span data-ttu-id="272a6-181">displayName</span><span class="sxs-lookup"><span data-stu-id="272a6-181">displayName</span></span>|<span data-ttu-id="272a6-182">String</span><span class="sxs-lookup"><span data-stu-id="272a6-182">String</span></span>|<span data-ttu-id="272a6-183">Отображаемого имени элемента</span><span class="sxs-lookup"><span data-stu-id="272a6-183">Display name of the item</span></span>|
|<span data-ttu-id="272a6-184">version</span><span class="sxs-lookup"><span data-stu-id="272a6-184">version</span></span>|<span data-ttu-id="272a6-185">String</span><span class="sxs-lookup"><span data-stu-id="272a6-185">String</span></span>|<span data-ttu-id="272a6-186">Версия элемента</span><span class="sxs-lookup"><span data-stu-id="272a6-186">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="272a6-187">Отклик</span><span class="sxs-lookup"><span data-stu-id="272a6-187">Response</span></span>
<span data-ttu-id="272a6-188">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="272a6-188">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="272a6-189">Пример</span><span class="sxs-lookup"><span data-stu-id="272a6-189">Example</span></span>

### <a name="request"></a><span data-ttu-id="272a6-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="272a6-190">Request</span></span>
<span data-ttu-id="272a6-191">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="272a6-191">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationSettings
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

### <a name="response"></a><span data-ttu-id="272a6-192">Отклик</span><span class="sxs-lookup"><span data-stu-id="272a6-192">Response</span></span>
<span data-ttu-id="272a6-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="272a6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




