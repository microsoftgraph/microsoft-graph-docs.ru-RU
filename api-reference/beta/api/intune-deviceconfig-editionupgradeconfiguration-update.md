---
title: Обновление объекта editionUpgradeConfiguration
description: Обновление свойств объекта editionUpgradeConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a4243a6e026eca2cb6edb6d4a471b02309677c9d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49206429"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="20ba1-103">Обновление объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="20ba1-103">Update editionUpgradeConfiguration</span></span>

<span data-ttu-id="20ba1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20ba1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20ba1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20ba1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20ba1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20ba1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20ba1-107">Обновление свойств объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-107">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20ba1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="20ba1-108">Prerequisites</span></span>
<span data-ttu-id="20ba1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20ba1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20ba1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20ba1-111">Permission type</span></span>|<span data-ttu-id="20ba1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20ba1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20ba1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20ba1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20ba1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20ba1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="20ba1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20ba1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20ba1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20ba1-116">Not supported.</span></span>|
|<span data-ttu-id="20ba1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="20ba1-117">Application</span></span>|<span data-ttu-id="20ba1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20ba1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20ba1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20ba1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="20ba1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="20ba1-120">Request headers</span></span>
|<span data-ttu-id="20ba1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20ba1-121">Header</span></span>|<span data-ttu-id="20ba1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="20ba1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20ba1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20ba1-123">Authorization</span></span>|<span data-ttu-id="20ba1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20ba1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20ba1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20ba1-125">Accept</span></span>|<span data-ttu-id="20ba1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20ba1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20ba1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20ba1-127">Request body</span></span>
<span data-ttu-id="20ba1-128">В теле запроса добавьте представление объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20ba1-128">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="20ba1-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-129">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="20ba1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="20ba1-130">Property</span></span>|<span data-ttu-id="20ba1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="20ba1-131">Type</span></span>|<span data-ttu-id="20ba1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="20ba1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20ba1-133">id</span><span class="sxs-lookup"><span data-stu-id="20ba1-133">id</span></span>|<span data-ttu-id="20ba1-134">String</span><span class="sxs-lookup"><span data-stu-id="20ba1-134">String</span></span>|<span data-ttu-id="20ba1-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="20ba1-135">Key of the entity.</span></span> <span data-ttu-id="20ba1-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20ba1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20ba1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="20ba1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20ba1-138">DateTimeOffset</span></span>|<span data-ttu-id="20ba1-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="20ba1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="20ba1-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20ba1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20ba1-141">roleScopeTagIds</span></span>|<span data-ttu-id="20ba1-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="20ba1-142">String collection</span></span>|<span data-ttu-id="20ba1-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="20ba1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="20ba1-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20ba1-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="20ba1-145">supportsScopeTags</span></span>|<span data-ttu-id="20ba1-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="20ba1-146">Boolean</span></span>|<span data-ttu-id="20ba1-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="20ba1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="20ba1-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="20ba1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="20ba1-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="20ba1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="20ba1-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20ba1-150">This property is read-only.</span></span> <span data-ttu-id="20ba1-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20ba1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="20ba1-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="20ba1-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="20ba1-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="20ba1-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="20ba1-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="20ba1-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20ba1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="20ba1-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="20ba1-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="20ba1-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="20ba1-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="20ba1-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="20ba1-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20ba1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="20ba1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="20ba1-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="20ba1-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="20ba1-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="20ba1-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="20ba1-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20ba1-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20ba1-164">createdDateTime</span></span>|<span data-ttu-id="20ba1-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20ba1-165">DateTimeOffset</span></span>|<span data-ttu-id="20ba1-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="20ba1-166">DateTime the object was created.</span></span> <span data-ttu-id="20ba1-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20ba1-168">description</span><span class="sxs-lookup"><span data-stu-id="20ba1-168">description</span></span>|<span data-ttu-id="20ba1-169">String</span><span class="sxs-lookup"><span data-stu-id="20ba1-169">String</span></span>|<span data-ttu-id="20ba1-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="20ba1-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="20ba1-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20ba1-172">displayName</span><span class="sxs-lookup"><span data-stu-id="20ba1-172">displayName</span></span>|<span data-ttu-id="20ba1-173">String</span><span class="sxs-lookup"><span data-stu-id="20ba1-173">String</span></span>|<span data-ttu-id="20ba1-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="20ba1-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="20ba1-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20ba1-176">version</span><span class="sxs-lookup"><span data-stu-id="20ba1-176">version</span></span>|<span data-ttu-id="20ba1-177">Int32</span><span class="sxs-lookup"><span data-stu-id="20ba1-177">Int32</span></span>|<span data-ttu-id="20ba1-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="20ba1-178">Version of the device configuration.</span></span> <span data-ttu-id="20ba1-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="20ba1-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="20ba1-180">licenseType</span><span class="sxs-lookup"><span data-stu-id="20ba1-180">licenseType</span></span>|[<span data-ttu-id="20ba1-181">едитионупграделиценсетипе</span><span class="sxs-lookup"><span data-stu-id="20ba1-181">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="20ba1-182">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="20ba1-182">Edition Upgrade License Type.</span></span> <span data-ttu-id="20ba1-183">Возможные значения: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="20ba1-183">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="20ba1-184">targetEdition</span><span class="sxs-lookup"><span data-stu-id="20ba1-184">targetEdition</span></span>|[<span data-ttu-id="20ba1-185">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="20ba1-185">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="20ba1-186">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="20ba1-186">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="20ba1-187">Возможные значения:,,,,,,,,,,,,,,,,,,, `windows10Enterprise` `windows10EnterpriseN` `windows10Education` `windows10EducationN` `windows10MobileEnterprise` `windows10HolographicEnterprise` `windows10Professional` `windows10ProfessionalN` `windows10ProfessionalEducation` `windows10ProfessionalEducationN` `windows10ProfessionalWorkstation` `windows10ProfessionalWorkstationN` `notConfigured` , `windows10Home` , `windows10HomeChina` , `windows10HomeN` `windows10HomeSingleLanguage` `windows10Mobile` `windows10IoTCore` `windows10IoTCoreCommercial` ,,,.</span><span class="sxs-lookup"><span data-stu-id="20ba1-187">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="20ba1-188">license</span><span class="sxs-lookup"><span data-stu-id="20ba1-188">license</span></span>|<span data-ttu-id="20ba1-189">String</span><span class="sxs-lookup"><span data-stu-id="20ba1-189">String</span></span>|<span data-ttu-id="20ba1-190">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="20ba1-190">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="20ba1-191">productKey</span><span class="sxs-lookup"><span data-stu-id="20ba1-191">productKey</span></span>|<span data-ttu-id="20ba1-192">String</span><span class="sxs-lookup"><span data-stu-id="20ba1-192">String</span></span>|<span data-ttu-id="20ba1-193">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="20ba1-193">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="20ba1-194">виндовссмоде</span><span class="sxs-lookup"><span data-stu-id="20ba1-194">windowsSMode</span></span>|[<span data-ttu-id="20ba1-195">виндовссмодеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="20ba1-195">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="20ba1-196">Конфигурация режима S.</span><span class="sxs-lookup"><span data-stu-id="20ba1-196">S mode configuration.</span></span> <span data-ttu-id="20ba1-197">Возможные значения: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="20ba1-197">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="20ba1-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="20ba1-198">Response</span></span>
<span data-ttu-id="20ba1-199">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="20ba1-199">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20ba1-200">Пример</span><span class="sxs-lookup"><span data-stu-id="20ba1-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="20ba1-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="20ba1-201">Request</span></span>
<span data-ttu-id="20ba1-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20ba1-202">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="20ba1-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="20ba1-203">Response</span></span>
<span data-ttu-id="20ba1-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20ba1-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




