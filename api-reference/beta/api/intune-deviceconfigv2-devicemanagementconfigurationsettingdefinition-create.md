---
title: Создание deviceManagementConfigurationSettingDefinition
description: Создайте новый объект deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0c421989d170e99f2ce06aa86f5c856afdbcdcae
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665212"
---
# <a name="create-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="fe592-103">Создание deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="fe592-103">Create deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="fe592-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe592-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe592-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe592-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe592-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe592-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe592-107">Создайте новый [объект deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fe592-107">Create a new [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe592-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fe592-108">Prerequisites</span></span>
<span data-ttu-id="fe592-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe592-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe592-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe592-111">Permission type</span></span>|<span data-ttu-id="fe592-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe592-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe592-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe592-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe592-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe592-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe592-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe592-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe592-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe592-116">Not supported.</span></span>|
|<span data-ttu-id="fe592-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fe592-117">Application</span></span>|<span data-ttu-id="fe592-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe592-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe592-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe592-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reusableSettings
POST /deviceManagement/configurationSettings
POST /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions
POST /deviceManagement/configurationPolicyTemplates/{deviceManagementConfigurationPolicyTemplateId}/settingTemplates/{deviceManagementConfigurationSettingTemplateId}/settingDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="fe592-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fe592-120">Request headers</span></span>
|<span data-ttu-id="fe592-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe592-121">Header</span></span>|<span data-ttu-id="fe592-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fe592-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe592-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe592-123">Authorization</span></span>|<span data-ttu-id="fe592-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe592-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe592-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe592-125">Accept</span></span>|<span data-ttu-id="fe592-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe592-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe592-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe592-127">Request body</span></span>
<span data-ttu-id="fe592-128">В теле запроса поставляем представление JSON для объекта deviceManagementConfigurationSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="fe592-128">In the request body, supply a JSON representation for the deviceManagementConfigurationSettingDefinition object.</span></span>

<span data-ttu-id="fe592-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementConfigurationSettingDefinition.</span><span class="sxs-lookup"><span data-stu-id="fe592-129">The following table shows the properties that are required when you create the deviceManagementConfigurationSettingDefinition.</span></span>

