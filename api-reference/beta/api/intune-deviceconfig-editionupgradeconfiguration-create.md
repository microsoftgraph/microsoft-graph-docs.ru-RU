---
title: Создание объекта editionUpgradeConfiguration
description: Создание объекта editionUpgradeConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ddfcffc24c8fc09230eb3d938ab7580d81a858aa
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736627"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="1572d-103">Создание объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="1572d-103">Create editionUpgradeConfiguration</span></span>

<span data-ttu-id="1572d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1572d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1572d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1572d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1572d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1572d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1572d-107">Создание объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1572d-107">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1572d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1572d-108">Prerequisites</span></span>
<span data-ttu-id="1572d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1572d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1572d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1572d-111">Permission type</span></span>|<span data-ttu-id="1572d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1572d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1572d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1572d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1572d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1572d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1572d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1572d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1572d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1572d-116">Not supported.</span></span>|
|<span data-ttu-id="1572d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1572d-117">Application</span></span>|<span data-ttu-id="1572d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1572d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1572d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1572d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1572d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1572d-120">Request headers</span></span>
|<span data-ttu-id="1572d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1572d-121">Header</span></span>|<span data-ttu-id="1572d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1572d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1572d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1572d-123">Authorization</span></span>|<span data-ttu-id="1572d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1572d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1572d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1572d-125">Accept</span></span>|<span data-ttu-id="1572d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1572d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1572d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1572d-127">Request body</span></span>
<span data-ttu-id="1572d-128">В теле запроса добавьте представление объекта editionUpgradeConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1572d-128">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="1572d-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1572d-129">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="1572d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1572d-130">Property</span></span>|<span data-ttu-id="1572d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1572d-131">Type</span></span>|<span data-ttu-id="1572d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1572d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1572d-133">id</span><span class="sxs-lookup"><span data-stu-id="1572d-133">id</span></span>|<span data-ttu-id="1572d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1572d-134">String</span></span>|<span data-ttu-id="1572d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1572d-135">Key of the entity.</span></span> <span data-ttu-id="1572d-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1572d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1572d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1572d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1572d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1572d-138">DateTimeOffset</span></span>|<span data-ttu-id="1572d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1572d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1572d-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1572d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1572d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1572d-141">roleScopeTagIds</span></span>|<span data-ttu-id="1572d-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1572d-142">String collection</span></span>|<span data-ttu-id="1572d-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1572d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1572d-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1572d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1572d-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1572d-145">supportsScopeTags</span></span>|<span data-ttu-id="1572d-146">Логический</span><span class="sxs-lookup"><span data-stu-id="1572d-146">Boolean</span></span>|<span data-ttu-id="1572d-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1572d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1572d-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1572d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1572d-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1572d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1572d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1572d-150">This property is read-only.</span></span> <span data-ttu-id="1572d-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1572d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1572d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1572d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1572d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1572d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1572d-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1572d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1572d-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1572d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1572d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1572d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1572d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1572d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1572d-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1572d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1572d-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1572d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1572d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1572d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1572d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1572d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1572d-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="1572d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1572d-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1572d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1572d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1572d-164">createdDateTime</span></span>|<span data-ttu-id="1572d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1572d-165">DateTimeOffset</span></span>|<span data-ttu-id="1572d-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1572d-166">DateTime the object was created.</span></span> <span data-ttu-id="1572d-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1572d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1572d-168">description</span><span class="sxs-lookup"><span data-stu-id="1572d-168">description</span></span>|<span data-ttu-id="1572d-169">Строка</span><span class="sxs-lookup"><span data-stu-id="1572d-169">String</span></span>|<span data-ttu-id="1572d-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1572d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1572d-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1572d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1572d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1572d-172">displayName</span></span>|<span data-ttu-id="1572d-173">Строка</span><span class="sxs-lookup"><span data-stu-id="1572d-173">String</span></span>|<span data-ttu-id="1572d-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1572d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1572d-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1572d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1572d-176">version</span><span class="sxs-lookup"><span data-stu-id="1572d-176">version</span></span>|<span data-ttu-id="1572d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1572d-177">Int32</span></span>|<span data-ttu-id="1572d-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1572d-178">Version of the device configuration.</span></span> <span data-ttu-id="1572d-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1572d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1572d-180">licenseType</span><span class="sxs-lookup"><span data-stu-id="1572d-180">licenseType</span></span>|[<span data-ttu-id="1572d-181">едитионупграделиценсетипе</span><span class="sxs-lookup"><span data-stu-id="1572d-181">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="1572d-182">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="1572d-182">Edition Upgrade License Type.</span></span> <span data-ttu-id="1572d-183">Возможные значения: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="1572d-183">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="1572d-184">targetEdition</span><span class="sxs-lookup"><span data-stu-id="1572d-184">targetEdition</span></span>|[<span data-ttu-id="1572d-185">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="1572d-185">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="1572d-186">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="1572d-186">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="1572d-187">Возможные значения:,,,,,,,,,,,,,,,,,,, `windows10Enterprise` `windows10EnterpriseN` `windows10Education` `windows10EducationN` `windows10MobileEnterprise` `windows10HolographicEnterprise` `windows10Professional` `windows10ProfessionalN` `windows10ProfessionalEducation` `windows10ProfessionalEducationN` `windows10ProfessionalWorkstation` `windows10ProfessionalWorkstationN` `notConfigured` , `windows10Home` , `windows10HomeChina` , `windows10HomeN` `windows10HomeSingleLanguage` `windows10Mobile` `windows10IoTCore` `windows10IoTCoreCommercial` ,,,.</span><span class="sxs-lookup"><span data-stu-id="1572d-187">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="1572d-188">license</span><span class="sxs-lookup"><span data-stu-id="1572d-188">license</span></span>|<span data-ttu-id="1572d-189">String</span><span class="sxs-lookup"><span data-stu-id="1572d-189">String</span></span>|<span data-ttu-id="1572d-190">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="1572d-190">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="1572d-191">productKey</span><span class="sxs-lookup"><span data-stu-id="1572d-191">productKey</span></span>|<span data-ttu-id="1572d-192">String</span><span class="sxs-lookup"><span data-stu-id="1572d-192">String</span></span>|<span data-ttu-id="1572d-193">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="1572d-193">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="1572d-194">виндовссмоде</span><span class="sxs-lookup"><span data-stu-id="1572d-194">windowsSMode</span></span>|[<span data-ttu-id="1572d-195">виндовссмодеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1572d-195">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="1572d-196">Конфигурация режима S.</span><span class="sxs-lookup"><span data-stu-id="1572d-196">S mode configuration.</span></span> <span data-ttu-id="1572d-197">Возможные значения: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="1572d-197">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="1572d-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="1572d-198">Response</span></span>
<span data-ttu-id="1572d-199">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1572d-199">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1572d-200">Пример</span><span class="sxs-lookup"><span data-stu-id="1572d-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="1572d-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="1572d-201">Request</span></span>
<span data-ttu-id="1572d-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1572d-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1204

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```

### <a name="response"></a><span data-ttu-id="1572d-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="1572d-203">Response</span></span>
<span data-ttu-id="1572d-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1572d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1376

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value",
  "windowsSMode": "block"
}
```





