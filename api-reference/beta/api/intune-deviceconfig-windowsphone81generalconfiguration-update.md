---
title: Обновление windowsPhone81GeneralConfiguration
description: Обновление свойств объекта windowsPhone81GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 041b94000581af0145daadd58abff760a3f14366
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48693425"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="4fad6-103">Обновление windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4fad6-103">Update windowsPhone81GeneralConfiguration</span></span>

<span data-ttu-id="4fad6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fad6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fad6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fad6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fad6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fad6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fad6-107">Обновление свойств объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-107">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fad6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4fad6-108">Prerequisites</span></span>
<span data-ttu-id="4fad6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fad6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fad6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fad6-111">Permission type</span></span>|<span data-ttu-id="4fad6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fad6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fad6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fad6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fad6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fad6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4fad6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fad6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fad6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fad6-116">Not supported.</span></span>|
|<span data-ttu-id="4fad6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4fad6-117">Application</span></span>|<span data-ttu-id="4fad6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fad6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fad6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fad6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4fad6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4fad6-120">Request headers</span></span>
|<span data-ttu-id="4fad6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4fad6-121">Header</span></span>|<span data-ttu-id="4fad6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4fad6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fad6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4fad6-123">Authorization</span></span>|<span data-ttu-id="4fad6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fad6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fad6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4fad6-125">Accept</span></span>|<span data-ttu-id="4fad6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fad6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fad6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4fad6-127">Request body</span></span>
<span data-ttu-id="4fad6-128">В теле запроса добавьте представление объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4fad6-128">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="4fad6-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-129">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="4fad6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fad6-130">Property</span></span>|<span data-ttu-id="4fad6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4fad6-131">Type</span></span>|<span data-ttu-id="4fad6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4fad6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fad6-133">id</span><span class="sxs-lookup"><span data-stu-id="4fad6-133">id</span></span>|<span data-ttu-id="4fad6-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4fad6-134">String</span></span>|<span data-ttu-id="4fad6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4fad6-135">Key of the entity.</span></span> <span data-ttu-id="4fad6-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fad6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fad6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4fad6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fad6-138">DateTimeOffset</span></span>|<span data-ttu-id="4fad6-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4fad6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4fad6-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fad6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4fad6-141">roleScopeTagIds</span></span>|<span data-ttu-id="4fad6-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4fad6-142">String collection</span></span>|<span data-ttu-id="4fad6-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4fad6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4fad6-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fad6-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4fad6-145">supportsScopeTags</span></span>|<span data-ttu-id="4fad6-146">Логический</span><span class="sxs-lookup"><span data-stu-id="4fad6-146">Boolean</span></span>|<span data-ttu-id="4fad6-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4fad6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4fad6-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4fad6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4fad6-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4fad6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4fad6-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fad6-150">This property is read-only.</span></span> <span data-ttu-id="4fad6-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fad6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4fad6-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4fad6-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4fad6-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4fad6-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4fad6-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4fad6-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fad6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4fad6-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4fad6-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4fad6-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4fad6-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4fad6-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4fad6-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fad6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4fad6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4fad6-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4fad6-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4fad6-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4fad6-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4fad6-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fad6-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4fad6-164">createdDateTime</span></span>|<span data-ttu-id="4fad6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fad6-165">DateTimeOffset</span></span>|<span data-ttu-id="4fad6-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4fad6-166">DateTime the object was created.</span></span> <span data-ttu-id="4fad6-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fad6-168">description</span><span class="sxs-lookup"><span data-stu-id="4fad6-168">description</span></span>|<span data-ttu-id="4fad6-169">Строка</span><span class="sxs-lookup"><span data-stu-id="4fad6-169">String</span></span>|<span data-ttu-id="4fad6-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4fad6-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4fad6-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fad6-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4fad6-172">displayName</span></span>|<span data-ttu-id="4fad6-173">Строка</span><span class="sxs-lookup"><span data-stu-id="4fad6-173">String</span></span>|<span data-ttu-id="4fad6-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4fad6-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4fad6-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fad6-176">version</span><span class="sxs-lookup"><span data-stu-id="4fad6-176">version</span></span>|<span data-ttu-id="4fad6-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4fad6-177">Int32</span></span>|<span data-ttu-id="4fad6-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4fad6-178">Version of the device configuration.</span></span> <span data-ttu-id="4fad6-179">Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4fad6-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fad6-180">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="4fad6-180">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="4fad6-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-181">Boolean</span></span>|<span data-ttu-id="4fad6-182">Указывает, применяется ли эта политика только к Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="4fad6-182">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="4fad6-183">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4fad6-183">This property is read-only.</span></span>|
|<span data-ttu-id="4fad6-184">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="4fad6-184">appsBlockCopyPaste</span></span>|<span data-ttu-id="4fad6-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-185">Boolean</span></span>|<span data-ttu-id="4fad6-186">Указывает, следует ли заблокировать копирование данных.</span><span class="sxs-lookup"><span data-stu-id="4fad6-186">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="4fad6-187">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="4fad6-187">bluetoothBlocked</span></span>|<span data-ttu-id="4fad6-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-188">Boolean</span></span>|<span data-ttu-id="4fad6-189">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="4fad6-189">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="4fad6-190">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4fad6-190">cameraBlocked</span></span>|<span data-ttu-id="4fad6-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-191">Boolean</span></span>|<span data-ttu-id="4fad6-192">Указывает, следует ли заблокировать камеру.</span><span class="sxs-lookup"><span data-stu-id="4fad6-192">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="4fad6-193">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="4fad6-193">cellularBlockWifiTethering</span></span>|<span data-ttu-id="4fad6-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-194">Boolean</span></span>|<span data-ttu-id="4fad6-195">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4fad6-195">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="4fad6-196">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="4fad6-196">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4fad6-197">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="4fad6-197">compliantAppsList</span></span>|<span data-ttu-id="4fad6-198">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="4fad6-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4fad6-199">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="4fad6-199">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="4fad6-200">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="4fad6-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4fad6-201">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="4fad6-201">compliantAppListType</span></span>|[<span data-ttu-id="4fad6-202">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="4fad6-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="4fad6-203">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="4fad6-203">List that is in the AppComplianceList.</span></span> <span data-ttu-id="4fad6-204">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="4fad6-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="4fad6-205">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="4fad6-205">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="4fad6-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-206">Boolean</span></span>|<span data-ttu-id="4fad6-207">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="4fad6-207">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4fad6-208">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="4fad6-208">emailBlockAddingAccounts</span></span>|<span data-ttu-id="4fad6-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-209">Boolean</span></span>|<span data-ttu-id="4fad6-210">Указывает, следует ли заблокировать пользовательские учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4fad6-210">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="4fad6-211">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="4fad6-211">locationServicesBlocked</span></span>|<span data-ttu-id="4fad6-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-212">Boolean</span></span>|<span data-ttu-id="4fad6-213">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="4fad6-213">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="4fad6-214">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="4fad6-214">microsoftAccountBlocked</span></span>|<span data-ttu-id="4fad6-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-215">Boolean</span></span>|<span data-ttu-id="4fad6-216">Указывает, следует ли запретить использовать учетную запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="4fad6-216">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="4fad6-217">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="4fad6-217">nfcBlocked</span></span>|<span data-ttu-id="4fad6-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-218">Boolean</span></span>|<span data-ttu-id="4fad6-219">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="4fad6-219">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="4fad6-220">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4fad6-220">passwordBlockSimple</span></span>|<span data-ttu-id="4fad6-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-221">Boolean</span></span>|<span data-ttu-id="4fad6-222">Указывает, следует ли заблокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="4fad6-222">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="4fad6-223">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4fad6-223">passwordExpirationDays</span></span>|<span data-ttu-id="4fad6-224">Int32</span><span class="sxs-lookup"><span data-stu-id="4fad6-224">Int32</span></span>|<span data-ttu-id="4fad6-225">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="4fad6-225">Number of days before the password expires.</span></span>|
|<span data-ttu-id="4fad6-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4fad6-226">passwordMinimumLength</span></span>|<span data-ttu-id="4fad6-227">Int32</span><span class="sxs-lookup"><span data-stu-id="4fad6-227">Int32</span></span>|<span data-ttu-id="4fad6-228">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="4fad6-228">Minimum length of passwords.</span></span>|
|<span data-ttu-id="4fad6-229">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4fad6-229">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4fad6-230">Int32</span><span class="sxs-lookup"><span data-stu-id="4fad6-230">Int32</span></span>|<span data-ttu-id="4fad6-231">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="4fad6-231">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="4fad6-232">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4fad6-232">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4fad6-233">Int32</span><span class="sxs-lookup"><span data-stu-id="4fad6-233">Int32</span></span>|<span data-ttu-id="4fad6-234">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="4fad6-234">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="4fad6-235">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4fad6-235">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4fad6-236">Int32</span><span class="sxs-lookup"><span data-stu-id="4fad6-236">Int32</span></span>|<span data-ttu-id="4fad6-237">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="4fad6-237">Number of previous passwords to block.</span></span> <span data-ttu-id="4fad6-238">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="4fad6-238">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4fad6-239">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4fad6-239">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4fad6-240">Int32</span><span class="sxs-lookup"><span data-stu-id="4fad6-240">Int32</span></span>|<span data-ttu-id="4fad6-241">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="4fad6-241">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="4fad6-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4fad6-242">passwordRequiredType</span></span>|[<span data-ttu-id="4fad6-243">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="4fad6-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4fad6-244">Необходимый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="4fad6-244">Password type that is required.</span></span> <span data-ttu-id="4fad6-245">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="4fad6-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4fad6-246">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4fad6-246">passwordRequired</span></span>|<span data-ttu-id="4fad6-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-247">Boolean</span></span>|<span data-ttu-id="4fad6-248">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="4fad6-248">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="4fad6-249">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4fad6-249">screenCaptureBlocked</span></span>|<span data-ttu-id="4fad6-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-250">Boolean</span></span>|<span data-ttu-id="4fad6-251">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="4fad6-251">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="4fad6-252">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="4fad6-252">storageBlockRemovableStorage</span></span>|<span data-ttu-id="4fad6-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-253">Boolean</span></span>|<span data-ttu-id="4fad6-254">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="4fad6-254">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="4fad6-255">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4fad6-255">storageRequireEncryption</span></span>|<span data-ttu-id="4fad6-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-256">Boolean</span></span>|<span data-ttu-id="4fad6-257">Указывает, обязательно ли шифрование.</span><span class="sxs-lookup"><span data-stu-id="4fad6-257">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="4fad6-258">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="4fad6-258">webBrowserBlocked</span></span>|<span data-ttu-id="4fad6-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-259">Boolean</span></span>|<span data-ttu-id="4fad6-260">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="4fad6-260">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="4fad6-261">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="4fad6-261">wifiBlocked</span></span>|<span data-ttu-id="4fad6-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-262">Boolean</span></span>|<span data-ttu-id="4fad6-263">Указывает, следует ли заблокировать Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4fad6-263">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="4fad6-264">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="4fad6-264">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="4fad6-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-265">Boolean</span></span>|<span data-ttu-id="4fad6-266">Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4fad6-266">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="4fad6-267">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="4fad6-267">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4fad6-268">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="4fad6-268">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="4fad6-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-269">Boolean</span></span>|<span data-ttu-id="4fad6-270">Указывает, следует ли запретить устройству сообщать об обнаруженных хот-спотах Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="4fad6-270">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="4fad6-271">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="4fad6-271">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4fad6-272">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="4fad6-272">windowsStoreBlocked</span></span>|<span data-ttu-id="4fad6-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fad6-273">Boolean</span></span>|<span data-ttu-id="4fad6-274">Указывает, следует ли заблокировать Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="4fad6-274">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="4fad6-275">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fad6-275">Response</span></span>
<span data-ttu-id="4fad6-276">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4fad6-276">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fad6-277">Пример</span><span class="sxs-lookup"><span data-stu-id="4fad6-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fad6-278">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fad6-278">Request</span></span>
<span data-ttu-id="4fad6-279">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fad6-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4fad6-280">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fad6-280">Response</span></span>
<span data-ttu-id="4fad6-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4fad6-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