|<span data-ttu-id="fe592-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe592-130">Property</span></span>|<span data-ttu-id="fe592-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fe592-131">Type</span></span>|<span data-ttu-id="fe592-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fe592-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe592-133">применимость</span><span class="sxs-lookup"><span data-stu-id="fe592-133">applicability</span></span>|[<span data-ttu-id="fe592-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="fe592-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="fe592-135">Сведения о том, какие параметры устройства применимы к</span><span class="sxs-lookup"><span data-stu-id="fe592-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="fe592-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="fe592-136">accessTypes</span></span>|[<span data-ttu-id="fe592-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="fe592-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="fe592-138">Режим доступа к режиму чтения и записи параметра.</span><span class="sxs-lookup"><span data-stu-id="fe592-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="fe592-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="fe592-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="fe592-140">keywords</span><span class="sxs-lookup"><span data-stu-id="fe592-140">keywords</span></span>|<span data-ttu-id="fe592-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fe592-141">String collection</span></span>|<span data-ttu-id="fe592-142">Маркеры для поиска параметров на</span><span class="sxs-lookup"><span data-stu-id="fe592-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="fe592-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="fe592-143">infoUrls</span></span>|<span data-ttu-id="fe592-144">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fe592-144">String collection</span></span>|<span data-ttu-id="fe592-145">Список ссылок, дополнительные сведения о параметре можно найти по адресу</span><span class="sxs-lookup"><span data-stu-id="fe592-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="fe592-146">возникновение</span><span class="sxs-lookup"><span data-stu-id="fe592-146">occurrence</span></span>|[<span data-ttu-id="fe592-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="fe592-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="fe592-148">Указывает, требуется ли параметр или нет.</span><span class="sxs-lookup"><span data-stu-id="fe592-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="fe592-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="fe592-149">baseUri</span></span>|<span data-ttu-id="fe592-150">Строка</span><span class="sxs-lookup"><span data-stu-id="fe592-150">String</span></span>|<span data-ttu-id="fe592-151">Базовый путь CSP</span><span class="sxs-lookup"><span data-stu-id="fe592-151">Base CSP Path</span></span>|
|<span data-ttu-id="fe592-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="fe592-152">offsetUri</span></span>|<span data-ttu-id="fe592-153">Строка</span><span class="sxs-lookup"><span data-stu-id="fe592-153">String</span></span>|<span data-ttu-id="fe592-154">Смещение пути CSP из базы</span><span class="sxs-lookup"><span data-stu-id="fe592-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="fe592-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="fe592-155">rootDefinitionId</span></span>|<span data-ttu-id="fe592-156">Строка</span><span class="sxs-lookup"><span data-stu-id="fe592-156">String</span></span>|<span data-ttu-id="fe592-157">Определение корневого параметра, если это параметр ребенка.</span><span class="sxs-lookup"><span data-stu-id="fe592-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="fe592-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="fe592-158">categoryId</span></span>|<span data-ttu-id="fe592-159">Строка</span><span class="sxs-lookup"><span data-stu-id="fe592-159">String</span></span>|<span data-ttu-id="fe592-160">Указывает группу области, в которой параметр настроен в указанном поставщике служб конфигурации (CSP)</span><span class="sxs-lookup"><span data-stu-id="fe592-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="fe592-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="fe592-161">settingUsage</span></span>|[<span data-ttu-id="fe592-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="fe592-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="fe592-163">Параметр типа, например конфигурации и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="fe592-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="fe592-164">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="fe592-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="fe592-165">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="fe592-165">uxBehavior</span></span>|[<span data-ttu-id="fe592-166">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="fe592-166">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="fe592-167">Настройка представления типа управления в UX.</span><span class="sxs-lookup"><span data-stu-id="fe592-167">Setting control type representation in the UX.</span></span> <span data-ttu-id="fe592-168">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="fe592-168">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="fe592-169">visibility</span><span class="sxs-lookup"><span data-stu-id="fe592-169">visibility</span></span>|[<span data-ttu-id="fe592-170">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="fe592-170">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="fe592-171">Настройка области видимости для UX.</span><span class="sxs-lookup"><span data-stu-id="fe592-171">Setting visibility scope to UX.</span></span> <span data-ttu-id="fe592-172">Возможные значения: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="fe592-172">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="fe592-173">referredSettingInformationList</span><span class="sxs-lookup"><span data-stu-id="fe592-173">referredSettingInformationList</span></span>|<span data-ttu-id="fe592-174">[коллекция deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md)</span><span class="sxs-lookup"><span data-stu-id="fe592-174">[deviceManagementConfigurationReferredSettingInformation](../resources/intune-deviceconfigv2-devicemanagementconfigurationreferredsettinginformation.md) collection</span></span>|<span data-ttu-id="fe592-175">Список переданных сведений о параметрах.</span><span class="sxs-lookup"><span data-stu-id="fe592-175">List of referred setting information.</span></span>|
|<span data-ttu-id="fe592-176">id</span><span class="sxs-lookup"><span data-stu-id="fe592-176">id</span></span>|<span data-ttu-id="fe592-177">Строка</span><span class="sxs-lookup"><span data-stu-id="fe592-177">String</span></span>|<span data-ttu-id="fe592-178">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="fe592-178">Identifier for item</span></span>|
|<span data-ttu-id="fe592-179">description</span><span class="sxs-lookup"><span data-stu-id="fe592-179">description</span></span>|<span data-ttu-id="fe592-180">Строка</span><span class="sxs-lookup"><span data-stu-id="fe592-180">String</span></span>|<span data-ttu-id="fe592-181">Описание элемента</span><span class="sxs-lookup"><span data-stu-id="fe592-181">Description of the item</span></span>|
|<span data-ttu-id="fe592-182">helpText</span><span class="sxs-lookup"><span data-stu-id="fe592-182">helpText</span></span>|<span data-ttu-id="fe592-183">Строка</span><span class="sxs-lookup"><span data-stu-id="fe592-183">String</span></span>|<span data-ttu-id="fe592-184">Справка текста элемента</span><span class="sxs-lookup"><span data-stu-id="fe592-184">Help text of the item</span></span>|
|<span data-ttu-id="fe592-185">name</span><span class="sxs-lookup"><span data-stu-id="fe592-185">name</span></span>|<span data-ttu-id="fe592-186">String</span><span class="sxs-lookup"><span data-stu-id="fe592-186">String</span></span>|<span data-ttu-id="fe592-187">Имя элемента</span><span class="sxs-lookup"><span data-stu-id="fe592-187">Name of the item</span></span>|
|<span data-ttu-id="fe592-188">displayName</span><span class="sxs-lookup"><span data-stu-id="fe592-188">displayName</span></span>|<span data-ttu-id="fe592-189">Строка</span><span class="sxs-lookup"><span data-stu-id="fe592-189">String</span></span>|<span data-ttu-id="fe592-190">Отображение имени элемента</span><span class="sxs-lookup"><span data-stu-id="fe592-190">Display name of the item</span></span>|
|<span data-ttu-id="fe592-191">version</span><span class="sxs-lookup"><span data-stu-id="fe592-191">version</span></span>|<span data-ttu-id="fe592-192">String</span><span class="sxs-lookup"><span data-stu-id="fe592-192">String</span></span>|<span data-ttu-id="fe592-193">Версия элемента</span><span class="sxs-lookup"><span data-stu-id="fe592-193">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="fe592-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe592-194">Response</span></span>
<span data-ttu-id="fe592-195">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fe592-195">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe592-196">Пример</span><span class="sxs-lookup"><span data-stu-id="fe592-196">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe592-197">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe592-197">Request</span></span>
<span data-ttu-id="fe592-198">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe592-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reusableSettings
Content-type: application/json
Content-length: 1258

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
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="fe592-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe592-199">Response</span></span>
<span data-ttu-id="fe592-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe592-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1307

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
```




