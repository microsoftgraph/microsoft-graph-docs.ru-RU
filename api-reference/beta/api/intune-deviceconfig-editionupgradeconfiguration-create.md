---
title: Создание объекта editionUpgradeConfiguration
description: Создание объекта editionUpgradeConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a45feaefd9a8540f8ed29b280d7ce234f9ccf0b0
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37168063"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="d0c68-103">Создание объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0c68-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="d0c68-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0c68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0c68-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0c68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0c68-106">Создание объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c68-106">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0c68-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d0c68-107">Prerequisites</span></span>
<span data-ttu-id="d0c68-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0c68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0c68-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0c68-110">Permission type</span></span>|<span data-ttu-id="d0c68-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0c68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0c68-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0c68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0c68-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0c68-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0c68-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0c68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0c68-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0c68-115">Not supported.</span></span>|
|<span data-ttu-id="d0c68-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0c68-116">Application</span></span>|<span data-ttu-id="d0c68-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0c68-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0c68-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0c68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d0c68-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0c68-119">Request headers</span></span>
|<span data-ttu-id="d0c68-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0c68-120">Header</span></span>|<span data-ttu-id="d0c68-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d0c68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0c68-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0c68-122">Authorization</span></span>|<span data-ttu-id="d0c68-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0c68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0c68-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d0c68-124">Accept</span></span>|<span data-ttu-id="d0c68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0c68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0c68-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d0c68-126">Request body</span></span>
<span data-ttu-id="d0c68-127">В теле запроса добавьте представление объекта editionUpgradeConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0c68-127">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="d0c68-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d0c68-128">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="d0c68-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0c68-129">Property</span></span>|<span data-ttu-id="d0c68-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d0c68-130">Type</span></span>|<span data-ttu-id="d0c68-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d0c68-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0c68-132">id</span><span class="sxs-lookup"><span data-stu-id="d0c68-132">id</span></span>|<span data-ttu-id="d0c68-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d0c68-133">String</span></span>|<span data-ttu-id="d0c68-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d0c68-134">Key of the entity.</span></span> <span data-ttu-id="d0c68-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c68-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c68-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0c68-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d0c68-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0c68-137">DateTimeOffset</span></span>|<span data-ttu-id="d0c68-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d0c68-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d0c68-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c68-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c68-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d0c68-140">roleScopeTagIds</span></span>|<span data-ttu-id="d0c68-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d0c68-141">String collection</span></span>|<span data-ttu-id="d0c68-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d0c68-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d0c68-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c68-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c68-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d0c68-144">supportsScopeTags</span></span>|<span data-ttu-id="d0c68-145">Boolean.</span><span class="sxs-lookup"><span data-stu-id="d0c68-145">Boolean</span></span>|<span data-ttu-id="d0c68-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d0c68-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d0c68-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d0c68-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d0c68-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d0c68-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d0c68-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d0c68-149">This property is read-only.</span></span> <span data-ttu-id="d0c68-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c68-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c68-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d0c68-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d0c68-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d0c68-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d0c68-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0c68-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d0c68-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c68-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c68-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d0c68-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d0c68-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d0c68-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d0c68-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0c68-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d0c68-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c68-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c68-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d0c68-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d0c68-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d0c68-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d0c68-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d0c68-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d0c68-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c68-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c68-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0c68-163">createdDateTime</span></span>|<span data-ttu-id="d0c68-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0c68-164">DateTimeOffset</span></span>|<span data-ttu-id="d0c68-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d0c68-165">DateTime the object was created.</span></span> <span data-ttu-id="d0c68-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c68-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c68-167">description</span><span class="sxs-lookup"><span data-stu-id="d0c68-167">description</span></span>|<span data-ttu-id="d0c68-168">String</span><span class="sxs-lookup"><span data-stu-id="d0c68-168">String</span></span>|<span data-ttu-id="d0c68-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0c68-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d0c68-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c68-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c68-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d0c68-171">displayName</span></span>|<span data-ttu-id="d0c68-172">Строка</span><span class="sxs-lookup"><span data-stu-id="d0c68-172">String</span></span>|<span data-ttu-id="d0c68-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0c68-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d0c68-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0c68-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c68-175">version</span><span class="sxs-lookup"><span data-stu-id="d0c68-175">version</span></span>|<span data-ttu-id="d0c68-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d0c68-176">Int32</span></span>|<span data-ttu-id="d0c68-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d0c68-177">Version of the device configuration.</span></span> <span data-ttu-id="d0c68-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d0c68-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0c68-179">licenseType</span><span class="sxs-lookup"><span data-stu-id="d0c68-179">licenseType</span></span>|[<span data-ttu-id="d0c68-180">едитионупграделиценсетипе</span><span class="sxs-lookup"><span data-stu-id="d0c68-180">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="d0c68-181">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="d0c68-181">Edition Upgrade License Type.</span></span> <span data-ttu-id="d0c68-182">Возможные значения: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="d0c68-182">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="d0c68-183">targetEdition</span><span class="sxs-lookup"><span data-stu-id="d0c68-183">targetEdition</span></span>|[<span data-ttu-id="d0c68-184">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="d0c68-184">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="d0c68-185">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="d0c68-185">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="d0c68-186">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN` `windows10MobileEnterprise` `windows10HolographicEnterprise` `windows10Professional` `windows10Home` `windows10HomeChina` `windows10HomeN` `windows10HomeSingleLanguage` `windows10Mobile` `windows10IoTCore` `windows10ProfessionalWorkstationN` `notConfigured`,,,,,,,,,,,,,,,,,,,,, `windows10ProfessionalN` `windows10ProfessionalEducation` `windows10ProfessionalEducationN` `windows10ProfessionalWorkstation` , `windows10IoTCoreCommercial`.</span><span class="sxs-lookup"><span data-stu-id="d0c68-186">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`, `windows10Home`, `windows10HomeChina`, `windows10HomeN`, `windows10HomeSingleLanguage`, `windows10Mobile`, `windows10IoTCore`, `windows10IoTCoreCommercial`.</span></span>|
|<span data-ttu-id="d0c68-187">license</span><span class="sxs-lookup"><span data-stu-id="d0c68-187">license</span></span>|<span data-ttu-id="d0c68-188">String</span><span class="sxs-lookup"><span data-stu-id="d0c68-188">String</span></span>|<span data-ttu-id="d0c68-189">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="d0c68-189">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="d0c68-190">productKey</span><span class="sxs-lookup"><span data-stu-id="d0c68-190">productKey</span></span>|<span data-ttu-id="d0c68-191">String</span><span class="sxs-lookup"><span data-stu-id="d0c68-191">String</span></span>|<span data-ttu-id="d0c68-192">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="d0c68-192">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="d0c68-193">виндовссмоде</span><span class="sxs-lookup"><span data-stu-id="d0c68-193">windowsSMode</span></span>|[<span data-ttu-id="d0c68-194">виндовссмодеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d0c68-194">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="d0c68-195">Конфигурация режима S.</span><span class="sxs-lookup"><span data-stu-id="d0c68-195">S mode configuration.</span></span> <span data-ttu-id="d0c68-196">Возможные значения: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="d0c68-196">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="d0c68-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0c68-197">Response</span></span>
<span data-ttu-id="d0c68-198">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d0c68-198">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0c68-199">Пример</span><span class="sxs-lookup"><span data-stu-id="d0c68-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0c68-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0c68-200">Request</span></span>
<span data-ttu-id="d0c68-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0c68-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d0c68-202">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0c68-202">Response</span></span>
<span data-ttu-id="d0c68-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d0c68-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




