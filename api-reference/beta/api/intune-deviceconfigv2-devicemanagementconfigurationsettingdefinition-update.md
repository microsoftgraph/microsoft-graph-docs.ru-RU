---
title: Обновление deviceManagementConfigurationSettingDefinition
description: Обновление свойств объекта deviceManagementConfigurationSettingDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 99a65dd140e8128e5459517e19c510c2a8114500
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146911"
---
# <a name="update-devicemanagementconfigurationsettingdefinition"></a><span data-ttu-id="f620d-103">Обновление deviceManagementConfigurationSettingDefinition</span><span class="sxs-lookup"><span data-stu-id="f620d-103">Update deviceManagementConfigurationSettingDefinition</span></span>

<span data-ttu-id="f620d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f620d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f620d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f620d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f620d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f620d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f620d-107">Обновление свойств объекта [deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f620d-107">Update the properties of a [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f620d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f620d-108">Prerequisites</span></span>
<span data-ttu-id="f620d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f620d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f620d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f620d-111">Permission type</span></span>|<span data-ttu-id="f620d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f620d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f620d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f620d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f620d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f620d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f620d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f620d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f620d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f620d-116">Not supported.</span></span>|
|<span data-ttu-id="f620d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f620d-117">Application</span></span>|<span data-ttu-id="f620d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f620d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f620d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f620d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}/settings/{deviceManagementConfigurationSettingId}/settingDefinitions/{deviceManagementConfigurationSettingDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="f620d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f620d-120">Request headers</span></span>
|<span data-ttu-id="f620d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f620d-121">Header</span></span>|<span data-ttu-id="f620d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f620d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f620d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f620d-123">Authorization</span></span>|<span data-ttu-id="f620d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f620d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f620d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f620d-125">Accept</span></span>|<span data-ttu-id="f620d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f620d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f620d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f620d-127">Request body</span></span>
<span data-ttu-id="f620d-128">В теле запроса поставляем представление JSON для [объекта deviceManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f620d-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object.</span></span>

<span data-ttu-id="f620d-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementConfigurationSettingDefinition.](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="f620d-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md).</span></span>

|<span data-ttu-id="f620d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f620d-130">Property</span></span>|<span data-ttu-id="f620d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f620d-131">Type</span></span>|<span data-ttu-id="f620d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f620d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f620d-133">применимость</span><span class="sxs-lookup"><span data-stu-id="f620d-133">applicability</span></span>|[<span data-ttu-id="f620d-134">deviceManagementConfigurationSettingApplicability</span><span class="sxs-lookup"><span data-stu-id="f620d-134">deviceManagementConfigurationSettingApplicability</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingapplicability.md)|<span data-ttu-id="f620d-135">Сведения о том, какие параметры устройства применимы к</span><span class="sxs-lookup"><span data-stu-id="f620d-135">Details which device setting is applicable on</span></span>|
|<span data-ttu-id="f620d-136">accessTypes</span><span class="sxs-lookup"><span data-stu-id="f620d-136">accessTypes</span></span>|[<span data-ttu-id="f620d-137">deviceManagementConfigurationSettingAccessTypes</span><span class="sxs-lookup"><span data-stu-id="f620d-137">deviceManagementConfigurationSettingAccessTypes</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingaccesstypes.md)|<span data-ttu-id="f620d-138">Режим доступа к режиму чтения и записи параметра.</span><span class="sxs-lookup"><span data-stu-id="f620d-138">Read/write access mode of the setting.</span></span> <span data-ttu-id="f620d-139">Возможные значения: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span><span class="sxs-lookup"><span data-stu-id="f620d-139">Possible values are: `none`, `add`, `copy`, `delete`, `get`, `replace`, `execute`.</span></span>|
|<span data-ttu-id="f620d-140">keywords</span><span class="sxs-lookup"><span data-stu-id="f620d-140">keywords</span></span>|<span data-ttu-id="f620d-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f620d-141">String collection</span></span>|<span data-ttu-id="f620d-142">Маркеры для поиска параметров на</span><span class="sxs-lookup"><span data-stu-id="f620d-142">Tokens which to search settings on</span></span>|
|<span data-ttu-id="f620d-143">infoUrls</span><span class="sxs-lookup"><span data-stu-id="f620d-143">infoUrls</span></span>|<span data-ttu-id="f620d-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f620d-144">String collection</span></span>|<span data-ttu-id="f620d-145">Список ссылок, дополнительные сведения о параметре можно найти по адресу</span><span class="sxs-lookup"><span data-stu-id="f620d-145">List of links more info for the setting can be found at</span></span>|
|<span data-ttu-id="f620d-146">возникновение</span><span class="sxs-lookup"><span data-stu-id="f620d-146">occurrence</span></span>|[<span data-ttu-id="f620d-147">deviceManagementConfigurationSettingOccurrence</span><span class="sxs-lookup"><span data-stu-id="f620d-147">deviceManagementConfigurationSettingOccurrence</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingoccurrence.md)|<span data-ttu-id="f620d-148">Указывает, требуется ли параметр или нет.</span><span class="sxs-lookup"><span data-stu-id="f620d-148">Indicates whether the setting is required or not</span></span>|
|<span data-ttu-id="f620d-149">baseUri</span><span class="sxs-lookup"><span data-stu-id="f620d-149">baseUri</span></span>|<span data-ttu-id="f620d-150">Строка</span><span class="sxs-lookup"><span data-stu-id="f620d-150">String</span></span>|<span data-ttu-id="f620d-151">Базовый путь CSP</span><span class="sxs-lookup"><span data-stu-id="f620d-151">Base CSP Path</span></span>|
|<span data-ttu-id="f620d-152">offsetUri</span><span class="sxs-lookup"><span data-stu-id="f620d-152">offsetUri</span></span>|<span data-ttu-id="f620d-153">Строка</span><span class="sxs-lookup"><span data-stu-id="f620d-153">String</span></span>|<span data-ttu-id="f620d-154">Смещение пути CSP из базы</span><span class="sxs-lookup"><span data-stu-id="f620d-154">Offset CSP Path from Base</span></span>|
|<span data-ttu-id="f620d-155">rootDefinitionId</span><span class="sxs-lookup"><span data-stu-id="f620d-155">rootDefinitionId</span></span>|<span data-ttu-id="f620d-156">Строка</span><span class="sxs-lookup"><span data-stu-id="f620d-156">String</span></span>|<span data-ttu-id="f620d-157">Определение корневого параметра, если это параметр ребенка.</span><span class="sxs-lookup"><span data-stu-id="f620d-157">Root setting definition if the setting is a child setting.</span></span>|
|<span data-ttu-id="f620d-158">categoryId</span><span class="sxs-lookup"><span data-stu-id="f620d-158">categoryId</span></span>|<span data-ttu-id="f620d-159">Строка</span><span class="sxs-lookup"><span data-stu-id="f620d-159">String</span></span>|<span data-ttu-id="f620d-160">Указывает группу области, в которой параметр настроен в указанном поставщике служб конфигурации (CSP)</span><span class="sxs-lookup"><span data-stu-id="f620d-160">Specifies the area group under which the setting is configured in a specified configuration service provider (CSP)</span></span>|
|<span data-ttu-id="f620d-161">settingUsage</span><span class="sxs-lookup"><span data-stu-id="f620d-161">settingUsage</span></span>|[<span data-ttu-id="f620d-162">deviceManagementConfigurationSettingUsage</span><span class="sxs-lookup"><span data-stu-id="f620d-162">deviceManagementConfigurationSettingUsage</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingusage.md)|<span data-ttu-id="f620d-163">Параметр типа, например конфигурации и соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="f620d-163">Setting type, for example, configuration and compliance.</span></span> <span data-ttu-id="f620d-164">Возможные значения: `none`, `configuration`.</span><span class="sxs-lookup"><span data-stu-id="f620d-164">Possible values are: `none`, `configuration`.</span></span>|
|<span data-ttu-id="f620d-165">uxBehavior</span><span class="sxs-lookup"><span data-stu-id="f620d-165">uxBehavior</span></span>|[<span data-ttu-id="f620d-166">deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="f620d-166">deviceManagementConfigurationControlType</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationcontroltype.md)|<span data-ttu-id="f620d-167">Настройка представления типа управления в UX.</span><span class="sxs-lookup"><span data-stu-id="f620d-167">Setting control type representation in the UX.</span></span> <span data-ttu-id="f620d-168">Возможные значения: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span><span class="sxs-lookup"><span data-stu-id="f620d-168">Possible values are: `default`, `dropdown`, `smallTextBox`, `largeTextBox`, `toggle`, `multiheaderGrid`, `contextPane`.</span></span>|
|<span data-ttu-id="f620d-169">visibility</span><span class="sxs-lookup"><span data-stu-id="f620d-169">visibility</span></span>|[<span data-ttu-id="f620d-170">deviceManagementConfigurationSettingVisibility</span><span class="sxs-lookup"><span data-stu-id="f620d-170">deviceManagementConfigurationSettingVisibility</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvisibility.md)|<span data-ttu-id="f620d-171">Настройка области видимости для UX.</span><span class="sxs-lookup"><span data-stu-id="f620d-171">Setting visibility scope to UX.</span></span> <span data-ttu-id="f620d-172">Возможные значения: `none`, `settingsCatalog`, `template`.</span><span class="sxs-lookup"><span data-stu-id="f620d-172">Possible values are: `none`, `settingsCatalog`, `template`.</span></span>|
|<span data-ttu-id="f620d-173">id</span><span class="sxs-lookup"><span data-stu-id="f620d-173">id</span></span>|<span data-ttu-id="f620d-174">Строка</span><span class="sxs-lookup"><span data-stu-id="f620d-174">String</span></span>|<span data-ttu-id="f620d-175">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="f620d-175">Identifier for item</span></span>|
|<span data-ttu-id="f620d-176">description</span><span class="sxs-lookup"><span data-stu-id="f620d-176">description</span></span>|<span data-ttu-id="f620d-177">Строка</span><span class="sxs-lookup"><span data-stu-id="f620d-177">String</span></span>|<span data-ttu-id="f620d-178">Описание элемента</span><span class="sxs-lookup"><span data-stu-id="f620d-178">Description of the item</span></span>|
|<span data-ttu-id="f620d-179">helpText</span><span class="sxs-lookup"><span data-stu-id="f620d-179">helpText</span></span>|<span data-ttu-id="f620d-180">Строка</span><span class="sxs-lookup"><span data-stu-id="f620d-180">String</span></span>|<span data-ttu-id="f620d-181">Справка текста элемента</span><span class="sxs-lookup"><span data-stu-id="f620d-181">Help text of the item</span></span>|
|<span data-ttu-id="f620d-182">name</span><span class="sxs-lookup"><span data-stu-id="f620d-182">name</span></span>|<span data-ttu-id="f620d-183">String</span><span class="sxs-lookup"><span data-stu-id="f620d-183">String</span></span>|<span data-ttu-id="f620d-184">Имя элемента</span><span class="sxs-lookup"><span data-stu-id="f620d-184">Name of the item</span></span>|
|<span data-ttu-id="f620d-185">displayName</span><span class="sxs-lookup"><span data-stu-id="f620d-185">displayName</span></span>|<span data-ttu-id="f620d-186">Строка</span><span class="sxs-lookup"><span data-stu-id="f620d-186">String</span></span>|<span data-ttu-id="f620d-187">Отображение имени элемента</span><span class="sxs-lookup"><span data-stu-id="f620d-187">Display name of the item</span></span>|
|<span data-ttu-id="f620d-188">version</span><span class="sxs-lookup"><span data-stu-id="f620d-188">version</span></span>|<span data-ttu-id="f620d-189">String</span><span class="sxs-lookup"><span data-stu-id="f620d-189">String</span></span>|<span data-ttu-id="f620d-190">Версия элемента</span><span class="sxs-lookup"><span data-stu-id="f620d-190">Item Version</span></span>|



## <a name="response"></a><span data-ttu-id="f620d-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="f620d-191">Response</span></span>
<span data-ttu-id="f620d-192">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f620d-192">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationSettingDefinition](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingdefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f620d-193">Пример</span><span class="sxs-lookup"><span data-stu-id="f620d-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="f620d-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="f620d-194">Request</span></span>
<span data-ttu-id="f620d-195">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f620d-195">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationSettings/{deviceManagementConfigurationSettingDefinitionId}
Content-type: application/json
Content-length: 1042

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
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="f620d-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="f620d-196">Response</span></span>
<span data-ttu-id="f620d-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f620d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1091

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
  "id": "7af649e5-49e5-7af6-e549-f67ae549f67a",
  "description": "Description value",
  "helpText": "Help Text value",
  "name": "Name value",
  "displayName": "Display Name value",
  "version": "Version value"
}
```




