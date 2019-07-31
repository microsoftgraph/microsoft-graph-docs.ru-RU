---
title: Обновление windowsPhone81GeneralConfiguration
description: Обновление свойств объекта windowsPhone81GeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0da557f0f8ea7d04eb8f0ee85ddf6ca1f9d1ad78
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982125"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="83970-103">Обновление windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="83970-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="83970-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83970-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83970-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83970-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83970-106">Обновление свойств объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-106">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83970-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="83970-107">Prerequisites</span></span>
<span data-ttu-id="83970-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83970-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83970-110">Permission type</span></span>|<span data-ttu-id="83970-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83970-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83970-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83970-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83970-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83970-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83970-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83970-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83970-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83970-115">Not supported.</span></span>|
|<span data-ttu-id="83970-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83970-116">Application</span></span>|<span data-ttu-id="83970-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83970-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83970-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83970-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="83970-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83970-119">Request headers</span></span>
|<span data-ttu-id="83970-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83970-120">Header</span></span>|<span data-ttu-id="83970-121">Значение</span><span class="sxs-lookup"><span data-stu-id="83970-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83970-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83970-122">Authorization</span></span>|<span data-ttu-id="83970-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83970-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83970-124">Accept</span><span class="sxs-lookup"><span data-stu-id="83970-124">Accept</span></span>|<span data-ttu-id="83970-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83970-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83970-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="83970-126">Request body</span></span>
<span data-ttu-id="83970-127">В теле запроса добавьте представление объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83970-127">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="83970-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-128">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="83970-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="83970-129">Property</span></span>|<span data-ttu-id="83970-130">Тип</span><span class="sxs-lookup"><span data-stu-id="83970-130">Type</span></span>|<span data-ttu-id="83970-131">Описание</span><span class="sxs-lookup"><span data-stu-id="83970-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83970-132">id</span><span class="sxs-lookup"><span data-stu-id="83970-132">id</span></span>|<span data-ttu-id="83970-133">String</span><span class="sxs-lookup"><span data-stu-id="83970-133">String</span></span>|<span data-ttu-id="83970-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="83970-134">Key of the entity.</span></span> <span data-ttu-id="83970-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83970-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83970-136">lastModifiedDateTime</span></span>|<span data-ttu-id="83970-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83970-137">DateTimeOffset</span></span>|<span data-ttu-id="83970-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="83970-138">DateTime the object was last modified.</span></span> <span data-ttu-id="83970-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83970-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83970-140">roleScopeTagIds</span></span>|<span data-ttu-id="83970-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="83970-141">String collection</span></span>|<span data-ttu-id="83970-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="83970-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="83970-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83970-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="83970-144">supportsScopeTags</span></span>|<span data-ttu-id="83970-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-145">Boolean</span></span>|<span data-ttu-id="83970-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="83970-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="83970-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="83970-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="83970-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="83970-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="83970-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83970-149">This property is read-only.</span></span> <span data-ttu-id="83970-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83970-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83970-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="83970-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="83970-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="83970-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="83970-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="83970-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83970-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83970-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="83970-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="83970-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="83970-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="83970-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="83970-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83970-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="83970-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="83970-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="83970-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="83970-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="83970-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="83970-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83970-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83970-163">createdDateTime</span></span>|<span data-ttu-id="83970-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83970-164">DateTimeOffset</span></span>|<span data-ttu-id="83970-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="83970-165">DateTime the object was created.</span></span> <span data-ttu-id="83970-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83970-167">description</span><span class="sxs-lookup"><span data-stu-id="83970-167">description</span></span>|<span data-ttu-id="83970-168">String</span><span class="sxs-lookup"><span data-stu-id="83970-168">String</span></span>|<span data-ttu-id="83970-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="83970-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83970-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83970-171">displayName</span><span class="sxs-lookup"><span data-stu-id="83970-171">displayName</span></span>|<span data-ttu-id="83970-172">Строка</span><span class="sxs-lookup"><span data-stu-id="83970-172">String</span></span>|<span data-ttu-id="83970-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="83970-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83970-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83970-175">version</span><span class="sxs-lookup"><span data-stu-id="83970-175">version</span></span>|<span data-ttu-id="83970-176">Int32</span><span class="sxs-lookup"><span data-stu-id="83970-176">Int32</span></span>|<span data-ttu-id="83970-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="83970-177">Version of the device configuration.</span></span> <span data-ttu-id="83970-178">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83970-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="83970-179">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="83970-179">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="83970-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-180">Boolean</span></span>|<span data-ttu-id="83970-181">Указывает, применяется ли эта политика только к Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="83970-181">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="83970-182">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83970-182">This property is read-only.</span></span>|
|<span data-ttu-id="83970-183">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="83970-183">appsBlockCopyPaste</span></span>|<span data-ttu-id="83970-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-184">Boolean</span></span>|<span data-ttu-id="83970-185">Указывает, следует ли заблокировать копирование данных.</span><span class="sxs-lookup"><span data-stu-id="83970-185">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="83970-186">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="83970-186">bluetoothBlocked</span></span>|<span data-ttu-id="83970-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-187">Boolean</span></span>|<span data-ttu-id="83970-188">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="83970-188">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="83970-189">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="83970-189">cameraBlocked</span></span>|<span data-ttu-id="83970-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-190">Boolean</span></span>|<span data-ttu-id="83970-191">Указывает, следует ли заблокировать камеру.</span><span class="sxs-lookup"><span data-stu-id="83970-191">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="83970-192">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="83970-192">cellularBlockWifiTethering</span></span>|<span data-ttu-id="83970-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-193">Boolean</span></span>|<span data-ttu-id="83970-194">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="83970-194">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="83970-195">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="83970-195">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="83970-196">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="83970-196">compliantAppsList</span></span>|<span data-ttu-id="83970-197">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="83970-197">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="83970-198">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="83970-198">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="83970-199">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="83970-199">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="83970-200">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="83970-200">compliantAppListType</span></span>|[<span data-ttu-id="83970-201">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="83970-201">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="83970-202">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="83970-202">List that is in the AppComplianceList.</span></span> <span data-ttu-id="83970-203">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="83970-203">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="83970-204">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="83970-204">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="83970-205">Логический</span><span class="sxs-lookup"><span data-stu-id="83970-205">Boolean</span></span>|<span data-ttu-id="83970-206">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="83970-206">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="83970-207">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="83970-207">emailBlockAddingAccounts</span></span>|<span data-ttu-id="83970-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-208">Boolean</span></span>|<span data-ttu-id="83970-209">Указывает, следует ли заблокировать пользовательские учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="83970-209">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="83970-210">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="83970-210">locationServicesBlocked</span></span>|<span data-ttu-id="83970-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-211">Boolean</span></span>|<span data-ttu-id="83970-212">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="83970-212">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="83970-213">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="83970-213">microsoftAccountBlocked</span></span>|<span data-ttu-id="83970-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-214">Boolean</span></span>|<span data-ttu-id="83970-215">Указывает, следует ли запретить использовать учетную запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="83970-215">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="83970-216">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="83970-216">nfcBlocked</span></span>|<span data-ttu-id="83970-217">Логический</span><span class="sxs-lookup"><span data-stu-id="83970-217">Boolean</span></span>|<span data-ttu-id="83970-218">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="83970-218">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="83970-219">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="83970-219">passwordBlockSimple</span></span>|<span data-ttu-id="83970-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-220">Boolean</span></span>|<span data-ttu-id="83970-221">Указывает, следует ли заблокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="83970-221">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="83970-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="83970-222">passwordExpirationDays</span></span>|<span data-ttu-id="83970-223">Int32</span><span class="sxs-lookup"><span data-stu-id="83970-223">Int32</span></span>|<span data-ttu-id="83970-224">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="83970-224">Number of days before the password expires.</span></span>|
|<span data-ttu-id="83970-225">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="83970-225">passwordMinimumLength</span></span>|<span data-ttu-id="83970-226">Int32</span><span class="sxs-lookup"><span data-stu-id="83970-226">Int32</span></span>|<span data-ttu-id="83970-227">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="83970-227">Minimum length of passwords.</span></span>|
|<span data-ttu-id="83970-228">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="83970-228">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="83970-229">Int32</span><span class="sxs-lookup"><span data-stu-id="83970-229">Int32</span></span>|<span data-ttu-id="83970-230">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="83970-230">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="83970-231">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="83970-231">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="83970-232">Int32</span><span class="sxs-lookup"><span data-stu-id="83970-232">Int32</span></span>|<span data-ttu-id="83970-233">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="83970-233">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="83970-234">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="83970-234">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="83970-235">Int32</span><span class="sxs-lookup"><span data-stu-id="83970-235">Int32</span></span>|<span data-ttu-id="83970-236">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="83970-236">Number of previous passwords to block.</span></span> <span data-ttu-id="83970-237">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="83970-237">Valid values 0 to 24</span></span>|
|<span data-ttu-id="83970-238">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="83970-238">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="83970-239">Int32</span><span class="sxs-lookup"><span data-stu-id="83970-239">Int32</span></span>|<span data-ttu-id="83970-240">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="83970-240">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="83970-241">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="83970-241">passwordRequiredType</span></span>|[<span data-ttu-id="83970-242">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="83970-242">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="83970-243">Необходимый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="83970-243">Password type that is required.</span></span> <span data-ttu-id="83970-244">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="83970-244">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="83970-245">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="83970-245">passwordRequired</span></span>|<span data-ttu-id="83970-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-246">Boolean</span></span>|<span data-ttu-id="83970-247">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="83970-247">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="83970-248">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="83970-248">screenCaptureBlocked</span></span>|<span data-ttu-id="83970-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-249">Boolean</span></span>|<span data-ttu-id="83970-250">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="83970-250">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="83970-251">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="83970-251">storageBlockRemovableStorage</span></span>|<span data-ttu-id="83970-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-252">Boolean</span></span>|<span data-ttu-id="83970-253">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="83970-253">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="83970-254">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="83970-254">storageRequireEncryption</span></span>|<span data-ttu-id="83970-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-255">Boolean</span></span>|<span data-ttu-id="83970-256">Указывает, обязательно ли шифрование.</span><span class="sxs-lookup"><span data-stu-id="83970-256">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="83970-257">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="83970-257">webBrowserBlocked</span></span>|<span data-ttu-id="83970-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-258">Boolean</span></span>|<span data-ttu-id="83970-259">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="83970-259">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="83970-260">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="83970-260">wifiBlocked</span></span>|<span data-ttu-id="83970-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-261">Boolean</span></span>|<span data-ttu-id="83970-262">Указывает, следует ли заблокировать Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="83970-262">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="83970-263">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="83970-263">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="83970-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-264">Boolean</span></span>|<span data-ttu-id="83970-265">Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="83970-265">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="83970-266">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="83970-266">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="83970-267">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="83970-267">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="83970-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-268">Boolean</span></span>|<span data-ttu-id="83970-269">Указывает, следует ли запретить устройству сообщать об обнаруженных хот-спотах Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="83970-269">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="83970-270">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="83970-270">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="83970-271">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="83970-271">windowsStoreBlocked</span></span>|<span data-ttu-id="83970-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="83970-272">Boolean</span></span>|<span data-ttu-id="83970-273">Указывает, следует ли заблокировать Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="83970-273">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="83970-274">Отклик</span><span class="sxs-lookup"><span data-stu-id="83970-274">Response</span></span>
<span data-ttu-id="83970-275">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="83970-275">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83970-276">Пример</span><span class="sxs-lookup"><span data-stu-id="83970-276">Example</span></span>

### <a name="request"></a><span data-ttu-id="83970-277">Запрос</span><span class="sxs-lookup"><span data-stu-id="83970-277">Request</span></span>
<span data-ttu-id="83970-278">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83970-278">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2326

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="83970-279">Отклик</span><span class="sxs-lookup"><span data-stu-id="83970-279">Response</span></span>
<span data-ttu-id="83970-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="83970-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2498

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
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
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```





