---
title: Обновление объекта iosGeneralDeviceConfiguration
description: Обновление свойств объекта iosGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71a2618af07d459d52c379a27e47f7c251c9d97d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923456"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="1d23b-103">Обновление объекта iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1d23b-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="1d23b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d23b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d23b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1d23b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d23b-106">Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d23b-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d23b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1d23b-107">Prerequisites</span></span>
<span data-ttu-id="1d23b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d23b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d23b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d23b-110">Permission type</span></span>|<span data-ttu-id="1d23b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d23b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d23b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d23b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d23b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d23b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1d23b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d23b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d23b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d23b-115">Not supported.</span></span>|
|<span data-ttu-id="1d23b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d23b-116">Application</span></span>|<span data-ttu-id="1d23b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d23b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d23b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d23b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1d23b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d23b-119">Request headers</span></span>
|<span data-ttu-id="1d23b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d23b-120">Header</span></span>|<span data-ttu-id="1d23b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1d23b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d23b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d23b-122">Authorization</span></span>|<span data-ttu-id="1d23b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d23b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d23b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1d23b-124">Accept</span></span>|<span data-ttu-id="1d23b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d23b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d23b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d23b-126">Request body</span></span>
<span data-ttu-id="1d23b-127">В тексте запроса добавьте представление объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d23b-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="1d23b-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d23b-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="1d23b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d23b-129">Property</span></span>|<span data-ttu-id="1d23b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1d23b-130">Type</span></span>|<span data-ttu-id="1d23b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1d23b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d23b-132">id</span><span class="sxs-lookup"><span data-stu-id="1d23b-132">id</span></span>|<span data-ttu-id="1d23b-133">String</span><span class="sxs-lookup"><span data-stu-id="1d23b-133">String</span></span>|<span data-ttu-id="1d23b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1d23b-134">Key of the entity.</span></span> <span data-ttu-id="1d23b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d23b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d23b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d23b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1d23b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d23b-137">DateTimeOffset</span></span>|<span data-ttu-id="1d23b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1d23b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1d23b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d23b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d23b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1d23b-140">roleScopeTagIds</span></span>|<span data-ttu-id="1d23b-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1d23b-141">String collection</span></span>|<span data-ttu-id="1d23b-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1d23b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1d23b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d23b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d23b-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1d23b-144">supportsScopeTags</span></span>|<span data-ttu-id="1d23b-145">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-145">Boolean</span></span>|<span data-ttu-id="1d23b-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1d23b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1d23b-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1d23b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1d23b-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1d23b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1d23b-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1d23b-149">This property is read-only.</span></span> <span data-ttu-id="1d23b-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d23b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d23b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1d23b-151">createdDateTime</span></span>|<span data-ttu-id="1d23b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d23b-152">DateTimeOffset</span></span>|<span data-ttu-id="1d23b-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1d23b-153">DateTime the object was created.</span></span> <span data-ttu-id="1d23b-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d23b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d23b-155">description</span><span class="sxs-lookup"><span data-stu-id="1d23b-155">description</span></span>|<span data-ttu-id="1d23b-156">String</span><span class="sxs-lookup"><span data-stu-id="1d23b-156">String</span></span>|<span data-ttu-id="1d23b-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1d23b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1d23b-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d23b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d23b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1d23b-159">displayName</span></span>|<span data-ttu-id="1d23b-160">Строка</span><span class="sxs-lookup"><span data-stu-id="1d23b-160">String</span></span>|<span data-ttu-id="1d23b-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1d23b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1d23b-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1d23b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d23b-163">version</span><span class="sxs-lookup"><span data-stu-id="1d23b-163">version</span></span>|<span data-ttu-id="1d23b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1d23b-164">Int32</span></span>|<span data-ttu-id="1d23b-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1d23b-165">Version of the device configuration.</span></span> <span data-ttu-id="1d23b-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1d23b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1d23b-167">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="1d23b-167">accountBlockModification</span></span>|<span data-ttu-id="1d23b-168">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-168">Boolean</span></span>|<span data-ttu-id="1d23b-169">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-169">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-170">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="1d23b-170">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="1d23b-171">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-171">Boolean</span></span>|<span data-ttu-id="1d23b-172">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-172">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="1d23b-173">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-173">airDropBlocked</span></span>|<span data-ttu-id="1d23b-174">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-174">Boolean</span></span>|<span data-ttu-id="1d23b-175">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-175">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-176">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="1d23b-176">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="1d23b-177">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-177">Boolean</span></span>|<span data-ttu-id="1d23b-178">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-178">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1d23b-179">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="1d23b-179">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="1d23b-180">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-180">Boolean</span></span>|<span data-ttu-id="1d23b-181">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="1d23b-181">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="1d23b-182">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="1d23b-182">appleWatchBlockPairing</span></span>|<span data-ttu-id="1d23b-183">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-183">Boolean</span></span>|<span data-ttu-id="1d23b-184">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-184">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1d23b-185">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="1d23b-185">appleWatchForceWristDetection</span></span>|<span data-ttu-id="1d23b-186">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-186">Boolean</span></span>|<span data-ttu-id="1d23b-187">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-187">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="1d23b-188">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-188">appleNewsBlocked</span></span>|<span data-ttu-id="1d23b-189">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-189">Boolean</span></span>|<span data-ttu-id="1d23b-190">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-190">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1d23b-191">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="1d23b-191">appsSingleAppModeList</span></span>|<span data-ttu-id="1d23b-192">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1d23b-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1d23b-193">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="1d23b-193">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="1d23b-194">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-194">Supervised only.</span></span> <span data-ttu-id="1d23b-195">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="1d23b-195">iOS 7.0 and later.</span></span> <span data-ttu-id="1d23b-196">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1d23b-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1d23b-197">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="1d23b-197">appsVisibilityList</span></span>|<span data-ttu-id="1d23b-198">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1d23b-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1d23b-199">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-199">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="1d23b-200">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="1d23b-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="1d23b-201">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="1d23b-201">appsVisibilityListType</span></span>|[<span data-ttu-id="1d23b-202">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="1d23b-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="1d23b-203">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="1d23b-203">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="1d23b-204">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="1d23b-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="1d23b-205">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="1d23b-205">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="1d23b-206">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-206">Boolean</span></span>|<span data-ttu-id="1d23b-207">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-207">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1d23b-208">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-208">appStoreBlocked</span></span>|<span data-ttu-id="1d23b-209">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-209">Boolean</span></span>|<span data-ttu-id="1d23b-210">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="1d23b-210">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="1d23b-211">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="1d23b-211">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="1d23b-212">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-212">Boolean</span></span>|<span data-ttu-id="1d23b-213">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="1d23b-213">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="1d23b-214">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="1d23b-214">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="1d23b-215">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-215">Boolean</span></span>|<span data-ttu-id="1d23b-216">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="1d23b-216">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="1d23b-217">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-217">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1d23b-218">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="1d23b-218">appStoreRequirePassword</span></span>|<span data-ttu-id="1d23b-219">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-219">Boolean</span></span>|<span data-ttu-id="1d23b-220">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="1d23b-220">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="1d23b-221">Аутофиллфорцеаусентикатион</span><span class="sxs-lookup"><span data-stu-id="1d23b-221">autoFillForceAuthentication</span></span>|<span data-ttu-id="1d23b-222">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-222">Boolean</span></span>|<span data-ttu-id="1d23b-223">Указывает, следует ли принудительно выполнять проверку подлинности пользователей перед автозаполнением паролей и сведений о кредитных картах в Safari и других приложениях на контролируемых устройствах.</span><span class="sxs-lookup"><span data-stu-id="1d23b-223">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="1d23b-224">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="1d23b-224">bluetoothBlockModification</span></span>|<span data-ttu-id="1d23b-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d23b-225">Boolean</span></span>|<span data-ttu-id="1d23b-226">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-226">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="1d23b-227">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-227">cameraBlocked</span></span>|<span data-ttu-id="1d23b-228">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-228">Boolean</span></span>|<span data-ttu-id="1d23b-229">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="1d23b-229">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="1d23b-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="1d23b-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="1d23b-231">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-231">Boolean</span></span>|<span data-ttu-id="1d23b-232">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="1d23b-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="1d23b-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="1d23b-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="1d23b-234">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-234">Boolean</span></span>|<span data-ttu-id="1d23b-235">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="1d23b-235">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="1d23b-236">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="1d23b-236">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="1d23b-237">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-237">Boolean</span></span>|<span data-ttu-id="1d23b-238">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-238">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-239">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="1d23b-239">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="1d23b-240">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-240">Boolean</span></span>|<span data-ttu-id="1d23b-241">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="1d23b-241">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="1d23b-242">Целлуларблоккпланмодификатион</span><span class="sxs-lookup"><span data-stu-id="1d23b-242">cellularBlockPlanModification</span></span>|<span data-ttu-id="1d23b-243">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-243">Boolean</span></span>|<span data-ttu-id="1d23b-244">Указывает, следует ли запретить пользователям изменять параметры плана сотовой связи на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="1d23b-244">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="1d23b-245">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="1d23b-245">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="1d23b-246">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-246">Boolean</span></span>|<span data-ttu-id="1d23b-247">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="1d23b-247">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="1d23b-248">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="1d23b-248">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="1d23b-249">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-249">Boolean</span></span>|<span data-ttu-id="1d23b-250">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="1d23b-250">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="1d23b-251">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="1d23b-251">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="1d23b-252">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-252">Boolean</span></span>|<span data-ttu-id="1d23b-253">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-253">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="1d23b-254">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="1d23b-254">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="1d23b-255">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-255">Boolean</span></span>|<span data-ttu-id="1d23b-256">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-256">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-257">Классрумфорцеаутоматикаллижоинклассес</span><span class="sxs-lookup"><span data-stu-id="1d23b-257">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="1d23b-258">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-258">Boolean</span></span>|<span data-ttu-id="1d23b-259">Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-259">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-260">Классрумфорцеунпромптедаппанддевицелокк</span><span class="sxs-lookup"><span data-stu-id="1d23b-260">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="1d23b-261">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-261">Boolean</span></span>|<span data-ttu-id="1d23b-262">Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся.</span><span class="sxs-lookup"><span data-stu-id="1d23b-262">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="1d23b-263">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-263">Supervised only.</span></span>|
|<span data-ttu-id="1d23b-264">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="1d23b-264">compliantAppsList</span></span>|<span data-ttu-id="1d23b-265">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="1d23b-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="1d23b-266">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="1d23b-266">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="1d23b-267">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="1d23b-267">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="1d23b-268">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="1d23b-268">compliantAppListType</span></span>|[<span data-ttu-id="1d23b-269">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="1d23b-269">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="1d23b-270">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="1d23b-270">List that is in the AppComplianceList.</span></span> <span data-ttu-id="1d23b-271">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="1d23b-271">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="1d23b-272">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="1d23b-272">configurationProfileBlockChanges</span></span>|<span data-ttu-id="1d23b-273">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-273">Boolean</span></span>|<span data-ttu-id="1d23b-274">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-274">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-275">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-275">definitionLookupBlocked</span></span>|<span data-ttu-id="1d23b-276">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-276">Boolean</span></span>|<span data-ttu-id="1d23b-277">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-277">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="1d23b-278">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="1d23b-278">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="1d23b-279">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-279">Boolean</span></span>|<span data-ttu-id="1d23b-280">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-280">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-281">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="1d23b-281">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="1d23b-282">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-282">Boolean</span></span>|<span data-ttu-id="1d23b-283">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-283">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-284">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="1d23b-284">deviceBlockNameModification</span></span>|<span data-ttu-id="1d23b-285">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-285">Boolean</span></span>|<span data-ttu-id="1d23b-286">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-286">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1d23b-287">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="1d23b-287">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="1d23b-288">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-288">Boolean</span></span>|<span data-ttu-id="1d23b-289">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="1d23b-289">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="1d23b-290">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="1d23b-290">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="1d23b-291">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-291">Boolean</span></span>|<span data-ttu-id="1d23b-292">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-292">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="1d23b-293">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="1d23b-293">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="1d23b-294">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-294">Boolean</span></span>|<span data-ttu-id="1d23b-295">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="1d23b-295">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="1d23b-296">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="1d23b-296">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="1d23b-297">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-297">Boolean</span></span>|<span data-ttu-id="1d23b-298">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="1d23b-298">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="1d23b-299">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="1d23b-299">emailInDomainSuffixes</span></span>|<span data-ttu-id="1d23b-300">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1d23b-300">String collection</span></span>|<span data-ttu-id="1d23b-301">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="1d23b-301">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="1d23b-302">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="1d23b-302">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="1d23b-303">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-303">Boolean</span></span>|<span data-ttu-id="1d23b-304">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="1d23b-304">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="1d23b-305">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="1d23b-305">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="1d23b-306">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-306">Boolean</span></span>|<span data-ttu-id="1d23b-307">Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="1d23b-307">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="1d23b-308">Есимблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="1d23b-308">esimBlockModification</span></span>|<span data-ttu-id="1d23b-309">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-309">Boolean</span></span>|<span data-ttu-id="1d23b-310">Указывает, следует ли разрешить добавление или удаление планов сотовой связи на eSIM контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="1d23b-310">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="1d23b-311">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-311">faceTimeBlocked</span></span>|<span data-ttu-id="1d23b-312">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-312">Boolean</span></span>|<span data-ttu-id="1d23b-313">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="1d23b-313">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="1d23b-314">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-314">findMyFriendsBlocked</span></span>|<span data-ttu-id="1d23b-315">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-315">Boolean</span></span>|<span data-ttu-id="1d23b-316">Указывает, следует ли заблокировать функцию "Найти друзей", когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-316">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-317">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="1d23b-317">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="1d23b-318">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-318">Boolean</span></span>|<span data-ttu-id="1d23b-319">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="1d23b-319">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="1d23b-320">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="1d23b-320">gamingBlockMultiplayer</span></span>|<span data-ttu-id="1d23b-321">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-321">Boolean</span></span>|<span data-ttu-id="1d23b-322">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="1d23b-322">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="1d23b-323">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-323">gameCenterBlocked</span></span>|<span data-ttu-id="1d23b-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d23b-324">Boolean</span></span>|<span data-ttu-id="1d23b-325">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-325">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-326">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-326">hostPairingBlocked</span></span>|<span data-ttu-id="1d23b-327">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-327">Boolean</span></span>|<span data-ttu-id="1d23b-328">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-328">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-329">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-329">iBooksStoreBlocked</span></span>|<span data-ttu-id="1d23b-330">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-330">Boolean</span></span>|<span data-ttu-id="1d23b-331">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-331">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-332">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="1d23b-332">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="1d23b-333">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-333">Boolean</span></span>|<span data-ttu-id="1d23b-334">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="1d23b-334">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="1d23b-335">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="1d23b-335">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="1d23b-336">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-336">Boolean</span></span>|<span data-ttu-id="1d23b-337">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="1d23b-337">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="1d23b-338">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="1d23b-338">iCloudBlockBackup</span></span>|<span data-ttu-id="1d23b-339">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-339">Boolean</span></span>|<span data-ttu-id="1d23b-340">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="1d23b-340">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="1d23b-341">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="1d23b-341">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="1d23b-342">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-342">Boolean</span></span>|<span data-ttu-id="1d23b-343">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="1d23b-343">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="1d23b-344">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="1d23b-344">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="1d23b-345">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-345">Boolean</span></span>|<span data-ttu-id="1d23b-346">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="1d23b-346">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="1d23b-347">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="1d23b-347">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="1d23b-348">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-348">Boolean</span></span>|<span data-ttu-id="1d23b-349">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="1d23b-349">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="1d23b-350">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="1d23b-350">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="1d23b-351">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-351">Boolean</span></span>|<span data-ttu-id="1d23b-352">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="1d23b-352">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="1d23b-353">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="1d23b-353">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="1d23b-354">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-354">Boolean</span></span>|<span data-ttu-id="1d23b-355">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="1d23b-355">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="1d23b-356">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="1d23b-356">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="1d23b-357">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-357">Boolean</span></span>|<span data-ttu-id="1d23b-358">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="1d23b-358">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="1d23b-359">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="1d23b-359">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="1d23b-360">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-360">Boolean</span></span>|<span data-ttu-id="1d23b-361">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="1d23b-361">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="1d23b-362">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="1d23b-362">iTunesBlockMusicService</span></span>|<span data-ttu-id="1d23b-363">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-363">Boolean</span></span>|<span data-ttu-id="1d23b-364">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-364">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="1d23b-365">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="1d23b-365">iTunesBlockRadio</span></span>|<span data-ttu-id="1d23b-366">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-366">Boolean</span></span>|<span data-ttu-id="1d23b-367">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-367">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="1d23b-368">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="1d23b-368">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="1d23b-369">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-369">Boolean</span></span>|<span data-ttu-id="1d23b-370">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-370">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="1d23b-371">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="1d23b-371">keyboardBlockDictation</span></span>|<span data-ttu-id="1d23b-372">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-372">Boolean</span></span>|<span data-ttu-id="1d23b-373">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-373">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-374">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="1d23b-374">keyboardBlockPredictive</span></span>|<span data-ttu-id="1d23b-375">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-375">Boolean</span></span>|<span data-ttu-id="1d23b-376">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-376">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="1d23b-377">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="1d23b-377">keyboardBlockShortcuts</span></span>|<span data-ttu-id="1d23b-378">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-378">Boolean</span></span>|<span data-ttu-id="1d23b-379">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-379">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1d23b-380">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="1d23b-380">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="1d23b-381">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-381">Boolean</span></span>|<span data-ttu-id="1d23b-382">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-382">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="1d23b-383">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="1d23b-383">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="1d23b-384">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-384">Boolean</span></span>|<span data-ttu-id="1d23b-385">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-385">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-386">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="1d23b-386">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="1d23b-387">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-387">Boolean</span></span>|<span data-ttu-id="1d23b-388">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-388">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-389">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="1d23b-389">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="1d23b-390">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-390">Boolean</span></span>|<span data-ttu-id="1d23b-391">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-391">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="1d23b-392">ФунЦитоналити этого свойства является избыточным по умолчанию для ОС и является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="1d23b-392">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="1d23b-393">Вместо этого используйте Киоскмодеблоккаутолокк.</span><span class="sxs-lookup"><span data-stu-id="1d23b-393">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="1d23b-394">Киоскмодеблоккаутолокк</span><span class="sxs-lookup"><span data-stu-id="1d23b-394">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="1d23b-395">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-395">Boolean</span></span>|<span data-ttu-id="1d23b-396">Указывает, следует ли блокировать автоматическую блокировку устройств в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-396">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-397">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="1d23b-397">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="1d23b-398">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-398">Boolean</span></span>|<span data-ttu-id="1d23b-399">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-399">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-400">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="1d23b-400">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="1d23b-401">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-401">Boolean</span></span>|<span data-ttu-id="1d23b-402">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-402">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="1d23b-403">ФунЦитоналити этого свойства является избыточным по умолчанию для ОС и является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="1d23b-403">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="1d23b-404">Вместо этого используйте Киоскмодеблоккринжерсвитч.</span><span class="sxs-lookup"><span data-stu-id="1d23b-404">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="1d23b-405">Киоскмодеблоккринжерсвитч</span><span class="sxs-lookup"><span data-stu-id="1d23b-405">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="1d23b-406">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-406">Boolean</span></span>|<span data-ttu-id="1d23b-407">Указывает, следует ли запретить использование переключателя звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-407">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-408">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="1d23b-408">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="1d23b-409">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-409">Boolean</span></span>|<span data-ttu-id="1d23b-410">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-410">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="1d23b-411">ФунЦитоналити этого свойства является избыточным по умолчанию для ОС и является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="1d23b-411">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="1d23b-412">Вместо этого используйте Киоскмодеблоккскринротатион.</span><span class="sxs-lookup"><span data-stu-id="1d23b-412">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="1d23b-413">Киоскмодеблоккскринротатион</span><span class="sxs-lookup"><span data-stu-id="1d23b-413">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="1d23b-414">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-414">Boolean</span></span>|<span data-ttu-id="1d23b-415">Указывает, следует ли блокировать поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-415">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-416">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="1d23b-416">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="1d23b-417">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-417">Boolean</span></span>|<span data-ttu-id="1d23b-418">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-418">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="1d23b-419">ФунЦитоналити этого свойства является избыточным по умолчанию для ОС и является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="1d23b-419">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="1d23b-420">Вместо этого используйте Киоскмодеблоккслипбуттон.</span><span class="sxs-lookup"><span data-stu-id="1d23b-420">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="1d23b-421">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="1d23b-421">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="1d23b-422">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-422">Boolean</span></span>|<span data-ttu-id="1d23b-423">Указывает, следует ли запретить использование кнопки "сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-423">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-424">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="1d23b-424">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="1d23b-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d23b-425">Boolean</span></span>|<span data-ttu-id="1d23b-426">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-426">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="1d23b-427">ФунЦитоналити этого свойства является избыточным по умолчанию для ОС и является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="1d23b-427">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="1d23b-428">Вместо этого используйте Киоскмодеблокктаучскрин.</span><span class="sxs-lookup"><span data-stu-id="1d23b-428">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="1d23b-429">Киоскмодеблокктаучскрин</span><span class="sxs-lookup"><span data-stu-id="1d23b-429">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="1d23b-430">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-430">Boolean</span></span>|<span data-ttu-id="1d23b-431">Указывает, следует ли запретить использование сенсорного экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-431">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-432">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="1d23b-432">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="1d23b-433">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-433">Boolean</span></span>|<span data-ttu-id="1d23b-434">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-434">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-435">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="1d23b-435">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="1d23b-436">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-436">Boolean</span></span>|<span data-ttu-id="1d23b-437">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-437">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="1d23b-438">ФунЦитоналити этого свойства является избыточным по умолчанию для ОС и является устаревшим.</span><span class="sxs-lookup"><span data-stu-id="1d23b-438">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="1d23b-439">Вместо этого используйте Киоскмодеблоккволумебуттонс.</span><span class="sxs-lookup"><span data-stu-id="1d23b-439">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="1d23b-440">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="1d23b-440">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="1d23b-441">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-441">Boolean</span></span>|<span data-ttu-id="1d23b-442">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="1d23b-442">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="1d23b-443">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="1d23b-443">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="1d23b-444">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-444">Boolean</span></span>|<span data-ttu-id="1d23b-445">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-445">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-446">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1d23b-446">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="1d23b-447">Строка</span><span class="sxs-lookup"><span data-stu-id="1d23b-447">String</span></span>|<span data-ttu-id="1d23b-448">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-448">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="1d23b-449">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="1d23b-449">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="1d23b-450">Киоскмодебуилтинаппид</span><span class="sxs-lookup"><span data-stu-id="1d23b-450">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="1d23b-451">Строка</span><span class="sxs-lookup"><span data-stu-id="1d23b-451">String</span></span>|<span data-ttu-id="1d23b-452">Идентификатор встроенных приложений для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-452">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="1d23b-453">Используется, когда KioskModeManagedAppId и KioskModeAppStoreUrl не заданы.</span><span class="sxs-lookup"><span data-stu-id="1d23b-453">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="1d23b-454">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="1d23b-454">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="1d23b-455">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-455">Boolean</span></span>|<span data-ttu-id="1d23b-456">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-456">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-457">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="1d23b-457">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="1d23b-458">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-458">Boolean</span></span>|<span data-ttu-id="1d23b-459">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-459">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-460">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="1d23b-460">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="1d23b-461">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-461">Boolean</span></span>|<span data-ttu-id="1d23b-462">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-462">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-463">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="1d23b-463">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="1d23b-464">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-464">Boolean</span></span>|<span data-ttu-id="1d23b-465">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-465">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-466">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="1d23b-466">kioskModeRequireZoom</span></span>|<span data-ttu-id="1d23b-467">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-467">Boolean</span></span>|<span data-ttu-id="1d23b-468">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-468">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="1d23b-469">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="1d23b-469">kioskModeManagedAppId</span></span>|<span data-ttu-id="1d23b-470">String</span><span class="sxs-lookup"><span data-stu-id="1d23b-470">String</span></span>|<span data-ttu-id="1d23b-471">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="1d23b-471">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="1d23b-472">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="1d23b-472">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="1d23b-473">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="1d23b-473">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="1d23b-474">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-474">Boolean</span></span>|<span data-ttu-id="1d23b-475">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="1d23b-475">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="1d23b-476">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="1d23b-476">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="1d23b-477">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-477">Boolean</span></span>|<span data-ttu-id="1d23b-478">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="1d23b-478">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="1d23b-479">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="1d23b-479">lockScreenBlockPassbook</span></span>|<span data-ttu-id="1d23b-480">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-480">Boolean</span></span>|<span data-ttu-id="1d23b-481">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="1d23b-481">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="1d23b-482">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="1d23b-482">lockScreenBlockTodayView</span></span>|<span data-ttu-id="1d23b-483">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-483">Boolean</span></span>|<span data-ttu-id="1d23b-484">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="1d23b-484">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="1d23b-485">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="1d23b-485">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="1d23b-486">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="1d23b-486">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="1d23b-487">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="1d23b-487">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="1d23b-488">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="1d23b-488">mediaContentRatingCanada</span></span>|[<span data-ttu-id="1d23b-489">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="1d23b-489">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="1d23b-490">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="1d23b-490">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="1d23b-491">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="1d23b-491">mediaContentRatingFrance</span></span>|[<span data-ttu-id="1d23b-492">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="1d23b-492">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="1d23b-493">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="1d23b-493">Media content rating settings for France</span></span>|
|<span data-ttu-id="1d23b-494">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="1d23b-494">mediaContentRatingGermany</span></span>|[<span data-ttu-id="1d23b-495">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="1d23b-495">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="1d23b-496">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="1d23b-496">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="1d23b-497">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="1d23b-497">mediaContentRatingIreland</span></span>|[<span data-ttu-id="1d23b-498">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="1d23b-498">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="1d23b-499">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="1d23b-499">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="1d23b-500">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="1d23b-500">mediaContentRatingJapan</span></span>|[<span data-ttu-id="1d23b-501">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="1d23b-501">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="1d23b-502">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="1d23b-502">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="1d23b-503">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="1d23b-503">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="1d23b-504">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="1d23b-504">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="1d23b-505">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="1d23b-505">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="1d23b-506">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="1d23b-506">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="1d23b-507">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="1d23b-507">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="1d23b-508">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="1d23b-508">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="1d23b-509">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="1d23b-509">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="1d23b-510">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="1d23b-510">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="1d23b-511">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="1d23b-511">Media content rating settings for United States</span></span>|
|<span data-ttu-id="1d23b-512">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="1d23b-512">networkUsageRules</span></span>|<span data-ttu-id="1d23b-513">Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="1d23b-513">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="1d23b-514">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="1d23b-514">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="1d23b-515">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="1d23b-515">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="1d23b-516">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="1d23b-516">mediaContentRatingApps</span></span>|[<span data-ttu-id="1d23b-517">Ратингаппстипе</span><span class="sxs-lookup"><span data-stu-id="1d23b-517">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="1d23b-518">Параметры оценки контента мультимедиа для приложений.</span><span class="sxs-lookup"><span data-stu-id="1d23b-518">Media content rating settings for Apps.</span></span> <span data-ttu-id="1d23b-519">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="1d23b-519">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="1d23b-520">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-520">messagesBlocked</span></span>|<span data-ttu-id="1d23b-521">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-521">Boolean</span></span>|<span data-ttu-id="1d23b-522">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="1d23b-522">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="1d23b-523">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="1d23b-523">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="1d23b-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d23b-524">Boolean</span></span>|<span data-ttu-id="1d23b-525">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-525">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="1d23b-526">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="1d23b-526">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="1d23b-527">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-527">Boolean</span></span>|<span data-ttu-id="1d23b-528">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="1d23b-528">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="1d23b-529">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="1d23b-529">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="1d23b-530">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-530">Boolean</span></span>|<span data-ttu-id="1d23b-531">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-531">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-532">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="1d23b-532">passcodeBlockModification</span></span>|<span data-ttu-id="1d23b-533">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-533">Boolean</span></span>|<span data-ttu-id="1d23b-534">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-534">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="1d23b-535">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="1d23b-535">passcodeBlockSimple</span></span>|<span data-ttu-id="1d23b-536">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-536">Boolean</span></span>|<span data-ttu-id="1d23b-537">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="1d23b-537">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="1d23b-538">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1d23b-538">passcodeExpirationDays</span></span>|<span data-ttu-id="1d23b-539">Int32</span><span class="sxs-lookup"><span data-stu-id="1d23b-539">Int32</span></span>|<span data-ttu-id="1d23b-540">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="1d23b-540">Number of days before the passcode expires.</span></span> <span data-ttu-id="1d23b-541">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="1d23b-541">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="1d23b-542">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1d23b-542">passcodeMinimumLength</span></span>|<span data-ttu-id="1d23b-543">Int32</span><span class="sxs-lookup"><span data-stu-id="1d23b-543">Int32</span></span>|<span data-ttu-id="1d23b-544">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="1d23b-544">Minimum length of passcode.</span></span> <span data-ttu-id="1d23b-545">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="1d23b-545">Valid values 4 to 14</span></span>|
|<span data-ttu-id="1d23b-546">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="1d23b-546">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="1d23b-547">Int32</span><span class="sxs-lookup"><span data-stu-id="1d23b-547">Int32</span></span>|<span data-ttu-id="1d23b-548">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="1d23b-548">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="1d23b-549">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1d23b-549">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1d23b-550">Int32</span><span class="sxs-lookup"><span data-stu-id="1d23b-550">Int32</span></span>|<span data-ttu-id="1d23b-551">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="1d23b-551">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1d23b-552">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="1d23b-552">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="1d23b-553">Int32</span><span class="sxs-lookup"><span data-stu-id="1d23b-553">Int32</span></span>|<span data-ttu-id="1d23b-554">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="1d23b-554">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="1d23b-555">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="1d23b-555">Valid values 0 to 4</span></span>|
|<span data-ttu-id="1d23b-556">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="1d23b-556">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="1d23b-557">Int32</span><span class="sxs-lookup"><span data-stu-id="1d23b-557">Int32</span></span>|<span data-ttu-id="1d23b-558">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="1d23b-558">Number of previous passcodes to block.</span></span> <span data-ttu-id="1d23b-559">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="1d23b-559">Valid values 1 to 24</span></span>|
|<span data-ttu-id="1d23b-560">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="1d23b-560">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="1d23b-561">Int32</span><span class="sxs-lookup"><span data-stu-id="1d23b-561">Int32</span></span>|<span data-ttu-id="1d23b-562">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="1d23b-562">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="1d23b-563">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="1d23b-563">Valid values 4 to 11</span></span>|
|<span data-ttu-id="1d23b-564">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="1d23b-564">passcodeRequiredType</span></span>|[<span data-ttu-id="1d23b-565">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="1d23b-565">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="1d23b-566">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="1d23b-566">Type of passcode that is required.</span></span> <span data-ttu-id="1d23b-567">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="1d23b-567">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="1d23b-568">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="1d23b-568">passcodeRequired</span></span>|<span data-ttu-id="1d23b-569">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-569">Boolean</span></span>|<span data-ttu-id="1d23b-570">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="1d23b-570">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="1d23b-571">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-571">podcastsBlocked</span></span>|<span data-ttu-id="1d23b-572">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-572">Boolean</span></span>|<span data-ttu-id="1d23b-573">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-573">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="1d23b-574">Проксимитиблокксетуптоневдевице</span><span class="sxs-lookup"><span data-stu-id="1d23b-574">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="1d23b-575">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-575">Boolean</span></span>|<span data-ttu-id="1d23b-576">Указывает, следует ли включить запрос на установку находящихся рядом устройств с защищенным устройством.</span><span class="sxs-lookup"><span data-stu-id="1d23b-576">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="1d23b-577">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="1d23b-577">safariBlockAutofill</span></span>|<span data-ttu-id="1d23b-578">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-578">Boolean</span></span>|<span data-ttu-id="1d23b-579">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="1d23b-579">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="1d23b-580">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="1d23b-580">safariBlockJavaScript</span></span>|<span data-ttu-id="1d23b-581">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-581">Boolean</span></span>|<span data-ttu-id="1d23b-582">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="1d23b-582">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="1d23b-583">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="1d23b-583">safariBlockPopups</span></span>|<span data-ttu-id="1d23b-584">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-584">Boolean</span></span>|<span data-ttu-id="1d23b-585">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="1d23b-585">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="1d23b-586">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-586">safariBlocked</span></span>|<span data-ttu-id="1d23b-587">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-587">Boolean</span></span>|<span data-ttu-id="1d23b-588">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="1d23b-588">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="1d23b-589">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="1d23b-589">safariCookieSettings</span></span>|[<span data-ttu-id="1d23b-590">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="1d23b-590">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="1d23b-591">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="1d23b-591">Cookie settings for Safari.</span></span> <span data-ttu-id="1d23b-592">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="1d23b-592">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="1d23b-593">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="1d23b-593">safariManagedDomains</span></span>|<span data-ttu-id="1d23b-594">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1d23b-594">String collection</span></span>|<span data-ttu-id="1d23b-595">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="1d23b-595">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="1d23b-596">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="1d23b-596">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="1d23b-597">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1d23b-597">String collection</span></span>|<span data-ttu-id="1d23b-598">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="1d23b-598">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="1d23b-599">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-599">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="1d23b-600">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="1d23b-600">safariRequireFraudWarning</span></span>|<span data-ttu-id="1d23b-601">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-601">Boolean</span></span>|<span data-ttu-id="1d23b-602">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="1d23b-602">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="1d23b-603">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-603">screenCaptureBlocked</span></span>|<span data-ttu-id="1d23b-604">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-604">Boolean</span></span>|<span data-ttu-id="1d23b-605">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="1d23b-605">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="1d23b-606">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-606">siriBlocked</span></span>|<span data-ttu-id="1d23b-607">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-607">Boolean</span></span>|<span data-ttu-id="1d23b-608">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="1d23b-608">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="1d23b-609">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-609">siriBlockedWhenLocked</span></span>|<span data-ttu-id="1d23b-610">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-610">Boolean</span></span>|<span data-ttu-id="1d23b-611">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="1d23b-611">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="1d23b-612">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="1d23b-612">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="1d23b-613">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-613">Boolean</span></span>|<span data-ttu-id="1d23b-614">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="1d23b-614">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="1d23b-615">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="1d23b-615">siriRequireProfanityFilter</span></span>|<span data-ttu-id="1d23b-616">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d23b-616">Boolean</span></span>|<span data-ttu-id="1d23b-617">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="1d23b-617">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="1d23b-618">Софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="1d23b-618">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="1d23b-619">Int32</span><span class="sxs-lookup"><span data-stu-id="1d23b-619">Int32</span></span>|<span data-ttu-id="1d23b-620">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="1d23b-620">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="1d23b-621">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="1d23b-621">Valid values 0 to 90</span></span>|
|<span data-ttu-id="1d23b-622">Софтвареупдатесфорцеделайед</span><span class="sxs-lookup"><span data-stu-id="1d23b-622">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="1d23b-623">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-623">Boolean</span></span>|<span data-ttu-id="1d23b-624">Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-624">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-625">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="1d23b-625">spotlightBlockInternetResults</span></span>|<span data-ttu-id="1d23b-626">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-626">Boolean</span></span>|<span data-ttu-id="1d23b-627">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="1d23b-627">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="1d23b-628">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-628">voiceDialingBlocked</span></span>|<span data-ttu-id="1d23b-629">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-629">Boolean</span></span>|<span data-ttu-id="1d23b-630">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="1d23b-630">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="1d23b-631">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="1d23b-631">wallpaperBlockModification</span></span>|<span data-ttu-id="1d23b-632">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-632">Boolean</span></span>|<span data-ttu-id="1d23b-633">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-633">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="1d23b-634">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="1d23b-634">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="1d23b-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d23b-635">Boolean</span></span>|<span data-ttu-id="1d23b-636">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="1d23b-636">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="1d23b-637">Классрумфорцерекуестпермиссионтолеавеклассес</span><span class="sxs-lookup"><span data-stu-id="1d23b-637">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="1d23b-638">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-638">Boolean</span></span>|<span data-ttu-id="1d23b-639">Указывает, является ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса (iOS 11,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-639">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="1d23b-640">Кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="1d23b-640">keychainBlockCloudSync</span></span>|<span data-ttu-id="1d23b-641">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-641">Boolean</span></span>|<span data-ttu-id="1d23b-642">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud.</span><span class="sxs-lookup"><span data-stu-id="1d23b-642">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="1d23b-643">Пкиблоккотаупдатес</span><span class="sxs-lookup"><span data-stu-id="1d23b-643">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="1d23b-644">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-644">Boolean</span></span>|<span data-ttu-id="1d23b-645">Указывает, блокируются ли обновления PKI беспроводной сети.</span><span class="sxs-lookup"><span data-stu-id="1d23b-645">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="1d23b-646">Если задать для этого ограничения значение false, проверки CRL и OCSP (iOS 7,0 и более поздних версий) не отключаются.</span><span class="sxs-lookup"><span data-stu-id="1d23b-646">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="1d23b-647">Привацифорцелимитадтраккинг</span><span class="sxs-lookup"><span data-stu-id="1d23b-647">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="1d23b-648">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-648">Boolean</span></span>|<span data-ttu-id="1d23b-649">Указывает, ограничено ли отслеживание AD. (iOS 7,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-649">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="1d23b-650">Ентерприсебукблоккбаккуп</span><span class="sxs-lookup"><span data-stu-id="1d23b-650">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="1d23b-651">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-651">Boolean</span></span>|<span data-ttu-id="1d23b-652">Указывает, блокируется ли резервное копирование корпоративной книги.</span><span class="sxs-lookup"><span data-stu-id="1d23b-652">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="1d23b-653">Ентерприсебукблоккметадатасинк</span><span class="sxs-lookup"><span data-stu-id="1d23b-653">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="1d23b-654">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-654">Boolean</span></span>|<span data-ttu-id="1d23b-655">Указывает, блокируется ли синхронизация заметок и выделений корпоративных книг.</span><span class="sxs-lookup"><span data-stu-id="1d23b-655">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="1d23b-656">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="1d23b-656">airPrintBlocked</span></span>|<span data-ttu-id="1d23b-657">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-657">Boolean</span></span>|<span data-ttu-id="1d23b-658">Указывает, заблокировано ли Аирпринт (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-658">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1d23b-659">Аирпринтблокккредентиалсстораже</span><span class="sxs-lookup"><span data-stu-id="1d23b-659">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="1d23b-660">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-660">Boolean</span></span>|<span data-ttu-id="1d23b-661">Указывает, заблокировано ли хранение цепочки ключей имени пользователя и пароля для Аирпринт (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-661">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1d23b-662">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="1d23b-662">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="1d23b-663">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-663">Boolean</span></span>|<span data-ttu-id="1d23b-664">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-664">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1d23b-665">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="1d23b-665">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="1d23b-666">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-666">Boolean</span></span>|<span data-ttu-id="1d23b-667">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="1d23b-667">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="1d23b-668">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-668">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1d23b-669">Блокксистемаппремовал</span><span class="sxs-lookup"><span data-stu-id="1d23b-669">blockSystemAppRemoval</span></span>|<span data-ttu-id="1d23b-670">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-670">Boolean</span></span>|<span data-ttu-id="1d23b-671">Указывает, заблокировано ли удаление системных приложений с устройства на контролируемом устройстве (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-671">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1d23b-672">Впнблокккреатион</span><span class="sxs-lookup"><span data-stu-id="1d23b-672">vpnBlockCreation</span></span>|<span data-ttu-id="1d23b-673">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-673">Boolean</span></span>|<span data-ttu-id="1d23b-674">Указывает, блокируется ли создание конфигураций VPN (iOS 11,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-674">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="1d23b-675">Аппремовалблоккед</span><span class="sxs-lookup"><span data-stu-id="1d23b-675">appRemovalBlocked</span></span>|<span data-ttu-id="1d23b-676">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-676">Boolean</span></span>|<span data-ttu-id="1d23b-677">Указывает, разрешено ли удаление приложений.</span><span class="sxs-lookup"><span data-stu-id="1d23b-677">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="1d23b-678">Усбрестриктедмодеблоккед</span><span class="sxs-lookup"><span data-stu-id="1d23b-678">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="1d23b-679">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-679">Boolean</span></span>|<span data-ttu-id="1d23b-680">Указывает, разрешена ли подключаться к стандарту USB, пока устройство заблокировано (iOS 11.4.1 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-680">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="1d23b-681">Пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="1d23b-681">passwordBlockAutoFill</span></span>|<span data-ttu-id="1d23b-682">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-682">Boolean</span></span>|<span data-ttu-id="1d23b-683">Указывает, разрешена ли функция автозаполнения паролей (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-683">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="1d23b-684">Пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="1d23b-684">passwordBlockProximityRequests</span></span>|<span data-ttu-id="1d23b-685">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-685">Boolean</span></span>|<span data-ttu-id="1d23b-686">Указывает, следует ли запретить запрашивать пароли с близлежащих устройств (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-686">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="1d23b-687">Пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="1d23b-687">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="1d23b-688">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-688">Boolean</span></span>|<span data-ttu-id="1d23b-689">Указывает, следует ли заблокировать общий доступ к паролям с помощью AirDrop паролей iOS 12,0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="1d23b-689">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="1d23b-690">Датеандтимефорцесетаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="1d23b-690">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="1d23b-691">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-691">Boolean</span></span>|<span data-ttu-id="1d23b-692">Указывает, включена ли функция даты и времени "автоматически задано" и не может быть отключена пользователем (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-692">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="1d23b-693">Контактсалловманажедтаунманажедврите</span><span class="sxs-lookup"><span data-stu-id="1d23b-693">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="1d23b-694">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-694">Boolean</span></span>|<span data-ttu-id="1d23b-695">Указывает, могут ли управляемые приложения записывать контакты в неуправляемые учетные записи контактов (iOS 12,0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="1d23b-695">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="1d23b-696">Контактсалловунманажедтоманажедреад</span><span class="sxs-lookup"><span data-stu-id="1d23b-696">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="1d23b-697">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-697">Boolean</span></span>|<span data-ttu-id="1d23b-698">Указывает, могут ли неуправляемые приложения читать из управляемых учетных записей контактов (iOS 12,0 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="1d23b-698">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="1d23b-699">Целлуларблоккперсоналхотспотмодификатион</span><span class="sxs-lookup"><span data-stu-id="1d23b-699">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="1d23b-700">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-700">Boolean</span></span>|<span data-ttu-id="1d23b-701">Указывает, следует ли запретить пользователю изменять параметр личных гиперобъектов (iOS 12,2 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="1d23b-701">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="1d23b-702">Сиридисаблесерверлоггинг</span><span class="sxs-lookup"><span data-stu-id="1d23b-702">siriDisableServerLogging</span></span>|<span data-ttu-id="1d23b-703">Логический</span><span class="sxs-lookup"><span data-stu-id="1d23b-703">Boolean</span></span>|<span data-ttu-id="1d23b-704">Указывает, отключено ли ведение журнала Siri на стороне сервера (iOS 12,2 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="1d23b-704">Indicates whether or not server-side Siri logging is disabled (iOS 12.2 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="1d23b-705">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d23b-705">Response</span></span>
<span data-ttu-id="1d23b-706">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1d23b-706">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d23b-707">Пример</span><span class="sxs-lookup"><span data-stu-id="1d23b-707">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d23b-708">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d23b-708">Request</span></span>
<span data-ttu-id="1d23b-709">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d23b-709">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 9386

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="1d23b-710">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d23b-710">Response</span></span>
<span data-ttu-id="1d23b-p139">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1d23b-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9558

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




