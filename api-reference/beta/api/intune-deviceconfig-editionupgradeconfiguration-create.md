---
title: Создание объекта editionUpgradeConfiguration
description: Создание объекта editionUpgradeConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0e35349ac9dd61675800a044754f2092cc767e1b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42753033"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="0f0be-103">Создание объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f0be-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="0f0be-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f0be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f0be-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f0be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f0be-106">Создание объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f0be-106">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f0be-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="0f0be-107">Prerequisites</span></span>
<span data-ttu-id="0f0be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f0be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f0be-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f0be-110">Permission type</span></span>|<span data-ttu-id="0f0be-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f0be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f0be-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f0be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f0be-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f0be-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f0be-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f0be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f0be-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f0be-115">Not supported.</span></span>|
|<span data-ttu-id="0f0be-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="0f0be-116">Application</span></span>|<span data-ttu-id="0f0be-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f0be-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f0be-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f0be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0f0be-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0f0be-119">Request headers</span></span>
|<span data-ttu-id="0f0be-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f0be-120">Header</span></span>|<span data-ttu-id="0f0be-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0f0be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f0be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f0be-122">Authorization</span></span>|<span data-ttu-id="0f0be-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f0be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f0be-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0f0be-124">Accept</span></span>|<span data-ttu-id="0f0be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f0be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f0be-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0f0be-126">Request body</span></span>
<span data-ttu-id="0f0be-127">В теле запроса добавьте представление объекта editionUpgradeConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f0be-127">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="0f0be-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0f0be-128">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="0f0be-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f0be-129">Property</span></span>|<span data-ttu-id="0f0be-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0f0be-130">Type</span></span>|<span data-ttu-id="0f0be-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0f0be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f0be-132">id</span><span class="sxs-lookup"><span data-stu-id="0f0be-132">id</span></span>|<span data-ttu-id="0f0be-133">Строка</span><span class="sxs-lookup"><span data-stu-id="0f0be-133">String</span></span>|<span data-ttu-id="0f0be-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0f0be-134">Key of the entity.</span></span> <span data-ttu-id="0f0be-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f0be-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f0be-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f0be-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0f0be-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f0be-137">DateTimeOffset</span></span>|<span data-ttu-id="0f0be-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0f0be-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0f0be-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f0be-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f0be-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f0be-140">roleScopeTagIds</span></span>|<span data-ttu-id="0f0be-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0f0be-141">String collection</span></span>|<span data-ttu-id="0f0be-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="0f0be-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0f0be-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f0be-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f0be-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="0f0be-144">supportsScopeTags</span></span>|<span data-ttu-id="0f0be-145">Логический</span><span class="sxs-lookup"><span data-stu-id="0f0be-145">Boolean</span></span>|<span data-ttu-id="0f0be-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="0f0be-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0f0be-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="0f0be-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0f0be-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="0f0be-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0f0be-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0f0be-149">This property is read-only.</span></span> <span data-ttu-id="0f0be-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f0be-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f0be-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0f0be-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0f0be-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0f0be-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0f0be-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0f0be-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0f0be-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f0be-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f0be-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0f0be-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0f0be-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0f0be-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0f0be-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0f0be-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0f0be-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f0be-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f0be-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0f0be-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0f0be-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="0f0be-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0f0be-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="0f0be-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0f0be-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f0be-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f0be-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f0be-163">createdDateTime</span></span>|<span data-ttu-id="0f0be-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f0be-164">DateTimeOffset</span></span>|<span data-ttu-id="0f0be-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0f0be-165">DateTime the object was created.</span></span> <span data-ttu-id="0f0be-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f0be-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f0be-167">description</span><span class="sxs-lookup"><span data-stu-id="0f0be-167">description</span></span>|<span data-ttu-id="0f0be-168">String</span><span class="sxs-lookup"><span data-stu-id="0f0be-168">String</span></span>|<span data-ttu-id="0f0be-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0f0be-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0f0be-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f0be-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f0be-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0f0be-171">displayName</span></span>|<span data-ttu-id="0f0be-172">Строка</span><span class="sxs-lookup"><span data-stu-id="0f0be-172">String</span></span>|<span data-ttu-id="0f0be-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0f0be-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0f0be-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0f0be-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f0be-175">version</span><span class="sxs-lookup"><span data-stu-id="0f0be-175">version</span></span>|<span data-ttu-id="0f0be-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0f0be-176">Int32</span></span>|<span data-ttu-id="0f0be-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0f0be-177">Version of the device configuration.</span></span> <span data-ttu-id="0f0be-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0f0be-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0f0be-179">licenseType</span><span class="sxs-lookup"><span data-stu-id="0f0be-179">licenseType</span></span>|[<span data-ttu-id="0f0be-180">едитионупграделиценсетипе</span><span class="sxs-lookup"><span data-stu-id="0f0be-180">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="0f0be-181">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="0f0be-181">Edition Upgrade License Type.</span></span> <span data-ttu-id="0f0be-182">Возможные значения: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="0f0be-182">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="0f0be-183">targetEdition</span><span class="sxs-lookup"><span data-stu-id="0f0be-183">targetEdition</span></span>|[<span data-ttu-id="0f0be-184">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="0f0be-184">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="0f0be-185">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="0f0be-185">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="0f0be-186">`windows10Enterprise`Возможные значения:, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN` `windows10MobileEnterprise` `windows10HolographicEnterprise` `windows10Professional` `notConfigured` `windows10Home` `windows10HomeChina` `windows10HomeN` `windows10HomeSingleLanguage` `windows10Mobile` `windows10IoTCore` `windows10IoTCoreCommercial`,,,,,,,,,,,,,,,,,,,,,,. `windows10ProfessionalN` `windows10ProfessionalEducation` `windows10ProfessionalEducationN` `windows10ProfessionalWorkstation` `windows10ProfessionalWorkstationN`</span><span class="sxs-lookup"><span data-stu-id="0f0be-186">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="0f0be-187">license</span><span class="sxs-lookup"><span data-stu-id="0f0be-187">license</span></span>|<span data-ttu-id="0f0be-188">String</span><span class="sxs-lookup"><span data-stu-id="0f0be-188">String</span></span>|<span data-ttu-id="0f0be-189">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="0f0be-189">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="0f0be-190">productKey</span><span class="sxs-lookup"><span data-stu-id="0f0be-190">productKey</span></span>|<span data-ttu-id="0f0be-191">String</span><span class="sxs-lookup"><span data-stu-id="0f0be-191">String</span></span>|<span data-ttu-id="0f0be-192">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="0f0be-192">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="0f0be-193">виндовссмоде</span><span class="sxs-lookup"><span data-stu-id="0f0be-193">windowsSMode</span></span>|[<span data-ttu-id="0f0be-194">виндовссмодеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0f0be-194">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="0f0be-195">Конфигурация режима S.</span><span class="sxs-lookup"><span data-stu-id="0f0be-195">S mode configuration.</span></span> <span data-ttu-id="0f0be-196">Возможные значения: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="0f0be-196">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="0f0be-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f0be-197">Response</span></span>
<span data-ttu-id="0f0be-198">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0f0be-198">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f0be-199">Пример</span><span class="sxs-lookup"><span data-stu-id="0f0be-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f0be-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f0be-200">Request</span></span>
<span data-ttu-id="0f0be-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f0be-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f0be-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f0be-202">Response</span></span>
<span data-ttu-id="0f0be-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f0be-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




