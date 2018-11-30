---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание нового объекта androidDeviceOwnerGeneralDeviceConfiguration.
ms.openlocfilehash: 0c95c47638378271d40f1c76327c1ea54e37e0cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082307"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="8522b-103">Создание androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8522b-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="8522b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8522b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8522b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8522b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8522b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8522b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8522b-107">Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8522b-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8522b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8522b-108">Prerequisites</span></span>
<span data-ttu-id="8522b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8522b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8522b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8522b-111">Permission type</span></span>|<span data-ttu-id="8522b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8522b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8522b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8522b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8522b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8522b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8522b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8522b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8522b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8522b-116">Not supported.</span></span>|
|<span data-ttu-id="8522b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8522b-117">Application</span></span>|<span data-ttu-id="8522b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8522b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8522b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8522b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8522b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8522b-120">Request headers</span></span>
|<span data-ttu-id="8522b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8522b-121">Header</span></span>|<span data-ttu-id="8522b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8522b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8522b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8522b-123">Authorization</span></span>|<span data-ttu-id="8522b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8522b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8522b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8522b-125">Accept</span></span>|<span data-ttu-id="8522b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8522b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8522b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8522b-127">Request body</span></span>
<span data-ttu-id="8522b-128">В тексте запроса укажите представление JSON для объекта androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8522b-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="8522b-129">В следующей таблице показаны свойства, которые необходимы для создания androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8522b-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="8522b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8522b-130">Property</span></span>|<span data-ttu-id="8522b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8522b-131">Type</span></span>|<span data-ttu-id="8522b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8522b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8522b-133">id</span><span class="sxs-lookup"><span data-stu-id="8522b-133">id</span></span>|<span data-ttu-id="8522b-134">String</span><span class="sxs-lookup"><span data-stu-id="8522b-134">String</span></span>|<span data-ttu-id="8522b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8522b-135">Key of the entity.</span></span> <span data-ttu-id="8522b-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8522b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8522b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8522b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8522b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8522b-138">DateTimeOffset</span></span>|<span data-ttu-id="8522b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8522b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8522b-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8522b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8522b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8522b-141">roleScopeTagIds</span></span>|<span data-ttu-id="8522b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8522b-142">String collection</span></span>|<span data-ttu-id="8522b-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8522b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8522b-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8522b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8522b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8522b-145">supportsScopeTags</span></span>|<span data-ttu-id="8522b-146">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-146">Boolean</span></span>|<span data-ttu-id="8522b-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="8522b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8522b-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="8522b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8522b-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8522b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8522b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8522b-150">This property is read-only.</span></span> <span data-ttu-id="8522b-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8522b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8522b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8522b-152">createdDateTime</span></span>|<span data-ttu-id="8522b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8522b-153">DateTimeOffset</span></span>|<span data-ttu-id="8522b-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8522b-154">DateTime the object was created.</span></span> <span data-ttu-id="8522b-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8522b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8522b-156">описание</span><span class="sxs-lookup"><span data-stu-id="8522b-156">description</span></span>|<span data-ttu-id="8522b-157">String</span><span class="sxs-lookup"><span data-stu-id="8522b-157">String</span></span>|<span data-ttu-id="8522b-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8522b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8522b-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8522b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8522b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8522b-160">displayName</span></span>|<span data-ttu-id="8522b-161">String</span><span class="sxs-lookup"><span data-stu-id="8522b-161">String</span></span>|<span data-ttu-id="8522b-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8522b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8522b-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8522b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8522b-164">version</span><span class="sxs-lookup"><span data-stu-id="8522b-164">version</span></span>|<span data-ttu-id="8522b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8522b-165">Int32</span></span>|<span data-ttu-id="8522b-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8522b-166">Version of the device configuration.</span></span> <span data-ttu-id="8522b-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8522b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8522b-168">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="8522b-168">accountsBlockModification</span></span>|<span data-ttu-id="8522b-169">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-169">Boolean</span></span>|<span data-ttu-id="8522b-170">Указывает, отключена ли добавлять и удалять учетные записи.</span><span class="sxs-lookup"><span data-stu-id="8522b-170">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="8522b-171">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="8522b-171">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="8522b-172">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-172">Boolean</span></span>|<span data-ttu-id="8522b-173">Указывает, может ли пользователь для включения неизвестных источников установки.</span><span class="sxs-lookup"><span data-stu-id="8522b-173">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="8522b-174">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="8522b-174">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="8522b-175">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="8522b-175">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="8522b-176">Указывает значение политики app автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="8522b-176">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="8522b-177">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="8522b-177">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="8522b-178">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="8522b-178">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="8522b-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="8522b-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="8522b-180">Указывает политику разрешений для запросов для разрешения среды выполнения, если один не определен для приложения, в частности.</span><span class="sxs-lookup"><span data-stu-id="8522b-180">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="8522b-181">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="8522b-181">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="8522b-182">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="8522b-182">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="8522b-183">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-183">Boolean</span></span>|<span data-ttu-id="8522b-184">Указывает, следует ли запретить пользователю Настройка bluetooth.</span><span class="sxs-lookup"><span data-stu-id="8522b-184">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="8522b-185">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="8522b-185">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="8522b-186">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-186">Boolean</span></span>|<span data-ttu-id="8522b-187">Указывает, следует ли запретить совместное использование контактов с помощью bluetooth пользователю.</span><span class="sxs-lookup"><span data-stu-id="8522b-187">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="8522b-188">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="8522b-188">cameraBlocked</span></span>|<span data-ttu-id="8522b-189">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-189">Boolean</span></span>|<span data-ttu-id="8522b-190">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="8522b-190">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="8522b-191">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="8522b-191">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="8522b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="8522b-192">Boolean</span></span>|<span data-ttu-id="8522b-193">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="8522b-193">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="8522b-194">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="8522b-194">dataRoamingBlocked</span></span>|<span data-ttu-id="8522b-195">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-195">Boolean</span></span>|<span data-ttu-id="8522b-196">Указывает, следует ли запретить пользователю перемещение данных.</span><span class="sxs-lookup"><span data-stu-id="8522b-196">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="8522b-197">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="8522b-197">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="8522b-198">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-198">Boolean</span></span>|<span data-ttu-id="8522b-199">Указывает ли пользователь вручную изменение даты и времени на устройстве</span><span class="sxs-lookup"><span data-stu-id="8522b-199">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="8522b-200">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="8522b-200">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="8522b-201">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8522b-201">String collection</span></span>|<span data-ttu-id="8522b-202">Список Google учетной записи по электронной почте, которые понадобятся для проверки подлинности после фабрики сбросить, прежде чем выполнить настройку устройства.</span><span class="sxs-lookup"><span data-stu-id="8522b-202">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="8522b-203">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="8522b-203">factoryResetBlocked</span></span>|<span data-ttu-id="8522b-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="8522b-204">Boolean</span></span>|<span data-ttu-id="8522b-205">Указывает, отключена ли параметр сброса фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="8522b-205">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="8522b-206">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="8522b-206">kioskModeApps</span></span>|<span data-ttu-id="8522b-207">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="8522b-207">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="8522b-208">Список управляемых приложений, которые будут отображаться, если устройство находится в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="8522b-208">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="8522b-209">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8522b-209">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8522b-210">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="8522b-210">microphoneForceMute</span></span>|<span data-ttu-id="8522b-211">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-211">Boolean</span></span>|<span data-ttu-id="8522b-212">Указывает, следует ли блокировать выключения звука микрофона на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8522b-212">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="8522b-213">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="8522b-213">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="8522b-214">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-214">Boolean</span></span>|<span data-ttu-id="8522b-215">Указывает, будет ли устройства разрешить подключение к временной сетевое подключение во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="8522b-215">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="8522b-216">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="8522b-216">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="8522b-217">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-217">Boolean</span></span>|<span data-ttu-id="8522b-218">Указывает, следует ли блокировать исходящей балки NFC.</span><span class="sxs-lookup"><span data-stu-id="8522b-218">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="8522b-219">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="8522b-219">passwordBlockKeyguard</span></span>|<span data-ttu-id="8522b-220">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-220">Boolean</span></span>|<span data-ttu-id="8522b-221">Указывает, отключена ли keyguard.</span><span class="sxs-lookup"><span data-stu-id="8522b-221">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="8522b-222">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8522b-222">passwordExpirationDays</span></span>|<span data-ttu-id="8522b-223">Int32</span><span class="sxs-lookup"><span data-stu-id="8522b-223">Int32</span></span>|<span data-ttu-id="8522b-224">Указывает время в секундах, пароль может быть задан для до истечения срока действия и требуется указать новый пароль.</span><span class="sxs-lookup"><span data-stu-id="8522b-224">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="8522b-225">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="8522b-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="8522b-226">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8522b-226">passwordMinimumLength</span></span>|<span data-ttu-id="8522b-227">Int32</span><span class="sxs-lookup"><span data-stu-id="8522b-227">Int32</span></span>|<span data-ttu-id="8522b-228">Указывает минимальную длину пароля на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8522b-228">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="8522b-229">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="8522b-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="8522b-230">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8522b-230">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8522b-231">Int32</span><span class="sxs-lookup"><span data-stu-id="8522b-231">Int32</span></span>|<span data-ttu-id="8522b-232">Простоя перед экрана времени ожидания в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="8522b-232">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8522b-233">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="8522b-233">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="8522b-234">Int32</span><span class="sxs-lookup"><span data-stu-id="8522b-234">Int32</span></span>|<span data-ttu-id="8522b-235">Длина журнал паролей, где пользователь не сможет ввести новый пароль, которые совпадают с любой пароль в журнале.</span><span class="sxs-lookup"><span data-stu-id="8522b-235">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="8522b-236">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="8522b-236">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8522b-237">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8522b-237">passwordRequiredType</span></span>|[<span data-ttu-id="8522b-238">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8522b-238">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="8522b-239">Указывает минимальную качество, необходимые на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8522b-239">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="8522b-240">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="8522b-240">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="8522b-241">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8522b-241">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8522b-242">Int32</span><span class="sxs-lookup"><span data-stu-id="8522b-242">Int32</span></span>|<span data-ttu-id="8522b-243">Указывает, сколько раз для ввода неправильного пароля перед Очистить устройство.</span><span class="sxs-lookup"><span data-stu-id="8522b-243">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="8522b-244">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="8522b-244">Valid values 4 to 11</span></span>|
|<span data-ttu-id="8522b-245">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="8522b-245">safeBootBlocked</span></span>|<span data-ttu-id="8522b-246">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-246">Boolean</span></span>|<span data-ttu-id="8522b-247">Указывает, следует ли перезагрузка отключенные устройства в безопасной загрузки.</span><span class="sxs-lookup"><span data-stu-id="8522b-247">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="8522b-248">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="8522b-248">screenCaptureBlocked</span></span>|<span data-ttu-id="8522b-249">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-249">Boolean</span></span>|<span data-ttu-id="8522b-250">Указывает, следует ли отключить возможность использовать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="8522b-250">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="8522b-251">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="8522b-251">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="8522b-252">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-252">Boolean</span></span>|<span data-ttu-id="8522b-253">Указывает, следует ли пользователь не Включение функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="8522b-253">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="8522b-254">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="8522b-254">securityRequireVerifyApps</span></span>|<span data-ttu-id="8522b-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="8522b-255">Boolean</span></span>|<span data-ttu-id="8522b-256">Указывает ли проверка приложений является обязательным.</span><span class="sxs-lookup"><span data-stu-id="8522b-256">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="8522b-257">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="8522b-257">statusBarBlocked</span></span>|<span data-ttu-id="8522b-258">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-258">Boolean</span></span>|<span data-ttu-id="8522b-259">Указывает, будет ли или состояние панели не действует, включая уведомления, параметры быстрого и других перекрытий экрана.</span><span class="sxs-lookup"><span data-stu-id="8522b-259">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="8522b-260">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="8522b-260">stayOnModes</span></span>|<span data-ttu-id="8522b-261">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="8522b-261">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="8522b-262">Список режимы, в которых хранятся устройства отображения включении.</span><span class="sxs-lookup"><span data-stu-id="8522b-262">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="8522b-263">Эта коллекция может содержать до 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="8522b-263">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="8522b-264">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="8522b-264">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="8522b-265">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="8522b-265">storageAllowUsb</span></span>|<span data-ttu-id="8522b-266">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-266">Boolean</span></span>|<span data-ttu-id="8522b-267">Указывает, следует ли разрешить USB запоминающих устройств.</span><span class="sxs-lookup"><span data-stu-id="8522b-267">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="8522b-268">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="8522b-268">storageBlockExternalMedia</span></span>|<span data-ttu-id="8522b-269">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-269">Boolean</span></span>|<span data-ttu-id="8522b-270">Указывает, следует ли блокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="8522b-270">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="8522b-271">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="8522b-271">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="8522b-272">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-272">Boolean</span></span>|<span data-ttu-id="8522b-273">Указывает, следует ли блокировать USB передачи файлов.</span><span class="sxs-lookup"><span data-stu-id="8522b-273">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="8522b-274">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="8522b-274">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="8522b-275">Int32</span><span class="sxs-lookup"><span data-stu-id="8522b-275">Int32</span></span>|<span data-ttu-id="8522b-276">Указывает количество минут после полуночи, начинающимся окно обновление системы.</span><span class="sxs-lookup"><span data-stu-id="8522b-276">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="8522b-277">Допустимые значения 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="8522b-277">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="8522b-278">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="8522b-278">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="8522b-279">Int32</span><span class="sxs-lookup"><span data-stu-id="8522b-279">Int32</span></span>|<span data-ttu-id="8522b-280">Указывает количество минут после полуночи, завершающей окне обновление системы.</span><span class="sxs-lookup"><span data-stu-id="8522b-280">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="8522b-281">Допустимые значения 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="8522b-281">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="8522b-282">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="8522b-282">systemUpdateInstallType</span></span>|[<span data-ttu-id="8522b-283">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="8522b-283">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="8522b-284">Тип обновления конфигурации системы.</span><span class="sxs-lookup"><span data-stu-id="8522b-284">The type of system update configuration.</span></span> <span data-ttu-id="8522b-285">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="8522b-285">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="8522b-286">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="8522b-286">usersBlockAdd</span></span>|<span data-ttu-id="8522b-287">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-287">Boolean</span></span>|<span data-ttu-id="8522b-288">Указывает, отключена ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="8522b-288">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="8522b-289">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="8522b-289">usersBlockRemove</span></span>|<span data-ttu-id="8522b-290">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-290">Boolean</span></span>|<span data-ttu-id="8522b-291">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="8522b-291">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="8522b-292">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="8522b-292">volumeBlockAdjustment</span></span>|<span data-ttu-id="8522b-293">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-293">Boolean</span></span>|<span data-ttu-id="8522b-294">Указывает, следует ли настройка отключенные громкости.</span><span class="sxs-lookup"><span data-stu-id="8522b-294">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="8522b-295">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="8522b-295">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="8522b-296">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-296">Boolean</span></span>|<span data-ttu-id="8522b-297">Указывает, следует ли пользователь не может изменять параметры подключения wifi.</span><span class="sxs-lookup"><span data-stu-id="8522b-297">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="8522b-298">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="8522b-298">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="8522b-299">Логический</span><span class="sxs-lookup"><span data-stu-id="8522b-299">Boolean</span></span>|<span data-ttu-id="8522b-300">Указывает, следует ли пользователь не может изменять только что сетей, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="8522b-300">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="8522b-301">Ответ</span><span class="sxs-lookup"><span data-stu-id="8522b-301">Response</span></span>
<span data-ttu-id="8522b-302">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8522b-302">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8522b-303">Пример</span><span class="sxs-lookup"><span data-stu-id="8522b-303">Example</span></span>
### <a name="request"></a><span data-ttu-id="8522b-304">Запрос</span><span class="sxs-lookup"><span data-stu-id="8522b-304">Request</span></span>
<span data-ttu-id="8522b-305">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8522b-305">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2156

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="8522b-306">Ответ</span><span class="sxs-lookup"><span data-stu-id="8522b-306">Response</span></span>
<span data-ttu-id="8522b-p123">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8522b-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2264

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
  "id": "edad943d-943d-edad-3d94-aded3d94aded",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "userChoice",
  "appsDefaultPermissionPolicy": "prompt",
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "Factory Reset Device Administrator Emails value"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordCountToBlock": 4,
  "passwordRequiredType": "required",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "ac"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 11,
  "systemUpdateWindowEndMinutesAfterMidnight": 9,
  "systemUpdateInstallType": "postpone",
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```





