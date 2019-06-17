---
title: Create iosGeneralDeviceConfiguration
description: Создание объекта iosGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18e7f464317481346dd2ba0933f90607de8c3635
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966728"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="9773c-103">Create iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9773c-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="9773c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9773c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9773c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9773c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9773c-106">Создание объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9773c-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9773c-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9773c-107">Prerequisites</span></span>
<span data-ttu-id="9773c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9773c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9773c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9773c-110">Permission type</span></span>|<span data-ttu-id="9773c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9773c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9773c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9773c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9773c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9773c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9773c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9773c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9773c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9773c-115">Not supported.</span></span>|
|<span data-ttu-id="9773c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9773c-116">Application</span></span>|<span data-ttu-id="9773c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9773c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9773c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9773c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9773c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9773c-119">Request headers</span></span>
|<span data-ttu-id="9773c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9773c-120">Header</span></span>|<span data-ttu-id="9773c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9773c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9773c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9773c-122">Authorization</span></span>|<span data-ttu-id="9773c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9773c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9773c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9773c-124">Accept</span></span>|<span data-ttu-id="9773c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9773c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9773c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9773c-126">Request body</span></span>
<span data-ttu-id="9773c-127">В теле запроса добавьте представление объекта iosGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9773c-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="9773c-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9773c-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="9773c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9773c-129">Property</span></span>|<span data-ttu-id="9773c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9773c-130">Type</span></span>|<span data-ttu-id="9773c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9773c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9773c-132">id</span><span class="sxs-lookup"><span data-stu-id="9773c-132">id</span></span>|<span data-ttu-id="9773c-133">String</span><span class="sxs-lookup"><span data-stu-id="9773c-133">String</span></span>|<span data-ttu-id="9773c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9773c-134">Key of the entity.</span></span> <span data-ttu-id="9773c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9773c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9773c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9773c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9773c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9773c-137">DateTimeOffset</span></span>|<span data-ttu-id="9773c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9773c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9773c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9773c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9773c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9773c-140">roleScopeTagIds</span></span>|<span data-ttu-id="9773c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9773c-141">String collection</span></span>|<span data-ttu-id="9773c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9773c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9773c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9773c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9773c-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="9773c-144">supportsScopeTags</span></span>|<span data-ttu-id="9773c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-145">Boolean</span></span>|<span data-ttu-id="9773c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9773c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9773c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="9773c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9773c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9773c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9773c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9773c-149">This property is read-only.</span></span> <span data-ttu-id="9773c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9773c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9773c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9773c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9773c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9773c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9773c-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9773c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9773c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9773c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9773c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9773c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9773c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9773c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9773c-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9773c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9773c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9773c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9773c-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="9773c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9773c-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="9773c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9773c-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9773c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9773c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9773c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9773c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9773c-163">createdDateTime</span></span>|<span data-ttu-id="9773c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9773c-164">DateTimeOffset</span></span>|<span data-ttu-id="9773c-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9773c-165">DateTime the object was created.</span></span> <span data-ttu-id="9773c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9773c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9773c-167">description</span><span class="sxs-lookup"><span data-stu-id="9773c-167">description</span></span>|<span data-ttu-id="9773c-168">String</span><span class="sxs-lookup"><span data-stu-id="9773c-168">String</span></span>|<span data-ttu-id="9773c-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9773c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9773c-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9773c-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9773c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9773c-171">displayName</span></span>|<span data-ttu-id="9773c-172">Строка</span><span class="sxs-lookup"><span data-stu-id="9773c-172">String</span></span>|<span data-ttu-id="9773c-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9773c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9773c-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9773c-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9773c-175">version</span><span class="sxs-lookup"><span data-stu-id="9773c-175">version</span></span>|<span data-ttu-id="9773c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9773c-176">Int32</span></span>|<span data-ttu-id="9773c-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9773c-177">Version of the device configuration.</span></span> <span data-ttu-id="9773c-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9773c-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9773c-179">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="9773c-179">accountBlockModification</span></span>|<span data-ttu-id="9773c-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-180">Boolean</span></span>|<span data-ttu-id="9773c-181">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-181">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-182">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="9773c-182">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="9773c-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-183">Boolean</span></span>|<span data-ttu-id="9773c-184">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-184">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="9773c-185">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-185">airDropBlocked</span></span>|<span data-ttu-id="9773c-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-186">Boolean</span></span>|<span data-ttu-id="9773c-187">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-187">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-188">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="9773c-188">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="9773c-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-189">Boolean</span></span>|<span data-ttu-id="9773c-190">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-190">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9773c-191">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="9773c-191">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="9773c-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-192">Boolean</span></span>|<span data-ttu-id="9773c-193">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="9773c-193">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="9773c-194">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="9773c-194">appleWatchBlockPairing</span></span>|<span data-ttu-id="9773c-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-195">Boolean</span></span>|<span data-ttu-id="9773c-196">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-196">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9773c-197">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="9773c-197">appleWatchForceWristDetection</span></span>|<span data-ttu-id="9773c-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-198">Boolean</span></span>|<span data-ttu-id="9773c-199">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-199">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="9773c-200">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-200">appleNewsBlocked</span></span>|<span data-ttu-id="9773c-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-201">Boolean</span></span>|<span data-ttu-id="9773c-202">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-202">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9773c-203">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="9773c-203">appsSingleAppModeList</span></span>|<span data-ttu-id="9773c-204">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="9773c-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9773c-205">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="9773c-205">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="9773c-206">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-206">Supervised only.</span></span> <span data-ttu-id="9773c-207">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="9773c-207">iOS 7.0 and later.</span></span> <span data-ttu-id="9773c-208">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="9773c-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9773c-209">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="9773c-209">appsVisibilityList</span></span>|<span data-ttu-id="9773c-210">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="9773c-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9773c-211">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-211">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="9773c-212">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="9773c-212">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="9773c-213">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="9773c-213">appsVisibilityListType</span></span>|[<span data-ttu-id="9773c-214">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="9773c-214">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="9773c-215">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="9773c-215">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="9773c-216">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="9773c-216">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="9773c-217">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="9773c-217">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="9773c-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-218">Boolean</span></span>|<span data-ttu-id="9773c-219">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-219">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9773c-220">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-220">appStoreBlocked</span></span>|<span data-ttu-id="9773c-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-221">Boolean</span></span>|<span data-ttu-id="9773c-222">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="9773c-222">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="9773c-223">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="9773c-223">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="9773c-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-224">Boolean</span></span>|<span data-ttu-id="9773c-225">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="9773c-225">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="9773c-226">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="9773c-226">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="9773c-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-227">Boolean</span></span>|<span data-ttu-id="9773c-228">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="9773c-228">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="9773c-229">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-229">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9773c-230">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="9773c-230">appStoreRequirePassword</span></span>|<span data-ttu-id="9773c-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-231">Boolean</span></span>|<span data-ttu-id="9773c-232">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="9773c-232">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="9773c-233">Аутофиллфорцеаусентикатион</span><span class="sxs-lookup"><span data-stu-id="9773c-233">autoFillForceAuthentication</span></span>|<span data-ttu-id="9773c-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-234">Boolean</span></span>|<span data-ttu-id="9773c-235">Указывает, следует ли принудительно выполнять проверку подлинности пользователей перед автозаполнением паролей и сведений о кредитных картах в Safari и других приложениях на контролируемых устройствах.</span><span class="sxs-lookup"><span data-stu-id="9773c-235">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="9773c-236">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="9773c-236">bluetoothBlockModification</span></span>|<span data-ttu-id="9773c-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-237">Boolean</span></span>|<span data-ttu-id="9773c-238">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-238">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="9773c-239">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-239">cameraBlocked</span></span>|<span data-ttu-id="9773c-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-240">Boolean</span></span>|<span data-ttu-id="9773c-241">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="9773c-241">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="9773c-242">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="9773c-242">cellularBlockDataRoaming</span></span>|<span data-ttu-id="9773c-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-243">Boolean</span></span>|<span data-ttu-id="9773c-244">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="9773c-244">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="9773c-245">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="9773c-245">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="9773c-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-246">Boolean</span></span>|<span data-ttu-id="9773c-247">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="9773c-247">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="9773c-248">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="9773c-248">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="9773c-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-249">Boolean</span></span>|<span data-ttu-id="9773c-250">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-250">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-251">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="9773c-251">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="9773c-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-252">Boolean</span></span>|<span data-ttu-id="9773c-253">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="9773c-253">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="9773c-254">Целлуларблоккпланмодификатион</span><span class="sxs-lookup"><span data-stu-id="9773c-254">cellularBlockPlanModification</span></span>|<span data-ttu-id="9773c-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-255">Boolean</span></span>|<span data-ttu-id="9773c-256">Указывает, следует ли запретить пользователям изменять параметры плана сотовой связи на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="9773c-256">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="9773c-257">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="9773c-257">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="9773c-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-258">Boolean</span></span>|<span data-ttu-id="9773c-259">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="9773c-259">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="9773c-260">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="9773c-260">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="9773c-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-261">Boolean</span></span>|<span data-ttu-id="9773c-262">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="9773c-262">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="9773c-263">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="9773c-263">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="9773c-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-264">Boolean</span></span>|<span data-ttu-id="9773c-265">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-265">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="9773c-266">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="9773c-266">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="9773c-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-267">Boolean</span></span>|<span data-ttu-id="9773c-268">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-268">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-269">Классрумфорцеаутоматикаллижоинклассес</span><span class="sxs-lookup"><span data-stu-id="9773c-269">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="9773c-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-270">Boolean</span></span>|<span data-ttu-id="9773c-271">Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-271">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-272">Классрумфорцеунпромптедаппанддевицелокк</span><span class="sxs-lookup"><span data-stu-id="9773c-272">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="9773c-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-273">Boolean</span></span>|<span data-ttu-id="9773c-274">Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся.</span><span class="sxs-lookup"><span data-stu-id="9773c-274">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="9773c-275">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-275">Supervised only.</span></span>|
|<span data-ttu-id="9773c-276">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="9773c-276">compliantAppsList</span></span>|<span data-ttu-id="9773c-277">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="9773c-277">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9773c-278">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="9773c-278">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="9773c-279">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="9773c-279">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="9773c-280">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="9773c-280">compliantAppListType</span></span>|[<span data-ttu-id="9773c-281">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="9773c-281">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="9773c-282">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="9773c-282">List that is in the AppComplianceList.</span></span> <span data-ttu-id="9773c-283">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="9773c-283">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="9773c-284">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="9773c-284">configurationProfileBlockChanges</span></span>|<span data-ttu-id="9773c-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-285">Boolean</span></span>|<span data-ttu-id="9773c-286">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-286">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-287">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-287">definitionLookupBlocked</span></span>|<span data-ttu-id="9773c-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-288">Boolean</span></span>|<span data-ttu-id="9773c-289">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-289">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="9773c-290">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="9773c-290">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="9773c-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-291">Boolean</span></span>|<span data-ttu-id="9773c-292">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-292">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-293">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="9773c-293">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="9773c-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-294">Boolean</span></span>|<span data-ttu-id="9773c-295">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-295">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-296">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="9773c-296">deviceBlockNameModification</span></span>|<span data-ttu-id="9773c-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-297">Boolean</span></span>|<span data-ttu-id="9773c-298">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-298">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9773c-299">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="9773c-299">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="9773c-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-300">Boolean</span></span>|<span data-ttu-id="9773c-301">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="9773c-301">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="9773c-302">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="9773c-302">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="9773c-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-303">Boolean</span></span>|<span data-ttu-id="9773c-304">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-304">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="9773c-305">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="9773c-305">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="9773c-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-306">Boolean</span></span>|<span data-ttu-id="9773c-307">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="9773c-307">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="9773c-308">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="9773c-308">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="9773c-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-309">Boolean</span></span>|<span data-ttu-id="9773c-310">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="9773c-310">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="9773c-311">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="9773c-311">emailInDomainSuffixes</span></span>|<span data-ttu-id="9773c-312">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9773c-312">String collection</span></span>|<span data-ttu-id="9773c-313">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="9773c-313">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="9773c-314">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="9773c-314">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="9773c-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-315">Boolean</span></span>|<span data-ttu-id="9773c-316">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="9773c-316">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="9773c-317">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="9773c-317">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="9773c-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-318">Boolean</span></span>|<span data-ttu-id="9773c-319">Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="9773c-319">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="9773c-320">Есимблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="9773c-320">esimBlockModification</span></span>|<span data-ttu-id="9773c-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-321">Boolean</span></span>|<span data-ttu-id="9773c-322">Указывает, следует ли разрешить добавление или удаление планов сотовой связи на eSIM контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="9773c-322">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="9773c-323">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-323">faceTimeBlocked</span></span>|<span data-ttu-id="9773c-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-324">Boolean</span></span>|<span data-ttu-id="9773c-325">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="9773c-325">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="9773c-326">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-326">findMyFriendsBlocked</span></span>|<span data-ttu-id="9773c-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-327">Boolean</span></span>|<span data-ttu-id="9773c-328">Указывает, следует ли заблокировать функцию "Найти друзей", когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-328">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-329">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="9773c-329">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="9773c-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-330">Boolean</span></span>|<span data-ttu-id="9773c-331">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="9773c-331">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="9773c-332">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="9773c-332">gamingBlockMultiplayer</span></span>|<span data-ttu-id="9773c-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-333">Boolean</span></span>|<span data-ttu-id="9773c-334">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="9773c-334">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="9773c-335">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-335">gameCenterBlocked</span></span>|<span data-ttu-id="9773c-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-336">Boolean</span></span>|<span data-ttu-id="9773c-337">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-337">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-338">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-338">hostPairingBlocked</span></span>|<span data-ttu-id="9773c-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-339">Boolean</span></span>|<span data-ttu-id="9773c-340">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-340">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-341">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-341">iBooksStoreBlocked</span></span>|<span data-ttu-id="9773c-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-342">Boolean</span></span>|<span data-ttu-id="9773c-343">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-343">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-344">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="9773c-344">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="9773c-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-345">Boolean</span></span>|<span data-ttu-id="9773c-346">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="9773c-346">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="9773c-347">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="9773c-347">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="9773c-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-348">Boolean</span></span>|<span data-ttu-id="9773c-349">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="9773c-349">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="9773c-350">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="9773c-350">iCloudBlockBackup</span></span>|<span data-ttu-id="9773c-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-351">Boolean</span></span>|<span data-ttu-id="9773c-352">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="9773c-352">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="9773c-353">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="9773c-353">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="9773c-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-354">Boolean</span></span>|<span data-ttu-id="9773c-355">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="9773c-355">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="9773c-356">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="9773c-356">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="9773c-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-357">Boolean</span></span>|<span data-ttu-id="9773c-358">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="9773c-358">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="9773c-359">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="9773c-359">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="9773c-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-360">Boolean</span></span>|<span data-ttu-id="9773c-361">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="9773c-361">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="9773c-362">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="9773c-362">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="9773c-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-363">Boolean</span></span>|<span data-ttu-id="9773c-364">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="9773c-364">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="9773c-365">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="9773c-365">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="9773c-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-366">Boolean</span></span>|<span data-ttu-id="9773c-367">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="9773c-367">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="9773c-368">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="9773c-368">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="9773c-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-369">Boolean</span></span>|<span data-ttu-id="9773c-370">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="9773c-370">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="9773c-371">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="9773c-371">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="9773c-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-372">Boolean</span></span>|<span data-ttu-id="9773c-373">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="9773c-373">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="9773c-374">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="9773c-374">iTunesBlockMusicService</span></span>|<span data-ttu-id="9773c-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-375">Boolean</span></span>|<span data-ttu-id="9773c-376">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-376">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="9773c-377">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="9773c-377">iTunesBlockRadio</span></span>|<span data-ttu-id="9773c-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-378">Boolean</span></span>|<span data-ttu-id="9773c-379">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-379">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="9773c-380">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="9773c-380">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="9773c-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-381">Boolean</span></span>|<span data-ttu-id="9773c-382">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-382">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="9773c-383">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="9773c-383">keyboardBlockDictation</span></span>|<span data-ttu-id="9773c-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-384">Boolean</span></span>|<span data-ttu-id="9773c-385">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-385">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-386">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="9773c-386">keyboardBlockPredictive</span></span>|<span data-ttu-id="9773c-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-387">Boolean</span></span>|<span data-ttu-id="9773c-388">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-388">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="9773c-389">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="9773c-389">keyboardBlockShortcuts</span></span>|<span data-ttu-id="9773c-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-390">Boolean</span></span>|<span data-ttu-id="9773c-391">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-391">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9773c-392">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="9773c-392">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="9773c-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-393">Boolean</span></span>|<span data-ttu-id="9773c-394">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-394">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="9773c-395">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="9773c-395">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="9773c-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-396">Boolean</span></span>|<span data-ttu-id="9773c-397">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-397">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-398">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="9773c-398">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="9773c-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-399">Boolean</span></span>|<span data-ttu-id="9773c-400">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-400">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-401">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="9773c-401">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="9773c-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-402">Boolean</span></span>|<span data-ttu-id="9773c-403">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-403">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="9773c-404">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="9773c-404">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="9773c-405">Вместо этого используйте Киоскмодеблоккаутолокк.</span><span class="sxs-lookup"><span data-stu-id="9773c-405">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="9773c-406">Киоскмодеблоккаутолокк</span><span class="sxs-lookup"><span data-stu-id="9773c-406">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="9773c-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-407">Boolean</span></span>|<span data-ttu-id="9773c-408">Указывает, следует ли блокировать автоматическую блокировку устройств в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-408">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-409">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="9773c-409">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="9773c-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-410">Boolean</span></span>|<span data-ttu-id="9773c-411">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-411">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-412">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="9773c-412">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="9773c-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-413">Boolean</span></span>|<span data-ttu-id="9773c-414">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-414">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="9773c-415">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="9773c-415">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="9773c-416">Вместо этого используйте Киоскмодеблоккринжерсвитч.</span><span class="sxs-lookup"><span data-stu-id="9773c-416">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="9773c-417">Киоскмодеблоккринжерсвитч</span><span class="sxs-lookup"><span data-stu-id="9773c-417">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="9773c-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-418">Boolean</span></span>|<span data-ttu-id="9773c-419">Указывает, следует ли запретить использование переключателя звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-419">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-420">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="9773c-420">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="9773c-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-421">Boolean</span></span>|<span data-ttu-id="9773c-422">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-422">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="9773c-423">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="9773c-423">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="9773c-424">Вместо этого используйте Киоскмодеблоккскринротатион.</span><span class="sxs-lookup"><span data-stu-id="9773c-424">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="9773c-425">Киоскмодеблоккскринротатион</span><span class="sxs-lookup"><span data-stu-id="9773c-425">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="9773c-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-426">Boolean</span></span>|<span data-ttu-id="9773c-427">Указывает, следует ли блокировать поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-427">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-428">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="9773c-428">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="9773c-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-429">Boolean</span></span>|<span data-ttu-id="9773c-430">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-430">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="9773c-431">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="9773c-431">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="9773c-432">Вместо этого используйте Киоскмодеблоккслипбуттон.</span><span class="sxs-lookup"><span data-stu-id="9773c-432">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="9773c-433">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="9773c-433">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="9773c-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-434">Boolean</span></span>|<span data-ttu-id="9773c-435">Указывает, следует ли запретить использование кнопки "сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-435">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-436">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="9773c-436">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="9773c-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-437">Boolean</span></span>|<span data-ttu-id="9773c-438">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-438">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="9773c-439">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="9773c-439">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="9773c-440">Вместо этого используйте Киоскмодеблокктаучскрин.</span><span class="sxs-lookup"><span data-stu-id="9773c-440">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="9773c-441">Киоскмодеблокктаучскрин</span><span class="sxs-lookup"><span data-stu-id="9773c-441">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="9773c-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-442">Boolean</span></span>|<span data-ttu-id="9773c-443">Указывает, следует ли запретить использование сенсорного экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-443">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-444">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="9773c-444">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="9773c-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-445">Boolean</span></span>|<span data-ttu-id="9773c-446">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-446">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-447">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="9773c-447">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="9773c-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-448">Boolean</span></span>|<span data-ttu-id="9773c-449">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-449">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="9773c-450">Функция этого свойства является избыточной по умолчанию для ОС и является устаревшей.</span><span class="sxs-lookup"><span data-stu-id="9773c-450">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="9773c-451">Вместо этого используйте Киоскмодеблоккволумебуттонс.</span><span class="sxs-lookup"><span data-stu-id="9773c-451">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="9773c-452">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="9773c-452">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="9773c-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-453">Boolean</span></span>|<span data-ttu-id="9773c-454">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="9773c-454">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="9773c-455">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="9773c-455">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="9773c-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-456">Boolean</span></span>|<span data-ttu-id="9773c-457">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-457">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-458">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9773c-458">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="9773c-459">String</span><span class="sxs-lookup"><span data-stu-id="9773c-459">String</span></span>|<span data-ttu-id="9773c-460">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-460">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="9773c-461">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="9773c-461">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="9773c-462">Киоскмодебуилтинаппид</span><span class="sxs-lookup"><span data-stu-id="9773c-462">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="9773c-463">String</span><span class="sxs-lookup"><span data-stu-id="9773c-463">String</span></span>|<span data-ttu-id="9773c-464">Идентификатор встроенных приложений для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-464">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="9773c-465">Используется, когда KioskModeManagedAppId и KioskModeAppStoreUrl не заданы.</span><span class="sxs-lookup"><span data-stu-id="9773c-465">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="9773c-466">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="9773c-466">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="9773c-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-467">Boolean</span></span>|<span data-ttu-id="9773c-468">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-468">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-469">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="9773c-469">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="9773c-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-470">Boolean</span></span>|<span data-ttu-id="9773c-471">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-471">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-472">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="9773c-472">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="9773c-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-473">Boolean</span></span>|<span data-ttu-id="9773c-474">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-474">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-475">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="9773c-475">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="9773c-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-476">Boolean</span></span>|<span data-ttu-id="9773c-477">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-477">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-478">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="9773c-478">kioskModeRequireZoom</span></span>|<span data-ttu-id="9773c-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-479">Boolean</span></span>|<span data-ttu-id="9773c-480">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-480">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="9773c-481">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="9773c-481">kioskModeManagedAppId</span></span>|<span data-ttu-id="9773c-482">String</span><span class="sxs-lookup"><span data-stu-id="9773c-482">String</span></span>|<span data-ttu-id="9773c-483">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9773c-483">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="9773c-484">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="9773c-484">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="9773c-485">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="9773c-485">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="9773c-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-486">Boolean</span></span>|<span data-ttu-id="9773c-487">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="9773c-487">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="9773c-488">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="9773c-488">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="9773c-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-489">Boolean</span></span>|<span data-ttu-id="9773c-490">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="9773c-490">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="9773c-491">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="9773c-491">lockScreenBlockPassbook</span></span>|<span data-ttu-id="9773c-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-492">Boolean</span></span>|<span data-ttu-id="9773c-493">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="9773c-493">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="9773c-494">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="9773c-494">lockScreenBlockTodayView</span></span>|<span data-ttu-id="9773c-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-495">Boolean</span></span>|<span data-ttu-id="9773c-496">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="9773c-496">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="9773c-497">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="9773c-497">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="9773c-498">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="9773c-498">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="9773c-499">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="9773c-499">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="9773c-500">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="9773c-500">mediaContentRatingCanada</span></span>|[<span data-ttu-id="9773c-501">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="9773c-501">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="9773c-502">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="9773c-502">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="9773c-503">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="9773c-503">mediaContentRatingFrance</span></span>|[<span data-ttu-id="9773c-504">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="9773c-504">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="9773c-505">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="9773c-505">Media content rating settings for France</span></span>|
|<span data-ttu-id="9773c-506">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="9773c-506">mediaContentRatingGermany</span></span>|[<span data-ttu-id="9773c-507">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="9773c-507">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="9773c-508">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="9773c-508">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="9773c-509">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="9773c-509">mediaContentRatingIreland</span></span>|[<span data-ttu-id="9773c-510">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="9773c-510">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="9773c-511">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="9773c-511">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="9773c-512">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="9773c-512">mediaContentRatingJapan</span></span>|[<span data-ttu-id="9773c-513">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="9773c-513">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="9773c-514">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="9773c-514">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="9773c-515">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="9773c-515">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="9773c-516">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="9773c-516">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="9773c-517">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="9773c-517">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="9773c-518">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="9773c-518">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="9773c-519">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="9773c-519">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="9773c-520">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="9773c-520">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="9773c-521">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="9773c-521">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="9773c-522">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="9773c-522">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="9773c-523">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="9773c-523">Media content rating settings for United States</span></span>|
|<span data-ttu-id="9773c-524">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="9773c-524">networkUsageRules</span></span>|<span data-ttu-id="9773c-525">Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="9773c-525">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="9773c-526">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="9773c-526">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="9773c-527">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="9773c-527">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="9773c-528">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="9773c-528">mediaContentRatingApps</span></span>|[<span data-ttu-id="9773c-529">Ратингаппстипе</span><span class="sxs-lookup"><span data-stu-id="9773c-529">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="9773c-530">Параметры оценки контента мультимедиа для приложений.</span><span class="sxs-lookup"><span data-stu-id="9773c-530">Media content rating settings for Apps.</span></span> <span data-ttu-id="9773c-531">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="9773c-531">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="9773c-532">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-532">messagesBlocked</span></span>|<span data-ttu-id="9773c-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-533">Boolean</span></span>|<span data-ttu-id="9773c-534">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="9773c-534">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="9773c-535">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="9773c-535">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="9773c-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-536">Boolean</span></span>|<span data-ttu-id="9773c-537">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-537">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="9773c-538">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="9773c-538">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="9773c-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-539">Boolean</span></span>|<span data-ttu-id="9773c-540">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="9773c-540">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="9773c-541">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="9773c-541">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="9773c-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-542">Boolean</span></span>|<span data-ttu-id="9773c-543">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-543">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="9773c-544">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="9773c-544">passcodeBlockModification</span></span>|<span data-ttu-id="9773c-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-545">Boolean</span></span>|<span data-ttu-id="9773c-546">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-546">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9773c-547">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9773c-547">passcodeBlockSimple</span></span>|<span data-ttu-id="9773c-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-548">Boolean</span></span>|<span data-ttu-id="9773c-549">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="9773c-549">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="9773c-550">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9773c-550">passcodeExpirationDays</span></span>|<span data-ttu-id="9773c-551">Int32</span><span class="sxs-lookup"><span data-stu-id="9773c-551">Int32</span></span>|<span data-ttu-id="9773c-552">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="9773c-552">Number of days before the passcode expires.</span></span> <span data-ttu-id="9773c-553">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="9773c-553">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="9773c-554">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9773c-554">passcodeMinimumLength</span></span>|<span data-ttu-id="9773c-555">Int32</span><span class="sxs-lookup"><span data-stu-id="9773c-555">Int32</span></span>|<span data-ttu-id="9773c-556">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="9773c-556">Minimum length of passcode.</span></span> <span data-ttu-id="9773c-557">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="9773c-557">Valid values 4 to 14</span></span>|
|<span data-ttu-id="9773c-558">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9773c-558">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9773c-559">Int32</span><span class="sxs-lookup"><span data-stu-id="9773c-559">Int32</span></span>|<span data-ttu-id="9773c-560">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="9773c-560">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="9773c-561">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9773c-561">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9773c-562">Int32</span><span class="sxs-lookup"><span data-stu-id="9773c-562">Int32</span></span>|<span data-ttu-id="9773c-563">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="9773c-563">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="9773c-564">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9773c-564">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="9773c-565">Int32</span><span class="sxs-lookup"><span data-stu-id="9773c-565">Int32</span></span>|<span data-ttu-id="9773c-566">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="9773c-566">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="9773c-567">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="9773c-567">Valid values 0 to 4</span></span>|
|<span data-ttu-id="9773c-568">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="9773c-568">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="9773c-569">Int32</span><span class="sxs-lookup"><span data-stu-id="9773c-569">Int32</span></span>|<span data-ttu-id="9773c-570">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="9773c-570">Number of previous passcodes to block.</span></span> <span data-ttu-id="9773c-571">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="9773c-571">Valid values 1 to 24</span></span>|
|<span data-ttu-id="9773c-572">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="9773c-572">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="9773c-573">Int32</span><span class="sxs-lookup"><span data-stu-id="9773c-573">Int32</span></span>|<span data-ttu-id="9773c-574">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="9773c-574">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="9773c-575">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="9773c-575">Valid values 4 to 11</span></span>|
|<span data-ttu-id="9773c-576">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="9773c-576">passcodeRequiredType</span></span>|[<span data-ttu-id="9773c-577">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="9773c-577">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9773c-578">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="9773c-578">Type of passcode that is required.</span></span> <span data-ttu-id="9773c-579">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="9773c-579">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9773c-580">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="9773c-580">passcodeRequired</span></span>|<span data-ttu-id="9773c-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-581">Boolean</span></span>|<span data-ttu-id="9773c-582">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="9773c-582">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="9773c-583">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-583">podcastsBlocked</span></span>|<span data-ttu-id="9773c-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-584">Boolean</span></span>|<span data-ttu-id="9773c-585">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-585">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="9773c-586">Проксимитиблокксетуптоневдевице</span><span class="sxs-lookup"><span data-stu-id="9773c-586">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="9773c-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-587">Boolean</span></span>|<span data-ttu-id="9773c-588">Указывает, следует ли включить запрос на установку находящихся рядом устройств с защищенным устройством.</span><span class="sxs-lookup"><span data-stu-id="9773c-588">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="9773c-589">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="9773c-589">safariBlockAutofill</span></span>|<span data-ttu-id="9773c-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-590">Boolean</span></span>|<span data-ttu-id="9773c-591">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="9773c-591">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="9773c-592">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="9773c-592">safariBlockJavaScript</span></span>|<span data-ttu-id="9773c-593">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-593">Boolean</span></span>|<span data-ttu-id="9773c-594">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="9773c-594">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="9773c-595">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="9773c-595">safariBlockPopups</span></span>|<span data-ttu-id="9773c-596">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-596">Boolean</span></span>|<span data-ttu-id="9773c-597">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="9773c-597">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="9773c-598">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-598">safariBlocked</span></span>|<span data-ttu-id="9773c-599">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-599">Boolean</span></span>|<span data-ttu-id="9773c-600">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="9773c-600">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="9773c-601">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="9773c-601">safariCookieSettings</span></span>|[<span data-ttu-id="9773c-602">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="9773c-602">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="9773c-603">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="9773c-603">Cookie settings for Safari.</span></span> <span data-ttu-id="9773c-604">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="9773c-604">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="9773c-605">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="9773c-605">safariManagedDomains</span></span>|<span data-ttu-id="9773c-606">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9773c-606">String collection</span></span>|<span data-ttu-id="9773c-607">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="9773c-607">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="9773c-608">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="9773c-608">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="9773c-609">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9773c-609">String collection</span></span>|<span data-ttu-id="9773c-610">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="9773c-610">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="9773c-611">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-611">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="9773c-612">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="9773c-612">safariRequireFraudWarning</span></span>|<span data-ttu-id="9773c-613">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-613">Boolean</span></span>|<span data-ttu-id="9773c-614">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="9773c-614">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="9773c-615">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-615">screenCaptureBlocked</span></span>|<span data-ttu-id="9773c-616">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-616">Boolean</span></span>|<span data-ttu-id="9773c-617">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="9773c-617">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="9773c-618">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-618">siriBlocked</span></span>|<span data-ttu-id="9773c-619">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-619">Boolean</span></span>|<span data-ttu-id="9773c-620">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="9773c-620">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="9773c-621">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="9773c-621">siriBlockedWhenLocked</span></span>|<span data-ttu-id="9773c-622">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-622">Boolean</span></span>|<span data-ttu-id="9773c-623">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="9773c-623">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="9773c-624">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="9773c-624">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="9773c-625">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-625">Boolean</span></span>|<span data-ttu-id="9773c-626">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="9773c-626">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="9773c-627">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="9773c-627">siriRequireProfanityFilter</span></span>|<span data-ttu-id="9773c-628">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-628">Boolean</span></span>|<span data-ttu-id="9773c-629">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="9773c-629">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="9773c-630">Софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="9773c-630">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="9773c-631">Int32</span><span class="sxs-lookup"><span data-stu-id="9773c-631">Int32</span></span>|<span data-ttu-id="9773c-632">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="9773c-632">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="9773c-633">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="9773c-633">Valid values 0 to 90</span></span>|
|<span data-ttu-id="9773c-634">Софтвареупдатесфорцеделайед</span><span class="sxs-lookup"><span data-stu-id="9773c-634">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="9773c-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-635">Boolean</span></span>|<span data-ttu-id="9773c-636">Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-636">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-637">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="9773c-637">spotlightBlockInternetResults</span></span>|<span data-ttu-id="9773c-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-638">Boolean</span></span>|<span data-ttu-id="9773c-639">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="9773c-639">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="9773c-640">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-640">voiceDialingBlocked</span></span>|<span data-ttu-id="9773c-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-641">Boolean</span></span>|<span data-ttu-id="9773c-642">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="9773c-642">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="9773c-643">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="9773c-643">wallpaperBlockModification</span></span>|<span data-ttu-id="9773c-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-644">Boolean</span></span>|<span data-ttu-id="9773c-645">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-645">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="9773c-646">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="9773c-646">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="9773c-647">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-647">Boolean</span></span>|<span data-ttu-id="9773c-648">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9773c-648">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9773c-649">Классрумфорцерекуестпермиссионтолеавеклассес</span><span class="sxs-lookup"><span data-stu-id="9773c-649">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="9773c-650">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-650">Boolean</span></span>|<span data-ttu-id="9773c-651">Указывает, является ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса (iOS 11,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-651">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="9773c-652">Кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="9773c-652">keychainBlockCloudSync</span></span>|<span data-ttu-id="9773c-653">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-653">Boolean</span></span>|<span data-ttu-id="9773c-654">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud.</span><span class="sxs-lookup"><span data-stu-id="9773c-654">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="9773c-655">Пкиблоккотаупдатес</span><span class="sxs-lookup"><span data-stu-id="9773c-655">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="9773c-656">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-656">Boolean</span></span>|<span data-ttu-id="9773c-657">Указывает, блокируются ли обновления PKI беспроводной сети.</span><span class="sxs-lookup"><span data-stu-id="9773c-657">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="9773c-658">Если задать для этого ограничения значение false, проверки CRL и OCSP (iOS 7,0 и более поздних версий) не отключаются.</span><span class="sxs-lookup"><span data-stu-id="9773c-658">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="9773c-659">Привацифорцелимитадтраккинг</span><span class="sxs-lookup"><span data-stu-id="9773c-659">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="9773c-660">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-660">Boolean</span></span>|<span data-ttu-id="9773c-661">Указывает, ограничено ли отслеживание AD. (iOS 7,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-661">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="9773c-662">Ентерприсебукблоккбаккуп</span><span class="sxs-lookup"><span data-stu-id="9773c-662">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="9773c-663">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-663">Boolean</span></span>|<span data-ttu-id="9773c-664">Указывает, блокируется ли резервное копирование корпоративной книги.</span><span class="sxs-lookup"><span data-stu-id="9773c-664">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="9773c-665">Ентерприсебукблоккметадатасинк</span><span class="sxs-lookup"><span data-stu-id="9773c-665">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="9773c-666">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-666">Boolean</span></span>|<span data-ttu-id="9773c-667">Указывает, блокируется ли синхронизация заметок и выделений корпоративных книг.</span><span class="sxs-lookup"><span data-stu-id="9773c-667">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="9773c-668">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="9773c-668">airPrintBlocked</span></span>|<span data-ttu-id="9773c-669">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-669">Boolean</span></span>|<span data-ttu-id="9773c-670">Указывает, заблокировано ли Аирпринт (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-670">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="9773c-671">Аирпринтблокккредентиалсстораже</span><span class="sxs-lookup"><span data-stu-id="9773c-671">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="9773c-672">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-672">Boolean</span></span>|<span data-ttu-id="9773c-673">Указывает, заблокировано ли хранение цепочки ключей имени пользователя и пароля для Аирпринт (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-673">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="9773c-674">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="9773c-674">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="9773c-675">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-675">Boolean</span></span>|<span data-ttu-id="9773c-676">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-676">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="9773c-677">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="9773c-677">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="9773c-678">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-678">Boolean</span></span>|<span data-ttu-id="9773c-679">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="9773c-679">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="9773c-680">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-680">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="9773c-681">Блокксистемаппремовал</span><span class="sxs-lookup"><span data-stu-id="9773c-681">blockSystemAppRemoval</span></span>|<span data-ttu-id="9773c-682">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-682">Boolean</span></span>|<span data-ttu-id="9773c-683">Указывает, заблокировано ли удаление системных приложений с устройства на контролируемом устройстве (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-683">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="9773c-684">Впнблокккреатион</span><span class="sxs-lookup"><span data-stu-id="9773c-684">vpnBlockCreation</span></span>|<span data-ttu-id="9773c-685">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-685">Boolean</span></span>|<span data-ttu-id="9773c-686">Указывает, блокируется ли создание конфигураций VPN (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-686">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="9773c-687">Аппремовалблоккед</span><span class="sxs-lookup"><span data-stu-id="9773c-687">appRemovalBlocked</span></span>|<span data-ttu-id="9773c-688">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-688">Boolean</span></span>|<span data-ttu-id="9773c-689">Указывает, разрешено ли удаление приложений.</span><span class="sxs-lookup"><span data-stu-id="9773c-689">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="9773c-690">Усбрестриктедмодеблоккед</span><span class="sxs-lookup"><span data-stu-id="9773c-690">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="9773c-691">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-691">Boolean</span></span>|<span data-ttu-id="9773c-692">Указывает, разрешена ли подключаться к стандарту USB, пока устройство заблокировано (iOS 11.4.1 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-692">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="9773c-693">Пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="9773c-693">passwordBlockAutoFill</span></span>|<span data-ttu-id="9773c-694">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-694">Boolean</span></span>|<span data-ttu-id="9773c-695">Указывает, разрешена ли функция автозаполнения паролей (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-695">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="9773c-696">Пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="9773c-696">passwordBlockProximityRequests</span></span>|<span data-ttu-id="9773c-697">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-697">Boolean</span></span>|<span data-ttu-id="9773c-698">Указывает, следует ли запретить запрашивать пароли с близлежащих устройств (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-698">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="9773c-699">Пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="9773c-699">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="9773c-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-700">Boolean</span></span>|<span data-ttu-id="9773c-701">Указывает, следует ли заблокировать общий доступ к паролям с помощью AirDrop паролей iOS 12,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="9773c-701">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="9773c-702">Датеандтимефорцесетаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="9773c-702">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="9773c-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-703">Boolean</span></span>|<span data-ttu-id="9773c-704">Указывает, включена ли функция даты и времени "автоматически задано" и не может быть отключена пользователем (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-704">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="9773c-705">Контактсалловманажедтаунманажедврите</span><span class="sxs-lookup"><span data-stu-id="9773c-705">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="9773c-706">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-706">Boolean</span></span>|<span data-ttu-id="9773c-707">Указывает, могут ли управляемые приложения записывать контакты в неуправляемые учетные записи контактов (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9773c-707">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="9773c-708">Контактсалловунманажедтоманажедреад</span><span class="sxs-lookup"><span data-stu-id="9773c-708">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="9773c-709">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-709">Boolean</span></span>|<span data-ttu-id="9773c-710">Указывает, могут ли неуправляемые приложения читать из управляемых учетных записей контактов (iOS 12,0 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="9773c-710">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="9773c-711">Целлуларблоккперсоналхотспотмодификатион</span><span class="sxs-lookup"><span data-stu-id="9773c-711">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="9773c-712">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-712">Boolean</span></span>|<span data-ttu-id="9773c-713">Указывает, следует ли запретить пользователю изменять параметр личных гиперобъектов (iOS 12,2 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="9773c-713">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="9773c-714">Сиридисаблесерверлоггинг</span><span class="sxs-lookup"><span data-stu-id="9773c-714">siriDisableServerLogging</span></span>|<span data-ttu-id="9773c-715">Boolean</span><span class="sxs-lookup"><span data-stu-id="9773c-715">Boolean</span></span>|<span data-ttu-id="9773c-716">Указывает, отключено ли ведение журнала Siri на стороне сервера (iOS 12,2 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="9773c-716">Indicates whether or not server-side Siri logging is disabled (iOS 12.2 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="9773c-717">Ответ</span><span class="sxs-lookup"><span data-stu-id="9773c-717">Response</span></span>
<span data-ttu-id="9773c-718">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9773c-718">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9773c-719">Пример</span><span class="sxs-lookup"><span data-stu-id="9773c-719">Example</span></span>

### <a name="request"></a><span data-ttu-id="9773c-720">Запрос</span><span class="sxs-lookup"><span data-stu-id="9773c-720">Request</span></span>
<span data-ttu-id="9773c-721">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9773c-721">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10159

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
  "siriDisableServerLogging": true
}
```

### <a name="response"></a><span data-ttu-id="9773c-722">Отклик</span><span class="sxs-lookup"><span data-stu-id="9773c-722">Response</span></span>
<span data-ttu-id="9773c-p142">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9773c-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10331

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
  "siriDisableServerLogging": true
}
```





