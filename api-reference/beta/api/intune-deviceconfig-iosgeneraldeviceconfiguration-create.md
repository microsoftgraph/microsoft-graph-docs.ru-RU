---
title: Create iosGeneralDeviceConfiguration
description: Создание объекта iosGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4eec23b3c57aba6ebca97f8c90722a3b2d519e66
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635946"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="a5c48-103">Create iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a5c48-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="a5c48-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5c48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5c48-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5c48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5c48-106">Создание объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5c48-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5c48-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a5c48-107">Prerequisites</span></span>
<span data-ttu-id="a5c48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5c48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5c48-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5c48-110">Permission type</span></span>|<span data-ttu-id="a5c48-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5c48-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5c48-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5c48-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5c48-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5c48-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5c48-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5c48-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5c48-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5c48-115">Not supported.</span></span>|
|<span data-ttu-id="a5c48-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5c48-116">Application</span></span>|<span data-ttu-id="a5c48-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5c48-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5c48-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5c48-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a5c48-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a5c48-119">Request headers</span></span>
|<span data-ttu-id="a5c48-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5c48-120">Header</span></span>|<span data-ttu-id="a5c48-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a5c48-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5c48-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5c48-122">Authorization</span></span>|<span data-ttu-id="a5c48-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5c48-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5c48-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a5c48-124">Accept</span></span>|<span data-ttu-id="a5c48-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5c48-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5c48-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5c48-126">Request body</span></span>
<span data-ttu-id="a5c48-127">В теле запроса добавьте представление объекта iosGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5c48-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="a5c48-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a5c48-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="a5c48-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5c48-129">Property</span></span>|<span data-ttu-id="a5c48-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a5c48-130">Type</span></span>|<span data-ttu-id="a5c48-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a5c48-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5c48-132">id</span><span class="sxs-lookup"><span data-stu-id="a5c48-132">id</span></span>|<span data-ttu-id="a5c48-133">String</span><span class="sxs-lookup"><span data-stu-id="a5c48-133">String</span></span>|<span data-ttu-id="a5c48-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a5c48-134">Key of the entity.</span></span> <span data-ttu-id="a5c48-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5c48-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c48-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5c48-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a5c48-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5c48-137">DateTimeOffset</span></span>|<span data-ttu-id="a5c48-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a5c48-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a5c48-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5c48-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c48-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a5c48-140">roleScopeTagIds</span></span>|<span data-ttu-id="a5c48-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a5c48-141">String collection</span></span>|<span data-ttu-id="a5c48-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a5c48-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a5c48-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5c48-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c48-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a5c48-144">supportsScopeTags</span></span>|<span data-ttu-id="a5c48-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-145">Boolean</span></span>|<span data-ttu-id="a5c48-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a5c48-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a5c48-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a5c48-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a5c48-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a5c48-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a5c48-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a5c48-149">This property is read-only.</span></span> <span data-ttu-id="a5c48-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5c48-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c48-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a5c48-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a5c48-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a5c48-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a5c48-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a5c48-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a5c48-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5c48-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c48-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a5c48-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a5c48-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a5c48-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a5c48-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a5c48-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a5c48-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5c48-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c48-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a5c48-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a5c48-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a5c48-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a5c48-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a5c48-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a5c48-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5c48-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c48-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5c48-163">createdDateTime</span></span>|<span data-ttu-id="a5c48-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5c48-164">DateTimeOffset</span></span>|<span data-ttu-id="a5c48-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a5c48-165">DateTime the object was created.</span></span> <span data-ttu-id="a5c48-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5c48-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c48-167">description</span><span class="sxs-lookup"><span data-stu-id="a5c48-167">description</span></span>|<span data-ttu-id="a5c48-168">String</span><span class="sxs-lookup"><span data-stu-id="a5c48-168">String</span></span>|<span data-ttu-id="a5c48-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a5c48-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a5c48-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5c48-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c48-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a5c48-171">displayName</span></span>|<span data-ttu-id="a5c48-172">Строка</span><span class="sxs-lookup"><span data-stu-id="a5c48-172">String</span></span>|<span data-ttu-id="a5c48-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a5c48-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a5c48-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5c48-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c48-175">version</span><span class="sxs-lookup"><span data-stu-id="a5c48-175">version</span></span>|<span data-ttu-id="a5c48-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a5c48-176">Int32</span></span>|<span data-ttu-id="a5c48-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a5c48-177">Version of the device configuration.</span></span> <span data-ttu-id="a5c48-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a5c48-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5c48-179">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="a5c48-179">accountBlockModification</span></span>|<span data-ttu-id="a5c48-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-180">Boolean</span></span>|<span data-ttu-id="a5c48-181">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-181">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-182">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="a5c48-182">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="a5c48-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-183">Boolean</span></span>|<span data-ttu-id="a5c48-184">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-184">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="a5c48-185">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-185">airDropBlocked</span></span>|<span data-ttu-id="a5c48-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-186">Boolean</span></span>|<span data-ttu-id="a5c48-187">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-187">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-188">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="a5c48-188">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="a5c48-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-189">Boolean</span></span>|<span data-ttu-id="a5c48-190">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-190">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5c48-191">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="a5c48-191">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="a5c48-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-192">Boolean</span></span>|<span data-ttu-id="a5c48-193">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="a5c48-193">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="a5c48-194">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="a5c48-194">appleWatchBlockPairing</span></span>|<span data-ttu-id="a5c48-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-195">Boolean</span></span>|<span data-ttu-id="a5c48-196">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-196">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5c48-197">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="a5c48-197">appleWatchForceWristDetection</span></span>|<span data-ttu-id="a5c48-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-198">Boolean</span></span>|<span data-ttu-id="a5c48-199">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-199">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="a5c48-200">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-200">appleNewsBlocked</span></span>|<span data-ttu-id="a5c48-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-201">Boolean</span></span>|<span data-ttu-id="a5c48-202">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-202">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5c48-203">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="a5c48-203">appsSingleAppModeList</span></span>|<span data-ttu-id="a5c48-204">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="a5c48-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a5c48-205">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="a5c48-205">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="a5c48-206">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-206">Supervised only.</span></span> <span data-ttu-id="a5c48-207">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="a5c48-207">iOS 7.0 and later.</span></span> <span data-ttu-id="a5c48-208">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a5c48-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a5c48-209">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="a5c48-209">appsVisibilityList</span></span>|<span data-ttu-id="a5c48-210">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="a5c48-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a5c48-211">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-211">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="a5c48-212">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="a5c48-212">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="a5c48-213">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="a5c48-213">appsVisibilityListType</span></span>|[<span data-ttu-id="a5c48-214">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="a5c48-214">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="a5c48-215">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="a5c48-215">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="a5c48-216">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="a5c48-216">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="a5c48-217">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="a5c48-217">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="a5c48-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-218">Boolean</span></span>|<span data-ttu-id="a5c48-219">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-219">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5c48-220">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-220">appStoreBlocked</span></span>|<span data-ttu-id="a5c48-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-221">Boolean</span></span>|<span data-ttu-id="a5c48-222">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="a5c48-222">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="a5c48-223">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="a5c48-223">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="a5c48-224">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="a5c48-224">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="a5c48-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-225">Boolean</span></span>|<span data-ttu-id="a5c48-226">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="a5c48-226">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="a5c48-227">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="a5c48-227">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="a5c48-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-228">Boolean</span></span>|<span data-ttu-id="a5c48-229">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="a5c48-229">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="a5c48-230">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-230">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5c48-231">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="a5c48-231">appStoreRequirePassword</span></span>|<span data-ttu-id="a5c48-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-232">Boolean</span></span>|<span data-ttu-id="a5c48-233">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="a5c48-233">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="a5c48-234">аутофиллфорцеаусентикатион</span><span class="sxs-lookup"><span data-stu-id="a5c48-234">autoFillForceAuthentication</span></span>|<span data-ttu-id="a5c48-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-235">Boolean</span></span>|<span data-ttu-id="a5c48-236">Указывает, следует ли принудительно выполнять проверку подлинности пользователей перед автозаполнением паролей и сведений о кредитных картах в Safari и других приложениях на контролируемых устройствах.</span><span class="sxs-lookup"><span data-stu-id="a5c48-236">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="a5c48-237">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="a5c48-237">bluetoothBlockModification</span></span>|<span data-ttu-id="a5c48-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-238">Boolean</span></span>|<span data-ttu-id="a5c48-239">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-239">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="a5c48-240">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-240">cameraBlocked</span></span>|<span data-ttu-id="a5c48-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-241">Boolean</span></span>|<span data-ttu-id="a5c48-242">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="a5c48-242">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="a5c48-243">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="a5c48-243">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="a5c48-244">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="a5c48-244">cellularBlockDataRoaming</span></span>|<span data-ttu-id="a5c48-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-245">Boolean</span></span>|<span data-ttu-id="a5c48-246">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="a5c48-246">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="a5c48-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="a5c48-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="a5c48-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-248">Boolean</span></span>|<span data-ttu-id="a5c48-249">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="a5c48-249">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="a5c48-250">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="a5c48-250">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="a5c48-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-251">Boolean</span></span>|<span data-ttu-id="a5c48-252">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-252">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-253">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="a5c48-253">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="a5c48-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-254">Boolean</span></span>|<span data-ttu-id="a5c48-255">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="a5c48-255">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="a5c48-256">целлуларблоккпланмодификатион</span><span class="sxs-lookup"><span data-stu-id="a5c48-256">cellularBlockPlanModification</span></span>|<span data-ttu-id="a5c48-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-257">Boolean</span></span>|<span data-ttu-id="a5c48-258">Указывает, следует ли запретить пользователям изменять параметры плана сотовой связи на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="a5c48-258">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="a5c48-259">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="a5c48-259">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="a5c48-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-260">Boolean</span></span>|<span data-ttu-id="a5c48-261">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="a5c48-261">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="a5c48-262">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="a5c48-262">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="a5c48-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-263">Boolean</span></span>|<span data-ttu-id="a5c48-264">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="a5c48-264">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="a5c48-265">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="a5c48-265">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="a5c48-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-266">Boolean</span></span>|<span data-ttu-id="a5c48-267">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-267">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="a5c48-268">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="a5c48-268">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="a5c48-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-269">Boolean</span></span>|<span data-ttu-id="a5c48-270">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-270">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-271">классрумфорцеаутоматикаллижоинклассес</span><span class="sxs-lookup"><span data-stu-id="a5c48-271">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="a5c48-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-272">Boolean</span></span>|<span data-ttu-id="a5c48-273">Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-273">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-274">классрумфорцеунпромптедаппанддевицелокк</span><span class="sxs-lookup"><span data-stu-id="a5c48-274">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="a5c48-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-275">Boolean</span></span>|<span data-ttu-id="a5c48-276">Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся.</span><span class="sxs-lookup"><span data-stu-id="a5c48-276">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="a5c48-277">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-277">Supervised only.</span></span>|
|<span data-ttu-id="a5c48-278">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="a5c48-278">compliantAppsList</span></span>|<span data-ttu-id="a5c48-279">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="a5c48-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a5c48-280">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="a5c48-280">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="a5c48-281">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="a5c48-281">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="a5c48-282">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="a5c48-282">compliantAppListType</span></span>|[<span data-ttu-id="a5c48-283">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="a5c48-283">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="a5c48-284">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="a5c48-284">List that is in the AppComplianceList.</span></span> <span data-ttu-id="a5c48-285">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="a5c48-285">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="a5c48-286">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="a5c48-286">configurationProfileBlockChanges</span></span>|<span data-ttu-id="a5c48-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-287">Boolean</span></span>|<span data-ttu-id="a5c48-288">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-288">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-289">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-289">definitionLookupBlocked</span></span>|<span data-ttu-id="a5c48-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-290">Boolean</span></span>|<span data-ttu-id="a5c48-291">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-291">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="a5c48-292">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="a5c48-292">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="a5c48-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-293">Boolean</span></span>|<span data-ttu-id="a5c48-294">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-294">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-295">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="a5c48-295">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="a5c48-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-296">Boolean</span></span>|<span data-ttu-id="a5c48-297">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-297">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-298">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="a5c48-298">deviceBlockNameModification</span></span>|<span data-ttu-id="a5c48-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-299">Boolean</span></span>|<span data-ttu-id="a5c48-300">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-300">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5c48-301">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="a5c48-301">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="a5c48-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-302">Boolean</span></span>|<span data-ttu-id="a5c48-303">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="a5c48-303">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="a5c48-304">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="a5c48-304">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="a5c48-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-305">Boolean</span></span>|<span data-ttu-id="a5c48-306">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-306">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="a5c48-307">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="a5c48-307">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="a5c48-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-308">Boolean</span></span>|<span data-ttu-id="a5c48-309">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="a5c48-309">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="a5c48-310">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="a5c48-310">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="a5c48-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-311">Boolean</span></span>|<span data-ttu-id="a5c48-312">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="a5c48-312">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="a5c48-313">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="a5c48-313">emailInDomainSuffixes</span></span>|<span data-ttu-id="a5c48-314">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a5c48-314">String collection</span></span>|<span data-ttu-id="a5c48-315">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="a5c48-315">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="a5c48-316">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="a5c48-316">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="a5c48-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-317">Boolean</span></span>|<span data-ttu-id="a5c48-318">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="a5c48-318">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="a5c48-319">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="a5c48-319">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="a5c48-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-320">Boolean</span></span>|<span data-ttu-id="a5c48-321">Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="a5c48-321">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="a5c48-322">есимблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="a5c48-322">esimBlockModification</span></span>|<span data-ttu-id="a5c48-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-323">Boolean</span></span>|<span data-ttu-id="a5c48-324">Указывает, следует ли разрешить добавление или удаление планов сотовой связи на eSIM контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="a5c48-324">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="a5c48-325">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-325">faceTimeBlocked</span></span>|<span data-ttu-id="a5c48-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-326">Boolean</span></span>|<span data-ttu-id="a5c48-327">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="a5c48-327">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="a5c48-328">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="a5c48-328">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="a5c48-329">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-329">findMyFriendsBlocked</span></span>|<span data-ttu-id="a5c48-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-330">Boolean</span></span>|<span data-ttu-id="a5c48-331">Указывает, следует ли заблокировать изменения для поиска друзей, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-331">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-332">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="a5c48-332">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="a5c48-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-333">Boolean</span></span>|<span data-ttu-id="a5c48-334">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="a5c48-334">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="a5c48-335">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="a5c48-335">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="a5c48-336">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="a5c48-336">gamingBlockMultiplayer</span></span>|<span data-ttu-id="a5c48-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-337">Boolean</span></span>|<span data-ttu-id="a5c48-338">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="a5c48-338">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="a5c48-339">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="a5c48-339">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="a5c48-340">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-340">gameCenterBlocked</span></span>|<span data-ttu-id="a5c48-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-341">Boolean</span></span>|<span data-ttu-id="a5c48-342">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-342">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-343">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-343">hostPairingBlocked</span></span>|<span data-ttu-id="a5c48-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-344">Boolean</span></span>|<span data-ttu-id="a5c48-345">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-345">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-346">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-346">iBooksStoreBlocked</span></span>|<span data-ttu-id="a5c48-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-347">Boolean</span></span>|<span data-ttu-id="a5c48-348">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-348">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-349">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="a5c48-349">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="a5c48-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-350">Boolean</span></span>|<span data-ttu-id="a5c48-351">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="a5c48-351">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="a5c48-352">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="a5c48-352">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="a5c48-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-353">Boolean</span></span>|<span data-ttu-id="a5c48-354">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="a5c48-354">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="a5c48-355">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="a5c48-355">iCloudBlockBackup</span></span>|<span data-ttu-id="a5c48-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-356">Boolean</span></span>|<span data-ttu-id="a5c48-357">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="a5c48-357">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="a5c48-358">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="a5c48-358">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="a5c48-359">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="a5c48-359">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="a5c48-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-360">Boolean</span></span>|<span data-ttu-id="a5c48-361">Указывает, следует ли заблокировать синхронизацию документов iCloud. Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="a5c48-361">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="a5c48-362">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="a5c48-362">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="a5c48-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-363">Boolean</span></span>|<span data-ttu-id="a5c48-364">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="a5c48-364">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="a5c48-365">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="a5c48-365">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="a5c48-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-366">Boolean</span></span>|<span data-ttu-id="a5c48-367">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="a5c48-367">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="a5c48-368">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="a5c48-368">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="a5c48-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-369">Boolean</span></span>|<span data-ttu-id="a5c48-370">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="a5c48-370">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="a5c48-371">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="a5c48-371">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="a5c48-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-372">Boolean</span></span>|<span data-ttu-id="a5c48-373">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="a5c48-373">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="a5c48-374">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="a5c48-374">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="a5c48-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-375">Boolean</span></span>|<span data-ttu-id="a5c48-376">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="a5c48-376">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="a5c48-377">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="a5c48-377">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="a5c48-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-378">Boolean</span></span>|<span data-ttu-id="a5c48-379">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="a5c48-379">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="a5c48-380">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="a5c48-380">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="a5c48-381">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="a5c48-381">iTunesBlockMusicService</span></span>|<span data-ttu-id="a5c48-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-382">Boolean</span></span>|<span data-ttu-id="a5c48-383">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-383">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="a5c48-384">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="a5c48-384">iTunesBlockRadio</span></span>|<span data-ttu-id="a5c48-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-385">Boolean</span></span>|<span data-ttu-id="a5c48-386">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-386">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="a5c48-387">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="a5c48-387">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="a5c48-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-388">Boolean</span></span>|<span data-ttu-id="a5c48-389">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-389">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="a5c48-390">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="a5c48-390">keyboardBlockDictation</span></span>|<span data-ttu-id="a5c48-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-391">Boolean</span></span>|<span data-ttu-id="a5c48-392">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-392">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-393">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="a5c48-393">keyboardBlockPredictive</span></span>|<span data-ttu-id="a5c48-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-394">Boolean</span></span>|<span data-ttu-id="a5c48-395">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-395">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="a5c48-396">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="a5c48-396">keyboardBlockShortcuts</span></span>|<span data-ttu-id="a5c48-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-397">Boolean</span></span>|<span data-ttu-id="a5c48-398">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-398">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5c48-399">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="a5c48-399">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="a5c48-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-400">Boolean</span></span>|<span data-ttu-id="a5c48-401">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-401">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="a5c48-402">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="a5c48-402">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="a5c48-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-403">Boolean</span></span>|<span data-ttu-id="a5c48-404">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-404">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-405">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="a5c48-405">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="a5c48-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-406">Boolean</span></span>|<span data-ttu-id="a5c48-407">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-407">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-408">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="a5c48-408">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="a5c48-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-409">Boolean</span></span>|<span data-ttu-id="a5c48-410">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-410">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="a5c48-411">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="a5c48-411">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="a5c48-412">Вместо этого используйте Киоскмодеблоккаутолокк.</span><span class="sxs-lookup"><span data-stu-id="a5c48-412">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="a5c48-413">киоскмодеблоккаутолокк</span><span class="sxs-lookup"><span data-stu-id="a5c48-413">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="a5c48-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-414">Boolean</span></span>|<span data-ttu-id="a5c48-415">Указывает, следует ли блокировать автоматическую блокировку устройств в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-415">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-416">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="a5c48-416">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="a5c48-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-417">Boolean</span></span>|<span data-ttu-id="a5c48-418">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-418">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-419">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="a5c48-419">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="a5c48-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-420">Boolean</span></span>|<span data-ttu-id="a5c48-421">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-421">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="a5c48-422">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="a5c48-422">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="a5c48-423">Вместо этого используйте Киоскмодеблоккринжерсвитч.</span><span class="sxs-lookup"><span data-stu-id="a5c48-423">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="a5c48-424">киоскмодеблоккринжерсвитч</span><span class="sxs-lookup"><span data-stu-id="a5c48-424">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="a5c48-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-425">Boolean</span></span>|<span data-ttu-id="a5c48-426">Указывает, следует ли запретить использование переключателя звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-426">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-427">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="a5c48-427">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="a5c48-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-428">Boolean</span></span>|<span data-ttu-id="a5c48-429">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-429">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="a5c48-430">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="a5c48-430">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="a5c48-431">Вместо этого используйте Киоскмодеблоккскринротатион.</span><span class="sxs-lookup"><span data-stu-id="a5c48-431">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="a5c48-432">киоскмодеблоккскринротатион</span><span class="sxs-lookup"><span data-stu-id="a5c48-432">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="a5c48-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-433">Boolean</span></span>|<span data-ttu-id="a5c48-434">Указывает, следует ли блокировать поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-434">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-435">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="a5c48-435">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="a5c48-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-436">Boolean</span></span>|<span data-ttu-id="a5c48-437">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-437">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="a5c48-438">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="a5c48-438">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="a5c48-439">Вместо этого используйте Киоскмодеблоккслипбуттон.</span><span class="sxs-lookup"><span data-stu-id="a5c48-439">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="a5c48-440">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="a5c48-440">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="a5c48-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-441">Boolean</span></span>|<span data-ttu-id="a5c48-442">Указывает, следует ли запретить использование кнопки "сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-442">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-443">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="a5c48-443">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="a5c48-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-444">Boolean</span></span>|<span data-ttu-id="a5c48-445">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-445">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="a5c48-446">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="a5c48-446">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="a5c48-447">Вместо этого используйте Киоскмодеблокктаучскрин.</span><span class="sxs-lookup"><span data-stu-id="a5c48-447">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="a5c48-448">киоскмодеблокктаучскрин</span><span class="sxs-lookup"><span data-stu-id="a5c48-448">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="a5c48-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-449">Boolean</span></span>|<span data-ttu-id="a5c48-450">Указывает, следует ли запретить использование сенсорного экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-450">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-451">киоскмодинаблевоицеконтрол</span><span class="sxs-lookup"><span data-stu-id="a5c48-451">kioskModeEnableVoiceControl</span></span>|<span data-ttu-id="a5c48-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-452">Boolean</span></span>|<span data-ttu-id="a5c48-453">Указывает, следует ли включить управление голосовым режимом в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-453">Indicates whether or not to enable voice control in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-454">киоскмодеалловвоицеконтролмодификатион</span><span class="sxs-lookup"><span data-stu-id="a5c48-454">kioskModeAllowVoiceControlModification</span></span>|<span data-ttu-id="a5c48-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-455">Boolean</span></span>|<span data-ttu-id="a5c48-456">Указывает, следует ли запретить пользователю переключать управление голосовым режимом в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-456">Indicates whether or not to allow the user to toggle voice control in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-457">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="a5c48-457">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="a5c48-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-458">Boolean</span></span>|<span data-ttu-id="a5c48-459">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-459">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-460">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="a5c48-460">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="a5c48-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-461">Boolean</span></span>|<span data-ttu-id="a5c48-462">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-462">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="a5c48-463">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="a5c48-463">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="a5c48-464">Вместо этого используйте Киоскмодеблоккволумебуттонс.</span><span class="sxs-lookup"><span data-stu-id="a5c48-464">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="a5c48-465">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="a5c48-465">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="a5c48-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-466">Boolean</span></span>|<span data-ttu-id="a5c48-467">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="a5c48-467">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="a5c48-468">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="a5c48-468">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="a5c48-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-469">Boolean</span></span>|<span data-ttu-id="a5c48-470">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-470">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-471">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a5c48-471">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="a5c48-472">Строка</span><span class="sxs-lookup"><span data-stu-id="a5c48-472">String</span></span>|<span data-ttu-id="a5c48-473">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-473">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="a5c48-474">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="a5c48-474">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="a5c48-475">киоскмодебуилтинаппид</span><span class="sxs-lookup"><span data-stu-id="a5c48-475">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="a5c48-476">Строка</span><span class="sxs-lookup"><span data-stu-id="a5c48-476">String</span></span>|<span data-ttu-id="a5c48-477">Идентификатор встроенных приложений для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-477">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="a5c48-478">Используется, когда KioskModeManagedAppId и KioskModeAppStoreUrl не заданы.</span><span class="sxs-lookup"><span data-stu-id="a5c48-478">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="a5c48-479">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="a5c48-479">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="a5c48-480">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-480">Boolean</span></span>|<span data-ttu-id="a5c48-481">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-481">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-482">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="a5c48-482">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="a5c48-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-483">Boolean</span></span>|<span data-ttu-id="a5c48-484">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-484">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-485">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="a5c48-485">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="a5c48-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-486">Boolean</span></span>|<span data-ttu-id="a5c48-487">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-487">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-488">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="a5c48-488">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="a5c48-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-489">Boolean</span></span>|<span data-ttu-id="a5c48-490">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-490">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-491">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="a5c48-491">kioskModeRequireZoom</span></span>|<span data-ttu-id="a5c48-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-492">Boolean</span></span>|<span data-ttu-id="a5c48-493">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-493">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="a5c48-494">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="a5c48-494">kioskModeManagedAppId</span></span>|<span data-ttu-id="a5c48-495">String</span><span class="sxs-lookup"><span data-stu-id="a5c48-495">String</span></span>|<span data-ttu-id="a5c48-496">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-496">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="a5c48-497">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="a5c48-497">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="a5c48-498">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="a5c48-498">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="a5c48-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-499">Boolean</span></span>|<span data-ttu-id="a5c48-500">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="a5c48-500">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="a5c48-501">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="a5c48-501">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="a5c48-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-502">Boolean</span></span>|<span data-ttu-id="a5c48-503">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="a5c48-503">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="a5c48-504">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="a5c48-504">lockScreenBlockPassbook</span></span>|<span data-ttu-id="a5c48-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-505">Boolean</span></span>|<span data-ttu-id="a5c48-506">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="a5c48-506">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="a5c48-507">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="a5c48-507">lockScreenBlockTodayView</span></span>|<span data-ttu-id="a5c48-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-508">Boolean</span></span>|<span data-ttu-id="a5c48-509">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="a5c48-509">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="a5c48-510">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="a5c48-510">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="a5c48-511">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="a5c48-511">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="a5c48-512">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="a5c48-512">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="a5c48-513">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="a5c48-513">mediaContentRatingCanada</span></span>|[<span data-ttu-id="a5c48-514">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="a5c48-514">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="a5c48-515">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="a5c48-515">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="a5c48-516">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="a5c48-516">mediaContentRatingFrance</span></span>|[<span data-ttu-id="a5c48-517">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="a5c48-517">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="a5c48-518">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="a5c48-518">Media content rating settings for France</span></span>|
|<span data-ttu-id="a5c48-519">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="a5c48-519">mediaContentRatingGermany</span></span>|[<span data-ttu-id="a5c48-520">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="a5c48-520">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="a5c48-521">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="a5c48-521">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="a5c48-522">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a5c48-522">mediaContentRatingIreland</span></span>|[<span data-ttu-id="a5c48-523">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a5c48-523">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="a5c48-524">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="a5c48-524">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="a5c48-525">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="a5c48-525">mediaContentRatingJapan</span></span>|[<span data-ttu-id="a5c48-526">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="a5c48-526">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="a5c48-527">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="a5c48-527">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="a5c48-528">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="a5c48-528">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="a5c48-529">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="a5c48-529">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="a5c48-530">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="a5c48-530">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="a5c48-531">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="a5c48-531">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="a5c48-532">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="a5c48-532">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="a5c48-533">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="a5c48-533">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="a5c48-534">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="a5c48-534">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="a5c48-535">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="a5c48-535">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="a5c48-536">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="a5c48-536">Media content rating settings for United States</span></span>|
|<span data-ttu-id="a5c48-537">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="a5c48-537">networkUsageRules</span></span>|<span data-ttu-id="a5c48-538">Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="a5c48-538">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="a5c48-539">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="a5c48-539">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="a5c48-540">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="a5c48-540">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="a5c48-541">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="a5c48-541">mediaContentRatingApps</span></span>|[<span data-ttu-id="a5c48-542">ратингаппстипе</span><span class="sxs-lookup"><span data-stu-id="a5c48-542">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="a5c48-543">Параметры оценки контента мультимедиа для приложений.</span><span class="sxs-lookup"><span data-stu-id="a5c48-543">Media content rating settings for Apps.</span></span> <span data-ttu-id="a5c48-544">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="a5c48-544">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="a5c48-545">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-545">messagesBlocked</span></span>|<span data-ttu-id="a5c48-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-546">Boolean</span></span>|<span data-ttu-id="a5c48-547">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="a5c48-547">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="a5c48-548">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="a5c48-548">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="a5c48-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-549">Boolean</span></span>|<span data-ttu-id="a5c48-550">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-550">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="a5c48-551">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="a5c48-551">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="a5c48-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-552">Boolean</span></span>|<span data-ttu-id="a5c48-553">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="a5c48-553">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="a5c48-554">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="a5c48-554">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="a5c48-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-555">Boolean</span></span>|<span data-ttu-id="a5c48-556">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-556">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-557">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="a5c48-557">passcodeBlockModification</span></span>|<span data-ttu-id="a5c48-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-558">Boolean</span></span>|<span data-ttu-id="a5c48-559">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-559">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="a5c48-560">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a5c48-560">passcodeBlockSimple</span></span>|<span data-ttu-id="a5c48-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-561">Boolean</span></span>|<span data-ttu-id="a5c48-562">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="a5c48-562">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="a5c48-563">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a5c48-563">passcodeExpirationDays</span></span>|<span data-ttu-id="a5c48-564">Int32</span><span class="sxs-lookup"><span data-stu-id="a5c48-564">Int32</span></span>|<span data-ttu-id="a5c48-565">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="a5c48-565">Number of days before the passcode expires.</span></span> <span data-ttu-id="a5c48-566">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="a5c48-566">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="a5c48-567">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a5c48-567">passcodeMinimumLength</span></span>|<span data-ttu-id="a5c48-568">Int32</span><span class="sxs-lookup"><span data-stu-id="a5c48-568">Int32</span></span>|<span data-ttu-id="a5c48-569">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="a5c48-569">Minimum length of passcode.</span></span> <span data-ttu-id="a5c48-570">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="a5c48-570">Valid values 4 to 14</span></span>|
|<span data-ttu-id="a5c48-571">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a5c48-571">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a5c48-572">Int32</span><span class="sxs-lookup"><span data-stu-id="a5c48-572">Int32</span></span>|<span data-ttu-id="a5c48-573">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="a5c48-573">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="a5c48-574">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a5c48-574">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a5c48-575">Int32</span><span class="sxs-lookup"><span data-stu-id="a5c48-575">Int32</span></span>|<span data-ttu-id="a5c48-576">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a5c48-576">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a5c48-577">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a5c48-577">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="a5c48-578">Int32</span><span class="sxs-lookup"><span data-stu-id="a5c48-578">Int32</span></span>|<span data-ttu-id="a5c48-579">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="a5c48-579">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="a5c48-580">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="a5c48-580">Valid values 0 to 4</span></span>|
|<span data-ttu-id="a5c48-581">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="a5c48-581">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="a5c48-582">Int32</span><span class="sxs-lookup"><span data-stu-id="a5c48-582">Int32</span></span>|<span data-ttu-id="a5c48-583">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="a5c48-583">Number of previous passcodes to block.</span></span> <span data-ttu-id="a5c48-584">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="a5c48-584">Valid values 1 to 24</span></span>|
|<span data-ttu-id="a5c48-585">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="a5c48-585">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="a5c48-586">Int32</span><span class="sxs-lookup"><span data-stu-id="a5c48-586">Int32</span></span>|<span data-ttu-id="a5c48-587">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="a5c48-587">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="a5c48-588">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="a5c48-588">Valid values 4 to 11</span></span>|
|<span data-ttu-id="a5c48-589">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="a5c48-589">passcodeRequiredType</span></span>|[<span data-ttu-id="a5c48-590">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="a5c48-590">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="a5c48-591">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="a5c48-591">Type of passcode that is required.</span></span> <span data-ttu-id="a5c48-592">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="a5c48-592">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a5c48-593">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="a5c48-593">passcodeRequired</span></span>|<span data-ttu-id="a5c48-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-594">Boolean</span></span>|<span data-ttu-id="a5c48-595">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="a5c48-595">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="a5c48-596">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-596">podcastsBlocked</span></span>|<span data-ttu-id="a5c48-597">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-597">Boolean</span></span>|<span data-ttu-id="a5c48-598">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-598">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="a5c48-599">проксимитиблокксетуптоневдевице</span><span class="sxs-lookup"><span data-stu-id="a5c48-599">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="a5c48-600">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-600">Boolean</span></span>|<span data-ttu-id="a5c48-601">Указывает, следует ли включить запрос на установку находящихся рядом устройств с защищенным устройством.</span><span class="sxs-lookup"><span data-stu-id="a5c48-601">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="a5c48-602">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="a5c48-602">safariBlockAutofill</span></span>|<span data-ttu-id="a5c48-603">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-603">Boolean</span></span>|<span data-ttu-id="a5c48-604">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="a5c48-604">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="a5c48-605">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="a5c48-605">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="a5c48-606">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="a5c48-606">safariBlockJavaScript</span></span>|<span data-ttu-id="a5c48-607">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-607">Boolean</span></span>|<span data-ttu-id="a5c48-608">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="a5c48-608">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="a5c48-609">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="a5c48-609">safariBlockPopups</span></span>|<span data-ttu-id="a5c48-610">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-610">Boolean</span></span>|<span data-ttu-id="a5c48-611">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="a5c48-611">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="a5c48-612">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-612">safariBlocked</span></span>|<span data-ttu-id="a5c48-613">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-613">Boolean</span></span>|<span data-ttu-id="a5c48-614">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="a5c48-614">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="a5c48-615">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="a5c48-615">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="a5c48-616">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="a5c48-616">safariCookieSettings</span></span>|[<span data-ttu-id="a5c48-617">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="a5c48-617">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="a5c48-618">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="a5c48-618">Cookie settings for Safari.</span></span> <span data-ttu-id="a5c48-619">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="a5c48-619">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="a5c48-620">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="a5c48-620">safariManagedDomains</span></span>|<span data-ttu-id="a5c48-621">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a5c48-621">String collection</span></span>|<span data-ttu-id="a5c48-622">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="a5c48-622">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="a5c48-623">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="a5c48-623">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="a5c48-624">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a5c48-624">String collection</span></span>|<span data-ttu-id="a5c48-625">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="a5c48-625">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="a5c48-626">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-626">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="a5c48-627">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="a5c48-627">safariRequireFraudWarning</span></span>|<span data-ttu-id="a5c48-628">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-628">Boolean</span></span>|<span data-ttu-id="a5c48-629">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="a5c48-629">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="a5c48-630">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-630">screenCaptureBlocked</span></span>|<span data-ttu-id="a5c48-631">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-631">Boolean</span></span>|<span data-ttu-id="a5c48-632">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="a5c48-632">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="a5c48-633">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-633">siriBlocked</span></span>|<span data-ttu-id="a5c48-634">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-634">Boolean</span></span>|<span data-ttu-id="a5c48-635">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="a5c48-635">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="a5c48-636">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-636">siriBlockedWhenLocked</span></span>|<span data-ttu-id="a5c48-637">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-637">Boolean</span></span>|<span data-ttu-id="a5c48-638">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="a5c48-638">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="a5c48-639">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="a5c48-639">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="a5c48-640">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-640">Boolean</span></span>|<span data-ttu-id="a5c48-641">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="a5c48-641">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="a5c48-642">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="a5c48-642">siriRequireProfanityFilter</span></span>|<span data-ttu-id="a5c48-643">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-643">Boolean</span></span>|<span data-ttu-id="a5c48-644">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="a5c48-644">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="a5c48-645">софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="a5c48-645">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="a5c48-646">Int32</span><span class="sxs-lookup"><span data-stu-id="a5c48-646">Int32</span></span>|<span data-ttu-id="a5c48-647">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="a5c48-647">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="a5c48-648">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="a5c48-648">Valid values 0 to 90</span></span>|
|<span data-ttu-id="a5c48-649">софтвареупдатесфорцеделайед</span><span class="sxs-lookup"><span data-stu-id="a5c48-649">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="a5c48-650">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-650">Boolean</span></span>|<span data-ttu-id="a5c48-651">Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-651">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-652">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="a5c48-652">spotlightBlockInternetResults</span></span>|<span data-ttu-id="a5c48-653">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-653">Boolean</span></span>|<span data-ttu-id="a5c48-654">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="a5c48-654">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="a5c48-655">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-655">voiceDialingBlocked</span></span>|<span data-ttu-id="a5c48-656">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-656">Boolean</span></span>|<span data-ttu-id="a5c48-657">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="a5c48-657">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="a5c48-658">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="a5c48-658">wallpaperBlockModification</span></span>|<span data-ttu-id="a5c48-659">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-659">Boolean</span></span>|<span data-ttu-id="a5c48-660">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-660">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="a5c48-661">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="a5c48-661">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="a5c48-662">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-662">Boolean</span></span>|<span data-ttu-id="a5c48-663">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="a5c48-663">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a5c48-664">классрумфорцерекуестпермиссионтолеавеклассес</span><span class="sxs-lookup"><span data-stu-id="a5c48-664">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="a5c48-665">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-665">Boolean</span></span>|<span data-ttu-id="a5c48-666">Указывает, является ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса (iOS 11,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-666">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="a5c48-667">кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="a5c48-667">keychainBlockCloudSync</span></span>|<span data-ttu-id="a5c48-668">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-668">Boolean</span></span>|<span data-ttu-id="a5c48-669">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud.</span><span class="sxs-lookup"><span data-stu-id="a5c48-669">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="a5c48-670">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="a5c48-670">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="a5c48-671">пкиблоккотаупдатес</span><span class="sxs-lookup"><span data-stu-id="a5c48-671">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="a5c48-672">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-672">Boolean</span></span>|<span data-ttu-id="a5c48-673">Указывает, блокируются ли обновления PKI беспроводной сети.</span><span class="sxs-lookup"><span data-stu-id="a5c48-673">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="a5c48-674">Если задать для этого ограничения значение false, проверки CRL и OCSP (iOS 7,0 и более поздних версий) не отключаются.</span><span class="sxs-lookup"><span data-stu-id="a5c48-674">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="a5c48-675">привацифорцелимитадтраккинг</span><span class="sxs-lookup"><span data-stu-id="a5c48-675">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="a5c48-676">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-676">Boolean</span></span>|<span data-ttu-id="a5c48-677">Указывает, ограничено ли отслеживание AD. (iOS 7,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-677">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="a5c48-678">ентерприсебукблоккбаккуп</span><span class="sxs-lookup"><span data-stu-id="a5c48-678">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="a5c48-679">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-679">Boolean</span></span>|<span data-ttu-id="a5c48-680">Указывает, блокируется ли резервное копирование корпоративной книги.</span><span class="sxs-lookup"><span data-stu-id="a5c48-680">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="a5c48-681">ентерприсебукблоккметадатасинк</span><span class="sxs-lookup"><span data-stu-id="a5c48-681">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="a5c48-682">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-682">Boolean</span></span>|<span data-ttu-id="a5c48-683">Указывает, блокируется ли синхронизация заметок и выделений корпоративных книг.</span><span class="sxs-lookup"><span data-stu-id="a5c48-683">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="a5c48-684">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="a5c48-684">airPrintBlocked</span></span>|<span data-ttu-id="a5c48-685">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-685">Boolean</span></span>|<span data-ttu-id="a5c48-686">Указывает, заблокировано ли Аирпринт (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-686">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="a5c48-687">аирпринтблокккредентиалсстораже</span><span class="sxs-lookup"><span data-stu-id="a5c48-687">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="a5c48-688">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-688">Boolean</span></span>|<span data-ttu-id="a5c48-689">Указывает, заблокировано ли хранение цепочки ключей имени пользователя и пароля для Аирпринт (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-689">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="a5c48-690">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="a5c48-690">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="a5c48-691">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-691">Boolean</span></span>|<span data-ttu-id="a5c48-692">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-692">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="a5c48-693">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="a5c48-693">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="a5c48-694">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-694">Boolean</span></span>|<span data-ttu-id="a5c48-695">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="a5c48-695">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="a5c48-696">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-696">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="a5c48-697">филеснетворкдривеакцессблоккед</span><span class="sxs-lookup"><span data-stu-id="a5c48-697">filesNetworkDriveAccessBlocked</span></span>|<span data-ttu-id="a5c48-698">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-698">Boolean</span></span>|<span data-ttu-id="a5c48-699">Указывает, могут ли устройства получать доступ к файлам или другим ресурсам на сетевом сервере с помощью протокола SMB.</span><span class="sxs-lookup"><span data-stu-id="a5c48-699">Indicates if devices can access files or other resources on a network server using the Server Message Block (SMB) protocol.</span></span> <span data-ttu-id="a5c48-700">Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="a5c48-700">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="a5c48-701">филесусбдривеакцессблоккед</span><span class="sxs-lookup"><span data-stu-id="a5c48-701">filesUsbDriveAccessBlocked</span></span>|<span data-ttu-id="a5c48-702">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-702">Boolean</span></span>|<span data-ttu-id="a5c48-703">Указывает, могут ли севицес с Access подключаться к файлам и открывать их на USB-диске.</span><span class="sxs-lookup"><span data-stu-id="a5c48-703">Indicates if sevices with access can connect to and open files on a USB drive.</span></span> <span data-ttu-id="a5c48-704">Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="a5c48-704">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="a5c48-705">вифиповеронфорцед</span><span class="sxs-lookup"><span data-stu-id="a5c48-705">wifiPowerOnForced</span></span>|<span data-ttu-id="a5c48-706">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-706">Boolean</span></span>|<span data-ttu-id="a5c48-707">Указывает, остается ли Wi-Fi On, даже если устройство находится в режиме "в самолете".</span><span class="sxs-lookup"><span data-stu-id="a5c48-707">Indicates whether or not Wi-Fi remains on, even when device is in airplane mode.</span></span> <span data-ttu-id="a5c48-708">Доступно для устройств с iOS и Ипадос версии 13,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="a5c48-708">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="a5c48-709">блокксистемаппремовал</span><span class="sxs-lookup"><span data-stu-id="a5c48-709">blockSystemAppRemoval</span></span>|<span data-ttu-id="a5c48-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-710">Boolean</span></span>|<span data-ttu-id="a5c48-711">Указывает, заблокировано ли удаление системных приложений с устройства на контролируемом устройстве (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-711">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="a5c48-712">впнблокккреатион</span><span class="sxs-lookup"><span data-stu-id="a5c48-712">vpnBlockCreation</span></span>|<span data-ttu-id="a5c48-713">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-713">Boolean</span></span>|<span data-ttu-id="a5c48-714">Указывает, блокируется ли создание конфигураций VPN (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-714">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="a5c48-715">аппремовалблоккед</span><span class="sxs-lookup"><span data-stu-id="a5c48-715">appRemovalBlocked</span></span>|<span data-ttu-id="a5c48-716">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-716">Boolean</span></span>|<span data-ttu-id="a5c48-717">Указывает, разрешено ли удаление приложений.</span><span class="sxs-lookup"><span data-stu-id="a5c48-717">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="a5c48-718">усбрестриктедмодеблоккед</span><span class="sxs-lookup"><span data-stu-id="a5c48-718">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="a5c48-719">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-719">Boolean</span></span>|<span data-ttu-id="a5c48-720">Указывает, разрешена ли подключаться к стандарту USB, пока устройство заблокировано (iOS 11.4.1 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-720">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="a5c48-721">пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="a5c48-721">passwordBlockAutoFill</span></span>|<span data-ttu-id="a5c48-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-722">Boolean</span></span>|<span data-ttu-id="a5c48-723">Указывает, разрешена ли функция автозаполнения паролей (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-723">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="a5c48-724">пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="a5c48-724">passwordBlockProximityRequests</span></span>|<span data-ttu-id="a5c48-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-725">Boolean</span></span>|<span data-ttu-id="a5c48-726">Указывает, следует ли запретить запрашивать пароли с близлежащих устройств (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-726">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="a5c48-727">пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="a5c48-727">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="a5c48-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-728">Boolean</span></span>|<span data-ttu-id="a5c48-729">Указывает, следует ли заблокировать общий доступ к паролям с помощью AirDrop паролей iOS 12,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="a5c48-729">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="a5c48-730">датеандтимефорцесетаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="a5c48-730">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="a5c48-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-731">Boolean</span></span>|<span data-ttu-id="a5c48-732">Указывает, включена ли функция даты и времени "автоматически задано" и не может быть отключена пользователем (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-732">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="a5c48-733">контактсалловманажедтаунманажедврите</span><span class="sxs-lookup"><span data-stu-id="a5c48-733">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="a5c48-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-734">Boolean</span></span>|<span data-ttu-id="a5c48-735">Указывает, могут ли управляемые приложения записывать контакты в неуправляемые учетные записи контактов (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="a5c48-735">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="a5c48-736">контактсалловунманажедтоманажедреад</span><span class="sxs-lookup"><span data-stu-id="a5c48-736">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="a5c48-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-737">Boolean</span></span>|<span data-ttu-id="a5c48-738">Указывает, могут ли неуправляемые приложения читать из управляемых учетных записей контактов (iOS 12,0 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="a5c48-738">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="a5c48-739">целлуларблоккперсоналхотспотмодификатион</span><span class="sxs-lookup"><span data-stu-id="a5c48-739">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="a5c48-740">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-740">Boolean</span></span>|<span data-ttu-id="a5c48-741">Указывает, следует ли запретить пользователю изменять параметр личных гиперобъектов (iOS 12,2 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="a5c48-741">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="a5c48-742">континуауспаскэйбоардблоккед</span><span class="sxs-lookup"><span data-stu-id="a5c48-742">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="a5c48-743">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-743">Boolean</span></span>|<span data-ttu-id="a5c48-744">Указывает, следует ли заблокировать клавиатуру непрерывного пути, когда устройство защищено (iOS 13 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="a5c48-744">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="a5c48-745">финдмидевицеинфиндмяппблоккед</span><span class="sxs-lookup"><span data-stu-id="a5c48-745">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="a5c48-746">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-746">Boolean</span></span>|<span data-ttu-id="a5c48-747">Указывает, следует ли заблокировать Поиск устройства, когда устройство защищено (iOS 13 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="a5c48-747">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="a5c48-748">финдмифриендсинфиндмяппблоккед</span><span class="sxs-lookup"><span data-stu-id="a5c48-748">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="a5c48-749">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-749">Boolean</span></span>|<span data-ttu-id="a5c48-750">Указывает, следует ли заблокировать "найти друзей", когда устройство защищено (iOS 13 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="a5c48-750">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="a5c48-751">итунесблоккед</span><span class="sxs-lookup"><span data-stu-id="a5c48-751">iTunesBlocked</span></span>|<span data-ttu-id="a5c48-752">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5c48-752">Boolean</span></span>|<span data-ttu-id="a5c48-753">Указывает, следует ли заблокировать приложение iTunes.</span><span class="sxs-lookup"><span data-stu-id="a5c48-753">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="a5c48-754">Для iOS 13 и более поздних версий требуется контролируемое устройство.</span><span class="sxs-lookup"><span data-stu-id="a5c48-754">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="a5c48-755">киоскмодеапптипе</span><span class="sxs-lookup"><span data-stu-id="a5c48-755">kioskModeAppType</span></span>|[<span data-ttu-id="a5c48-756">иоскиоскмодеапптипе</span><span class="sxs-lookup"><span data-stu-id="a5c48-756">iosKioskModeAppType</span></span>](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|<span data-ttu-id="a5c48-757">Тип приложения, которое будет запускаться в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="a5c48-757">Type of app to run in kiosk mode.</span></span> <span data-ttu-id="a5c48-758">Возможные значения: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span><span class="sxs-lookup"><span data-stu-id="a5c48-758">Possible values are: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span></span>|



## <a name="response"></a><span data-ttu-id="a5c48-759">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5c48-759">Response</span></span>
<span data-ttu-id="a5c48-760">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a5c48-760">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5c48-761">Пример</span><span class="sxs-lookup"><span data-stu-id="a5c48-761">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5c48-762">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5c48-762">Request</span></span>
<span data-ttu-id="a5c48-763">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5c48-763">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10518

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
  "iTunesBlocked": true,
  "kioskModeAppType": "appStoreApp"
}
```

### <a name="response"></a><span data-ttu-id="a5c48-764">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5c48-764">Response</span></span>
<span data-ttu-id="a5c48-p157">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a5c48-p157">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10690

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
  "iTunesBlocked": true,
  "kioskModeAppType": "appStoreApp"
}
```





