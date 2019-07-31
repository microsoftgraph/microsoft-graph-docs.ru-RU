---
title: Создание объекта editionUpgradeConfiguration
description: Создание объекта editionUpgradeConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7b7cbd0ff8af9ee9c26f2ef477d1836a93a4030d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35948854"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="9ff00-103">Создание объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="9ff00-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="9ff00-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ff00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ff00-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ff00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ff00-106">Создание объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff00-106">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ff00-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9ff00-107">Prerequisites</span></span>
<span data-ttu-id="9ff00-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ff00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ff00-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ff00-110">Permission type</span></span>|<span data-ttu-id="9ff00-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ff00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ff00-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ff00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ff00-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ff00-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ff00-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ff00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ff00-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ff00-115">Not supported.</span></span>|
|<span data-ttu-id="9ff00-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ff00-116">Application</span></span>|<span data-ttu-id="9ff00-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ff00-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ff00-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ff00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9ff00-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ff00-119">Request headers</span></span>
|<span data-ttu-id="9ff00-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ff00-120">Header</span></span>|<span data-ttu-id="9ff00-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9ff00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ff00-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ff00-122">Authorization</span></span>|<span data-ttu-id="9ff00-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ff00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ff00-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9ff00-124">Accept</span></span>|<span data-ttu-id="9ff00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ff00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ff00-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9ff00-126">Request body</span></span>
<span data-ttu-id="9ff00-127">В теле запроса добавьте представление объекта editionUpgradeConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ff00-127">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="9ff00-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9ff00-128">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="9ff00-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ff00-129">Property</span></span>|<span data-ttu-id="9ff00-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9ff00-130">Type</span></span>|<span data-ttu-id="9ff00-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9ff00-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ff00-132">id</span><span class="sxs-lookup"><span data-stu-id="9ff00-132">id</span></span>|<span data-ttu-id="9ff00-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9ff00-133">String</span></span>|<span data-ttu-id="9ff00-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9ff00-134">Key of the entity.</span></span> <span data-ttu-id="9ff00-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff00-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff00-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ff00-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9ff00-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ff00-137">DateTimeOffset</span></span>|<span data-ttu-id="9ff00-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9ff00-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9ff00-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff00-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff00-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ff00-140">roleScopeTagIds</span></span>|<span data-ttu-id="9ff00-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9ff00-141">String collection</span></span>|<span data-ttu-id="9ff00-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9ff00-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ff00-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff00-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff00-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="9ff00-144">supportsScopeTags</span></span>|<span data-ttu-id="9ff00-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ff00-145">Boolean</span></span>|<span data-ttu-id="9ff00-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9ff00-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9ff00-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="9ff00-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9ff00-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9ff00-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9ff00-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ff00-149">This property is read-only.</span></span> <span data-ttu-id="9ff00-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff00-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff00-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ff00-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9ff00-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9ff00-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9ff00-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9ff00-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9ff00-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff00-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff00-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ff00-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9ff00-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9ff00-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9ff00-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9ff00-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9ff00-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff00-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff00-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="9ff00-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9ff00-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="9ff00-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9ff00-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9ff00-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9ff00-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff00-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff00-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ff00-163">createdDateTime</span></span>|<span data-ttu-id="9ff00-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ff00-164">DateTimeOffset</span></span>|<span data-ttu-id="9ff00-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9ff00-165">DateTime the object was created.</span></span> <span data-ttu-id="9ff00-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff00-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff00-167">description</span><span class="sxs-lookup"><span data-stu-id="9ff00-167">description</span></span>|<span data-ttu-id="9ff00-168">String</span><span class="sxs-lookup"><span data-stu-id="9ff00-168">String</span></span>|<span data-ttu-id="9ff00-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9ff00-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ff00-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff00-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff00-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9ff00-171">displayName</span></span>|<span data-ttu-id="9ff00-172">Строка</span><span class="sxs-lookup"><span data-stu-id="9ff00-172">String</span></span>|<span data-ttu-id="9ff00-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9ff00-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ff00-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ff00-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff00-175">version</span><span class="sxs-lookup"><span data-stu-id="9ff00-175">version</span></span>|<span data-ttu-id="9ff00-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff00-176">Int32</span></span>|<span data-ttu-id="9ff00-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9ff00-177">Version of the device configuration.</span></span> <span data-ttu-id="9ff00-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ff00-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff00-179">licenseType</span><span class="sxs-lookup"><span data-stu-id="9ff00-179">licenseType</span></span>|[<span data-ttu-id="9ff00-180">Едитионупграделиценсетипе</span><span class="sxs-lookup"><span data-stu-id="9ff00-180">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="9ff00-181">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="9ff00-181">Edition Upgrade License Type.</span></span> <span data-ttu-id="9ff00-182">Возможные значения: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="9ff00-182">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="9ff00-183">targetEdition</span><span class="sxs-lookup"><span data-stu-id="9ff00-183">targetEdition</span></span>|[<span data-ttu-id="9ff00-184">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="9ff00-184">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="9ff00-185">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="9ff00-185">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="9ff00-186">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN` `windows10MobileEnterprise` `windows10HolographicEnterprise` `windows10Professional` `windows10Home` `windows10HomeChina` `windows10HomeN` `windows10HomeSingleLanguage` `windows10Mobile` `windows10IoTCore` `windows10ProfessionalWorkstationN` `notConfigured`,,,,,,,,,,,,,,,,,,,,, `windows10ProfessionalN` `windows10ProfessionalEducation` `windows10ProfessionalEducationN` `windows10ProfessionalWorkstation` , `windows10IoTCoreCommercial`.</span><span class="sxs-lookup"><span data-stu-id="9ff00-186">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="9ff00-187">license</span><span class="sxs-lookup"><span data-stu-id="9ff00-187">license</span></span>|<span data-ttu-id="9ff00-188">String</span><span class="sxs-lookup"><span data-stu-id="9ff00-188">String</span></span>|<span data-ttu-id="9ff00-189">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="9ff00-189">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="9ff00-190">productKey</span><span class="sxs-lookup"><span data-stu-id="9ff00-190">productKey</span></span>|<span data-ttu-id="9ff00-191">String</span><span class="sxs-lookup"><span data-stu-id="9ff00-191">String</span></span>|<span data-ttu-id="9ff00-192">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="9ff00-192">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="9ff00-193">Виндовссмоде</span><span class="sxs-lookup"><span data-stu-id="9ff00-193">windowsSMode</span></span>|[<span data-ttu-id="9ff00-194">Виндовссмодеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9ff00-194">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="9ff00-195">Конфигурация режима S.</span><span class="sxs-lookup"><span data-stu-id="9ff00-195">S mode configuration.</span></span> <span data-ttu-id="9ff00-196">Возможные значения: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="9ff00-196">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="9ff00-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ff00-197">Response</span></span>
<span data-ttu-id="9ff00-198">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9ff00-198">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ff00-199">Пример</span><span class="sxs-lookup"><span data-stu-id="9ff00-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ff00-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ff00-200">Request</span></span>
<span data-ttu-id="9ff00-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ff00-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ff00-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ff00-202">Response</span></span>
<span data-ttu-id="9ff00-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ff00-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





