---
title: Обновление объекта editionUpgradeConfiguration
description: Обновление свойств объекта editionUpgradeConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21b74c743fc4be19e08fa5fa6b54fb5c8e9c55ef
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37168070"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="8580c-103">Обновление объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="8580c-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="8580c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8580c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8580c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8580c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8580c-106">Обновление свойств объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8580c-106">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8580c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8580c-107">Prerequisites</span></span>
<span data-ttu-id="8580c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8580c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8580c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8580c-110">Permission type</span></span>|<span data-ttu-id="8580c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8580c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8580c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8580c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8580c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8580c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8580c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8580c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8580c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8580c-115">Not supported.</span></span>|
|<span data-ttu-id="8580c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8580c-116">Application</span></span>|<span data-ttu-id="8580c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8580c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8580c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8580c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8580c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8580c-119">Request headers</span></span>
|<span data-ttu-id="8580c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8580c-120">Header</span></span>|<span data-ttu-id="8580c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8580c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8580c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8580c-122">Authorization</span></span>|<span data-ttu-id="8580c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8580c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8580c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8580c-124">Accept</span></span>|<span data-ttu-id="8580c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8580c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8580c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8580c-126">Request body</span></span>
<span data-ttu-id="8580c-127">В теле запроса добавьте представление объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8580c-127">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="8580c-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8580c-128">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="8580c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8580c-129">Property</span></span>|<span data-ttu-id="8580c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8580c-130">Type</span></span>|<span data-ttu-id="8580c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8580c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8580c-132">id</span><span class="sxs-lookup"><span data-stu-id="8580c-132">id</span></span>|<span data-ttu-id="8580c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8580c-133">String</span></span>|<span data-ttu-id="8580c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8580c-134">Key of the entity.</span></span> <span data-ttu-id="8580c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8580c-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8580c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8580c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8580c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8580c-137">DateTimeOffset</span></span>|<span data-ttu-id="8580c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8580c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8580c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8580c-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8580c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8580c-140">roleScopeTagIds</span></span>|<span data-ttu-id="8580c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8580c-141">String collection</span></span>|<span data-ttu-id="8580c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8580c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8580c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8580c-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8580c-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8580c-144">supportsScopeTags</span></span>|<span data-ttu-id="8580c-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="8580c-145">Boolean</span></span>|<span data-ttu-id="8580c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8580c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8580c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8580c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8580c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8580c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8580c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8580c-149">This property is read-only.</span></span> <span data-ttu-id="8580c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8580c-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8580c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8580c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8580c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8580c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8580c-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8580c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8580c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8580c-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8580c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8580c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8580c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8580c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8580c-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8580c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8580c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8580c-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8580c-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="8580c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8580c-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="8580c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8580c-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8580c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8580c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8580c-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8580c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8580c-163">createdDateTime</span></span>|<span data-ttu-id="8580c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8580c-164">DateTimeOffset</span></span>|<span data-ttu-id="8580c-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8580c-165">DateTime the object was created.</span></span> <span data-ttu-id="8580c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8580c-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8580c-167">description</span><span class="sxs-lookup"><span data-stu-id="8580c-167">description</span></span>|<span data-ttu-id="8580c-168">String</span><span class="sxs-lookup"><span data-stu-id="8580c-168">String</span></span>|<span data-ttu-id="8580c-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8580c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8580c-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8580c-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8580c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8580c-171">displayName</span></span>|<span data-ttu-id="8580c-172">Строка</span><span class="sxs-lookup"><span data-stu-id="8580c-172">String</span></span>|<span data-ttu-id="8580c-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8580c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8580c-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8580c-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8580c-175">version</span><span class="sxs-lookup"><span data-stu-id="8580c-175">version</span></span>|<span data-ttu-id="8580c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8580c-176">Int32</span></span>|<span data-ttu-id="8580c-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8580c-177">Version of the device configuration.</span></span> <span data-ttu-id="8580c-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8580c-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8580c-179">licenseType</span><span class="sxs-lookup"><span data-stu-id="8580c-179">licenseType</span></span>|[<span data-ttu-id="8580c-180">едитионупграделиценсетипе</span><span class="sxs-lookup"><span data-stu-id="8580c-180">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="8580c-181">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="8580c-181">Edition Upgrade License Type.</span></span> <span data-ttu-id="8580c-182">Возможные значения: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="8580c-182">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="8580c-183">targetEdition</span><span class="sxs-lookup"><span data-stu-id="8580c-183">targetEdition</span></span>|[<span data-ttu-id="8580c-184">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="8580c-184">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="8580c-185">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="8580c-185">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="8580c-186">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN` `windows10MobileEnterprise` `windows10HolographicEnterprise` `windows10Professional` `windows10Home` `windows10HomeChina` `windows10HomeN` `windows10HomeSingleLanguage` `windows10Mobile` `windows10IoTCore` `windows10ProfessionalWorkstationN` `notConfigured`,,,,,,,,,,,,,,,,,,,,, `windows10ProfessionalN` `windows10ProfessionalEducation` `windows10ProfessionalEducationN` `windows10ProfessionalWorkstation` , `windows10IoTCoreCommercial`.</span><span class="sxs-lookup"><span data-stu-id="8580c-186">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="8580c-187">license</span><span class="sxs-lookup"><span data-stu-id="8580c-187">license</span></span>|<span data-ttu-id="8580c-188">String</span><span class="sxs-lookup"><span data-stu-id="8580c-188">String</span></span>|<span data-ttu-id="8580c-189">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="8580c-189">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="8580c-190">productKey</span><span class="sxs-lookup"><span data-stu-id="8580c-190">productKey</span></span>|<span data-ttu-id="8580c-191">String</span><span class="sxs-lookup"><span data-stu-id="8580c-191">String</span></span>|<span data-ttu-id="8580c-192">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="8580c-192">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="8580c-193">виндовссмоде</span><span class="sxs-lookup"><span data-stu-id="8580c-193">windowsSMode</span></span>|[<span data-ttu-id="8580c-194">виндовссмодеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8580c-194">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="8580c-195">Конфигурация режима S.</span><span class="sxs-lookup"><span data-stu-id="8580c-195">S mode configuration.</span></span> <span data-ttu-id="8580c-196">Возможные значения: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="8580c-196">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="8580c-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="8580c-197">Response</span></span>
<span data-ttu-id="8580c-198">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8580c-198">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8580c-199">Пример</span><span class="sxs-lookup"><span data-stu-id="8580c-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="8580c-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="8580c-200">Request</span></span>
<span data-ttu-id="8580c-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8580c-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="8580c-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="8580c-202">Response</span></span>
<span data-ttu-id="8580c-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8580c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




