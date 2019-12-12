---
title: Create iosGeneralDeviceConfiguration
description: Создание объекта iosGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ddb2f83641ed80c187abfa1ab2a8a40fa9d8ac6a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39948895"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="86a3b-103">Create iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="86a3b-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="86a3b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86a3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86a3b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86a3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86a3b-106">Создание объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86a3b-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86a3b-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="86a3b-107">Prerequisites</span></span>
<span data-ttu-id="86a3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86a3b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86a3b-110">Permission type</span></span>|<span data-ttu-id="86a3b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86a3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86a3b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86a3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86a3b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86a3b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86a3b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86a3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86a3b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86a3b-115">Not supported.</span></span>|
|<span data-ttu-id="86a3b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86a3b-116">Application</span></span>|<span data-ttu-id="86a3b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86a3b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86a3b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86a3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="86a3b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86a3b-119">Request headers</span></span>
|<span data-ttu-id="86a3b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86a3b-120">Header</span></span>|<span data-ttu-id="86a3b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="86a3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86a3b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86a3b-122">Authorization</span></span>|<span data-ttu-id="86a3b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86a3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86a3b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="86a3b-124">Accept</span></span>|<span data-ttu-id="86a3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86a3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86a3b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="86a3b-126">Request body</span></span>
<span data-ttu-id="86a3b-127">В теле запроса добавьте представление объекта iosGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86a3b-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="86a3b-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="86a3b-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="86a3b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="86a3b-129">Property</span></span>|<span data-ttu-id="86a3b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="86a3b-130">Type</span></span>|<span data-ttu-id="86a3b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="86a3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86a3b-132">id</span><span class="sxs-lookup"><span data-stu-id="86a3b-132">id</span></span>|<span data-ttu-id="86a3b-133">String</span><span class="sxs-lookup"><span data-stu-id="86a3b-133">String</span></span>|<span data-ttu-id="86a3b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="86a3b-134">Key of the entity.</span></span> <span data-ttu-id="86a3b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86a3b-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86a3b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86a3b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="86a3b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86a3b-137">DateTimeOffset</span></span>|<span data-ttu-id="86a3b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="86a3b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="86a3b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86a3b-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86a3b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86a3b-140">roleScopeTagIds</span></span>|<span data-ttu-id="86a3b-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="86a3b-141">String collection</span></span>|<span data-ttu-id="86a3b-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="86a3b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="86a3b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86a3b-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86a3b-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="86a3b-144">supportsScopeTags</span></span>|<span data-ttu-id="86a3b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-145">Boolean</span></span>|<span data-ttu-id="86a3b-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="86a3b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="86a3b-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="86a3b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="86a3b-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="86a3b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="86a3b-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="86a3b-149">This property is read-only.</span></span> <span data-ttu-id="86a3b-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86a3b-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86a3b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86a3b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="86a3b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="86a3b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="86a3b-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="86a3b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="86a3b-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86a3b-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86a3b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86a3b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="86a3b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="86a3b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="86a3b-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="86a3b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="86a3b-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86a3b-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86a3b-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86a3b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="86a3b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="86a3b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="86a3b-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="86a3b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="86a3b-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86a3b-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86a3b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86a3b-163">createdDateTime</span></span>|<span data-ttu-id="86a3b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86a3b-164">DateTimeOffset</span></span>|<span data-ttu-id="86a3b-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="86a3b-165">DateTime the object was created.</span></span> <span data-ttu-id="86a3b-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86a3b-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86a3b-167">description</span><span class="sxs-lookup"><span data-stu-id="86a3b-167">description</span></span>|<span data-ttu-id="86a3b-168">String</span><span class="sxs-lookup"><span data-stu-id="86a3b-168">String</span></span>|<span data-ttu-id="86a3b-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="86a3b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="86a3b-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86a3b-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86a3b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="86a3b-171">displayName</span></span>|<span data-ttu-id="86a3b-172">Строка</span><span class="sxs-lookup"><span data-stu-id="86a3b-172">String</span></span>|<span data-ttu-id="86a3b-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="86a3b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="86a3b-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="86a3b-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86a3b-175">version</span><span class="sxs-lookup"><span data-stu-id="86a3b-175">version</span></span>|<span data-ttu-id="86a3b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="86a3b-176">Int32</span></span>|<span data-ttu-id="86a3b-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="86a3b-177">Version of the device configuration.</span></span> <span data-ttu-id="86a3b-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="86a3b-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="86a3b-179">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="86a3b-179">accountBlockModification</span></span>|<span data-ttu-id="86a3b-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-180">Boolean</span></span>|<span data-ttu-id="86a3b-181">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-181">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-182">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="86a3b-182">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="86a3b-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-183">Boolean</span></span>|<span data-ttu-id="86a3b-184">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-184">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="86a3b-185">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-185">airDropBlocked</span></span>|<span data-ttu-id="86a3b-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-186">Boolean</span></span>|<span data-ttu-id="86a3b-187">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-187">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-188">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="86a3b-188">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="86a3b-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-189">Boolean</span></span>|<span data-ttu-id="86a3b-190">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-190">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="86a3b-191">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="86a3b-191">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="86a3b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-192">Boolean</span></span>|<span data-ttu-id="86a3b-193">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="86a3b-193">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="86a3b-194">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="86a3b-194">appleWatchBlockPairing</span></span>|<span data-ttu-id="86a3b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-195">Boolean</span></span>|<span data-ttu-id="86a3b-196">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-196">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="86a3b-197">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="86a3b-197">appleWatchForceWristDetection</span></span>|<span data-ttu-id="86a3b-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-198">Boolean</span></span>|<span data-ttu-id="86a3b-199">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-199">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="86a3b-200">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-200">appleNewsBlocked</span></span>|<span data-ttu-id="86a3b-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-201">Boolean</span></span>|<span data-ttu-id="86a3b-202">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-202">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="86a3b-203">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="86a3b-203">appsSingleAppModeList</span></span>|<span data-ttu-id="86a3b-204">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="86a3b-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="86a3b-205">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="86a3b-205">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="86a3b-206">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-206">Supervised only.</span></span> <span data-ttu-id="86a3b-207">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="86a3b-207">iOS 7.0 and later.</span></span> <span data-ttu-id="86a3b-208">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="86a3b-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="86a3b-209">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="86a3b-209">appsVisibilityList</span></span>|<span data-ttu-id="86a3b-210">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="86a3b-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="86a3b-211">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-211">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="86a3b-212">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="86a3b-212">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="86a3b-213">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="86a3b-213">appsVisibilityListType</span></span>|[<span data-ttu-id="86a3b-214">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="86a3b-214">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="86a3b-215">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="86a3b-215">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="86a3b-216">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="86a3b-216">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="86a3b-217">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="86a3b-217">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="86a3b-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-218">Boolean</span></span>|<span data-ttu-id="86a3b-219">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-219">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="86a3b-220">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-220">appStoreBlocked</span></span>|<span data-ttu-id="86a3b-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-221">Boolean</span></span>|<span data-ttu-id="86a3b-222">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="86a3b-222">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="86a3b-223">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="86a3b-223">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="86a3b-224">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="86a3b-224">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="86a3b-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-225">Boolean</span></span>|<span data-ttu-id="86a3b-226">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="86a3b-226">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="86a3b-227">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="86a3b-227">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="86a3b-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-228">Boolean</span></span>|<span data-ttu-id="86a3b-229">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="86a3b-229">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="86a3b-230">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-230">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="86a3b-231">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="86a3b-231">appStoreRequirePassword</span></span>|<span data-ttu-id="86a3b-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-232">Boolean</span></span>|<span data-ttu-id="86a3b-233">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="86a3b-233">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="86a3b-234">аутофиллфорцеаусентикатион</span><span class="sxs-lookup"><span data-stu-id="86a3b-234">autoFillForceAuthentication</span></span>|<span data-ttu-id="86a3b-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-235">Boolean</span></span>|<span data-ttu-id="86a3b-236">Указывает, следует ли принудительно выполнять проверку подлинности пользователей перед автозаполнением паролей и сведений о кредитных картах в Safari и других приложениях на контролируемых устройствах.</span><span class="sxs-lookup"><span data-stu-id="86a3b-236">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="86a3b-237">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="86a3b-237">bluetoothBlockModification</span></span>|<span data-ttu-id="86a3b-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-238">Boolean</span></span>|<span data-ttu-id="86a3b-239">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-239">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="86a3b-240">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-240">cameraBlocked</span></span>|<span data-ttu-id="86a3b-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-241">Boolean</span></span>|<span data-ttu-id="86a3b-242">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="86a3b-242">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="86a3b-243">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="86a3b-243">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="86a3b-244">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="86a3b-244">cellularBlockDataRoaming</span></span>|<span data-ttu-id="86a3b-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-245">Boolean</span></span>|<span data-ttu-id="86a3b-246">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="86a3b-246">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="86a3b-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="86a3b-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="86a3b-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-248">Boolean</span></span>|<span data-ttu-id="86a3b-249">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="86a3b-249">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="86a3b-250">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="86a3b-250">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="86a3b-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-251">Boolean</span></span>|<span data-ttu-id="86a3b-252">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-252">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-253">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="86a3b-253">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="86a3b-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-254">Boolean</span></span>|<span data-ttu-id="86a3b-255">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="86a3b-255">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="86a3b-256">целлуларблоккпланмодификатион</span><span class="sxs-lookup"><span data-stu-id="86a3b-256">cellularBlockPlanModification</span></span>|<span data-ttu-id="86a3b-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-257">Boolean</span></span>|<span data-ttu-id="86a3b-258">Указывает, следует ли запретить пользователям изменять параметры плана сотовой связи на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="86a3b-258">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="86a3b-259">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="86a3b-259">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="86a3b-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-260">Boolean</span></span>|<span data-ttu-id="86a3b-261">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="86a3b-261">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="86a3b-262">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="86a3b-262">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="86a3b-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-263">Boolean</span></span>|<span data-ttu-id="86a3b-264">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="86a3b-264">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="86a3b-265">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="86a3b-265">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="86a3b-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-266">Boolean</span></span>|<span data-ttu-id="86a3b-267">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-267">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="86a3b-268">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="86a3b-268">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="86a3b-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-269">Boolean</span></span>|<span data-ttu-id="86a3b-270">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-270">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-271">классрумфорцеаутоматикаллижоинклассес</span><span class="sxs-lookup"><span data-stu-id="86a3b-271">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="86a3b-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-272">Boolean</span></span>|<span data-ttu-id="86a3b-273">Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-273">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-274">классрумфорцеунпромптедаппанддевицелокк</span><span class="sxs-lookup"><span data-stu-id="86a3b-274">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="86a3b-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-275">Boolean</span></span>|<span data-ttu-id="86a3b-276">Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся.</span><span class="sxs-lookup"><span data-stu-id="86a3b-276">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="86a3b-277">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-277">Supervised only.</span></span>|
|<span data-ttu-id="86a3b-278">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="86a3b-278">compliantAppsList</span></span>|<span data-ttu-id="86a3b-279">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="86a3b-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="86a3b-280">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="86a3b-280">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="86a3b-281">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="86a3b-281">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="86a3b-282">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="86a3b-282">compliantAppListType</span></span>|[<span data-ttu-id="86a3b-283">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="86a3b-283">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="86a3b-284">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="86a3b-284">List that is in the AppComplianceList.</span></span> <span data-ttu-id="86a3b-285">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="86a3b-285">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="86a3b-286">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="86a3b-286">configurationProfileBlockChanges</span></span>|<span data-ttu-id="86a3b-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-287">Boolean</span></span>|<span data-ttu-id="86a3b-288">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-288">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-289">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-289">definitionLookupBlocked</span></span>|<span data-ttu-id="86a3b-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-290">Boolean</span></span>|<span data-ttu-id="86a3b-291">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-291">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="86a3b-292">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="86a3b-292">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="86a3b-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-293">Boolean</span></span>|<span data-ttu-id="86a3b-294">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-294">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-295">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="86a3b-295">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="86a3b-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-296">Boolean</span></span>|<span data-ttu-id="86a3b-297">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-297">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-298">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="86a3b-298">deviceBlockNameModification</span></span>|<span data-ttu-id="86a3b-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-299">Boolean</span></span>|<span data-ttu-id="86a3b-300">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-300">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="86a3b-301">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="86a3b-301">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="86a3b-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-302">Boolean</span></span>|<span data-ttu-id="86a3b-303">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="86a3b-303">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="86a3b-304">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="86a3b-304">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="86a3b-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-305">Boolean</span></span>|<span data-ttu-id="86a3b-306">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-306">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="86a3b-307">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="86a3b-307">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="86a3b-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-308">Boolean</span></span>|<span data-ttu-id="86a3b-309">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="86a3b-309">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="86a3b-310">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="86a3b-310">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="86a3b-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-311">Boolean</span></span>|<span data-ttu-id="86a3b-312">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="86a3b-312">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="86a3b-313">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="86a3b-313">emailInDomainSuffixes</span></span>|<span data-ttu-id="86a3b-314">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="86a3b-314">String collection</span></span>|<span data-ttu-id="86a3b-315">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="86a3b-315">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="86a3b-316">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="86a3b-316">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="86a3b-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-317">Boolean</span></span>|<span data-ttu-id="86a3b-318">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="86a3b-318">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="86a3b-319">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="86a3b-319">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="86a3b-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-320">Boolean</span></span>|<span data-ttu-id="86a3b-321">Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="86a3b-321">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="86a3b-322">есимблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="86a3b-322">esimBlockModification</span></span>|<span data-ttu-id="86a3b-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-323">Boolean</span></span>|<span data-ttu-id="86a3b-324">Указывает, следует ли разрешить добавление или удаление планов сотовой связи на eSIM контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="86a3b-324">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="86a3b-325">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-325">faceTimeBlocked</span></span>|<span data-ttu-id="86a3b-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-326">Boolean</span></span>|<span data-ttu-id="86a3b-327">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="86a3b-327">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="86a3b-328">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="86a3b-328">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="86a3b-329">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-329">findMyFriendsBlocked</span></span>|<span data-ttu-id="86a3b-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-330">Boolean</span></span>|<span data-ttu-id="86a3b-331">Указывает, следует ли заблокировать изменения для поиска друзей, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-331">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-332">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="86a3b-332">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="86a3b-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-333">Boolean</span></span>|<span data-ttu-id="86a3b-334">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="86a3b-334">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="86a3b-335">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="86a3b-335">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="86a3b-336">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="86a3b-336">gamingBlockMultiplayer</span></span>|<span data-ttu-id="86a3b-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-337">Boolean</span></span>|<span data-ttu-id="86a3b-338">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="86a3b-338">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="86a3b-339">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="86a3b-339">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="86a3b-340">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-340">gameCenterBlocked</span></span>|<span data-ttu-id="86a3b-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-341">Boolean</span></span>|<span data-ttu-id="86a3b-342">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-342">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-343">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-343">hostPairingBlocked</span></span>|<span data-ttu-id="86a3b-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-344">Boolean</span></span>|<span data-ttu-id="86a3b-345">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-345">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-346">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-346">iBooksStoreBlocked</span></span>|<span data-ttu-id="86a3b-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-347">Boolean</span></span>|<span data-ttu-id="86a3b-348">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-348">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-349">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="86a3b-349">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="86a3b-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-350">Boolean</span></span>|<span data-ttu-id="86a3b-351">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="86a3b-351">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="86a3b-352">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="86a3b-352">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="86a3b-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-353">Boolean</span></span>|<span data-ttu-id="86a3b-354">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="86a3b-354">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="86a3b-355">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="86a3b-355">iCloudBlockBackup</span></span>|<span data-ttu-id="86a3b-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-356">Boolean</span></span>|<span data-ttu-id="86a3b-357">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="86a3b-357">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="86a3b-358">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="86a3b-358">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="86a3b-359">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="86a3b-359">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="86a3b-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-360">Boolean</span></span>|<span data-ttu-id="86a3b-361">Указывает, следует ли заблокировать синхронизацию документов iCloud. Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="86a3b-361">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="86a3b-362">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="86a3b-362">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="86a3b-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-363">Boolean</span></span>|<span data-ttu-id="86a3b-364">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="86a3b-364">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="86a3b-365">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="86a3b-365">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="86a3b-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-366">Boolean</span></span>|<span data-ttu-id="86a3b-367">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="86a3b-367">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="86a3b-368">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="86a3b-368">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="86a3b-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-369">Boolean</span></span>|<span data-ttu-id="86a3b-370">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="86a3b-370">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="86a3b-371">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="86a3b-371">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="86a3b-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-372">Boolean</span></span>|<span data-ttu-id="86a3b-373">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="86a3b-373">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="86a3b-374">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="86a3b-374">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="86a3b-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-375">Boolean</span></span>|<span data-ttu-id="86a3b-376">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="86a3b-376">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="86a3b-377">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="86a3b-377">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="86a3b-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-378">Boolean</span></span>|<span data-ttu-id="86a3b-379">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="86a3b-379">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="86a3b-380">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="86a3b-380">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="86a3b-381">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="86a3b-381">iTunesBlockMusicService</span></span>|<span data-ttu-id="86a3b-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-382">Boolean</span></span>|<span data-ttu-id="86a3b-383">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-383">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="86a3b-384">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="86a3b-384">iTunesBlockRadio</span></span>|<span data-ttu-id="86a3b-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-385">Boolean</span></span>|<span data-ttu-id="86a3b-386">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-386">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="86a3b-387">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="86a3b-387">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="86a3b-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-388">Boolean</span></span>|<span data-ttu-id="86a3b-389">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-389">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="86a3b-390">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="86a3b-390">keyboardBlockDictation</span></span>|<span data-ttu-id="86a3b-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-391">Boolean</span></span>|<span data-ttu-id="86a3b-392">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-392">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-393">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="86a3b-393">keyboardBlockPredictive</span></span>|<span data-ttu-id="86a3b-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-394">Boolean</span></span>|<span data-ttu-id="86a3b-395">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-395">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="86a3b-396">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="86a3b-396">keyboardBlockShortcuts</span></span>|<span data-ttu-id="86a3b-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-397">Boolean</span></span>|<span data-ttu-id="86a3b-398">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-398">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="86a3b-399">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="86a3b-399">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="86a3b-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-400">Boolean</span></span>|<span data-ttu-id="86a3b-401">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-401">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="86a3b-402">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="86a3b-402">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="86a3b-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-403">Boolean</span></span>|<span data-ttu-id="86a3b-404">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-404">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-405">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="86a3b-405">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="86a3b-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-406">Boolean</span></span>|<span data-ttu-id="86a3b-407">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-407">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-408">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="86a3b-408">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="86a3b-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-409">Boolean</span></span>|<span data-ttu-id="86a3b-410">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-410">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="86a3b-411">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="86a3b-411">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="86a3b-412">Вместо этого используйте Киоскмодеблоккаутолокк.</span><span class="sxs-lookup"><span data-stu-id="86a3b-412">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="86a3b-413">киоскмодеблоккаутолокк</span><span class="sxs-lookup"><span data-stu-id="86a3b-413">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="86a3b-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-414">Boolean</span></span>|<span data-ttu-id="86a3b-415">Указывает, следует ли блокировать автоматическую блокировку устройств в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-415">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-416">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="86a3b-416">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="86a3b-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-417">Boolean</span></span>|<span data-ttu-id="86a3b-418">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-418">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-419">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="86a3b-419">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="86a3b-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-420">Boolean</span></span>|<span data-ttu-id="86a3b-421">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-421">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="86a3b-422">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="86a3b-422">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="86a3b-423">Вместо этого используйте Киоскмодеблоккринжерсвитч.</span><span class="sxs-lookup"><span data-stu-id="86a3b-423">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="86a3b-424">киоскмодеблоккринжерсвитч</span><span class="sxs-lookup"><span data-stu-id="86a3b-424">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="86a3b-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-425">Boolean</span></span>|<span data-ttu-id="86a3b-426">Указывает, следует ли запретить использование переключателя звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-426">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-427">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="86a3b-427">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="86a3b-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-428">Boolean</span></span>|<span data-ttu-id="86a3b-429">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-429">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="86a3b-430">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="86a3b-430">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="86a3b-431">Вместо этого используйте Киоскмодеблоккскринротатион.</span><span class="sxs-lookup"><span data-stu-id="86a3b-431">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="86a3b-432">киоскмодеблоккскринротатион</span><span class="sxs-lookup"><span data-stu-id="86a3b-432">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="86a3b-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-433">Boolean</span></span>|<span data-ttu-id="86a3b-434">Указывает, следует ли блокировать поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-434">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-435">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="86a3b-435">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="86a3b-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-436">Boolean</span></span>|<span data-ttu-id="86a3b-437">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-437">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="86a3b-438">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="86a3b-438">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="86a3b-439">Вместо этого используйте Киоскмодеблоккслипбуттон.</span><span class="sxs-lookup"><span data-stu-id="86a3b-439">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="86a3b-440">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="86a3b-440">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="86a3b-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-441">Boolean</span></span>|<span data-ttu-id="86a3b-442">Указывает, следует ли запретить использование кнопки "сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-442">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-443">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="86a3b-443">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="86a3b-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-444">Boolean</span></span>|<span data-ttu-id="86a3b-445">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-445">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="86a3b-446">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="86a3b-446">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="86a3b-447">Вместо этого используйте Киоскмодеблокктаучскрин.</span><span class="sxs-lookup"><span data-stu-id="86a3b-447">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="86a3b-448">киоскмодеблокктаучскрин</span><span class="sxs-lookup"><span data-stu-id="86a3b-448">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="86a3b-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-449">Boolean</span></span>|<span data-ttu-id="86a3b-450">Указывает, следует ли запретить использование сенсорного экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-450">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-451">киоскмодинаблевоицеконтрол</span><span class="sxs-lookup"><span data-stu-id="86a3b-451">kioskModeEnableVoiceControl</span></span>|<span data-ttu-id="86a3b-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-452">Boolean</span></span>|<span data-ttu-id="86a3b-453">Указывает, следует ли включить управление голосовым режимом в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-453">Indicates whether or not to enable voice control in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-454">киоскмодеалловвоицеконтролмодификатион</span><span class="sxs-lookup"><span data-stu-id="86a3b-454">kioskModeAllowVoiceControlModification</span></span>|<span data-ttu-id="86a3b-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-455">Boolean</span></span>|<span data-ttu-id="86a3b-456">Указывает, следует ли запретить пользователю переключать управление голосовым режимом в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-456">Indicates whether or not to allow the user to toggle voice control in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-457">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="86a3b-457">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="86a3b-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-458">Boolean</span></span>|<span data-ttu-id="86a3b-459">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-459">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-460">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="86a3b-460">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="86a3b-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-461">Boolean</span></span>|<span data-ttu-id="86a3b-462">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-462">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="86a3b-463">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="86a3b-463">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="86a3b-464">Вместо этого используйте Киоскмодеблоккволумебуттонс.</span><span class="sxs-lookup"><span data-stu-id="86a3b-464">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="86a3b-465">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="86a3b-465">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="86a3b-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-466">Boolean</span></span>|<span data-ttu-id="86a3b-467">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="86a3b-467">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="86a3b-468">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="86a3b-468">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="86a3b-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-469">Boolean</span></span>|<span data-ttu-id="86a3b-470">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-470">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-471">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="86a3b-471">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="86a3b-472">Строка</span><span class="sxs-lookup"><span data-stu-id="86a3b-472">String</span></span>|<span data-ttu-id="86a3b-473">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-473">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="86a3b-474">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="86a3b-474">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="86a3b-475">киоскмодебуилтинаппид</span><span class="sxs-lookup"><span data-stu-id="86a3b-475">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="86a3b-476">Строка</span><span class="sxs-lookup"><span data-stu-id="86a3b-476">String</span></span>|<span data-ttu-id="86a3b-477">Идентификатор встроенных приложений для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-477">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="86a3b-478">Используется, когда KioskModeManagedAppId и KioskModeAppStoreUrl не заданы.</span><span class="sxs-lookup"><span data-stu-id="86a3b-478">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="86a3b-479">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="86a3b-479">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="86a3b-480">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-480">Boolean</span></span>|<span data-ttu-id="86a3b-481">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-481">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-482">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="86a3b-482">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="86a3b-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-483">Boolean</span></span>|<span data-ttu-id="86a3b-484">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-484">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-485">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="86a3b-485">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="86a3b-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-486">Boolean</span></span>|<span data-ttu-id="86a3b-487">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-487">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-488">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="86a3b-488">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="86a3b-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-489">Boolean</span></span>|<span data-ttu-id="86a3b-490">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-490">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-491">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="86a3b-491">kioskModeRequireZoom</span></span>|<span data-ttu-id="86a3b-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-492">Boolean</span></span>|<span data-ttu-id="86a3b-493">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-493">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="86a3b-494">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="86a3b-494">kioskModeManagedAppId</span></span>|<span data-ttu-id="86a3b-495">String</span><span class="sxs-lookup"><span data-stu-id="86a3b-495">String</span></span>|<span data-ttu-id="86a3b-496">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="86a3b-496">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="86a3b-497">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="86a3b-497">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="86a3b-498">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="86a3b-498">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="86a3b-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-499">Boolean</span></span>|<span data-ttu-id="86a3b-500">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="86a3b-500">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="86a3b-501">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="86a3b-501">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="86a3b-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-502">Boolean</span></span>|<span data-ttu-id="86a3b-503">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="86a3b-503">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="86a3b-504">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="86a3b-504">lockScreenBlockPassbook</span></span>|<span data-ttu-id="86a3b-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-505">Boolean</span></span>|<span data-ttu-id="86a3b-506">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="86a3b-506">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="86a3b-507">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="86a3b-507">lockScreenBlockTodayView</span></span>|<span data-ttu-id="86a3b-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-508">Boolean</span></span>|<span data-ttu-id="86a3b-509">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="86a3b-509">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="86a3b-510">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="86a3b-510">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="86a3b-511">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="86a3b-511">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="86a3b-512">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="86a3b-512">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="86a3b-513">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="86a3b-513">mediaContentRatingCanada</span></span>|[<span data-ttu-id="86a3b-514">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="86a3b-514">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="86a3b-515">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="86a3b-515">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="86a3b-516">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="86a3b-516">mediaContentRatingFrance</span></span>|[<span data-ttu-id="86a3b-517">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="86a3b-517">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="86a3b-518">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="86a3b-518">Media content rating settings for France</span></span>|
|<span data-ttu-id="86a3b-519">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="86a3b-519">mediaContentRatingGermany</span></span>|[<span data-ttu-id="86a3b-520">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="86a3b-520">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="86a3b-521">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="86a3b-521">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="86a3b-522">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="86a3b-522">mediaContentRatingIreland</span></span>|[<span data-ttu-id="86a3b-523">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="86a3b-523">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="86a3b-524">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="86a3b-524">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="86a3b-525">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="86a3b-525">mediaContentRatingJapan</span></span>|[<span data-ttu-id="86a3b-526">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="86a3b-526">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="86a3b-527">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="86a3b-527">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="86a3b-528">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="86a3b-528">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="86a3b-529">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="86a3b-529">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="86a3b-530">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="86a3b-530">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="86a3b-531">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="86a3b-531">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="86a3b-532">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="86a3b-532">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="86a3b-533">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="86a3b-533">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="86a3b-534">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="86a3b-534">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="86a3b-535">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="86a3b-535">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="86a3b-536">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="86a3b-536">Media content rating settings for United States</span></span>|
|<span data-ttu-id="86a3b-537">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="86a3b-537">networkUsageRules</span></span>|<span data-ttu-id="86a3b-538">Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="86a3b-538">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="86a3b-539">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="86a3b-539">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="86a3b-540">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="86a3b-540">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="86a3b-541">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="86a3b-541">mediaContentRatingApps</span></span>|[<span data-ttu-id="86a3b-542">ратингаппстипе</span><span class="sxs-lookup"><span data-stu-id="86a3b-542">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="86a3b-543">Параметры оценки контента мультимедиа для приложений.</span><span class="sxs-lookup"><span data-stu-id="86a3b-543">Media content rating settings for Apps.</span></span> <span data-ttu-id="86a3b-544">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="86a3b-544">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="86a3b-545">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-545">messagesBlocked</span></span>|<span data-ttu-id="86a3b-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-546">Boolean</span></span>|<span data-ttu-id="86a3b-547">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="86a3b-547">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="86a3b-548">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="86a3b-548">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="86a3b-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-549">Boolean</span></span>|<span data-ttu-id="86a3b-550">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-550">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="86a3b-551">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="86a3b-551">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="86a3b-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-552">Boolean</span></span>|<span data-ttu-id="86a3b-553">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="86a3b-553">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="86a3b-554">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="86a3b-554">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="86a3b-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-555">Boolean</span></span>|<span data-ttu-id="86a3b-556">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-556">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-557">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="86a3b-557">passcodeBlockModification</span></span>|<span data-ttu-id="86a3b-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-558">Boolean</span></span>|<span data-ttu-id="86a3b-559">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-559">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="86a3b-560">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="86a3b-560">passcodeBlockSimple</span></span>|<span data-ttu-id="86a3b-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-561">Boolean</span></span>|<span data-ttu-id="86a3b-562">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="86a3b-562">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="86a3b-563">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="86a3b-563">passcodeExpirationDays</span></span>|<span data-ttu-id="86a3b-564">Int32</span><span class="sxs-lookup"><span data-stu-id="86a3b-564">Int32</span></span>|<span data-ttu-id="86a3b-565">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="86a3b-565">Number of days before the passcode expires.</span></span> <span data-ttu-id="86a3b-566">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="86a3b-566">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="86a3b-567">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="86a3b-567">passcodeMinimumLength</span></span>|<span data-ttu-id="86a3b-568">Int32</span><span class="sxs-lookup"><span data-stu-id="86a3b-568">Int32</span></span>|<span data-ttu-id="86a3b-569">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="86a3b-569">Minimum length of passcode.</span></span> <span data-ttu-id="86a3b-570">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="86a3b-570">Valid values 4 to 14</span></span>|
|<span data-ttu-id="86a3b-571">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="86a3b-571">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="86a3b-572">Int32</span><span class="sxs-lookup"><span data-stu-id="86a3b-572">Int32</span></span>|<span data-ttu-id="86a3b-573">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="86a3b-573">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="86a3b-574">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="86a3b-574">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="86a3b-575">Int32</span><span class="sxs-lookup"><span data-stu-id="86a3b-575">Int32</span></span>|<span data-ttu-id="86a3b-576">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="86a3b-576">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="86a3b-577">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="86a3b-577">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="86a3b-578">Int32</span><span class="sxs-lookup"><span data-stu-id="86a3b-578">Int32</span></span>|<span data-ttu-id="86a3b-579">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="86a3b-579">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="86a3b-580">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="86a3b-580">Valid values 0 to 4</span></span>|
|<span data-ttu-id="86a3b-581">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="86a3b-581">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="86a3b-582">Int32</span><span class="sxs-lookup"><span data-stu-id="86a3b-582">Int32</span></span>|<span data-ttu-id="86a3b-583">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="86a3b-583">Number of previous passcodes to block.</span></span> <span data-ttu-id="86a3b-584">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="86a3b-584">Valid values 1 to 24</span></span>|
|<span data-ttu-id="86a3b-585">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="86a3b-585">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="86a3b-586">Int32</span><span class="sxs-lookup"><span data-stu-id="86a3b-586">Int32</span></span>|<span data-ttu-id="86a3b-587">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="86a3b-587">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="86a3b-588">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="86a3b-588">Valid values 4 to 11</span></span>|
|<span data-ttu-id="86a3b-589">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="86a3b-589">passcodeRequiredType</span></span>|[<span data-ttu-id="86a3b-590">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="86a3b-590">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="86a3b-591">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="86a3b-591">Type of passcode that is required.</span></span> <span data-ttu-id="86a3b-592">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="86a3b-592">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="86a3b-593">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="86a3b-593">passcodeRequired</span></span>|<span data-ttu-id="86a3b-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-594">Boolean</span></span>|<span data-ttu-id="86a3b-595">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="86a3b-595">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="86a3b-596">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-596">podcastsBlocked</span></span>|<span data-ttu-id="86a3b-597">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-597">Boolean</span></span>|<span data-ttu-id="86a3b-598">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-598">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="86a3b-599">проксимитиблокксетуптоневдевице</span><span class="sxs-lookup"><span data-stu-id="86a3b-599">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="86a3b-600">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-600">Boolean</span></span>|<span data-ttu-id="86a3b-601">Указывает, следует ли включить запрос на установку находящихся рядом устройств с защищенным устройством.</span><span class="sxs-lookup"><span data-stu-id="86a3b-601">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="86a3b-602">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="86a3b-602">safariBlockAutofill</span></span>|<span data-ttu-id="86a3b-603">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-603">Boolean</span></span>|<span data-ttu-id="86a3b-604">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="86a3b-604">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="86a3b-605">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="86a3b-605">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="86a3b-606">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="86a3b-606">safariBlockJavaScript</span></span>|<span data-ttu-id="86a3b-607">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-607">Boolean</span></span>|<span data-ttu-id="86a3b-608">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="86a3b-608">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="86a3b-609">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="86a3b-609">safariBlockPopups</span></span>|<span data-ttu-id="86a3b-610">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-610">Boolean</span></span>|<span data-ttu-id="86a3b-611">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="86a3b-611">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="86a3b-612">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-612">safariBlocked</span></span>|<span data-ttu-id="86a3b-613">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-613">Boolean</span></span>|<span data-ttu-id="86a3b-614">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="86a3b-614">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="86a3b-615">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="86a3b-615">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="86a3b-616">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="86a3b-616">safariCookieSettings</span></span>|[<span data-ttu-id="86a3b-617">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="86a3b-617">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="86a3b-618">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="86a3b-618">Cookie settings for Safari.</span></span> <span data-ttu-id="86a3b-619">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="86a3b-619">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="86a3b-620">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="86a3b-620">safariManagedDomains</span></span>|<span data-ttu-id="86a3b-621">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="86a3b-621">String collection</span></span>|<span data-ttu-id="86a3b-622">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="86a3b-622">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="86a3b-623">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="86a3b-623">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="86a3b-624">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="86a3b-624">String collection</span></span>|<span data-ttu-id="86a3b-625">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="86a3b-625">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="86a3b-626">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-626">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="86a3b-627">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="86a3b-627">safariRequireFraudWarning</span></span>|<span data-ttu-id="86a3b-628">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-628">Boolean</span></span>|<span data-ttu-id="86a3b-629">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="86a3b-629">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="86a3b-630">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-630">screenCaptureBlocked</span></span>|<span data-ttu-id="86a3b-631">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-631">Boolean</span></span>|<span data-ttu-id="86a3b-632">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="86a3b-632">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="86a3b-633">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-633">siriBlocked</span></span>|<span data-ttu-id="86a3b-634">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-634">Boolean</span></span>|<span data-ttu-id="86a3b-635">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="86a3b-635">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="86a3b-636">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-636">siriBlockedWhenLocked</span></span>|<span data-ttu-id="86a3b-637">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-637">Boolean</span></span>|<span data-ttu-id="86a3b-638">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="86a3b-638">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="86a3b-639">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="86a3b-639">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="86a3b-640">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-640">Boolean</span></span>|<span data-ttu-id="86a3b-641">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="86a3b-641">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="86a3b-642">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="86a3b-642">siriRequireProfanityFilter</span></span>|<span data-ttu-id="86a3b-643">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-643">Boolean</span></span>|<span data-ttu-id="86a3b-644">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="86a3b-644">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="86a3b-645">софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="86a3b-645">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="86a3b-646">Int32</span><span class="sxs-lookup"><span data-stu-id="86a3b-646">Int32</span></span>|<span data-ttu-id="86a3b-647">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="86a3b-647">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="86a3b-648">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="86a3b-648">Valid values 0 to 90</span></span>|
|<span data-ttu-id="86a3b-649">софтвареупдатесфорцеделайед</span><span class="sxs-lookup"><span data-stu-id="86a3b-649">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="86a3b-650">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-650">Boolean</span></span>|<span data-ttu-id="86a3b-651">Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-651">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-652">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="86a3b-652">spotlightBlockInternetResults</span></span>|<span data-ttu-id="86a3b-653">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-653">Boolean</span></span>|<span data-ttu-id="86a3b-654">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="86a3b-654">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="86a3b-655">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-655">voiceDialingBlocked</span></span>|<span data-ttu-id="86a3b-656">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-656">Boolean</span></span>|<span data-ttu-id="86a3b-657">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="86a3b-657">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="86a3b-658">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="86a3b-658">wallpaperBlockModification</span></span>|<span data-ttu-id="86a3b-659">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-659">Boolean</span></span>|<span data-ttu-id="86a3b-660">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-660">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="86a3b-661">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="86a3b-661">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="86a3b-662">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-662">Boolean</span></span>|<span data-ttu-id="86a3b-663">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="86a3b-663">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="86a3b-664">классрумфорцерекуестпермиссионтолеавеклассес</span><span class="sxs-lookup"><span data-stu-id="86a3b-664">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="86a3b-665">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-665">Boolean</span></span>|<span data-ttu-id="86a3b-666">Указывает, является ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса (iOS 11,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-666">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="86a3b-667">кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="86a3b-667">keychainBlockCloudSync</span></span>|<span data-ttu-id="86a3b-668">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-668">Boolean</span></span>|<span data-ttu-id="86a3b-669">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud.</span><span class="sxs-lookup"><span data-stu-id="86a3b-669">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="86a3b-670">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="86a3b-670">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="86a3b-671">пкиблоккотаупдатес</span><span class="sxs-lookup"><span data-stu-id="86a3b-671">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="86a3b-672">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-672">Boolean</span></span>|<span data-ttu-id="86a3b-673">Указывает, блокируются ли обновления PKI беспроводной сети.</span><span class="sxs-lookup"><span data-stu-id="86a3b-673">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="86a3b-674">Если задать для этого ограничения значение false, проверки CRL и OCSP (iOS 7,0 и более поздних версий) не отключаются.</span><span class="sxs-lookup"><span data-stu-id="86a3b-674">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="86a3b-675">привацифорцелимитадтраккинг</span><span class="sxs-lookup"><span data-stu-id="86a3b-675">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="86a3b-676">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-676">Boolean</span></span>|<span data-ttu-id="86a3b-677">Указывает, ограничено ли отслеживание AD. (iOS 7,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-677">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="86a3b-678">ентерприсебукблоккбаккуп</span><span class="sxs-lookup"><span data-stu-id="86a3b-678">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="86a3b-679">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-679">Boolean</span></span>|<span data-ttu-id="86a3b-680">Указывает, блокируется ли резервное копирование корпоративной книги.</span><span class="sxs-lookup"><span data-stu-id="86a3b-680">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="86a3b-681">ентерприсебукблоккметадатасинк</span><span class="sxs-lookup"><span data-stu-id="86a3b-681">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="86a3b-682">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-682">Boolean</span></span>|<span data-ttu-id="86a3b-683">Указывает, блокируется ли синхронизация заметок и выделений корпоративных книг.</span><span class="sxs-lookup"><span data-stu-id="86a3b-683">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="86a3b-684">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="86a3b-684">airPrintBlocked</span></span>|<span data-ttu-id="86a3b-685">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-685">Boolean</span></span>|<span data-ttu-id="86a3b-686">Указывает, заблокировано ли Аирпринт (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-686">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="86a3b-687">аирпринтблокккредентиалсстораже</span><span class="sxs-lookup"><span data-stu-id="86a3b-687">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="86a3b-688">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-688">Boolean</span></span>|<span data-ttu-id="86a3b-689">Указывает, заблокировано ли хранение цепочки ключей имени пользователя и пароля для Аирпринт (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-689">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="86a3b-690">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="86a3b-690">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="86a3b-691">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-691">Boolean</span></span>|<span data-ttu-id="86a3b-692">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-692">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="86a3b-693">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="86a3b-693">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="86a3b-694">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-694">Boolean</span></span>|<span data-ttu-id="86a3b-695">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="86a3b-695">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="86a3b-696">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-696">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="86a3b-697">филеснетворкдривеакцессблоккед</span><span class="sxs-lookup"><span data-stu-id="86a3b-697">filesNetworkDriveAccessBlocked</span></span>|<span data-ttu-id="86a3b-698">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-698">Boolean</span></span>|<span data-ttu-id="86a3b-699">Указывает, могут ли устройства получать доступ к файлам или другим ресурсам на сетевом сервере с помощью протокола SMB.</span><span class="sxs-lookup"><span data-stu-id="86a3b-699">Indicates if devices can access files or other resources on a network server using the Server Message Block (SMB) protocol.</span></span> <span data-ttu-id="86a3b-700">Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="86a3b-700">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="86a3b-701">филесусбдривеакцессблоккед</span><span class="sxs-lookup"><span data-stu-id="86a3b-701">filesUsbDriveAccessBlocked</span></span>|<span data-ttu-id="86a3b-702">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-702">Boolean</span></span>|<span data-ttu-id="86a3b-703">Указывает, могут ли севицес с Access подключаться к файлам и открывать их на USB-диске.</span><span class="sxs-lookup"><span data-stu-id="86a3b-703">Indicates if sevices with access can connect to and open files on a USB drive.</span></span> <span data-ttu-id="86a3b-704">Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="86a3b-704">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="86a3b-705">вифиповеронфорцед</span><span class="sxs-lookup"><span data-stu-id="86a3b-705">wifiPowerOnForced</span></span>|<span data-ttu-id="86a3b-706">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-706">Boolean</span></span>|<span data-ttu-id="86a3b-707">Указывает, остается ли Wi-Fi On, даже если устройство находится в режиме "в самолете".</span><span class="sxs-lookup"><span data-stu-id="86a3b-707">Indicates whether or not Wi-Fi remains on, even when device is in airplane mode.</span></span> <span data-ttu-id="86a3b-708">Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="86a3b-708">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="86a3b-709">блокксистемаппремовал</span><span class="sxs-lookup"><span data-stu-id="86a3b-709">blockSystemAppRemoval</span></span>|<span data-ttu-id="86a3b-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-710">Boolean</span></span>|<span data-ttu-id="86a3b-711">Указывает, заблокировано ли удаление системных приложений с устройства на контролируемом устройстве (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-711">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="86a3b-712">впнблокккреатион</span><span class="sxs-lookup"><span data-stu-id="86a3b-712">vpnBlockCreation</span></span>|<span data-ttu-id="86a3b-713">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-713">Boolean</span></span>|<span data-ttu-id="86a3b-714">Указывает, блокируется ли создание конфигураций VPN (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-714">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="86a3b-715">аппремовалблоккед</span><span class="sxs-lookup"><span data-stu-id="86a3b-715">appRemovalBlocked</span></span>|<span data-ttu-id="86a3b-716">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-716">Boolean</span></span>|<span data-ttu-id="86a3b-717">Указывает, разрешено ли удаление приложений.</span><span class="sxs-lookup"><span data-stu-id="86a3b-717">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="86a3b-718">усбрестриктедмодеблоккед</span><span class="sxs-lookup"><span data-stu-id="86a3b-718">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="86a3b-719">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-719">Boolean</span></span>|<span data-ttu-id="86a3b-720">Указывает, разрешена ли подключаться к стандарту USB, пока устройство заблокировано (iOS 11.4.1 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-720">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="86a3b-721">пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="86a3b-721">passwordBlockAutoFill</span></span>|<span data-ttu-id="86a3b-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-722">Boolean</span></span>|<span data-ttu-id="86a3b-723">Указывает, разрешена ли функция автозаполнения паролей (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-723">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="86a3b-724">пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="86a3b-724">passwordBlockProximityRequests</span></span>|<span data-ttu-id="86a3b-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-725">Boolean</span></span>|<span data-ttu-id="86a3b-726">Указывает, следует ли запретить запрашивать пароли с близлежащих устройств (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-726">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="86a3b-727">пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="86a3b-727">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="86a3b-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-728">Boolean</span></span>|<span data-ttu-id="86a3b-729">Указывает, следует ли заблокировать общий доступ к паролям с помощью AirDrop паролей iOS 12,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="86a3b-729">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="86a3b-730">датеандтимефорцесетаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="86a3b-730">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="86a3b-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-731">Boolean</span></span>|<span data-ttu-id="86a3b-732">Указывает, включена ли функция даты и времени "автоматически задано" и не может быть отключена пользователем (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-732">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="86a3b-733">контактсалловманажедтаунманажедврите</span><span class="sxs-lookup"><span data-stu-id="86a3b-733">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="86a3b-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-734">Boolean</span></span>|<span data-ttu-id="86a3b-735">Указывает, могут ли управляемые приложения записывать контакты в неуправляемые учетные записи контактов (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="86a3b-735">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="86a3b-736">контактсалловунманажедтоманажедреад</span><span class="sxs-lookup"><span data-stu-id="86a3b-736">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="86a3b-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-737">Boolean</span></span>|<span data-ttu-id="86a3b-738">Указывает, могут ли неуправляемые приложения читать из управляемых учетных записей контактов (iOS 12,0 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="86a3b-738">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="86a3b-739">целлуларблоккперсоналхотспотмодификатион</span><span class="sxs-lookup"><span data-stu-id="86a3b-739">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="86a3b-740">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-740">Boolean</span></span>|<span data-ttu-id="86a3b-741">Указывает, следует ли запретить пользователю изменять параметр личных гиперобъектов (iOS 12,2 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="86a3b-741">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="86a3b-742">континуауспаскэйбоардблоккед</span><span class="sxs-lookup"><span data-stu-id="86a3b-742">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="86a3b-743">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-743">Boolean</span></span>|<span data-ttu-id="86a3b-744">Указывает, следует ли заблокировать клавиатуру непрерывного пути, когда устройство защищено (iOS 13 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="86a3b-744">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="86a3b-745">финдмидевицеинфиндмяппблоккед</span><span class="sxs-lookup"><span data-stu-id="86a3b-745">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="86a3b-746">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-746">Boolean</span></span>|<span data-ttu-id="86a3b-747">Указывает, следует ли заблокировать Поиск устройства, когда устройство защищено (iOS 13 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="86a3b-747">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="86a3b-748">финдмифриендсинфиндмяппблоккед</span><span class="sxs-lookup"><span data-stu-id="86a3b-748">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="86a3b-749">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-749">Boolean</span></span>|<span data-ttu-id="86a3b-750">Указывает, следует ли заблокировать "найти друзей", когда устройство защищено (iOS 13 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="86a3b-750">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="86a3b-751">итунесблоккед</span><span class="sxs-lookup"><span data-stu-id="86a3b-751">iTunesBlocked</span></span>|<span data-ttu-id="86a3b-752">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a3b-752">Boolean</span></span>|<span data-ttu-id="86a3b-753">Указывает, следует ли заблокировать приложение iTunes.</span><span class="sxs-lookup"><span data-stu-id="86a3b-753">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="86a3b-754">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="86a3b-754">Requires a supervised device for iOS 13 and later.</span></span>|



## <a name="response"></a><span data-ttu-id="86a3b-755">Ответ</span><span class="sxs-lookup"><span data-stu-id="86a3b-755">Response</span></span>
<span data-ttu-id="86a3b-756">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="86a3b-756">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86a3b-757">Пример</span><span class="sxs-lookup"><span data-stu-id="86a3b-757">Example</span></span>

### <a name="request"></a><span data-ttu-id="86a3b-758">Запрос</span><span class="sxs-lookup"><span data-stu-id="86a3b-758">Request</span></span>
<span data-ttu-id="86a3b-759">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86a3b-759">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10480

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
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="86a3b-760">Отклик</span><span class="sxs-lookup"><span data-stu-id="86a3b-760">Response</span></span>
<span data-ttu-id="86a3b-p156">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86a3b-p156">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10652

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
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "iTunesBlocked": true
}
```





