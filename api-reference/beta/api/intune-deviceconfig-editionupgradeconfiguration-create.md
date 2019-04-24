---
title: Создание объекта editionUpgradeConfiguration
description: Создание объекта editionUpgradeConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d85b5ef2655582f8d8d2aef531de6edf55c88e7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467724"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="bca9e-103">Создание объекта editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="bca9e-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="bca9e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bca9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bca9e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bca9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bca9e-106">Создание объекта [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bca9e-106">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bca9e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bca9e-107">Prerequisites</span></span>
<span data-ttu-id="bca9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bca9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bca9e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bca9e-110">Permission type</span></span>|<span data-ttu-id="bca9e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bca9e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bca9e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bca9e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bca9e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bca9e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bca9e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bca9e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bca9e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bca9e-115">Not supported.</span></span>|
|<span data-ttu-id="bca9e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bca9e-116">Application</span></span>|<span data-ttu-id="bca9e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bca9e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bca9e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bca9e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bca9e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bca9e-119">Request headers</span></span>
|<span data-ttu-id="bca9e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bca9e-120">Header</span></span>|<span data-ttu-id="bca9e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bca9e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bca9e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bca9e-122">Authorization</span></span>|<span data-ttu-id="bca9e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bca9e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bca9e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bca9e-124">Accept</span></span>|<span data-ttu-id="bca9e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bca9e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bca9e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bca9e-126">Request body</span></span>
<span data-ttu-id="bca9e-127">В теле запроса добавьте представление объекта editionUpgradeConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bca9e-127">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="bca9e-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта editionUpgradeConfiguration.</span><span class="sxs-lookup"><span data-stu-id="bca9e-128">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="bca9e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bca9e-129">Property</span></span>|<span data-ttu-id="bca9e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bca9e-130">Type</span></span>|<span data-ttu-id="bca9e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bca9e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bca9e-132">id</span><span class="sxs-lookup"><span data-stu-id="bca9e-132">id</span></span>|<span data-ttu-id="bca9e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="bca9e-133">String</span></span>|<span data-ttu-id="bca9e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bca9e-134">Key of the entity.</span></span> <span data-ttu-id="bca9e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bca9e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bca9e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bca9e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="bca9e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bca9e-137">DateTimeOffset</span></span>|<span data-ttu-id="bca9e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="bca9e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="bca9e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bca9e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bca9e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bca9e-140">roleScopeTagIds</span></span>|<span data-ttu-id="bca9e-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bca9e-141">String collection</span></span>|<span data-ttu-id="bca9e-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="bca9e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bca9e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bca9e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bca9e-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="bca9e-144">supportsScopeTags</span></span>|<span data-ttu-id="bca9e-145">Логический</span><span class="sxs-lookup"><span data-stu-id="bca9e-145">Boolean</span></span>|<span data-ttu-id="bca9e-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="bca9e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bca9e-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="bca9e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bca9e-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="bca9e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bca9e-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bca9e-149">This property is read-only.</span></span> <span data-ttu-id="bca9e-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bca9e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bca9e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bca9e-151">createdDateTime</span></span>|<span data-ttu-id="bca9e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bca9e-152">DateTimeOffset</span></span>|<span data-ttu-id="bca9e-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="bca9e-153">DateTime the object was created.</span></span> <span data-ttu-id="bca9e-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bca9e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bca9e-155">description</span><span class="sxs-lookup"><span data-stu-id="bca9e-155">description</span></span>|<span data-ttu-id="bca9e-156">String</span><span class="sxs-lookup"><span data-stu-id="bca9e-156">String</span></span>|<span data-ttu-id="bca9e-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bca9e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bca9e-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bca9e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bca9e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="bca9e-159">displayName</span></span>|<span data-ttu-id="bca9e-160">Строка</span><span class="sxs-lookup"><span data-stu-id="bca9e-160">String</span></span>|<span data-ttu-id="bca9e-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bca9e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bca9e-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bca9e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bca9e-163">version</span><span class="sxs-lookup"><span data-stu-id="bca9e-163">version</span></span>|<span data-ttu-id="bca9e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="bca9e-164">Int32</span></span>|<span data-ttu-id="bca9e-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="bca9e-165">Version of the device configuration.</span></span> <span data-ttu-id="bca9e-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bca9e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bca9e-167">licenseType</span><span class="sxs-lookup"><span data-stu-id="bca9e-167">licenseType</span></span>|[<span data-ttu-id="bca9e-168">Едитионупграделиценсетипе</span><span class="sxs-lookup"><span data-stu-id="bca9e-168">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="bca9e-169">Тип лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="bca9e-169">Edition Upgrade License Type.</span></span> <span data-ttu-id="bca9e-170">Возможные значения: `productKey`, `licenseFile`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="bca9e-170">Possible values are: `productKey`, `licenseFile`, `notConfigured`.</span></span>|
|<span data-ttu-id="bca9e-171">targetEdition</span><span class="sxs-lookup"><span data-stu-id="bca9e-171">targetEdition</span></span>|[<span data-ttu-id="bca9e-172">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="bca9e-172">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="bca9e-173">Целевой выпуск для обновления.</span><span class="sxs-lookup"><span data-stu-id="bca9e-173">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="bca9e-174">Возможные значения: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="bca9e-174">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`, `notConfigured`.</span></span>|
|<span data-ttu-id="bca9e-175">license</span><span class="sxs-lookup"><span data-stu-id="bca9e-175">license</span></span>|<span data-ttu-id="bca9e-176">String</span><span class="sxs-lookup"><span data-stu-id="bca9e-176">String</span></span>|<span data-ttu-id="bca9e-177">Содержимое файла лицензии для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="bca9e-177">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="bca9e-178">productKey</span><span class="sxs-lookup"><span data-stu-id="bca9e-178">productKey</span></span>|<span data-ttu-id="bca9e-179">String</span><span class="sxs-lookup"><span data-stu-id="bca9e-179">String</span></span>|<span data-ttu-id="bca9e-180">Ключ продукта для обновления выпуска.</span><span class="sxs-lookup"><span data-stu-id="bca9e-180">Edition Upgrade Product Key.</span></span>|
|<span data-ttu-id="bca9e-181">Виндовссмоде</span><span class="sxs-lookup"><span data-stu-id="bca9e-181">windowsSMode</span></span>|[<span data-ttu-id="bca9e-182">Виндовссмодеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="bca9e-182">windowsSModeConfiguration</span></span>](../resources/intune-deviceconfig-windowssmodeconfiguration.md)|<span data-ttu-id="bca9e-183">Конфигурация режима S.</span><span class="sxs-lookup"><span data-stu-id="bca9e-183">S mode configuration.</span></span> <span data-ttu-id="bca9e-184">Возможные значения: `noRestriction`, `block`, `unlock`.</span><span class="sxs-lookup"><span data-stu-id="bca9e-184">Possible values are: `noRestriction`, `block`, `unlock`.</span></span>|



## <a name="response"></a><span data-ttu-id="bca9e-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="bca9e-185">Response</span></span>
<span data-ttu-id="bca9e-186">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bca9e-186">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bca9e-187">Пример</span><span class="sxs-lookup"><span data-stu-id="bca9e-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="bca9e-188">Запрос</span><span class="sxs-lookup"><span data-stu-id="bca9e-188">Request</span></span>
<span data-ttu-id="bca9e-189">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bca9e-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 431

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="bca9e-190">Отклик</span><span class="sxs-lookup"><span data-stu-id="bca9e-190">Response</span></span>
<span data-ttu-id="bca9e-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bca9e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 603

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





