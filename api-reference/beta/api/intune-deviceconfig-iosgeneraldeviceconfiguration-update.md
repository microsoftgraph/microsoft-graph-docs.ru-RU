---
title: Обновление объекта iosGeneralDeviceConfiguration
description: Обновление свойств объекта iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6f6bea4ac6012a2f7b6fcd9c3d57bdb8d4b46555
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867233"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="ddb91-103">Обновление объекта iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ddb91-103">Update iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="ddb91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddb91-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddb91-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb91-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddb91-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddb91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddb91-107">Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-107">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ddb91-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ddb91-108">Prerequisites</span></span>
<span data-ttu-id="ddb91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ddb91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddb91-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ddb91-111">Permission type</span></span>|<span data-ttu-id="ddb91-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ddb91-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddb91-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ddb91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ddb91-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb91-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ddb91-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ddb91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddb91-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddb91-116">Not supported.</span></span>|
|<span data-ttu-id="ddb91-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ddb91-117">Application</span></span>|<span data-ttu-id="ddb91-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddb91-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddb91-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ddb91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ddb91-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ddb91-120">Request headers</span></span>
|<span data-ttu-id="ddb91-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ddb91-121">Header</span></span>|<span data-ttu-id="ddb91-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ddb91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddb91-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ddb91-123">Authorization</span></span>|<span data-ttu-id="ddb91-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ddb91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddb91-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ddb91-125">Accept</span></span>|<span data-ttu-id="ddb91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ddb91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddb91-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ddb91-127">Request body</span></span>
<span data-ttu-id="ddb91-128">В тексте запроса добавьте представление объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddb91-128">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="ddb91-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-129">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="ddb91-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddb91-130">Property</span></span>|<span data-ttu-id="ddb91-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ddb91-131">Type</span></span>|<span data-ttu-id="ddb91-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ddb91-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddb91-133">id</span><span class="sxs-lookup"><span data-stu-id="ddb91-133">id</span></span>|<span data-ttu-id="ddb91-134">String</span><span class="sxs-lookup"><span data-stu-id="ddb91-134">String</span></span>|<span data-ttu-id="ddb91-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ddb91-135">Key of the entity.</span></span> <span data-ttu-id="ddb91-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb91-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddb91-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ddb91-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddb91-138">DateTimeOffset</span></span>|<span data-ttu-id="ddb91-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ddb91-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ddb91-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb91-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ddb91-141">roleScopeTagIds</span></span>|<span data-ttu-id="ddb91-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ddb91-142">String collection</span></span>|<span data-ttu-id="ddb91-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="ddb91-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ddb91-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb91-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ddb91-145">supportsScopeTags</span></span>|<span data-ttu-id="ddb91-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-146">Boolean</span></span>|<span data-ttu-id="ddb91-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ddb91-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ddb91-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="ddb91-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ddb91-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ddb91-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ddb91-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ddb91-150">This property is read-only.</span></span> <span data-ttu-id="ddb91-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb91-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ddb91-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ddb91-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ddb91-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ddb91-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ddb91-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ddb91-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb91-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ddb91-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ddb91-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ddb91-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ddb91-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ddb91-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ddb91-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb91-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ddb91-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ddb91-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ddb91-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ddb91-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ddb91-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ddb91-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb91-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddb91-164">createdDateTime</span></span>|<span data-ttu-id="ddb91-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddb91-165">DateTimeOffset</span></span>|<span data-ttu-id="ddb91-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ddb91-166">DateTime the object was created.</span></span> <span data-ttu-id="ddb91-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb91-168">description</span><span class="sxs-lookup"><span data-stu-id="ddb91-168">description</span></span>|<span data-ttu-id="ddb91-169">String</span><span class="sxs-lookup"><span data-stu-id="ddb91-169">String</span></span>|<span data-ttu-id="ddb91-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ddb91-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ddb91-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb91-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ddb91-172">displayName</span></span>|<span data-ttu-id="ddb91-173">String</span><span class="sxs-lookup"><span data-stu-id="ddb91-173">String</span></span>|<span data-ttu-id="ddb91-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ddb91-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ddb91-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb91-176">version</span><span class="sxs-lookup"><span data-stu-id="ddb91-176">version</span></span>|<span data-ttu-id="ddb91-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ddb91-177">Int32</span></span>|<span data-ttu-id="ddb91-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ddb91-178">Version of the device configuration.</span></span> <span data-ttu-id="ddb91-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ddb91-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddb91-180">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-180">accountBlockModification</span></span>|<span data-ttu-id="ddb91-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-181">Boolean</span></span>|<span data-ttu-id="ddb91-182">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-182">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-183">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="ddb91-183">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="ddb91-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-184">Boolean</span></span>|<span data-ttu-id="ddb91-185">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-185">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="ddb91-186">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-186">airDropBlocked</span></span>|<span data-ttu-id="ddb91-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-187">Boolean</span></span>|<span data-ttu-id="ddb91-188">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-188">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-189">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="ddb91-189">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="ddb91-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-190">Boolean</span></span>|<span data-ttu-id="ddb91-191">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-191">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddb91-192">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="ddb91-192">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="ddb91-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-193">Boolean</span></span>|<span data-ttu-id="ddb91-194">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="ddb91-194">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="ddb91-195">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="ddb91-195">appleWatchBlockPairing</span></span>|<span data-ttu-id="ddb91-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-196">Boolean</span></span>|<span data-ttu-id="ddb91-197">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-197">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddb91-198">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="ddb91-198">appleWatchForceWristDetection</span></span>|<span data-ttu-id="ddb91-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-199">Boolean</span></span>|<span data-ttu-id="ddb91-200">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-200">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="ddb91-201">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-201">appleNewsBlocked</span></span>|<span data-ttu-id="ddb91-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-202">Boolean</span></span>|<span data-ttu-id="ddb91-203">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-203">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddb91-204">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="ddb91-204">appsSingleAppModeList</span></span>|<span data-ttu-id="ddb91-205">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ddb91-205">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ddb91-206">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="ddb91-206">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="ddb91-207">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-207">Supervised only.</span></span> <span data-ttu-id="ddb91-208">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="ddb91-208">iOS 7.0 and later.</span></span> <span data-ttu-id="ddb91-209">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="ddb91-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="ddb91-210">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="ddb91-210">appsVisibilityList</span></span>|<span data-ttu-id="ddb91-211">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ddb91-211">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ddb91-212">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-212">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="ddb91-213">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ddb91-213">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ddb91-214">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="ddb91-214">appsVisibilityListType</span></span>|[<span data-ttu-id="ddb91-215">appListType</span><span class="sxs-lookup"><span data-stu-id="ddb91-215">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="ddb91-216">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="ddb91-216">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="ddb91-217">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="ddb91-217">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ddb91-218">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="ddb91-218">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="ddb91-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-219">Boolean</span></span>|<span data-ttu-id="ddb91-220">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-220">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddb91-221">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-221">appStoreBlocked</span></span>|<span data-ttu-id="ddb91-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-222">Boolean</span></span>|<span data-ttu-id="ddb91-223">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="ddb91-223">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="ddb91-224">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-224">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="ddb91-225">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="ddb91-225">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="ddb91-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-226">Boolean</span></span>|<span data-ttu-id="ddb91-227">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="ddb91-227">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="ddb91-228">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="ddb91-228">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="ddb91-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-229">Boolean</span></span>|<span data-ttu-id="ddb91-230">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="ddb91-230">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="ddb91-231">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-231">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddb91-232">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="ddb91-232">appStoreRequirePassword</span></span>|<span data-ttu-id="ddb91-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-233">Boolean</span></span>|<span data-ttu-id="ddb91-234">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="ddb91-234">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="ddb91-235">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="ddb91-235">autoFillForceAuthentication</span></span>|<span data-ttu-id="ddb91-236">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-236">Boolean</span></span>|<span data-ttu-id="ddb91-237">Указывает, следует ли принудительно использовать проверку подлинности пользователей перед автозаполнением паролей и сведений о кредитных картах в Safari и других приложениях на контролируемых устройствах.</span><span class="sxs-lookup"><span data-stu-id="ddb91-237">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="ddb91-238">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-238">bluetoothBlockModification</span></span>|<span data-ttu-id="ddb91-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-239">Boolean</span></span>|<span data-ttu-id="ddb91-240">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-240">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="ddb91-241">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-241">cameraBlocked</span></span>|<span data-ttu-id="ddb91-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-242">Boolean</span></span>|<span data-ttu-id="ddb91-243">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="ddb91-243">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="ddb91-244">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-244">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="ddb91-245">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="ddb91-245">cellularBlockDataRoaming</span></span>|<span data-ttu-id="ddb91-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-246">Boolean</span></span>|<span data-ttu-id="ddb91-247">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="ddb91-247">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="ddb91-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="ddb91-248">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="ddb91-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-249">Boolean</span></span>|<span data-ttu-id="ddb91-250">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="ddb91-250">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="ddb91-251">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-251">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="ddb91-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-252">Boolean</span></span>|<span data-ttu-id="ddb91-253">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-253">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-254">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="ddb91-254">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="ddb91-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-255">Boolean</span></span>|<span data-ttu-id="ddb91-256">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="ddb91-256">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="ddb91-257">cellularBlockPlanModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-257">cellularBlockPlanModification</span></span>|<span data-ttu-id="ddb91-258">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-258">Boolean</span></span>|<span data-ttu-id="ddb91-259">Указывает, следует ли разрешить пользователям изменять параметры сотовой программы на контролируемом устройстве.</span><span class="sxs-lookup"><span data-stu-id="ddb91-259">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="ddb91-260">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="ddb91-260">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="ddb91-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-261">Boolean</span></span>|<span data-ttu-id="ddb91-262">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="ddb91-262">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="ddb91-263">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="ddb91-263">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="ddb91-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-264">Boolean</span></span>|<span data-ttu-id="ddb91-265">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="ddb91-265">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="ddb91-266">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ddb91-266">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="ddb91-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-267">Boolean</span></span>|<span data-ttu-id="ddb91-268">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-268">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ddb91-269">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="ddb91-269">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="ddb91-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-270">Boolean</span></span>|<span data-ttu-id="ddb91-271">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-271">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-272">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="ddb91-272">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="ddb91-273">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-273">Boolean</span></span>|<span data-ttu-id="ddb91-274">Указывает, следует ли автоматически давать разрешения на запросы преподавателя, не подсказывая учащемуся, когда устройство находится в контролируемом режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-274">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-275">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="ddb91-275">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="ddb91-276">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-276">Boolean</span></span>|<span data-ttu-id="ddb91-277">Указывает, следует ли разрешить преподавателю заблокировать приложения или устройство без запроса учащегося.</span><span class="sxs-lookup"><span data-stu-id="ddb91-277">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="ddb91-278">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-278">Supervised only.</span></span>|
|<span data-ttu-id="ddb91-279">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="ddb91-279">compliantAppsList</span></span>|<span data-ttu-id="ddb91-280">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="ddb91-280">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="ddb91-281">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="ddb91-281">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="ddb91-282">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ddb91-282">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="ddb91-283">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="ddb91-283">compliantAppListType</span></span>|[<span data-ttu-id="ddb91-284">appListType</span><span class="sxs-lookup"><span data-stu-id="ddb91-284">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="ddb91-285">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="ddb91-285">List that is in the AppComplianceList.</span></span> <span data-ttu-id="ddb91-286">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="ddb91-286">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="ddb91-287">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="ddb91-287">configurationProfileBlockChanges</span></span>|<span data-ttu-id="ddb91-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-288">Boolean</span></span>|<span data-ttu-id="ddb91-289">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-289">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-290">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-290">definitionLookupBlocked</span></span>|<span data-ttu-id="ddb91-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-291">Boolean</span></span>|<span data-ttu-id="ddb91-292">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-292">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="ddb91-293">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="ddb91-293">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="ddb91-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-294">Boolean</span></span>|<span data-ttu-id="ddb91-295">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-295">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-296">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="ddb91-296">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="ddb91-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-297">Boolean</span></span>|<span data-ttu-id="ddb91-298">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-298">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-299">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-299">deviceBlockNameModification</span></span>|<span data-ttu-id="ddb91-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-300">Boolean</span></span>|<span data-ttu-id="ddb91-301">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-301">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddb91-302">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="ddb91-302">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="ddb91-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-303">Boolean</span></span>|<span data-ttu-id="ddb91-304">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="ddb91-304">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="ddb91-305">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-305">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="ddb91-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-306">Boolean</span></span>|<span data-ttu-id="ddb91-307">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-307">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="ddb91-308">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="ddb91-308">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="ddb91-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-309">Boolean</span></span>|<span data-ttu-id="ddb91-310">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="ddb91-310">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="ddb91-311">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="ddb91-311">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="ddb91-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-312">Boolean</span></span>|<span data-ttu-id="ddb91-313">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="ddb91-313">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="ddb91-314">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="ddb91-314">emailInDomainSuffixes</span></span>|<span data-ttu-id="ddb91-315">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ddb91-315">String collection</span></span>|<span data-ttu-id="ddb91-316">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="ddb91-316">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="ddb91-317">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="ddb91-317">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="ddb91-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-318">Boolean</span></span>|<span data-ttu-id="ddb91-319">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="ddb91-319">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="ddb91-320">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-320">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="ddb91-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-321">Boolean</span></span>|<span data-ttu-id="ddb91-322">\[Неоконфигурированная настройка этого параметра и установка значения "true" не влияет \] на устройство.</span><span class="sxs-lookup"><span data-stu-id="ddb91-322">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="ddb91-323">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-323">esimBlockModification</span></span>|<span data-ttu-id="ddb91-324">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-324">Boolean</span></span>|<span data-ttu-id="ddb91-325">Указывает, следует ли разрешить добавление или удаление сотовых планов на eSIM контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="ddb91-325">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="ddb91-326">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-326">faceTimeBlocked</span></span>|<span data-ttu-id="ddb91-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-327">Boolean</span></span>|<span data-ttu-id="ddb91-328">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="ddb91-328">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="ddb91-329">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-329">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="ddb91-330">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-330">findMyFriendsBlocked</span></span>|<span data-ttu-id="ddb91-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-331">Boolean</span></span>|<span data-ttu-id="ddb91-332">Указывает, следует ли блокировать изменения в "Найти друзей", когда устройство находится в режиме контроля.</span><span class="sxs-lookup"><span data-stu-id="ddb91-332">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-333">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="ddb91-333">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="ddb91-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-334">Boolean</span></span>|<span data-ttu-id="ddb91-335">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="ddb91-335">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="ddb91-336">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-336">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="ddb91-337">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="ddb91-337">gamingBlockMultiplayer</span></span>|<span data-ttu-id="ddb91-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-338">Boolean</span></span>|<span data-ttu-id="ddb91-339">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="ddb91-339">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="ddb91-340">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-340">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="ddb91-341">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-341">gameCenterBlocked</span></span>|<span data-ttu-id="ddb91-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-342">Boolean</span></span>|<span data-ttu-id="ddb91-343">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-343">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-344">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-344">hostPairingBlocked</span></span>|<span data-ttu-id="ddb91-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-345">Boolean</span></span>|<span data-ttu-id="ddb91-346">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-346">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-347">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-347">iBooksStoreBlocked</span></span>|<span data-ttu-id="ddb91-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-348">Boolean</span></span>|<span data-ttu-id="ddb91-349">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-349">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-350">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="ddb91-350">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="ddb91-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-351">Boolean</span></span>|<span data-ttu-id="ddb91-352">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="ddb91-352">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="ddb91-353">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="ddb91-353">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="ddb91-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-354">Boolean</span></span>|<span data-ttu-id="ddb91-355">Указывает, следует ли блокировать пользователю продолжение работы, начатой на устройстве iOS, на другое устройство iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="ddb91-355">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="ddb91-356">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="ddb91-356">iCloudBlockBackup</span></span>|<span data-ttu-id="ddb91-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-357">Boolean</span></span>|<span data-ttu-id="ddb91-358">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="ddb91-358">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="ddb91-359">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-359">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="ddb91-360">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="ddb91-360">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="ddb91-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-361">Boolean</span></span>|<span data-ttu-id="ddb91-362">Указывает, следует ли блокировать синхронизацию документов iCloud. Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-362">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="ddb91-363">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="ddb91-363">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="ddb91-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-364">Boolean</span></span>|<span data-ttu-id="ddb91-365">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="ddb91-365">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="ddb91-366">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="ddb91-366">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="ddb91-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-367">Boolean</span></span>|<span data-ttu-id="ddb91-368">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="ddb91-368">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="ddb91-369">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="ddb91-369">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="ddb91-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-370">Boolean</span></span>|<span data-ttu-id="ddb91-371">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="ddb91-371">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="ddb91-372">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="ddb91-372">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="ddb91-373">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-373">Boolean</span></span>|<span data-ttu-id="ddb91-374">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="ddb91-374">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="ddb91-375">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="ddb91-375">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="ddb91-376">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-376">Boolean</span></span>|<span data-ttu-id="ddb91-377">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="ddb91-377">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="ddb91-378">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="ddb91-378">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="ddb91-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-379">Boolean</span></span>|<span data-ttu-id="ddb91-380">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="ddb91-380">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="ddb91-381">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-381">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="ddb91-382">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="ddb91-382">iTunesBlockMusicService</span></span>|<span data-ttu-id="ddb91-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-383">Boolean</span></span>|<span data-ttu-id="ddb91-384">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-384">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="ddb91-385">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="ddb91-385">iTunesBlockRadio</span></span>|<span data-ttu-id="ddb91-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-386">Boolean</span></span>|<span data-ttu-id="ddb91-387">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-387">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ddb91-388">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="ddb91-388">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="ddb91-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-389">Boolean</span></span>|<span data-ttu-id="ddb91-390">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-390">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ddb91-391">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="ddb91-391">keyboardBlockDictation</span></span>|<span data-ttu-id="ddb91-392">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-392">Boolean</span></span>|<span data-ttu-id="ddb91-393">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-393">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-394">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="ddb91-394">keyboardBlockPredictive</span></span>|<span data-ttu-id="ddb91-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-395">Boolean</span></span>|<span data-ttu-id="ddb91-396">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-396">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ddb91-397">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="ddb91-397">keyboardBlockShortcuts</span></span>|<span data-ttu-id="ddb91-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-398">Boolean</span></span>|<span data-ttu-id="ddb91-399">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-399">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddb91-400">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="ddb91-400">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="ddb91-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-401">Boolean</span></span>|<span data-ttu-id="ddb91-402">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-402">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="ddb91-403">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="ddb91-403">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="ddb91-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-404">Boolean</span></span>|<span data-ttu-id="ddb91-405">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-405">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-406">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="ddb91-406">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="ddb91-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-407">Boolean</span></span>|<span data-ttu-id="ddb91-408">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-408">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-409">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="ddb91-409">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="ddb91-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-410">Boolean</span></span>|<span data-ttu-id="ddb91-411">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-411">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="ddb91-412">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="ddb91-412">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="ddb91-413">Вместо этого используйте KioskModeBlockAutoLock.</span><span class="sxs-lookup"><span data-stu-id="ddb91-413">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="ddb91-414">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="ddb91-414">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="ddb91-415">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-415">Boolean</span></span>|<span data-ttu-id="ddb91-416">Указывает, следует ли блокировать автоматическую блокировку устройства во время работы в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-416">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-417">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="ddb91-417">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="ddb91-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-418">Boolean</span></span>|<span data-ttu-id="ddb91-419">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-419">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-420">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="ddb91-420">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="ddb91-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-421">Boolean</span></span>|<span data-ttu-id="ddb91-422">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-422">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="ddb91-423">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="ddb91-423">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="ddb91-424">Вместо этого используйте KioskModeBlockRingerSwitch.</span><span class="sxs-lookup"><span data-stu-id="ddb91-424">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="ddb91-425">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="ddb91-425">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="ddb91-426">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-426">Boolean</span></span>|<span data-ttu-id="ddb91-427">Указывает, следует ли блокировать использование переключателя звона во время работы в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-427">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-428">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="ddb91-428">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="ddb91-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-429">Boolean</span></span>|<span data-ttu-id="ddb91-430">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-430">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="ddb91-431">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="ddb91-431">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="ddb91-432">Вместо этого используйте kioskModeBlockScreenRotation.</span><span class="sxs-lookup"><span data-stu-id="ddb91-432">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="ddb91-433">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="ddb91-433">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="ddb91-434">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-434">Boolean</span></span>|<span data-ttu-id="ddb91-435">Указывает, следует ли блокировать поворот экрана во время работы в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-435">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-436">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="ddb91-436">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="ddb91-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-437">Boolean</span></span>|<span data-ttu-id="ddb91-438">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-438">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="ddb91-439">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="ddb91-439">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="ddb91-440">Вместо этого используйте kioskModeBlockSleepButton.</span><span class="sxs-lookup"><span data-stu-id="ddb91-440">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="ddb91-441">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="ddb91-441">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="ddb91-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-442">Boolean</span></span>|<span data-ttu-id="ddb91-443">Указывает, следует ли блокировать использование кнопки сна во время работы в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-443">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-444">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="ddb91-444">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="ddb91-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-445">Boolean</span></span>|<span data-ttu-id="ddb91-446">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-446">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="ddb91-447">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="ddb91-447">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="ddb91-448">Вместо этого используйте kioskModeBlockTouchscreen.</span><span class="sxs-lookup"><span data-stu-id="ddb91-448">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="ddb91-449">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="ddb91-449">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="ddb91-450">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-450">Boolean</span></span>|<span data-ttu-id="ddb91-451">Указывает, следует ли блокировать использование сенсорного экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-451">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-452">kioskModeEnableVoiceControl</span><span class="sxs-lookup"><span data-stu-id="ddb91-452">kioskModeEnableVoiceControl</span></span>|<span data-ttu-id="ddb91-453">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-453">Boolean</span></span>|<span data-ttu-id="ddb91-454">Указывает, следует ли включить голосовое управление в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-454">Indicates whether or not to enable voice control in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-455">kioskModeAllowVoiceControlModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-455">kioskModeAllowVoiceControlModification</span></span>|<span data-ttu-id="ddb91-456">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-456">Boolean</span></span>|<span data-ttu-id="ddb91-457">Указывает, следует ли разрешить пользователю управлять голосом в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-457">Indicates whether or not to allow the user to toggle voice control in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-458">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="ddb91-458">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="ddb91-459">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-459">Boolean</span></span>|<span data-ttu-id="ddb91-460">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-460">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-461">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="ddb91-461">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="ddb91-462">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-462">Boolean</span></span>|<span data-ttu-id="ddb91-463">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-463">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="ddb91-464">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="ddb91-464">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="ddb91-465">Вместо этого используйте kioskModeBlockVolumeButtons.</span><span class="sxs-lookup"><span data-stu-id="ddb91-465">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="ddb91-466">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="ddb91-466">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="ddb91-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-467">Boolean</span></span>|<span data-ttu-id="ddb91-468">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="ddb91-468">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="ddb91-469">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="ddb91-469">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="ddb91-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-470">Boolean</span></span>|<span data-ttu-id="ddb91-471">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-471">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-472">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ddb91-472">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="ddb91-473">String</span><span class="sxs-lookup"><span data-stu-id="ddb91-473">String</span></span>|<span data-ttu-id="ddb91-474">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-474">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="ddb91-475">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="ddb91-475">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="ddb91-476">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="ddb91-476">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="ddb91-477">String</span><span class="sxs-lookup"><span data-stu-id="ddb91-477">String</span></span>|<span data-ttu-id="ddb91-478">ID для встроенных приложений, которые можно использовать для режима киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-478">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="ddb91-479">Используется, когда не заданы KioskModeManagedAppId и KioskModeAppStoreUrl.</span><span class="sxs-lookup"><span data-stu-id="ddb91-479">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="ddb91-480">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="ddb91-480">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="ddb91-481">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-481">Boolean</span></span>|<span data-ttu-id="ddb91-482">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-482">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-483">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="ddb91-483">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="ddb91-484">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-484">Boolean</span></span>|<span data-ttu-id="ddb91-485">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-485">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-486">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="ddb91-486">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="ddb91-487">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-487">Boolean</span></span>|<span data-ttu-id="ddb91-488">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-488">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-489">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="ddb91-489">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="ddb91-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-490">Boolean</span></span>|<span data-ttu-id="ddb91-491">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-491">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-492">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="ddb91-492">kioskModeRequireZoom</span></span>|<span data-ttu-id="ddb91-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-493">Boolean</span></span>|<span data-ttu-id="ddb91-494">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-494">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="ddb91-495">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="ddb91-495">kioskModeManagedAppId</span></span>|<span data-ttu-id="ddb91-496">String</span><span class="sxs-lookup"><span data-stu-id="ddb91-496">String</span></span>|<span data-ttu-id="ddb91-497">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-497">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="ddb91-498">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="ddb91-498">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="ddb91-499">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="ddb91-499">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="ddb91-500">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-500">Boolean</span></span>|<span data-ttu-id="ddb91-501">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="ddb91-501">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="ddb91-502">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="ddb91-502">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="ddb91-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-503">Boolean</span></span>|<span data-ttu-id="ddb91-504">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="ddb91-504">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="ddb91-505">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="ddb91-505">lockScreenBlockPassbook</span></span>|<span data-ttu-id="ddb91-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-506">Boolean</span></span>|<span data-ttu-id="ddb91-507">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="ddb91-507">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="ddb91-508">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="ddb91-508">lockScreenBlockTodayView</span></span>|<span data-ttu-id="ddb91-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-509">Boolean</span></span>|<span data-ttu-id="ddb91-510">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="ddb91-510">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="ddb91-511">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ddb91-511">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="ddb91-512">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="ddb91-512">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="ddb91-513">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="ddb91-513">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="ddb91-514">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ddb91-514">mediaContentRatingCanada</span></span>|[<span data-ttu-id="ddb91-515">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="ddb91-515">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="ddb91-516">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="ddb91-516">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="ddb91-517">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ddb91-517">mediaContentRatingFrance</span></span>|[<span data-ttu-id="ddb91-518">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="ddb91-518">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="ddb91-519">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="ddb91-519">Media content rating settings for France</span></span>|
|<span data-ttu-id="ddb91-520">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ddb91-520">mediaContentRatingGermany</span></span>|[<span data-ttu-id="ddb91-521">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="ddb91-521">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="ddb91-522">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="ddb91-522">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="ddb91-523">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ddb91-523">mediaContentRatingIreland</span></span>|[<span data-ttu-id="ddb91-524">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="ddb91-524">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="ddb91-525">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="ddb91-525">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="ddb91-526">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ddb91-526">mediaContentRatingJapan</span></span>|[<span data-ttu-id="ddb91-527">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ddb91-527">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="ddb91-528">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="ddb91-528">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="ddb91-529">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ddb91-529">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="ddb91-530">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ddb91-530">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="ddb91-531">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="ddb91-531">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="ddb91-532">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ddb91-532">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="ddb91-533">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="ddb91-533">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="ddb91-534">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="ddb91-534">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="ddb91-535">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ddb91-535">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="ddb91-536">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ddb91-536">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="ddb91-537">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="ddb91-537">Media content rating settings for United States</span></span>|
|<span data-ttu-id="ddb91-538">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="ddb91-538">networkUsageRules</span></span>|<span data-ttu-id="ddb91-539">Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="ddb91-539">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="ddb91-540">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="ddb91-540">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="ddb91-541">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ddb91-541">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="ddb91-542">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="ddb91-542">mediaContentRatingApps</span></span>|[<span data-ttu-id="ddb91-543">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="ddb91-543">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="ddb91-544">Параметры оценки контента мультимедиа для приложений.</span><span class="sxs-lookup"><span data-stu-id="ddb91-544">Media content rating settings for Apps.</span></span> <span data-ttu-id="ddb91-545">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="ddb91-545">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="ddb91-546">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-546">messagesBlocked</span></span>|<span data-ttu-id="ddb91-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-547">Boolean</span></span>|<span data-ttu-id="ddb91-548">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="ddb91-548">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="ddb91-549">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-549">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="ddb91-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-550">Boolean</span></span>|<span data-ttu-id="ddb91-551">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-551">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ddb91-552">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="ddb91-552">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="ddb91-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-553">Boolean</span></span>|<span data-ttu-id="ddb91-554">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="ddb91-554">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="ddb91-555">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-555">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="ddb91-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-556">Boolean</span></span>|<span data-ttu-id="ddb91-557">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-557">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-558">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-558">passcodeBlockModification</span></span>|<span data-ttu-id="ddb91-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-559">Boolean</span></span>|<span data-ttu-id="ddb91-560">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-560">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="ddb91-561">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="ddb91-561">passcodeBlockSimple</span></span>|<span data-ttu-id="ddb91-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-562">Boolean</span></span>|<span data-ttu-id="ddb91-563">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="ddb91-563">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="ddb91-564">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ddb91-564">passcodeExpirationDays</span></span>|<span data-ttu-id="ddb91-565">Int32</span><span class="sxs-lookup"><span data-stu-id="ddb91-565">Int32</span></span>|<span data-ttu-id="ddb91-566">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="ddb91-566">Number of days before the passcode expires.</span></span> <span data-ttu-id="ddb91-567">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="ddb91-567">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="ddb91-568">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ddb91-568">passcodeMinimumLength</span></span>|<span data-ttu-id="ddb91-569">Int32</span><span class="sxs-lookup"><span data-stu-id="ddb91-569">Int32</span></span>|<span data-ttu-id="ddb91-570">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="ddb91-570">Minimum length of passcode.</span></span> <span data-ttu-id="ddb91-571">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="ddb91-571">Valid values 4 to 14</span></span>|
|<span data-ttu-id="ddb91-572">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="ddb91-572">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="ddb91-573">Int32</span><span class="sxs-lookup"><span data-stu-id="ddb91-573">Int32</span></span>|<span data-ttu-id="ddb91-574">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="ddb91-574">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="ddb91-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="ddb91-575">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="ddb91-576">Int32</span><span class="sxs-lookup"><span data-stu-id="ddb91-576">Int32</span></span>|<span data-ttu-id="ddb91-577">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ddb91-577">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="ddb91-578">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="ddb91-578">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="ddb91-579">Int32</span><span class="sxs-lookup"><span data-stu-id="ddb91-579">Int32</span></span>|<span data-ttu-id="ddb91-580">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="ddb91-580">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="ddb91-581">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="ddb91-581">Valid values 0 to 4</span></span>|
|<span data-ttu-id="ddb91-582">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="ddb91-582">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="ddb91-583">Int32</span><span class="sxs-lookup"><span data-stu-id="ddb91-583">Int32</span></span>|<span data-ttu-id="ddb91-584">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="ddb91-584">Number of previous passcodes to block.</span></span> <span data-ttu-id="ddb91-585">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="ddb91-585">Valid values 1 to 24</span></span>|
|<span data-ttu-id="ddb91-586">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="ddb91-586">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="ddb91-587">Int32</span><span class="sxs-lookup"><span data-stu-id="ddb91-587">Int32</span></span>|<span data-ttu-id="ddb91-588">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="ddb91-588">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="ddb91-589">Допустимые значения от 2 до 11</span><span class="sxs-lookup"><span data-stu-id="ddb91-589">Valid values 2 to 11</span></span>|
|<span data-ttu-id="ddb91-590">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="ddb91-590">passcodeRequiredType</span></span>|[<span data-ttu-id="ddb91-591">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="ddb91-591">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="ddb91-592">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="ddb91-592">Type of passcode that is required.</span></span> <span data-ttu-id="ddb91-593">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="ddb91-593">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="ddb91-594">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="ddb91-594">passcodeRequired</span></span>|<span data-ttu-id="ddb91-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-595">Boolean</span></span>|<span data-ttu-id="ddb91-596">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="ddb91-596">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="ddb91-597">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-597">podcastsBlocked</span></span>|<span data-ttu-id="ddb91-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-598">Boolean</span></span>|<span data-ttu-id="ddb91-599">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-599">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="ddb91-600">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="ddb91-600">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="ddb91-601">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-601">Boolean</span></span>|<span data-ttu-id="ddb91-602">Указывает, следует ли включить запрос на установку расположенных поблизости устройств с помощью контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="ddb91-602">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="ddb91-603">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="ddb91-603">safariBlockAutofill</span></span>|<span data-ttu-id="ddb91-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-604">Boolean</span></span>|<span data-ttu-id="ddb91-605">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="ddb91-605">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="ddb91-606">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-606">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="ddb91-607">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="ddb91-607">safariBlockJavaScript</span></span>|<span data-ttu-id="ddb91-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-608">Boolean</span></span>|<span data-ttu-id="ddb91-609">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="ddb91-609">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="ddb91-610">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="ddb91-610">safariBlockPopups</span></span>|<span data-ttu-id="ddb91-611">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-611">Boolean</span></span>|<span data-ttu-id="ddb91-612">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="ddb91-612">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="ddb91-613">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-613">safariBlocked</span></span>|<span data-ttu-id="ddb91-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-614">Boolean</span></span>|<span data-ttu-id="ddb91-615">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="ddb91-615">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="ddb91-616">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-616">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="ddb91-617">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ddb91-617">safariCookieSettings</span></span>|[<span data-ttu-id="ddb91-618">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="ddb91-618">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="ddb91-619">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="ddb91-619">Cookie settings for Safari.</span></span> <span data-ttu-id="ddb91-620">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="ddb91-620">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="ddb91-621">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="ddb91-621">safariManagedDomains</span></span>|<span data-ttu-id="ddb91-622">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ddb91-622">String collection</span></span>|<span data-ttu-id="ddb91-623">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="ddb91-623">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="ddb91-624">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="ddb91-624">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="ddb91-625">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ddb91-625">String collection</span></span>|<span data-ttu-id="ddb91-626">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="ddb91-626">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="ddb91-627">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-627">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="ddb91-628">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="ddb91-628">safariRequireFraudWarning</span></span>|<span data-ttu-id="ddb91-629">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-629">Boolean</span></span>|<span data-ttu-id="ddb91-630">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="ddb91-630">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="ddb91-631">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-631">screenCaptureBlocked</span></span>|<span data-ttu-id="ddb91-632">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-632">Boolean</span></span>|<span data-ttu-id="ddb91-633">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="ddb91-633">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="ddb91-634">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-634">siriBlocked</span></span>|<span data-ttu-id="ddb91-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-635">Boolean</span></span>|<span data-ttu-id="ddb91-636">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="ddb91-636">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="ddb91-637">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-637">siriBlockedWhenLocked</span></span>|<span data-ttu-id="ddb91-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-638">Boolean</span></span>|<span data-ttu-id="ddb91-639">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="ddb91-639">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="ddb91-640">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="ddb91-640">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="ddb91-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-641">Boolean</span></span>|<span data-ttu-id="ddb91-642">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="ddb91-642">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="ddb91-643">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="ddb91-643">siriRequireProfanityFilter</span></span>|<span data-ttu-id="ddb91-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-644">Boolean</span></span>|<span data-ttu-id="ddb91-645">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="ddb91-645">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="ddb91-646">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="ddb91-646">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="ddb91-647">Int32</span><span class="sxs-lookup"><span data-stu-id="ddb91-647">Int32</span></span>|<span data-ttu-id="ddb91-648">Задает время, за которое будет отламывно обновление программного обеспечения для контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="ddb91-648">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="ddb91-649">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="ddb91-649">Valid values 0 to 90</span></span>|
|<span data-ttu-id="ddb91-650">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="ddb91-650">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="ddb91-651">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-651">Boolean</span></span>|<span data-ttu-id="ddb91-652">Указывает, задерживать или не задерживать видимость обновлений программного обеспечения, когда устройство находится в контролируемом режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-652">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-653">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="ddb91-653">spotlightBlockInternetResults</span></span>|<span data-ttu-id="ddb91-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-654">Boolean</span></span>|<span data-ttu-id="ddb91-655">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="ddb91-655">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="ddb91-656">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-656">voiceDialingBlocked</span></span>|<span data-ttu-id="ddb91-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-657">Boolean</span></span>|<span data-ttu-id="ddb91-658">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="ddb91-658">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="ddb91-659">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-659">wallpaperBlockModification</span></span>|<span data-ttu-id="ddb91-660">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-660">Boolean</span></span>|<span data-ttu-id="ddb91-661">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="ddb91-661">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="ddb91-662">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="ddb91-662">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="ddb91-663">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-663">Boolean</span></span>|<span data-ttu-id="ddb91-664">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="ddb91-664">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="ddb91-665">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="ddb91-665">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="ddb91-666">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-666">Boolean</span></span>|<span data-ttu-id="ddb91-667">Указывает, будет ли учащийся, зарегистрированный на неугодном курсе через Класс, запрашивать разрешения у преподавателя при попытке покинуть курс (iOS 11.3 и более поздний).</span><span class="sxs-lookup"><span data-stu-id="ddb91-667">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="ddb91-668">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="ddb91-668">keychainBlockCloudSync</span></span>|<span data-ttu-id="ddb91-669">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-669">Boolean</span></span>|<span data-ttu-id="ddb91-670">Указывает, заблокирована ли синхронизация ключей iCloud.</span><span class="sxs-lookup"><span data-stu-id="ddb91-670">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="ddb91-671">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-671">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="ddb91-672">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="ddb91-672">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="ddb91-673">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-673">Boolean</span></span>|<span data-ttu-id="ddb91-674">Указывает, заблокированы ли обновления PKI на воздухе.</span><span class="sxs-lookup"><span data-stu-id="ddb91-674">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="ddb91-675">Настройка этого ограничения для false не отключает проверки CRL и OCSP (iOS 7.0 и более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-675">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="ddb91-676">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="ddb91-676">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="ddb91-677">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-677">Boolean</span></span>|<span data-ttu-id="ddb91-678">Указывает, ограничено ли отслеживание. (iOS 7.0 и более поздний).</span><span class="sxs-lookup"><span data-stu-id="ddb91-678">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="ddb91-679">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="ddb91-679">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="ddb91-680">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-680">Boolean</span></span>|<span data-ttu-id="ddb91-681">Указывает, заблокирована или не заблокирована книга предприятия.</span><span class="sxs-lookup"><span data-stu-id="ddb91-681">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="ddb91-682">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="ddb91-682">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="ddb91-683">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-683">Boolean</span></span>|<span data-ttu-id="ddb91-684">Указывает, заблокирована ли синхронизация записей и выделений для корпоративных книг.</span><span class="sxs-lookup"><span data-stu-id="ddb91-684">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="ddb91-685">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-685">airPrintBlocked</span></span>|<span data-ttu-id="ddb91-686">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-686">Boolean</span></span>|<span data-ttu-id="ddb91-687">Указывает, заблокирована или не заблокирована AirPrint (iOS 11.0 и более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-687">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ddb91-688">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="ddb91-688">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="ddb91-689">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-689">Boolean</span></span>|<span data-ttu-id="ddb91-690">Указывает, заблокировано ли хранение имени пользователя и пароля для Airprint (iOS 11.0 и более поздней части).</span><span class="sxs-lookup"><span data-stu-id="ddb91-690">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ddb91-691">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="ddb91-691">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="ddb91-692">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-692">Boolean</span></span>|<span data-ttu-id="ddb91-693">Указывает, требуются ли доверенные сертификаты для связи печати TLS (iOS 11.0 и более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-693">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ddb91-694">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="ddb91-694">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="ddb91-695">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-695">Boolean</span></span>|<span data-ttu-id="ddb91-696">Указывает, заблокировано ли обнаружение принтеров AirPrint для iBeacon.</span><span class="sxs-lookup"><span data-stu-id="ddb91-696">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="ddb91-697">Это предотвращает фишинговые маячки Bluetooth AirPrint для сетевого трафика (iOS 11.0 и более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-697">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ddb91-698">filesNetworkDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-698">filesNetworkDriveAccessBlocked</span></span>|<span data-ttu-id="ddb91-699">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-699">Boolean</span></span>|<span data-ttu-id="ddb91-700">Указывает, могут ли устройства получать доступ к файлам или другим ресурсам на сетевом сервере с помощью протокола Блокировка сообщений сервера (SMB).</span><span class="sxs-lookup"><span data-stu-id="ddb91-700">Indicates if devices can access files or other resources on a network server using the Server Message Block (SMB) protocol.</span></span> <span data-ttu-id="ddb91-701">Доступно для устройств с iOS и iPadOS версий 13.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="ddb91-701">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="ddb91-702">filesUsbDriveAccessBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-702">filesUsbDriveAccessBlocked</span></span>|<span data-ttu-id="ddb91-703">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-703">Boolean</span></span>|<span data-ttu-id="ddb91-704">Указывает, могут ли севики с доступом подключаться к файлам и открывать их на USB-диске.</span><span class="sxs-lookup"><span data-stu-id="ddb91-704">Indicates if sevices with access can connect to and open files on a USB drive.</span></span> <span data-ttu-id="ddb91-705">Доступно для устройств с iOS и iPadOS версий 13.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="ddb91-705">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="ddb91-706">wifiPowerOnForced</span><span class="sxs-lookup"><span data-stu-id="ddb91-706">wifiPowerOnForced</span></span>|<span data-ttu-id="ddb91-707">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-707">Boolean</span></span>|<span data-ttu-id="ddb91-708">Указывает, остается ли Wi-Fi, даже если устройство находится в режиме самолета.</span><span class="sxs-lookup"><span data-stu-id="ddb91-708">Indicates whether or not Wi-Fi remains on, even when device is in airplane mode.</span></span> <span data-ttu-id="ddb91-709">Доступно для устройств с iOS и iPadOS версий 13.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="ddb91-709">Available for devices running iOS and iPadOS, versions 13.0 and later.</span></span>|
|<span data-ttu-id="ddb91-710">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="ddb91-710">blockSystemAppRemoval</span></span>|<span data-ttu-id="ddb91-711">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-711">Boolean</span></span>|<span data-ttu-id="ddb91-712">Указывает, блокируется ли удаление системных приложений с устройства на контролируемом устройстве (iOS 11.0 и более поздней части).</span><span class="sxs-lookup"><span data-stu-id="ddb91-712">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ddb91-713">VPNBlockCreation</span><span class="sxs-lookup"><span data-stu-id="ddb91-713">vpnBlockCreation</span></span>|<span data-ttu-id="ddb91-714">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-714">Boolean</span></span>|<span data-ttu-id="ddb91-715">Указывает, заблокировано ли создание конфигураций VPN (iOS 11.0 и более поздней части).</span><span class="sxs-lookup"><span data-stu-id="ddb91-715">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="ddb91-716">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-716">appRemovalBlocked</span></span>|<span data-ttu-id="ddb91-717">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-717">Boolean</span></span>|<span data-ttu-id="ddb91-718">Указывает, разрешено ли удаление приложений.</span><span class="sxs-lookup"><span data-stu-id="ddb91-718">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="ddb91-719">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-719">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="ddb91-720">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-720">Boolean</span></span>|<span data-ttu-id="ddb91-721">Указывает, разрешено ли подключение к USB-аксессуарам во время блокировки устройства (iOS 11.4.1 и более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-721">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="ddb91-722">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="ddb91-722">passwordBlockAutoFill</span></span>|<span data-ttu-id="ddb91-723">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-723">Boolean</span></span>|<span data-ttu-id="ddb91-724">Указывает, разрешена ли функция паролей AutoFill (iOS 12.0 и более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-724">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ddb91-725">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="ddb91-725">passwordBlockProximityRequests</span></span>|<span data-ttu-id="ddb91-726">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-726">Boolean</span></span>|<span data-ttu-id="ddb91-727">Указывает, следует ли блокировать запрашивающие пароли с близлежащих устройств (iOS 12.0 и более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-727">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ddb91-728">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="ddb91-728">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="ddb91-729">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-729">Boolean</span></span>|<span data-ttu-id="ddb91-730">Указывает, следует ли блокировать совместное использование паролей с помощью паролей AirDrop с функцией iOS 12.0 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-730">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ddb91-731">dateAndTimeForceSetAutomatically</span><span class="sxs-lookup"><span data-stu-id="ddb91-731">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="ddb91-732">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-732">Boolean</span></span>|<span data-ttu-id="ddb91-733">Указывает, включена ли функция "Дата и время автоматически" и не может быть отключена пользователем (iOS 12.0 и более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-733">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ddb91-734">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="ddb91-734">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="ddb91-735">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-735">Boolean</span></span>|<span data-ttu-id="ddb91-736">Указывает, могут ли управляемые приложения записывать контакты в учетные записи неугодных контактов (iOS 12.0 и более поздние).</span><span class="sxs-lookup"><span data-stu-id="ddb91-736">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="ddb91-737">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="ddb91-737">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="ddb91-738">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-738">Boolean</span></span>|<span data-ttu-id="ddb91-739">Указывает, могут ли неуправляемые приложения читать из учетных записей управляемых контактов (iOS 12.0 или более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-739">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="ddb91-740">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="ddb91-740">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="ddb91-741">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-741">Boolean</span></span>|<span data-ttu-id="ddb91-742">Указывает, следует ли блокировать пользователю изменение личных параметров точки доступа (iOS 12.2 или более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-742">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="ddb91-743">continuousPathKeyboardBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-743">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="ddb91-744">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-744">Boolean</span></span>|<span data-ttu-id="ddb91-745">Указывает, следует ли блокировать клавиатуру непрерывного пути при контроле устройства (iOS 13 или более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-745">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="ddb91-746">findMyDeviceInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-746">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="ddb91-747">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-747">Boolean</span></span>|<span data-ttu-id="ddb91-748">Указывает, следует ли блокировать find My Device, когда устройство контролируется (iOS 13 или более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-748">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="ddb91-749">findMyFriendsInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-749">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="ddb91-750">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-750">Boolean</span></span>|<span data-ttu-id="ddb91-751">Указывает, следует ли блокировать "Найти друзей", когда устройство находится под наблюдением (iOS 13 или более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-751">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="ddb91-752">iTunesBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-752">iTunesBlocked</span></span>|<span data-ttu-id="ddb91-753">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-753">Boolean</span></span>|<span data-ttu-id="ddb91-754">Указывает, следует ли блокировать приложение iTunes.</span><span class="sxs-lookup"><span data-stu-id="ddb91-754">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="ddb91-755">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-755">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="ddb91-756">sharedDeviceBlockTemporarySessions</span><span class="sxs-lookup"><span data-stu-id="ddb91-756">sharedDeviceBlockTemporarySessions</span></span>|<span data-ttu-id="ddb91-757">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-757">Boolean</span></span>|<span data-ttu-id="ddb91-758">Указывает, следует ли блокировать временные сеансы на общих iPads (iOS 13.4 или более поздней).</span><span class="sxs-lookup"><span data-stu-id="ddb91-758">Indicates whether or not to block temporary sessions on Shared iPads (iOS 13.4 or later).</span></span>|
|<span data-ttu-id="ddb91-759">appClipsBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-759">appClipsBlocked</span></span>|<span data-ttu-id="ddb91-760">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-760">Boolean</span></span>|<span data-ttu-id="ddb91-761">Не позволяет пользователю добавлять какие-либо клипы приложений и удаляет существующие клипы приложений на устройстве.</span><span class="sxs-lookup"><span data-stu-id="ddb91-761">Prevents a user from adding any App Clips and removes any existing App Clips on the device.</span></span>|
|<span data-ttu-id="ddb91-762">applePersonalizedAdsBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-762">applePersonalizedAdsBlocked</span></span>|<span data-ttu-id="ddb91-763">Логический</span><span class="sxs-lookup"><span data-stu-id="ddb91-763">Boolean</span></span>|<span data-ttu-id="ddb91-764">Ограничивает персонализированную рекламу Apple, если это так.</span><span class="sxs-lookup"><span data-stu-id="ddb91-764">Limits Apple personalized advertising when true.</span></span> <span data-ttu-id="ddb91-765">Доступна в iOS 14 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="ddb91-765">Available in iOS 14 and later.</span></span>|
|<span data-ttu-id="ddb91-766">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="ddb91-766">nfcBlocked</span></span>|<span data-ttu-id="ddb91-767">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddb91-767">Boolean</span></span>|<span data-ttu-id="ddb91-768">Отключить NFC, чтобы предотвратить сопряжение устройств с другими устройствами с поддержкой NFC.</span><span class="sxs-lookup"><span data-stu-id="ddb91-768">Disable NFC to prevent devices from pairing with other NFC-enabled devices.</span></span> <span data-ttu-id="ddb91-769">Доступно для устройств iOS/iPadOS с 14.2 и более поздним доступом.</span><span class="sxs-lookup"><span data-stu-id="ddb91-769">Available for iOS/iPadOS devices running 14.2 and later.</span></span>|
|<span data-ttu-id="ddb91-770">kioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="ddb91-770">kioskModeAppType</span></span>|[<span data-ttu-id="ddb91-771">iosKioskModeAppType</span><span class="sxs-lookup"><span data-stu-id="ddb91-771">iosKioskModeAppType</span></span>](../resources/intune-deviceconfig-ioskioskmodeapptype.md)|<span data-ttu-id="ddb91-772">Тип приложения для работы в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="ddb91-772">Type of app to run in kiosk mode.</span></span> <span data-ttu-id="ddb91-773">Возможные значения: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span><span class="sxs-lookup"><span data-stu-id="ddb91-773">Possible values are: `notConfigured`, `appStoreApp`, `managedApp`, `builtInApp`.</span></span>|



## <a name="response"></a><span data-ttu-id="ddb91-774">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddb91-774">Response</span></span>
<span data-ttu-id="ddb91-775">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ddb91-775">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddb91-776">Пример</span><span class="sxs-lookup"><span data-stu-id="ddb91-776">Example</span></span>

### <a name="request"></a><span data-ttu-id="ddb91-777">Запрос</span><span class="sxs-lookup"><span data-stu-id="ddb91-777">Request</span></span>
<span data-ttu-id="ddb91-778">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ddb91-778">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 10656

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
  "sharedDeviceBlockTemporarySessions": true,
  "appClipsBlocked": true,
  "applePersonalizedAdsBlocked": true,
  "nfcBlocked": true,
  "kioskModeAppType": "appStoreApp"
}
```

### <a name="response"></a><span data-ttu-id="ddb91-779">Отклик</span><span class="sxs-lookup"><span data-stu-id="ddb91-779">Response</span></span>
<span data-ttu-id="ddb91-p159">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ddb91-p159">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10828

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
  "sharedDeviceBlockTemporarySessions": true,
  "appClipsBlocked": true,
  "applePersonalizedAdsBlocked": true,
  "nfcBlocked": true,
  "kioskModeAppType": "appStoreApp"
}
```




