---
title: Обновление объекта iosGeneralDeviceConfiguration
description: Обновление свойств объекта iosGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 72f0312cf219a28dc06747cc095a52b65b1caeea
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533814"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="d9438-103">Обновление объекта iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d9438-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="d9438-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9438-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9438-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9438-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9438-106">Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9438-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9438-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d9438-107">Prerequisites</span></span>
<span data-ttu-id="d9438-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9438-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9438-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9438-110">Permission type</span></span>|<span data-ttu-id="d9438-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9438-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9438-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9438-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9438-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9438-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d9438-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9438-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9438-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9438-115">Not supported.</span></span>|
|<span data-ttu-id="d9438-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d9438-116">Application</span></span>|<span data-ttu-id="d9438-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9438-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9438-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9438-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d9438-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9438-119">Request headers</span></span>
|<span data-ttu-id="d9438-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d9438-120">Header</span></span>|<span data-ttu-id="d9438-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d9438-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9438-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d9438-122">Authorization</span></span>|<span data-ttu-id="d9438-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9438-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9438-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d9438-124">Accept</span></span>|<span data-ttu-id="d9438-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9438-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9438-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d9438-126">Request body</span></span>
<span data-ttu-id="d9438-127">В тексте запроса добавьте представление объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9438-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="d9438-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9438-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="d9438-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9438-129">Property</span></span>|<span data-ttu-id="d9438-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d9438-130">Type</span></span>|<span data-ttu-id="d9438-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d9438-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9438-132">id</span><span class="sxs-lookup"><span data-stu-id="d9438-132">id</span></span>|<span data-ttu-id="d9438-133">String</span><span class="sxs-lookup"><span data-stu-id="d9438-133">String</span></span>|<span data-ttu-id="d9438-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d9438-134">Key of the entity.</span></span> <span data-ttu-id="d9438-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9438-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9438-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9438-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d9438-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9438-137">DateTimeOffset</span></span>|<span data-ttu-id="d9438-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d9438-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d9438-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9438-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9438-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d9438-140">roleScopeTagIds</span></span>|<span data-ttu-id="d9438-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d9438-141">String collection</span></span>|<span data-ttu-id="d9438-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d9438-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d9438-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9438-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9438-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d9438-144">supportsScopeTags</span></span>|<span data-ttu-id="d9438-145">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-145">Boolean</span></span>|<span data-ttu-id="d9438-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d9438-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d9438-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d9438-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d9438-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d9438-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d9438-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d9438-149">This property is read-only.</span></span> <span data-ttu-id="d9438-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9438-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9438-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d9438-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d9438-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d9438-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d9438-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d9438-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d9438-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9438-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9438-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d9438-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d9438-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d9438-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d9438-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d9438-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d9438-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9438-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9438-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d9438-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d9438-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d9438-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d9438-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d9438-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d9438-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9438-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9438-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9438-163">createdDateTime</span></span>|<span data-ttu-id="d9438-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9438-164">DateTimeOffset</span></span>|<span data-ttu-id="d9438-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d9438-165">DateTime the object was created.</span></span> <span data-ttu-id="d9438-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9438-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9438-167">description</span><span class="sxs-lookup"><span data-stu-id="d9438-167">description</span></span>|<span data-ttu-id="d9438-168">String</span><span class="sxs-lookup"><span data-stu-id="d9438-168">String</span></span>|<span data-ttu-id="d9438-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d9438-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d9438-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9438-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9438-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d9438-171">displayName</span></span>|<span data-ttu-id="d9438-172">Строка</span><span class="sxs-lookup"><span data-stu-id="d9438-172">String</span></span>|<span data-ttu-id="d9438-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d9438-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d9438-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d9438-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9438-175">version</span><span class="sxs-lookup"><span data-stu-id="d9438-175">version</span></span>|<span data-ttu-id="d9438-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d9438-176">Int32</span></span>|<span data-ttu-id="d9438-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d9438-177">Version of the device configuration.</span></span> <span data-ttu-id="d9438-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d9438-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d9438-179">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="d9438-179">accountBlockModification</span></span>|<span data-ttu-id="d9438-180">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-180">Boolean</span></span>|<span data-ttu-id="d9438-181">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-181">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-182">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="d9438-182">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="d9438-183">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-183">Boolean</span></span>|<span data-ttu-id="d9438-184">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-184">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="d9438-185">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-185">airDropBlocked</span></span>|<span data-ttu-id="d9438-186">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-186">Boolean</span></span>|<span data-ttu-id="d9438-187">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-187">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-188">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="d9438-188">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="d9438-189">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-189">Boolean</span></span>|<span data-ttu-id="d9438-190">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-190">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d9438-191">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="d9438-191">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="d9438-192">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-192">Boolean</span></span>|<span data-ttu-id="d9438-193">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="d9438-193">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="d9438-194">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="d9438-194">appleWatchBlockPairing</span></span>|<span data-ttu-id="d9438-195">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-195">Boolean</span></span>|<span data-ttu-id="d9438-196">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-196">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d9438-197">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="d9438-197">appleWatchForceWristDetection</span></span>|<span data-ttu-id="d9438-198">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-198">Boolean</span></span>|<span data-ttu-id="d9438-199">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-199">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="d9438-200">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-200">appleNewsBlocked</span></span>|<span data-ttu-id="d9438-201">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-201">Boolean</span></span>|<span data-ttu-id="d9438-202">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-202">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d9438-203">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="d9438-203">appsSingleAppModeList</span></span>|<span data-ttu-id="d9438-204">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d9438-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d9438-205">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="d9438-205">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="d9438-206">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-206">Supervised only.</span></span> <span data-ttu-id="d9438-207">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="d9438-207">iOS 7.0 and later.</span></span> <span data-ttu-id="d9438-208">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d9438-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d9438-209">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="d9438-209">appsVisibilityList</span></span>|<span data-ttu-id="d9438-210">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d9438-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d9438-211">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-211">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="d9438-212">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="d9438-212">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d9438-213">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="d9438-213">appsVisibilityListType</span></span>|[<span data-ttu-id="d9438-214">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="d9438-214">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d9438-215">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="d9438-215">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="d9438-216">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d9438-216">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d9438-217">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="d9438-217">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="d9438-218">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-218">Boolean</span></span>|<span data-ttu-id="d9438-219">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-219">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d9438-220">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-220">appStoreBlocked</span></span>|<span data-ttu-id="d9438-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9438-221">Boolean</span></span>|<span data-ttu-id="d9438-222">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="d9438-222">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="d9438-223">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d9438-223">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d9438-224">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="d9438-224">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="d9438-225">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-225">Boolean</span></span>|<span data-ttu-id="d9438-226">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="d9438-226">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="d9438-227">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="d9438-227">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="d9438-228">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-228">Boolean</span></span>|<span data-ttu-id="d9438-229">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="d9438-229">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="d9438-230">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-230">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d9438-231">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="d9438-231">appStoreRequirePassword</span></span>|<span data-ttu-id="d9438-232">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-232">Boolean</span></span>|<span data-ttu-id="d9438-233">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="d9438-233">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="d9438-234">аутофиллфорцеаусентикатион</span><span class="sxs-lookup"><span data-stu-id="d9438-234">autoFillForceAuthentication</span></span>|<span data-ttu-id="d9438-235">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-235">Boolean</span></span>|<span data-ttu-id="d9438-236">Указывает, следует ли принудительно выполнять проверку подлинности пользователей перед автозаполнением паролей и сведений о кредитных картах в Safari и других приложениях на контролируемых устройствах.</span><span class="sxs-lookup"><span data-stu-id="d9438-236">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="d9438-237">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="d9438-237">bluetoothBlockModification</span></span>|<span data-ttu-id="d9438-238">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-238">Boolean</span></span>|<span data-ttu-id="d9438-239">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-239">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="d9438-240">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-240">cameraBlocked</span></span>|<span data-ttu-id="d9438-241">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-241">Boolean</span></span>|<span data-ttu-id="d9438-242">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="d9438-242">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="d9438-243">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d9438-243">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d9438-244">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="d9438-244">cellularBlockDataRoaming</span></span>|<span data-ttu-id="d9438-245">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-245">Boolean</span></span>|<span data-ttu-id="d9438-246">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="d9438-246">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="d9438-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="d9438-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="d9438-248">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-248">Boolean</span></span>|<span data-ttu-id="d9438-249">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="d9438-249">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="d9438-250">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="d9438-250">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="d9438-251">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-251">Boolean</span></span>|<span data-ttu-id="d9438-252">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-252">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-253">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="d9438-253">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="d9438-254">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-254">Boolean</span></span>|<span data-ttu-id="d9438-255">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="d9438-255">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="d9438-256">целлуларблоккпланмодификатион</span><span class="sxs-lookup"><span data-stu-id="d9438-256">cellularBlockPlanModification</span></span>|<span data-ttu-id="d9438-257">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-257">Boolean</span></span>|<span data-ttu-id="d9438-258">Указывает, следует ли запретить пользователям изменять параметры плана сотовой связи на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="d9438-258">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="d9438-259">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="d9438-259">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="d9438-260">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-260">Boolean</span></span>|<span data-ttu-id="d9438-261">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="d9438-261">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="d9438-262">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="d9438-262">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="d9438-263">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-263">Boolean</span></span>|<span data-ttu-id="d9438-264">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="d9438-264">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="d9438-265">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d9438-265">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="d9438-266">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-266">Boolean</span></span>|<span data-ttu-id="d9438-267">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-267">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d9438-268">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d9438-268">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="d9438-269">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-269">Boolean</span></span>|<span data-ttu-id="d9438-270">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-270">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-271">классрумфорцеаутоматикаллижоинклассес</span><span class="sxs-lookup"><span data-stu-id="d9438-271">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="d9438-272">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-272">Boolean</span></span>|<span data-ttu-id="d9438-273">Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-273">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-274">классрумфорцеунпромптедаппанддевицелокк</span><span class="sxs-lookup"><span data-stu-id="d9438-274">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="d9438-275">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-275">Boolean</span></span>|<span data-ttu-id="d9438-276">Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся.</span><span class="sxs-lookup"><span data-stu-id="d9438-276">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="d9438-277">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-277">Supervised only.</span></span>|
|<span data-ttu-id="d9438-278">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="d9438-278">compliantAppsList</span></span>|<span data-ttu-id="d9438-279">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="d9438-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d9438-280">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="d9438-280">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="d9438-281">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="d9438-281">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d9438-282">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="d9438-282">compliantAppListType</span></span>|[<span data-ttu-id="d9438-283">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="d9438-283">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d9438-284">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="d9438-284">List that is in the AppComplianceList.</span></span> <span data-ttu-id="d9438-285">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="d9438-285">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d9438-286">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="d9438-286">configurationProfileBlockChanges</span></span>|<span data-ttu-id="d9438-287">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-287">Boolean</span></span>|<span data-ttu-id="d9438-288">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-288">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-289">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-289">definitionLookupBlocked</span></span>|<span data-ttu-id="d9438-290">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-290">Boolean</span></span>|<span data-ttu-id="d9438-291">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-291">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="d9438-292">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="d9438-292">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="d9438-293">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-293">Boolean</span></span>|<span data-ttu-id="d9438-294">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-294">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-295">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="d9438-295">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="d9438-296">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-296">Boolean</span></span>|<span data-ttu-id="d9438-297">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-297">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-298">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="d9438-298">deviceBlockNameModification</span></span>|<span data-ttu-id="d9438-299">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-299">Boolean</span></span>|<span data-ttu-id="d9438-300">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-300">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d9438-301">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="d9438-301">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="d9438-302">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-302">Boolean</span></span>|<span data-ttu-id="d9438-303">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="d9438-303">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="d9438-304">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="d9438-304">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="d9438-305">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-305">Boolean</span></span>|<span data-ttu-id="d9438-306">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-306">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="d9438-307">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="d9438-307">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="d9438-308">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-308">Boolean</span></span>|<span data-ttu-id="d9438-309">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="d9438-309">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="d9438-310">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="d9438-310">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="d9438-311">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-311">Boolean</span></span>|<span data-ttu-id="d9438-312">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="d9438-312">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="d9438-313">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="d9438-313">emailInDomainSuffixes</span></span>|<span data-ttu-id="d9438-314">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d9438-314">String collection</span></span>|<span data-ttu-id="d9438-315">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="d9438-315">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="d9438-316">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="d9438-316">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="d9438-317">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-317">Boolean</span></span>|<span data-ttu-id="d9438-318">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="d9438-318">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="d9438-319">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="d9438-319">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="d9438-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9438-320">Boolean</span></span>|<span data-ttu-id="d9438-321">Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="d9438-321">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="d9438-322">есимблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="d9438-322">esimBlockModification</span></span>|<span data-ttu-id="d9438-323">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-323">Boolean</span></span>|<span data-ttu-id="d9438-324">Указывает, следует ли разрешить добавление или удаление планов сотовой связи на eSIM контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="d9438-324">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="d9438-325">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-325">faceTimeBlocked</span></span>|<span data-ttu-id="d9438-326">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-326">Boolean</span></span>|<span data-ttu-id="d9438-327">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="d9438-327">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="d9438-328">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d9438-328">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d9438-329">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-329">findMyFriendsBlocked</span></span>|<span data-ttu-id="d9438-330">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-330">Boolean</span></span>|<span data-ttu-id="d9438-331">Указывает, следует ли заблокировать изменения для поиска друзей, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-331">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-332">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="d9438-332">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="d9438-333">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-333">Boolean</span></span>|<span data-ttu-id="d9438-334">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="d9438-334">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="d9438-335">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d9438-335">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d9438-336">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="d9438-336">gamingBlockMultiplayer</span></span>|<span data-ttu-id="d9438-337">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-337">Boolean</span></span>|<span data-ttu-id="d9438-338">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="d9438-338">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="d9438-339">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d9438-339">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d9438-340">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-340">gameCenterBlocked</span></span>|<span data-ttu-id="d9438-341">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-341">Boolean</span></span>|<span data-ttu-id="d9438-342">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-342">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-343">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-343">hostPairingBlocked</span></span>|<span data-ttu-id="d9438-344">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-344">Boolean</span></span>|<span data-ttu-id="d9438-345">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-345">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-346">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-346">iBooksStoreBlocked</span></span>|<span data-ttu-id="d9438-347">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-347">Boolean</span></span>|<span data-ttu-id="d9438-348">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-348">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-349">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="d9438-349">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="d9438-350">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-350">Boolean</span></span>|<span data-ttu-id="d9438-351">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="d9438-351">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="d9438-352">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="d9438-352">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="d9438-353">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-353">Boolean</span></span>|<span data-ttu-id="d9438-354">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="d9438-354">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="d9438-355">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="d9438-355">iCloudBlockBackup</span></span>|<span data-ttu-id="d9438-356">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-356">Boolean</span></span>|<span data-ttu-id="d9438-357">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="d9438-357">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="d9438-358">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d9438-358">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d9438-359">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="d9438-359">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="d9438-360">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-360">Boolean</span></span>|<span data-ttu-id="d9438-361">Указывает, следует ли заблокировать синхронизацию документов iCloud. Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d9438-361">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d9438-362">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="d9438-362">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="d9438-363">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-363">Boolean</span></span>|<span data-ttu-id="d9438-364">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="d9438-364">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="d9438-365">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="d9438-365">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="d9438-366">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-366">Boolean</span></span>|<span data-ttu-id="d9438-367">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="d9438-367">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="d9438-368">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="d9438-368">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="d9438-369">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-369">Boolean</span></span>|<span data-ttu-id="d9438-370">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="d9438-370">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="d9438-371">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="d9438-371">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="d9438-372">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-372">Boolean</span></span>|<span data-ttu-id="d9438-373">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="d9438-373">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="d9438-374">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="d9438-374">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="d9438-375">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-375">Boolean</span></span>|<span data-ttu-id="d9438-376">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="d9438-376">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="d9438-377">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="d9438-377">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="d9438-378">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-378">Boolean</span></span>|<span data-ttu-id="d9438-379">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="d9438-379">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="d9438-380">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d9438-380">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d9438-381">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="d9438-381">iTunesBlockMusicService</span></span>|<span data-ttu-id="d9438-382">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-382">Boolean</span></span>|<span data-ttu-id="d9438-383">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-383">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="d9438-384">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="d9438-384">iTunesBlockRadio</span></span>|<span data-ttu-id="d9438-385">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-385">Boolean</span></span>|<span data-ttu-id="d9438-386">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-386">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d9438-387">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="d9438-387">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="d9438-388">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-388">Boolean</span></span>|<span data-ttu-id="d9438-389">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-389">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d9438-390">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="d9438-390">keyboardBlockDictation</span></span>|<span data-ttu-id="d9438-391">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-391">Boolean</span></span>|<span data-ttu-id="d9438-392">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-392">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-393">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="d9438-393">keyboardBlockPredictive</span></span>|<span data-ttu-id="d9438-394">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-394">Boolean</span></span>|<span data-ttu-id="d9438-395">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-395">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d9438-396">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="d9438-396">keyboardBlockShortcuts</span></span>|<span data-ttu-id="d9438-397">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-397">Boolean</span></span>|<span data-ttu-id="d9438-398">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-398">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d9438-399">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="d9438-399">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="d9438-400">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-400">Boolean</span></span>|<span data-ttu-id="d9438-401">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-401">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="d9438-402">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="d9438-402">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="d9438-403">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-403">Boolean</span></span>|<span data-ttu-id="d9438-404">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-404">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-405">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="d9438-405">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="d9438-406">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-406">Boolean</span></span>|<span data-ttu-id="d9438-407">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-407">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-408">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="d9438-408">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="d9438-409">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-409">Boolean</span></span>|<span data-ttu-id="d9438-410">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-410">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="d9438-411">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="d9438-411">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d9438-412">Вместо этого используйте Киоскмодеблоккаутолокк.</span><span class="sxs-lookup"><span data-stu-id="d9438-412">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="d9438-413">киоскмодеблоккаутолокк</span><span class="sxs-lookup"><span data-stu-id="d9438-413">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="d9438-414">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-414">Boolean</span></span>|<span data-ttu-id="d9438-415">Указывает, следует ли блокировать автоматическую блокировку устройств в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-415">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-416">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="d9438-416">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="d9438-417">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-417">Boolean</span></span>|<span data-ttu-id="d9438-418">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-418">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-419">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="d9438-419">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="d9438-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9438-420">Boolean</span></span>|<span data-ttu-id="d9438-421">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-421">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="d9438-422">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="d9438-422">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d9438-423">Вместо этого используйте Киоскмодеблоккринжерсвитч.</span><span class="sxs-lookup"><span data-stu-id="d9438-423">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="d9438-424">киоскмодеблоккринжерсвитч</span><span class="sxs-lookup"><span data-stu-id="d9438-424">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="d9438-425">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-425">Boolean</span></span>|<span data-ttu-id="d9438-426">Указывает, следует ли запретить использование переключателя звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-426">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-427">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="d9438-427">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="d9438-428">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-428">Boolean</span></span>|<span data-ttu-id="d9438-429">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-429">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="d9438-430">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="d9438-430">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d9438-431">Вместо этого используйте Киоскмодеблоккскринротатион.</span><span class="sxs-lookup"><span data-stu-id="d9438-431">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="d9438-432">киоскмодеблоккскринротатион</span><span class="sxs-lookup"><span data-stu-id="d9438-432">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="d9438-433">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-433">Boolean</span></span>|<span data-ttu-id="d9438-434">Указывает, следует ли блокировать поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-434">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-435">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="d9438-435">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="d9438-436">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-436">Boolean</span></span>|<span data-ttu-id="d9438-437">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-437">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="d9438-438">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="d9438-438">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d9438-439">Вместо этого используйте Киоскмодеблоккслипбуттон.</span><span class="sxs-lookup"><span data-stu-id="d9438-439">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="d9438-440">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="d9438-440">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="d9438-441">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-441">Boolean</span></span>|<span data-ttu-id="d9438-442">Указывает, следует ли запретить использование кнопки "сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-442">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-443">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="d9438-443">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="d9438-444">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-444">Boolean</span></span>|<span data-ttu-id="d9438-445">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-445">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="d9438-446">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="d9438-446">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d9438-447">Вместо этого используйте Киоскмодеблокктаучскрин.</span><span class="sxs-lookup"><span data-stu-id="d9438-447">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="d9438-448">киоскмодеблокктаучскрин</span><span class="sxs-lookup"><span data-stu-id="d9438-448">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="d9438-449">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-449">Boolean</span></span>|<span data-ttu-id="d9438-450">Указывает, следует ли запретить использование сенсорного экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-450">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-451">киоскмодинаблевоицеконтрол</span><span class="sxs-lookup"><span data-stu-id="d9438-451">kioskModeEnableVoiceControl</span></span>|<span data-ttu-id="d9438-452">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-452">Boolean</span></span>|<span data-ttu-id="d9438-453">Указывает, следует ли включить управление голосовым режимом в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-453">Indicates whether or not to enable voice control in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-454">киоскмодеалловвоицеконтролмодификатион</span><span class="sxs-lookup"><span data-stu-id="d9438-454">kioskModeAllowVoiceControlModification</span></span>|<span data-ttu-id="d9438-455">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-455">Boolean</span></span>|<span data-ttu-id="d9438-456">Указывает, следует ли запретить пользователю переключать управление голосовым режимом в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-456">Indicates whether or not to allow the user to toggle voice control in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-457">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="d9438-457">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="d9438-458">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-458">Boolean</span></span>|<span data-ttu-id="d9438-459">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-459">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-460">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="d9438-460">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="d9438-461">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-461">Boolean</span></span>|<span data-ttu-id="d9438-462">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-462">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="d9438-463">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="d9438-463">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="d9438-464">Вместо этого используйте Киоскмодеблоккволумебуттонс.</span><span class="sxs-lookup"><span data-stu-id="d9438-464">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="d9438-465">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="d9438-465">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="d9438-466">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-466">Boolean</span></span>|<span data-ttu-id="d9438-467">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="d9438-467">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="d9438-468">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="d9438-468">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="d9438-469">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-469">Boolean</span></span>|<span data-ttu-id="d9438-470">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-470">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-471">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="d9438-471">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="d9438-472">String</span><span class="sxs-lookup"><span data-stu-id="d9438-472">String</span></span>|<span data-ttu-id="d9438-473">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-473">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="d9438-474">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="d9438-474">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="d9438-475">киоскмодебуилтинаппид</span><span class="sxs-lookup"><span data-stu-id="d9438-475">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="d9438-476">String</span><span class="sxs-lookup"><span data-stu-id="d9438-476">String</span></span>|<span data-ttu-id="d9438-477">Идентификатор встроенных приложений для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-477">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="d9438-478">Используется, когда KioskModeManagedAppId и KioskModeAppStoreUrl не заданы.</span><span class="sxs-lookup"><span data-stu-id="d9438-478">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="d9438-479">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="d9438-479">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="d9438-480">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-480">Boolean</span></span>|<span data-ttu-id="d9438-481">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-481">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-482">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="d9438-482">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="d9438-483">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-483">Boolean</span></span>|<span data-ttu-id="d9438-484">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-484">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-485">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="d9438-485">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="d9438-486">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-486">Boolean</span></span>|<span data-ttu-id="d9438-487">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-487">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-488">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="d9438-488">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="d9438-489">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-489">Boolean</span></span>|<span data-ttu-id="d9438-490">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-490">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-491">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="d9438-491">kioskModeRequireZoom</span></span>|<span data-ttu-id="d9438-492">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-492">Boolean</span></span>|<span data-ttu-id="d9438-493">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-493">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="d9438-494">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="d9438-494">kioskModeManagedAppId</span></span>|<span data-ttu-id="d9438-495">String</span><span class="sxs-lookup"><span data-stu-id="d9438-495">String</span></span>|<span data-ttu-id="d9438-496">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="d9438-496">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="d9438-497">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="d9438-497">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="d9438-498">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="d9438-498">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="d9438-499">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-499">Boolean</span></span>|<span data-ttu-id="d9438-500">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="d9438-500">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="d9438-501">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="d9438-501">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="d9438-502">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-502">Boolean</span></span>|<span data-ttu-id="d9438-503">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="d9438-503">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="d9438-504">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="d9438-504">lockScreenBlockPassbook</span></span>|<span data-ttu-id="d9438-505">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-505">Boolean</span></span>|<span data-ttu-id="d9438-506">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="d9438-506">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="d9438-507">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="d9438-507">lockScreenBlockTodayView</span></span>|<span data-ttu-id="d9438-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9438-508">Boolean</span></span>|<span data-ttu-id="d9438-509">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="d9438-509">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="d9438-510">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d9438-510">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="d9438-511">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d9438-511">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="d9438-512">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="d9438-512">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="d9438-513">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="d9438-513">mediaContentRatingCanada</span></span>|[<span data-ttu-id="d9438-514">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="d9438-514">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="d9438-515">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="d9438-515">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="d9438-516">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d9438-516">mediaContentRatingFrance</span></span>|[<span data-ttu-id="d9438-517">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d9438-517">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="d9438-518">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="d9438-518">Media content rating settings for France</span></span>|
|<span data-ttu-id="d9438-519">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d9438-519">mediaContentRatingGermany</span></span>|[<span data-ttu-id="d9438-520">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="d9438-520">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="d9438-521">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="d9438-521">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="d9438-522">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="d9438-522">mediaContentRatingIreland</span></span>|[<span data-ttu-id="d9438-523">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="d9438-523">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="d9438-524">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="d9438-524">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="d9438-525">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d9438-525">mediaContentRatingJapan</span></span>|[<span data-ttu-id="d9438-526">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="d9438-526">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="d9438-527">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="d9438-527">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="d9438-528">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d9438-528">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="d9438-529">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d9438-529">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="d9438-530">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="d9438-530">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="d9438-531">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="d9438-531">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="d9438-532">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="d9438-532">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="d9438-533">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="d9438-533">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="d9438-534">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d9438-534">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="d9438-535">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d9438-535">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="d9438-536">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="d9438-536">Media content rating settings for United States</span></span>|
|<span data-ttu-id="d9438-537">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="d9438-537">networkUsageRules</span></span>|<span data-ttu-id="d9438-538">Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="d9438-538">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="d9438-539">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="d9438-539">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="d9438-540">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="d9438-540">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="d9438-541">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="d9438-541">mediaContentRatingApps</span></span>|[<span data-ttu-id="d9438-542">ратингаппстипе</span><span class="sxs-lookup"><span data-stu-id="d9438-542">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="d9438-543">Параметры оценки контента мультимедиа для приложений.</span><span class="sxs-lookup"><span data-stu-id="d9438-543">Media content rating settings for Apps.</span></span> <span data-ttu-id="d9438-544">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="d9438-544">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="d9438-545">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-545">messagesBlocked</span></span>|<span data-ttu-id="d9438-546">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-546">Boolean</span></span>|<span data-ttu-id="d9438-547">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="d9438-547">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="d9438-548">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="d9438-548">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="d9438-549">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-549">Boolean</span></span>|<span data-ttu-id="d9438-550">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-550">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d9438-551">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d9438-551">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="d9438-552">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-552">Boolean</span></span>|<span data-ttu-id="d9438-553">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="d9438-553">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="d9438-554">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="d9438-554">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="d9438-555">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-555">Boolean</span></span>|<span data-ttu-id="d9438-556">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-556">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="d9438-557">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="d9438-557">passcodeBlockModification</span></span>|<span data-ttu-id="d9438-558">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-558">Boolean</span></span>|<span data-ttu-id="d9438-559">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-559">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="d9438-560">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d9438-560">passcodeBlockSimple</span></span>|<span data-ttu-id="d9438-561">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-561">Boolean</span></span>|<span data-ttu-id="d9438-562">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="d9438-562">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="d9438-563">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d9438-563">passcodeExpirationDays</span></span>|<span data-ttu-id="d9438-564">Int32</span><span class="sxs-lookup"><span data-stu-id="d9438-564">Int32</span></span>|<span data-ttu-id="d9438-565">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="d9438-565">Number of days before the passcode expires.</span></span> <span data-ttu-id="d9438-566">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="d9438-566">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="d9438-567">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d9438-567">passcodeMinimumLength</span></span>|<span data-ttu-id="d9438-568">Int32</span><span class="sxs-lookup"><span data-stu-id="d9438-568">Int32</span></span>|<span data-ttu-id="d9438-569">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="d9438-569">Minimum length of passcode.</span></span> <span data-ttu-id="d9438-570">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="d9438-570">Valid values 4 to 14</span></span>|
|<span data-ttu-id="d9438-571">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d9438-571">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d9438-572">Int32</span><span class="sxs-lookup"><span data-stu-id="d9438-572">Int32</span></span>|<span data-ttu-id="d9438-573">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="d9438-573">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="d9438-574">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d9438-574">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d9438-575">Int32</span><span class="sxs-lookup"><span data-stu-id="d9438-575">Int32</span></span>|<span data-ttu-id="d9438-576">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="d9438-576">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d9438-577">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d9438-577">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="d9438-578">Int32</span><span class="sxs-lookup"><span data-stu-id="d9438-578">Int32</span></span>|<span data-ttu-id="d9438-579">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="d9438-579">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="d9438-580">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="d9438-580">Valid values 0 to 4</span></span>|
|<span data-ttu-id="d9438-581">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="d9438-581">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="d9438-582">Int32</span><span class="sxs-lookup"><span data-stu-id="d9438-582">Int32</span></span>|<span data-ttu-id="d9438-583">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="d9438-583">Number of previous passcodes to block.</span></span> <span data-ttu-id="d9438-584">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="d9438-584">Valid values 1 to 24</span></span>|
|<span data-ttu-id="d9438-585">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="d9438-585">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="d9438-586">Int32</span><span class="sxs-lookup"><span data-stu-id="d9438-586">Int32</span></span>|<span data-ttu-id="d9438-587">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="d9438-587">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="d9438-588">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="d9438-588">Valid values 4 to 11</span></span>|
|<span data-ttu-id="d9438-589">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="d9438-589">passcodeRequiredType</span></span>|[<span data-ttu-id="d9438-590">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="d9438-590">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d9438-591">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="d9438-591">Type of passcode that is required.</span></span> <span data-ttu-id="d9438-592">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d9438-592">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d9438-593">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="d9438-593">passcodeRequired</span></span>|<span data-ttu-id="d9438-594">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-594">Boolean</span></span>|<span data-ttu-id="d9438-595">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="d9438-595">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="d9438-596">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-596">podcastsBlocked</span></span>|<span data-ttu-id="d9438-597">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-597">Boolean</span></span>|<span data-ttu-id="d9438-598">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-598">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="d9438-599">проксимитиблокксетуптоневдевице</span><span class="sxs-lookup"><span data-stu-id="d9438-599">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="d9438-600">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-600">Boolean</span></span>|<span data-ttu-id="d9438-601">Указывает, следует ли включить запрос на установку находящихся рядом устройств с защищенным устройством.</span><span class="sxs-lookup"><span data-stu-id="d9438-601">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="d9438-602">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="d9438-602">safariBlockAutofill</span></span>|<span data-ttu-id="d9438-603">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-603">Boolean</span></span>|<span data-ttu-id="d9438-604">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="d9438-604">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="d9438-605">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d9438-605">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d9438-606">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="d9438-606">safariBlockJavaScript</span></span>|<span data-ttu-id="d9438-607">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-607">Boolean</span></span>|<span data-ttu-id="d9438-608">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="d9438-608">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="d9438-609">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="d9438-609">safariBlockPopups</span></span>|<span data-ttu-id="d9438-610">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-610">Boolean</span></span>|<span data-ttu-id="d9438-611">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="d9438-611">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="d9438-612">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-612">safariBlocked</span></span>|<span data-ttu-id="d9438-613">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9438-613">Boolean</span></span>|<span data-ttu-id="d9438-614">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="d9438-614">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="d9438-615">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d9438-615">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d9438-616">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d9438-616">safariCookieSettings</span></span>|[<span data-ttu-id="d9438-617">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="d9438-617">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="d9438-618">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="d9438-618">Cookie settings for Safari.</span></span> <span data-ttu-id="d9438-619">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="d9438-619">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="d9438-620">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="d9438-620">safariManagedDomains</span></span>|<span data-ttu-id="d9438-621">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d9438-621">String collection</span></span>|<span data-ttu-id="d9438-622">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="d9438-622">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="d9438-623">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="d9438-623">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="d9438-624">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d9438-624">String collection</span></span>|<span data-ttu-id="d9438-625">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="d9438-625">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="d9438-626">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-626">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="d9438-627">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="d9438-627">safariRequireFraudWarning</span></span>|<span data-ttu-id="d9438-628">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-628">Boolean</span></span>|<span data-ttu-id="d9438-629">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="d9438-629">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="d9438-630">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-630">screenCaptureBlocked</span></span>|<span data-ttu-id="d9438-631">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-631">Boolean</span></span>|<span data-ttu-id="d9438-632">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="d9438-632">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="d9438-633">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-633">siriBlocked</span></span>|<span data-ttu-id="d9438-634">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-634">Boolean</span></span>|<span data-ttu-id="d9438-635">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="d9438-635">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="d9438-636">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="d9438-636">siriBlockedWhenLocked</span></span>|<span data-ttu-id="d9438-637">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-637">Boolean</span></span>|<span data-ttu-id="d9438-638">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="d9438-638">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="d9438-639">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="d9438-639">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="d9438-640">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-640">Boolean</span></span>|<span data-ttu-id="d9438-641">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="d9438-641">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="d9438-642">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="d9438-642">siriRequireProfanityFilter</span></span>|<span data-ttu-id="d9438-643">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-643">Boolean</span></span>|<span data-ttu-id="d9438-644">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="d9438-644">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="d9438-645">софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="d9438-645">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="d9438-646">Int32</span><span class="sxs-lookup"><span data-stu-id="d9438-646">Int32</span></span>|<span data-ttu-id="d9438-647">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="d9438-647">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="d9438-648">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="d9438-648">Valid values 0 to 90</span></span>|
|<span data-ttu-id="d9438-649">софтвареупдатесфорцеделайед</span><span class="sxs-lookup"><span data-stu-id="d9438-649">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="d9438-650">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-650">Boolean</span></span>|<span data-ttu-id="d9438-651">Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-651">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-652">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="d9438-652">spotlightBlockInternetResults</span></span>|<span data-ttu-id="d9438-653">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-653">Boolean</span></span>|<span data-ttu-id="d9438-654">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="d9438-654">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="d9438-655">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-655">voiceDialingBlocked</span></span>|<span data-ttu-id="d9438-656">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-656">Boolean</span></span>|<span data-ttu-id="d9438-657">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="d9438-657">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="d9438-658">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="d9438-658">wallpaperBlockModification</span></span>|<span data-ttu-id="d9438-659">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-659">Boolean</span></span>|<span data-ttu-id="d9438-660">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-660">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="d9438-661">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="d9438-661">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="d9438-662">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9438-662">Boolean</span></span>|<span data-ttu-id="d9438-663">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="d9438-663">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d9438-664">классрумфорцерекуестпермиссионтолеавеклассес</span><span class="sxs-lookup"><span data-stu-id="d9438-664">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="d9438-665">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-665">Boolean</span></span>|<span data-ttu-id="d9438-666">Указывает, является ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса (iOS 11,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-666">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="d9438-667">кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="d9438-667">keychainBlockCloudSync</span></span>|<span data-ttu-id="d9438-668">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-668">Boolean</span></span>|<span data-ttu-id="d9438-669">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud.</span><span class="sxs-lookup"><span data-stu-id="d9438-669">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="d9438-670">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d9438-670">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="d9438-671">пкиблоккотаупдатес</span><span class="sxs-lookup"><span data-stu-id="d9438-671">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="d9438-672">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-672">Boolean</span></span>|<span data-ttu-id="d9438-673">Указывает, блокируются ли обновления PKI беспроводной сети.</span><span class="sxs-lookup"><span data-stu-id="d9438-673">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="d9438-674">Если задать для этого ограничения значение false, проверки CRL и OCSP (iOS 7,0 и более поздних версий) не отключаются.</span><span class="sxs-lookup"><span data-stu-id="d9438-674">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="d9438-675">привацифорцелимитадтраккинг</span><span class="sxs-lookup"><span data-stu-id="d9438-675">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="d9438-676">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-676">Boolean</span></span>|<span data-ttu-id="d9438-677">Указывает, ограничено ли отслеживание AD. (iOS 7,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-677">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="d9438-678">ентерприсебукблоккбаккуп</span><span class="sxs-lookup"><span data-stu-id="d9438-678">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="d9438-679">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-679">Boolean</span></span>|<span data-ttu-id="d9438-680">Указывает, блокируется ли резервное копирование корпоративной книги.</span><span class="sxs-lookup"><span data-stu-id="d9438-680">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="d9438-681">ентерприсебукблоккметадатасинк</span><span class="sxs-lookup"><span data-stu-id="d9438-681">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="d9438-682">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-682">Boolean</span></span>|<span data-ttu-id="d9438-683">Указывает, блокируется ли синхронизация заметок и выделений корпоративных книг.</span><span class="sxs-lookup"><span data-stu-id="d9438-683">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="d9438-684">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="d9438-684">airPrintBlocked</span></span>|<span data-ttu-id="d9438-685">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-685">Boolean</span></span>|<span data-ttu-id="d9438-686">Указывает, заблокировано ли Аирпринт (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-686">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d9438-687">аирпринтблокккредентиалсстораже</span><span class="sxs-lookup"><span data-stu-id="d9438-687">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="d9438-688">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-688">Boolean</span></span>|<span data-ttu-id="d9438-689">Указывает, заблокировано ли хранение цепочки ключей имени пользователя и пароля для Аирпринт (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-689">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d9438-690">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="d9438-690">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="d9438-691">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-691">Boolean</span></span>|<span data-ttu-id="d9438-692">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-692">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d9438-693">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="d9438-693">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="d9438-694">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-694">Boolean</span></span>|<span data-ttu-id="d9438-695">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="d9438-695">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="d9438-696">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-696">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d9438-697">филеснетворкдривеакцессблоккед</span><span class="sxs-lookup"><span data-stu-id="d9438-697">filesNetworkDriveAccessBlocked</span></span>|<span data-ttu-id="d9438-698">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-698">Boolean</span></span>|<span data-ttu-id="d9438-699">Указывает, могут ли устройства получать доступ к файлам или другим ресурсам на сетевом сервере с помощью протокола SMB.</span><span class="sxs-lookup"><span data-stu-id="d9438-699">Indicates if devices can access files or other resources on a network server using the Server Message Block (SMB) protocol.</span></span> <span data-ttu-id="d9438-700">Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="d9438-700">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="d9438-701">филесусбдривеакцессблоккед</span><span class="sxs-lookup"><span data-stu-id="d9438-701">filesUsbDriveAccessBlocked</span></span>|<span data-ttu-id="d9438-702">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-702">Boolean</span></span>|<span data-ttu-id="d9438-703">Указывает, могут ли севицес с Access подключаться к файлам и открывать их на USB-диске.</span><span class="sxs-lookup"><span data-stu-id="d9438-703">Indicates if sevices with access can connect to and open files on a USB drive.</span></span> <span data-ttu-id="d9438-704">Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="d9438-704">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="d9438-705">вифиповеронфорцед</span><span class="sxs-lookup"><span data-stu-id="d9438-705">wifiPowerOnForced</span></span>|<span data-ttu-id="d9438-706">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-706">Boolean</span></span>|<span data-ttu-id="d9438-707">Указывает, остается ли Wi-Fi On, даже если устройство находится в режиме "в самолете".</span><span class="sxs-lookup"><span data-stu-id="d9438-707">Indicates whether or not Wi-Fi remains on, even when device is in airplane mode.</span></span> <span data-ttu-id="d9438-708">Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="d9438-708">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="d9438-709">блокксистемаппремовал</span><span class="sxs-lookup"><span data-stu-id="d9438-709">blockSystemAppRemoval</span></span>|<span data-ttu-id="d9438-710">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-710">Boolean</span></span>|<span data-ttu-id="d9438-711">Указывает, заблокировано ли удаление системных приложений с устройства на контролируемом устройстве (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-711">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d9438-712">впнблокккреатион</span><span class="sxs-lookup"><span data-stu-id="d9438-712">vpnBlockCreation</span></span>|<span data-ttu-id="d9438-713">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-713">Boolean</span></span>|<span data-ttu-id="d9438-714">Указывает, блокируется ли создание конфигураций VPN (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-714">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="d9438-715">аппремовалблоккед</span><span class="sxs-lookup"><span data-stu-id="d9438-715">appRemovalBlocked</span></span>|<span data-ttu-id="d9438-716">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-716">Boolean</span></span>|<span data-ttu-id="d9438-717">Указывает, разрешено ли удаление приложений.</span><span class="sxs-lookup"><span data-stu-id="d9438-717">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="d9438-718">усбрестриктедмодеблоккед</span><span class="sxs-lookup"><span data-stu-id="d9438-718">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="d9438-719">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-719">Boolean</span></span>|<span data-ttu-id="d9438-720">Указывает, разрешена ли подключаться к стандарту USB, пока устройство заблокировано (iOS 11.4.1 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-720">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="d9438-721">пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="d9438-721">passwordBlockAutoFill</span></span>|<span data-ttu-id="d9438-722">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-722">Boolean</span></span>|<span data-ttu-id="d9438-723">Указывает, разрешена ли функция автозаполнения паролей (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-723">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d9438-724">пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="d9438-724">passwordBlockProximityRequests</span></span>|<span data-ttu-id="d9438-725">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-725">Boolean</span></span>|<span data-ttu-id="d9438-726">Указывает, следует ли запретить запрашивать пароли с близлежащих устройств (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-726">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d9438-727">пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="d9438-727">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="d9438-728">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-728">Boolean</span></span>|<span data-ttu-id="d9438-729">Указывает, следует ли заблокировать общий доступ к паролям с помощью AirDrop паролей iOS 12,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="d9438-729">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d9438-730">датеандтимефорцесетаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="d9438-730">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="d9438-731">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-731">Boolean</span></span>|<span data-ttu-id="d9438-732">Указывает, включена ли функция даты и времени "автоматически задано" и не может быть отключена пользователем (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-732">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d9438-733">контактсалловманажедтаунманажедврите</span><span class="sxs-lookup"><span data-stu-id="d9438-733">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="d9438-734">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-734">Boolean</span></span>|<span data-ttu-id="d9438-735">Указывает, могут ли управляемые приложения записывать контакты в неуправляемые учетные записи контактов (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="d9438-735">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="d9438-736">контактсалловунманажедтоманажедреад</span><span class="sxs-lookup"><span data-stu-id="d9438-736">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="d9438-737">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-737">Boolean</span></span>|<span data-ttu-id="d9438-738">Указывает, могут ли неуправляемые приложения читать из управляемых учетных записей контактов (iOS 12,0 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="d9438-738">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="d9438-739">целлуларблоккперсоналхотспотмодификатион</span><span class="sxs-lookup"><span data-stu-id="d9438-739">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="d9438-740">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-740">Boolean</span></span>|<span data-ttu-id="d9438-741">Указывает, следует ли запретить пользователю изменять параметр личных гиперобъектов (iOS 12,2 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="d9438-741">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="d9438-742">сиридисаблесерверлоггинг</span><span class="sxs-lookup"><span data-stu-id="d9438-742">siriDisableServerLogging</span></span>|<span data-ttu-id="d9438-743">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-743">Boolean</span></span>|<span data-ttu-id="d9438-744">Указывает, отключено ли ведение журнала Siri на стороне сервера (iOS 12,2 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="d9438-744">Indicates whether or not server-side Siri logging is disabled (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="d9438-745">континуауспаскэйбоардблоккед</span><span class="sxs-lookup"><span data-stu-id="d9438-745">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="d9438-746">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-746">Boolean</span></span>|<span data-ttu-id="d9438-747">Указывает, следует ли заблокировать клавиатуру непрерывного пути, когда устройство защищено (iOS 13 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="d9438-747">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="d9438-748">финдмидевицеинфиндмяппблоккед</span><span class="sxs-lookup"><span data-stu-id="d9438-748">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="d9438-749">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-749">Boolean</span></span>|<span data-ttu-id="d9438-750">Указывает, следует ли заблокировать Поиск устройства, когда устройство защищено (iOS 13 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="d9438-750">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="d9438-751">финдмифриендсинфиндмяппблоккед</span><span class="sxs-lookup"><span data-stu-id="d9438-751">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="d9438-752">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-752">Boolean</span></span>|<span data-ttu-id="d9438-753">Указывает, следует ли заблокировать "найти друзей", когда устройство защищено (iOS 13 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="d9438-753">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="d9438-754">итунесблоккед</span><span class="sxs-lookup"><span data-stu-id="d9438-754">iTunesBlocked</span></span>|<span data-ttu-id="d9438-755">Логический</span><span class="sxs-lookup"><span data-stu-id="d9438-755">Boolean</span></span>|<span data-ttu-id="d9438-756">Указывает, следует ли заблокировать приложение iTunes.</span><span class="sxs-lookup"><span data-stu-id="d9438-756">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="d9438-757">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="d9438-757">Requires a supervised device for iOS 13 and later.</span></span>|



## <a name="response"></a><span data-ttu-id="d9438-758">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9438-758">Response</span></span>
<span data-ttu-id="d9438-759">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d9438-759">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9438-760">Пример</span><span class="sxs-lookup"><span data-stu-id="d9438-760">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9438-761">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9438-761">Request</span></span>
<span data-ttu-id="d9438-762">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d9438-762">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 10517

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
  "kioskModeEnableVoiceControl": true,
  "kioskModeAllowVoiceControlModification": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "filesNetworkDriveAccessBlocked": true,
  "filesUsbDriveAccessBlocked": true,
  "wifiPowerOnForced": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "siriDisableServerLogging": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="d9438-763">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9438-763">Response</span></span>
<span data-ttu-id="d9438-p156">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9438-p156">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10689

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
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
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
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
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
  "kioskModeEnableVoiceControl": true,
  "kioskModeAllowVoiceControlModification": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "filesNetworkDriveAccessBlocked": true,
  "filesUsbDriveAccessBlocked": true,
  "wifiPowerOnForced": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "siriDisableServerLogging": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true
}
```






