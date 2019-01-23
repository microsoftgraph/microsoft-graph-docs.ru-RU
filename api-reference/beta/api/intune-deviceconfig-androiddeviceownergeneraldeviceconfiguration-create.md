---
title: Создание androidDeviceOwnerGeneralDeviceConfiguration
description: Создание нового объекта androidDeviceOwnerGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 93df53db7c19df9134370f9dbd703d99f631b688
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421223"
---
# <a name="create-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="5156b-103">Создание androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5156b-103">Create androidDeviceOwnerGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="5156b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5156b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5156b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5156b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5156b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5156b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5156b-107">Создание нового объекта [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5156b-107">Create a new [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5156b-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="5156b-108">Prerequisites</span></span>
<span data-ttu-id="5156b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5156b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5156b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5156b-111">Permission type</span></span>|<span data-ttu-id="5156b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5156b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5156b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5156b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5156b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5156b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5156b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5156b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5156b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5156b-116">Not supported.</span></span>|
|<span data-ttu-id="5156b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5156b-117">Application</span></span>|<span data-ttu-id="5156b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5156b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5156b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5156b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5156b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5156b-120">Request headers</span></span>
|<span data-ttu-id="5156b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5156b-121">Header</span></span>|<span data-ttu-id="5156b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5156b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5156b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5156b-123">Authorization</span></span>|<span data-ttu-id="5156b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5156b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5156b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5156b-125">Accept</span></span>|<span data-ttu-id="5156b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5156b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5156b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5156b-127">Request body</span></span>
<span data-ttu-id="5156b-128">В тексте запроса укажите представление JSON для объекта androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5156b-128">In the request body, supply a JSON representation for the androidDeviceOwnerGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="5156b-129">В следующей таблице показаны свойства, которые необходимы для создания androidDeviceOwnerGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5156b-129">The following table shows the properties that are required when you create the androidDeviceOwnerGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="5156b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5156b-130">Property</span></span>|<span data-ttu-id="5156b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5156b-131">Type</span></span>|<span data-ttu-id="5156b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5156b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5156b-133">id</span><span class="sxs-lookup"><span data-stu-id="5156b-133">id</span></span>|<span data-ttu-id="5156b-134">String</span><span class="sxs-lookup"><span data-stu-id="5156b-134">String</span></span>|<span data-ttu-id="5156b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5156b-135">Key of the entity.</span></span> <span data-ttu-id="5156b-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5156b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5156b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5156b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5156b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5156b-138">DateTimeOffset</span></span>|<span data-ttu-id="5156b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5156b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5156b-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5156b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5156b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5156b-141">roleScopeTagIds</span></span>|<span data-ttu-id="5156b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5156b-142">String collection</span></span>|<span data-ttu-id="5156b-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5156b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5156b-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5156b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5156b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5156b-145">supportsScopeTags</span></span>|<span data-ttu-id="5156b-146">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-146">Boolean</span></span>|<span data-ttu-id="5156b-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="5156b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5156b-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="5156b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5156b-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5156b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5156b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5156b-150">This property is read-only.</span></span> <span data-ttu-id="5156b-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5156b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5156b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5156b-152">createdDateTime</span></span>|<span data-ttu-id="5156b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5156b-153">DateTimeOffset</span></span>|<span data-ttu-id="5156b-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5156b-154">DateTime the object was created.</span></span> <span data-ttu-id="5156b-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5156b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5156b-156">description</span><span class="sxs-lookup"><span data-stu-id="5156b-156">description</span></span>|<span data-ttu-id="5156b-157">String</span><span class="sxs-lookup"><span data-stu-id="5156b-157">String</span></span>|<span data-ttu-id="5156b-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5156b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5156b-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5156b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5156b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="5156b-160">displayName</span></span>|<span data-ttu-id="5156b-161">String</span><span class="sxs-lookup"><span data-stu-id="5156b-161">String</span></span>|<span data-ttu-id="5156b-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5156b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5156b-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5156b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5156b-164">version</span><span class="sxs-lookup"><span data-stu-id="5156b-164">version</span></span>|<span data-ttu-id="5156b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5156b-165">Int32</span></span>|<span data-ttu-id="5156b-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5156b-166">Version of the device configuration.</span></span> <span data-ttu-id="5156b-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5156b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5156b-168">accountsBlockModification</span><span class="sxs-lookup"><span data-stu-id="5156b-168">accountsBlockModification</span></span>|<span data-ttu-id="5156b-169">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-169">Boolean</span></span>|<span data-ttu-id="5156b-170">Указывает, отключена ли добавлять и удалять учетные записи.</span><span class="sxs-lookup"><span data-stu-id="5156b-170">Indicates whether or not adding or removing accounts is disabled.</span></span>|
|<span data-ttu-id="5156b-171">appsAllowInstallFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="5156b-171">appsAllowInstallFromUnknownSources</span></span>|<span data-ttu-id="5156b-172">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-172">Boolean</span></span>|<span data-ttu-id="5156b-173">Указывает, может ли пользователь для включения неизвестных источников установки.</span><span class="sxs-lookup"><span data-stu-id="5156b-173">Indicates whether or not the user is allowed to enable to unknown sources setting.</span></span>|
|<span data-ttu-id="5156b-174">appsAutoUpdatePolicy</span><span class="sxs-lookup"><span data-stu-id="5156b-174">appsAutoUpdatePolicy</span></span>|[<span data-ttu-id="5156b-175">androidDeviceOwnerAppAutoUpdatePolicyType</span><span class="sxs-lookup"><span data-stu-id="5156b-175">androidDeviceOwnerAppAutoUpdatePolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|<span data-ttu-id="5156b-176">Указывает значение политики app автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="5156b-176">Indicates the value of the app auto update policy.</span></span> <span data-ttu-id="5156b-177">Возможные значения: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span><span class="sxs-lookup"><span data-stu-id="5156b-177">Possible values are: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.</span></span>|
|<span data-ttu-id="5156b-178">appsDefaultPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="5156b-178">appsDefaultPermissionPolicy</span></span>|[<span data-ttu-id="5156b-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="5156b-179">androidDeviceOwnerDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|<span data-ttu-id="5156b-180">Указывает политику разрешений для запросов для разрешения среды выполнения, если один не определен для приложения, в частности.</span><span class="sxs-lookup"><span data-stu-id="5156b-180">Indicates the permission policy for requests for runtime permissions if one is not defined for the app specifically.</span></span> <span data-ttu-id="5156b-181">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="5156b-181">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="5156b-182">appsRecommendSkippingFirstUseHints</span><span class="sxs-lookup"><span data-stu-id="5156b-182">appsRecommendSkippingFirstUseHints</span></span>|<span data-ttu-id="5156b-183">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-183">Boolean</span></span>|<span data-ttu-id="5156b-184">Рекомендуется все приложения или не пропустить все первого время использования подсказки, которые могут добавлены.</span><span class="sxs-lookup"><span data-stu-id="5156b-184">Whether or not to recommend all apps skip any first-time-use hints they may have added.</span></span>|
|<span data-ttu-id="5156b-185">bluetoothBlockConfiguration</span><span class="sxs-lookup"><span data-stu-id="5156b-185">bluetoothBlockConfiguration</span></span>|<span data-ttu-id="5156b-186">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-186">Boolean</span></span>|<span data-ttu-id="5156b-187">Указывает, следует ли запретить пользователю Настройка bluetooth.</span><span class="sxs-lookup"><span data-stu-id="5156b-187">Indicates whether or not to block a user from configuring bluetooth.</span></span>|
|<span data-ttu-id="5156b-188">bluetoothBlockContactSharing</span><span class="sxs-lookup"><span data-stu-id="5156b-188">bluetoothBlockContactSharing</span></span>|<span data-ttu-id="5156b-189">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-189">Boolean</span></span>|<span data-ttu-id="5156b-190">Указывает, следует ли запретить совместное использование контактов с помощью bluetooth пользователю.</span><span class="sxs-lookup"><span data-stu-id="5156b-190">Indicates whether or not to block a user from sharing contacts via bluetooth.</span></span>|
|<span data-ttu-id="5156b-191">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="5156b-191">cameraBlocked</span></span>|<span data-ttu-id="5156b-192">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-192">Boolean</span></span>|<span data-ttu-id="5156b-193">Указывает, следует ли отключить использование камеры.</span><span class="sxs-lookup"><span data-stu-id="5156b-193">Indicates whether or not to disable the use of the camera.</span></span>|
|<span data-ttu-id="5156b-194">cellularBlockWiFiTethering</span><span class="sxs-lookup"><span data-stu-id="5156b-194">cellularBlockWiFiTethering</span></span>|<span data-ttu-id="5156b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="5156b-195">Boolean</span></span>|<span data-ttu-id="5156b-196">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="5156b-196">Indicates whether or not to block Wi-Fi tethering.</span></span>|
|<span data-ttu-id="5156b-197">dataRoamingBlocked</span><span class="sxs-lookup"><span data-stu-id="5156b-197">dataRoamingBlocked</span></span>|<span data-ttu-id="5156b-198">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-198">Boolean</span></span>|<span data-ttu-id="5156b-199">Указывает, следует ли запретить пользователю перемещение данных.</span><span class="sxs-lookup"><span data-stu-id="5156b-199">Indicates whether or not to block a user from data roaming.</span></span>|
|<span data-ttu-id="5156b-200">dateTimeConfigurationBlocked</span><span class="sxs-lookup"><span data-stu-id="5156b-200">dateTimeConfigurationBlocked</span></span>|<span data-ttu-id="5156b-201">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-201">Boolean</span></span>|<span data-ttu-id="5156b-202">Указывает ли пользователь вручную изменение даты и времени на устройстве</span><span class="sxs-lookup"><span data-stu-id="5156b-202">Indicates whether or not to block the user from manually changing the date or time on the device</span></span>|
|<span data-ttu-id="5156b-203">factoryResetDeviceAdministratorEmails</span><span class="sxs-lookup"><span data-stu-id="5156b-203">factoryResetDeviceAdministratorEmails</span></span>|<span data-ttu-id="5156b-204">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5156b-204">String collection</span></span>|<span data-ttu-id="5156b-205">Список Google учетной записи по электронной почте, которые понадобятся для проверки подлинности после фабрики сбросить, прежде чем выполнить настройку устройства.</span><span class="sxs-lookup"><span data-stu-id="5156b-205">List of Google account emails that will be required to authenticate after a device is factory reset before it can be set up.</span></span>|
|<span data-ttu-id="5156b-206">factoryResetBlocked</span><span class="sxs-lookup"><span data-stu-id="5156b-206">factoryResetBlocked</span></span>|<span data-ttu-id="5156b-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="5156b-207">Boolean</span></span>|<span data-ttu-id="5156b-208">Указывает, отключена ли параметр сброса фабрики в параметрах.</span><span class="sxs-lookup"><span data-stu-id="5156b-208">Indicates whether or not the factory reset option in settings is disabled.</span></span>|
|<span data-ttu-id="5156b-209">kioskModeApps</span><span class="sxs-lookup"><span data-stu-id="5156b-209">kioskModeApps</span></span>|<span data-ttu-id="5156b-210">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="5156b-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="5156b-211">Список управляемых приложений, которые будут отображаться, если устройство находится в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="5156b-211">A list of managed apps that will be shown when the device is in Kiosk Mode.</span></span> <span data-ttu-id="5156b-212">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5156b-212">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5156b-213">kioskModeWallpaperUrl</span><span class="sxs-lookup"><span data-stu-id="5156b-213">kioskModeWallpaperUrl</span></span>|<span data-ttu-id="5156b-214">String</span><span class="sxs-lookup"><span data-stu-id="5156b-214">String</span></span>|<span data-ttu-id="5156b-215">URL-адрес в образ общего доступа для использования для фонового рисунка, когда устройство в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="5156b-215">URL to a publicly accessible image to use for the wallpaper when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="5156b-216">kioskModeExitCode</span><span class="sxs-lookup"><span data-stu-id="5156b-216">kioskModeExitCode</span></span>|<span data-ttu-id="5156b-217">String</span><span class="sxs-lookup"><span data-stu-id="5156b-217">String</span></span>|<span data-ttu-id="5156b-218">Выйдите из кода, чтобы позволить пользователю для выхода в полноэкранном режиме, когда устройство в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="5156b-218">Exit code to allow a user to escape from Kiosk Mode when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="5156b-219">kioskModeVirtualHomeButtonEnabled</span><span class="sxs-lookup"><span data-stu-id="5156b-219">kioskModeVirtualHomeButtonEnabled</span></span>|<span data-ttu-id="5156b-220">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-220">Boolean</span></span>|<span data-ttu-id="5156b-221">Следует ли отображение виртуальных Домашняя страница кнопки, если устройство находится в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="5156b-221">Whether or not to display a virtual home button when the device is in Kiosk Mode.</span></span>|
|<span data-ttu-id="5156b-222">microphoneForceMute</span><span class="sxs-lookup"><span data-stu-id="5156b-222">microphoneForceMute</span></span>|<span data-ttu-id="5156b-223">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-223">Boolean</span></span>|<span data-ttu-id="5156b-224">Указывает, следует ли блокировать выключения звука микрофона на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5156b-224">Indicates whether or not to block unmuting the microphone on the device.</span></span>|
|<span data-ttu-id="5156b-225">networkEscapeHatchAllowed</span><span class="sxs-lookup"><span data-stu-id="5156b-225">networkEscapeHatchAllowed</span></span>|<span data-ttu-id="5156b-226">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-226">Boolean</span></span>|<span data-ttu-id="5156b-227">Указывает, будет ли устройства разрешить подключение к временной сетевое подключение во время загрузки.</span><span class="sxs-lookup"><span data-stu-id="5156b-227">Indicates whether or not the device will allow connecting to a temporary network connection at boot time.</span></span>|
|<span data-ttu-id="5156b-228">nfcBlockOutgoingBeam</span><span class="sxs-lookup"><span data-stu-id="5156b-228">nfcBlockOutgoingBeam</span></span>|<span data-ttu-id="5156b-229">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-229">Boolean</span></span>|<span data-ttu-id="5156b-230">Указывает, следует ли блокировать исходящей балки NFC.</span><span class="sxs-lookup"><span data-stu-id="5156b-230">Indicates whether or not to block NFC outgoing beam.</span></span>|
|<span data-ttu-id="5156b-231">passwordBlockKeyguard</span><span class="sxs-lookup"><span data-stu-id="5156b-231">passwordBlockKeyguard</span></span>|<span data-ttu-id="5156b-232">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-232">Boolean</span></span>|<span data-ttu-id="5156b-233">Указывает, отключена ли keyguard.</span><span class="sxs-lookup"><span data-stu-id="5156b-233">Indicates whether or not the keyguard is disabled.</span></span>|
|<span data-ttu-id="5156b-234">passwordBlockKeyguardFeatures</span><span class="sxs-lookup"><span data-stu-id="5156b-234">passwordBlockKeyguardFeatures</span></span>|<span data-ttu-id="5156b-235">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5156b-235">[androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md) collection</span></span>|<span data-ttu-id="5156b-236">Список компонентов keyguard устройства для блокировки.</span><span class="sxs-lookup"><span data-stu-id="5156b-236">List of device keyguard features to block.</span></span> <span data-ttu-id="5156b-237">Эта коллекция может содержать не более 7 элементов.</span><span class="sxs-lookup"><span data-stu-id="5156b-237">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="5156b-238">Возможные значения: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span><span class="sxs-lookup"><span data-stu-id="5156b-238">Possible values are: `notConfigured`, `camera`, `notifications`, `unredactedNotifications`, `trustAgents`, `fingerprint`, `remoteInput`, `allFeatures`.</span></span>|
|<span data-ttu-id="5156b-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5156b-239">passwordExpirationDays</span></span>|<span data-ttu-id="5156b-240">Int32</span><span class="sxs-lookup"><span data-stu-id="5156b-240">Int32</span></span>|<span data-ttu-id="5156b-241">Указывает время в секундах, пароль может быть задан для до истечения срока действия и требуется указать новый пароль.</span><span class="sxs-lookup"><span data-stu-id="5156b-241">Indicates the amount of time in seconds that a password can be set for before it expires and a new password will be required.</span></span> <span data-ttu-id="5156b-242">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="5156b-242">Valid values 1 to 365</span></span>|
|<span data-ttu-id="5156b-243">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5156b-243">passwordMinimumLength</span></span>|<span data-ttu-id="5156b-244">Int32</span><span class="sxs-lookup"><span data-stu-id="5156b-244">Int32</span></span>|<span data-ttu-id="5156b-245">Указывает минимальную длину пароля на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5156b-245">Indicates the minimum length of the password required on the device.</span></span> <span data-ttu-id="5156b-246">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="5156b-246">Valid values 4 to 16</span></span>|
|<span data-ttu-id="5156b-247">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="5156b-247">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="5156b-248">Int32</span><span class="sxs-lookup"><span data-stu-id="5156b-248">Int32</span></span>|<span data-ttu-id="5156b-249">Простоя перед экрана времени ожидания в миллисекундах.</span><span class="sxs-lookup"><span data-stu-id="5156b-249">Milliseconds of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="5156b-250">passwordPreviousPasswordCountToBlock</span><span class="sxs-lookup"><span data-stu-id="5156b-250">passwordPreviousPasswordCountToBlock</span></span>|<span data-ttu-id="5156b-251">Int32</span><span class="sxs-lookup"><span data-stu-id="5156b-251">Int32</span></span>|<span data-ttu-id="5156b-252">Длина журнал паролей, где пользователь не сможет ввести новый пароль, которые совпадают с любой пароль в журнале.</span><span class="sxs-lookup"><span data-stu-id="5156b-252">Indicates the length of password history, where the user will not be able to enter a new password that is the same as any password in the history.</span></span> <span data-ttu-id="5156b-253">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="5156b-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="5156b-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5156b-254">passwordRequiredType</span></span>|[<span data-ttu-id="5156b-255">androidDeviceOwnerRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5156b-255">androidDeviceOwnerRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|<span data-ttu-id="5156b-256">Указывает минимальную качество, необходимые на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5156b-256">Indicates the minimum password quality required on the device.</span></span> <span data-ttu-id="5156b-257">Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="5156b-257">Possible values are: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="5156b-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="5156b-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="5156b-259">Int32</span><span class="sxs-lookup"><span data-stu-id="5156b-259">Int32</span></span>|<span data-ttu-id="5156b-260">Указывает, сколько раз для ввода неправильного пароля перед Очистить устройство.</span><span class="sxs-lookup"><span data-stu-id="5156b-260">Indicates the number of times a user can enter an incorrect password before the device is wiped.</span></span> <span data-ttu-id="5156b-261">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="5156b-261">Valid values 4 to 11</span></span>|
|<span data-ttu-id="5156b-262">safeBootBlocked</span><span class="sxs-lookup"><span data-stu-id="5156b-262">safeBootBlocked</span></span>|<span data-ttu-id="5156b-263">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-263">Boolean</span></span>|<span data-ttu-id="5156b-264">Указывает, следует ли перезагрузка отключенные устройства в безопасной загрузки.</span><span class="sxs-lookup"><span data-stu-id="5156b-264">Indicates whether or not rebooting the device into safe boot is disabled.</span></span>|
|<span data-ttu-id="5156b-265">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="5156b-265">screenCaptureBlocked</span></span>|<span data-ttu-id="5156b-266">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-266">Boolean</span></span>|<span data-ttu-id="5156b-267">Указывает, следует ли отключить возможность использовать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="5156b-267">Indicates whether or not to disable the capability to take screenshots.</span></span>|
|<span data-ttu-id="5156b-268">securityAllowDebuggingFeatures</span><span class="sxs-lookup"><span data-stu-id="5156b-268">securityAllowDebuggingFeatures</span></span>|<span data-ttu-id="5156b-269">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-269">Boolean</span></span>|<span data-ttu-id="5156b-270">Указывает, следует ли пользователь не Включение функции отладки на устройстве.</span><span class="sxs-lookup"><span data-stu-id="5156b-270">Indicates whether or not to block the user from enabling debugging features on the device.</span></span>|
|<span data-ttu-id="5156b-271">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="5156b-271">securityRequireVerifyApps</span></span>|<span data-ttu-id="5156b-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="5156b-272">Boolean</span></span>|<span data-ttu-id="5156b-273">Указывает ли проверка приложений является обязательным.</span><span class="sxs-lookup"><span data-stu-id="5156b-273">Indicates whether or not verify apps is required.</span></span>|
|<span data-ttu-id="5156b-274">statusBarBlocked</span><span class="sxs-lookup"><span data-stu-id="5156b-274">statusBarBlocked</span></span>|<span data-ttu-id="5156b-275">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-275">Boolean</span></span>|<span data-ttu-id="5156b-276">Указывает, будет ли или состояние панели не действует, включая уведомления, параметры быстрого и других перекрытий экрана.</span><span class="sxs-lookup"><span data-stu-id="5156b-276">Indicates whether or the status bar is disabled, including notifications, quick settings and other screen overlays.</span></span>|
|<span data-ttu-id="5156b-277">stayOnModes</span><span class="sxs-lookup"><span data-stu-id="5156b-277">stayOnModes</span></span>|<span data-ttu-id="5156b-278">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="5156b-278">[androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md) collection</span></span>|<span data-ttu-id="5156b-279">Список режимы, в которых хранятся устройства отображения включении.</span><span class="sxs-lookup"><span data-stu-id="5156b-279">List of modes in which the device's display will stay powered-on.</span></span> <span data-ttu-id="5156b-280">Эта коллекция может содержать до 4 элементов.</span><span class="sxs-lookup"><span data-stu-id="5156b-280">This collection can contain a maximum of 4 elements.</span></span> <span data-ttu-id="5156b-281">Возможные значения: `notConfigured`, `ac`, `usb`, `wireless`.</span><span class="sxs-lookup"><span data-stu-id="5156b-281">Possible values are: `notConfigured`, `ac`, `usb`, `wireless`.</span></span>|
|<span data-ttu-id="5156b-282">storageAllowUsb</span><span class="sxs-lookup"><span data-stu-id="5156b-282">storageAllowUsb</span></span>|<span data-ttu-id="5156b-283">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-283">Boolean</span></span>|<span data-ttu-id="5156b-284">Указывает, следует ли разрешить USB запоминающих устройств.</span><span class="sxs-lookup"><span data-stu-id="5156b-284">Indicates whether or not to allow USB mass storage.</span></span>|
|<span data-ttu-id="5156b-285">storageBlockExternalMedia</span><span class="sxs-lookup"><span data-stu-id="5156b-285">storageBlockExternalMedia</span></span>|<span data-ttu-id="5156b-286">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-286">Boolean</span></span>|<span data-ttu-id="5156b-287">Указывает, следует ли блокировать внешний носитель.</span><span class="sxs-lookup"><span data-stu-id="5156b-287">Indicates whether or not to block external media.</span></span>|
|<span data-ttu-id="5156b-288">storageBlockUsbFileTransfer</span><span class="sxs-lookup"><span data-stu-id="5156b-288">storageBlockUsbFileTransfer</span></span>|<span data-ttu-id="5156b-289">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-289">Boolean</span></span>|<span data-ttu-id="5156b-290">Указывает, следует ли блокировать USB передачи файлов.</span><span class="sxs-lookup"><span data-stu-id="5156b-290">Indicates whether or not to block USB file transfer.</span></span>|
|<span data-ttu-id="5156b-291">systemUpdateWindowStartMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="5156b-291">systemUpdateWindowStartMinutesAfterMidnight</span></span>|<span data-ttu-id="5156b-292">Int32</span><span class="sxs-lookup"><span data-stu-id="5156b-292">Int32</span></span>|<span data-ttu-id="5156b-293">Указывает количество минут после полуночи, начинающимся окно обновление системы.</span><span class="sxs-lookup"><span data-stu-id="5156b-293">Indicates the number of minutes after midnight that the system update window starts.</span></span> <span data-ttu-id="5156b-294">Допустимые значения 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="5156b-294">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="5156b-295">systemUpdateWindowEndMinutesAfterMidnight</span><span class="sxs-lookup"><span data-stu-id="5156b-295">systemUpdateWindowEndMinutesAfterMidnight</span></span>|<span data-ttu-id="5156b-296">Int32</span><span class="sxs-lookup"><span data-stu-id="5156b-296">Int32</span></span>|<span data-ttu-id="5156b-297">Указывает количество минут после полуночи, завершающей окне обновление системы.</span><span class="sxs-lookup"><span data-stu-id="5156b-297">Indicates the number of minutes after midnight that the system update window ends.</span></span> <span data-ttu-id="5156b-298">Допустимые значения 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="5156b-298">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="5156b-299">systemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="5156b-299">systemUpdateInstallType</span></span>|[<span data-ttu-id="5156b-300">androidDeviceOwnerSystemUpdateInstallType</span><span class="sxs-lookup"><span data-stu-id="5156b-300">androidDeviceOwnerSystemUpdateInstallType</span></span>](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|<span data-ttu-id="5156b-301">Тип обновления конфигурации системы.</span><span class="sxs-lookup"><span data-stu-id="5156b-301">The type of system update configuration.</span></span> <span data-ttu-id="5156b-302">Возможные значения: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="5156b-302">Possible values are: `deviceDefault`, `postpone`, `windowed`, `automatic`.</span></span>|
|<span data-ttu-id="5156b-303">systemWindowsBlocked</span><span class="sxs-lookup"><span data-stu-id="5156b-303">systemWindowsBlocked</span></span>|<span data-ttu-id="5156b-304">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-304">Boolean</span></span>|<span data-ttu-id="5156b-305">Блокировать Android системы или не запрашивать пользователя windows, как всплывающие уведомления, phone действия и оповещения системы.</span><span class="sxs-lookup"><span data-stu-id="5156b-305">Whether or not to block Android system prompt windows, like toasts, phone activities, and system alerts.</span></span>|
|<span data-ttu-id="5156b-306">usersBlockAdd</span><span class="sxs-lookup"><span data-stu-id="5156b-306">usersBlockAdd</span></span>|<span data-ttu-id="5156b-307">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-307">Boolean</span></span>|<span data-ttu-id="5156b-308">Указывает, отключена ли добавление пользователей и профилей.</span><span class="sxs-lookup"><span data-stu-id="5156b-308">Indicates whether or not adding users and profiles is disabled.</span></span>|
|<span data-ttu-id="5156b-309">usersBlockRemove</span><span class="sxs-lookup"><span data-stu-id="5156b-309">usersBlockRemove</span></span>|<span data-ttu-id="5156b-310">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-310">Boolean</span></span>|<span data-ttu-id="5156b-311">Указывает, следует ли отключить удаление других пользователей с устройства.</span><span class="sxs-lookup"><span data-stu-id="5156b-311">Indicates whether or not to disable removing other users from the device.</span></span>|
|<span data-ttu-id="5156b-312">volumeBlockAdjustment</span><span class="sxs-lookup"><span data-stu-id="5156b-312">volumeBlockAdjustment</span></span>|<span data-ttu-id="5156b-313">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-313">Boolean</span></span>|<span data-ttu-id="5156b-314">Указывает, следует ли настройка отключенные громкости.</span><span class="sxs-lookup"><span data-stu-id="5156b-314">Indicates whether or not adjusting the master volume is disabled.</span></span>|
|<span data-ttu-id="5156b-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="5156b-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="5156b-316">String</span><span class="sxs-lookup"><span data-stu-id="5156b-316">String</span></span>|<span data-ttu-id="5156b-317">Имя пакета приложения для Android для приложения, которое будет обрабатывать всегда на через VPN.</span><span class="sxs-lookup"><span data-stu-id="5156b-317">Android app package name for app that will handle an always-on VPN connection.</span></span>|
|<span data-ttu-id="5156b-318">vpnAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="5156b-318">vpnAlwaysOnLockdownMode</span></span>|<span data-ttu-id="5156b-319">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-319">Boolean</span></span>|<span data-ttu-id="5156b-320">Если всегда на VPN упаковка имя заданной, ли для блокировки сетевого трафика при отключении этого VPN.</span><span class="sxs-lookup"><span data-stu-id="5156b-320">If an always on VPN package name is specified, whether or not to lock network traffic when that VPN is disconnected.</span></span>|
|<span data-ttu-id="5156b-321">wifiBlockEditConfigurations</span><span class="sxs-lookup"><span data-stu-id="5156b-321">wifiBlockEditConfigurations</span></span>|<span data-ttu-id="5156b-322">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-322">Boolean</span></span>|<span data-ttu-id="5156b-323">Указывает, следует ли пользователь не может изменять параметры подключения wifi.</span><span class="sxs-lookup"><span data-stu-id="5156b-323">Indicates whether or not to block the user from editing the wifi connection settings.</span></span>|
|<span data-ttu-id="5156b-324">wifiBlockEditPolicyDefinedConfigurations</span><span class="sxs-lookup"><span data-stu-id="5156b-324">wifiBlockEditPolicyDefinedConfigurations</span></span>|<span data-ttu-id="5156b-325">Логический</span><span class="sxs-lookup"><span data-stu-id="5156b-325">Boolean</span></span>|<span data-ttu-id="5156b-326">Указывает, следует ли пользователь не может изменять только что сетей, определенные политикой.</span><span class="sxs-lookup"><span data-stu-id="5156b-326">Indicates whether or not to block the user from editing just the networks defined by the policy.</span></span>|



## <a name="response"></a><span data-ttu-id="5156b-327">Отклик</span><span class="sxs-lookup"><span data-stu-id="5156b-327">Response</span></span>
<span data-ttu-id="5156b-328">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5156b-328">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5156b-329">Пример</span><span class="sxs-lookup"><span data-stu-id="5156b-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="5156b-330">Запрос</span><span class="sxs-lookup"><span data-stu-id="5156b-330">Request</span></span>
<span data-ttu-id="5156b-331">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5156b-331">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2517

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
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
  "appsRecommendSkippingFirstUseHints": true,
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
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
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
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```

### <a name="response"></a><span data-ttu-id="5156b-332">Отклик</span><span class="sxs-lookup"><span data-stu-id="5156b-332">Response</span></span>
<span data-ttu-id="5156b-p124">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5156b-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2689

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
  "appsRecommendSkippingFirstUseHints": true,
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
  "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
  "kioskModeExitCode": "Kiosk Mode Exit Code value",
  "kioskModeVirtualHomeButtonEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "camera"
  ],
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
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```




