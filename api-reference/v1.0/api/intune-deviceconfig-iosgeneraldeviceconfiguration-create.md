---
title: Create iosGeneralDeviceConfiguration
description: Создание объекта iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb12b8650123860ce2586f5027f44d4ccecdc797
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979135"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="54300-103">Create iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="54300-103">Create iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="54300-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54300-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54300-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54300-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54300-106">Создание объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54300-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54300-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="54300-107">Prerequisites</span></span>
<span data-ttu-id="54300-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54300-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54300-110">Permission type</span></span>|<span data-ttu-id="54300-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54300-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54300-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54300-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54300-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54300-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54300-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54300-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54300-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54300-115">Not supported.</span></span>|
|<span data-ttu-id="54300-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54300-116">Application</span></span>|<span data-ttu-id="54300-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54300-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54300-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54300-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="54300-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="54300-119">Request headers</span></span>
|<span data-ttu-id="54300-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54300-120">Header</span></span>|<span data-ttu-id="54300-121">Значение</span><span class="sxs-lookup"><span data-stu-id="54300-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54300-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54300-122">Authorization</span></span>|<span data-ttu-id="54300-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54300-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54300-124">Accept</span><span class="sxs-lookup"><span data-stu-id="54300-124">Accept</span></span>|<span data-ttu-id="54300-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54300-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54300-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="54300-126">Request body</span></span>
<span data-ttu-id="54300-127">В теле запроса добавьте представление объекта iosGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54300-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="54300-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="54300-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="54300-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="54300-129">Property</span></span>|<span data-ttu-id="54300-130">Тип</span><span class="sxs-lookup"><span data-stu-id="54300-130">Type</span></span>|<span data-ttu-id="54300-131">Описание</span><span class="sxs-lookup"><span data-stu-id="54300-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54300-132">id</span><span class="sxs-lookup"><span data-stu-id="54300-132">id</span></span>|<span data-ttu-id="54300-133">String</span><span class="sxs-lookup"><span data-stu-id="54300-133">String</span></span>|<span data-ttu-id="54300-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="54300-134">Key of the entity.</span></span> <span data-ttu-id="54300-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54300-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54300-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54300-136">lastModifiedDateTime</span></span>|<span data-ttu-id="54300-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54300-137">DateTimeOffset</span></span>|<span data-ttu-id="54300-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="54300-138">DateTime the object was last modified.</span></span> <span data-ttu-id="54300-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54300-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54300-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54300-140">createdDateTime</span></span>|<span data-ttu-id="54300-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54300-141">DateTimeOffset</span></span>|<span data-ttu-id="54300-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="54300-142">DateTime the object was created.</span></span> <span data-ttu-id="54300-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54300-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54300-144">description</span><span class="sxs-lookup"><span data-stu-id="54300-144">description</span></span>|<span data-ttu-id="54300-145">String</span><span class="sxs-lookup"><span data-stu-id="54300-145">String</span></span>|<span data-ttu-id="54300-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54300-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54300-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54300-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54300-148">displayName</span><span class="sxs-lookup"><span data-stu-id="54300-148">displayName</span></span>|<span data-ttu-id="54300-149">String</span><span class="sxs-lookup"><span data-stu-id="54300-149">String</span></span>|<span data-ttu-id="54300-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54300-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54300-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54300-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54300-152">version</span><span class="sxs-lookup"><span data-stu-id="54300-152">version</span></span>|<span data-ttu-id="54300-153">Int32</span><span class="sxs-lookup"><span data-stu-id="54300-153">Int32</span></span>|<span data-ttu-id="54300-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54300-154">Version of the device configuration.</span></span> <span data-ttu-id="54300-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54300-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54300-156">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="54300-156">accountBlockModification</span></span>|<span data-ttu-id="54300-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-157">Boolean</span></span>|<span data-ttu-id="54300-158">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-158">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="54300-159">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="54300-159">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="54300-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-160">Boolean</span></span>|<span data-ttu-id="54300-161">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-161">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="54300-162">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-162">airDropBlocked</span></span>|<span data-ttu-id="54300-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-163">Boolean</span></span>|<span data-ttu-id="54300-164">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-164">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="54300-165">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="54300-165">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="54300-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-166">Boolean</span></span>|<span data-ttu-id="54300-167">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-167">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="54300-168">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="54300-168">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="54300-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-169">Boolean</span></span>|<span data-ttu-id="54300-170">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="54300-170">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="54300-171">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="54300-171">appleWatchBlockPairing</span></span>|<span data-ttu-id="54300-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-172">Boolean</span></span>|<span data-ttu-id="54300-173">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-173">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="54300-174">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="54300-174">appleWatchForceWristDetection</span></span>|<span data-ttu-id="54300-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-175">Boolean</span></span>|<span data-ttu-id="54300-176">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-176">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="54300-177">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-177">appleNewsBlocked</span></span>|<span data-ttu-id="54300-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-178">Boolean</span></span>|<span data-ttu-id="54300-179">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-179">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="54300-180">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="54300-180">appsSingleAppModeList</span></span>|<span data-ttu-id="54300-181">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="54300-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="54300-182">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="54300-182">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="54300-183">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-183">Supervised only.</span></span> <span data-ttu-id="54300-184">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="54300-184">iOS 7.0 and later.</span></span> <span data-ttu-id="54300-185">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="54300-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="54300-186">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="54300-186">appsVisibilityList</span></span>|<span data-ttu-id="54300-187">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="54300-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="54300-188">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-188">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="54300-189">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="54300-189">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="54300-190">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="54300-190">appsVisibilityListType</span></span>|[<span data-ttu-id="54300-191">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="54300-191">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="54300-192">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="54300-192">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="54300-193">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="54300-193">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="54300-194">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="54300-194">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="54300-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-195">Boolean</span></span>|<span data-ttu-id="54300-196">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-196">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="54300-197">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-197">appStoreBlocked</span></span>|<span data-ttu-id="54300-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-198">Boolean</span></span>|<span data-ttu-id="54300-199">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="54300-199">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="54300-200">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="54300-200">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="54300-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-201">Boolean</span></span>|<span data-ttu-id="54300-202">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="54300-202">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="54300-203">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="54300-203">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="54300-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-204">Boolean</span></span>|<span data-ttu-id="54300-205">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="54300-205">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="54300-206">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-206">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="54300-207">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="54300-207">appStoreRequirePassword</span></span>|<span data-ttu-id="54300-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-208">Boolean</span></span>|<span data-ttu-id="54300-209">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="54300-209">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="54300-210">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="54300-210">bluetoothBlockModification</span></span>|<span data-ttu-id="54300-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-211">Boolean</span></span>|<span data-ttu-id="54300-212">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-212">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="54300-213">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-213">cameraBlocked</span></span>|<span data-ttu-id="54300-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-214">Boolean</span></span>|<span data-ttu-id="54300-215">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="54300-215">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="54300-216">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="54300-216">cellularBlockDataRoaming</span></span>|<span data-ttu-id="54300-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-217">Boolean</span></span>|<span data-ttu-id="54300-218">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="54300-218">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="54300-219">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="54300-219">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="54300-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-220">Boolean</span></span>|<span data-ttu-id="54300-221">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="54300-221">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="54300-222">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="54300-222">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="54300-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-223">Boolean</span></span>|<span data-ttu-id="54300-224">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-224">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="54300-225">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="54300-225">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="54300-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-226">Boolean</span></span>|<span data-ttu-id="54300-227">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="54300-227">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="54300-228">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="54300-228">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="54300-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-229">Boolean</span></span>|<span data-ttu-id="54300-230">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="54300-230">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="54300-231">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="54300-231">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="54300-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-232">Boolean</span></span>|<span data-ttu-id="54300-233">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="54300-233">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="54300-234">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="54300-234">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="54300-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-235">Boolean</span></span>|<span data-ttu-id="54300-236">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-236">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="54300-237">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="54300-237">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="54300-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-238">Boolean</span></span>|<span data-ttu-id="54300-239">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-239">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="54300-240">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="54300-240">compliantAppsList</span></span>|<span data-ttu-id="54300-241">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="54300-241">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="54300-242">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="54300-242">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="54300-243">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="54300-243">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="54300-244">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="54300-244">compliantAppListType</span></span>|[<span data-ttu-id="54300-245">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="54300-245">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="54300-246">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="54300-246">List that is in the AppComplianceList.</span></span> <span data-ttu-id="54300-247">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="54300-247">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="54300-248">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="54300-248">configurationProfileBlockChanges</span></span>|<span data-ttu-id="54300-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-249">Boolean</span></span>|<span data-ttu-id="54300-250">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-250">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="54300-251">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-251">definitionLookupBlocked</span></span>|<span data-ttu-id="54300-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-252">Boolean</span></span>|<span data-ttu-id="54300-253">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-253">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="54300-254">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="54300-254">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="54300-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-255">Boolean</span></span>|<span data-ttu-id="54300-256">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-256">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="54300-257">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="54300-257">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="54300-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-258">Boolean</span></span>|<span data-ttu-id="54300-259">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-259">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="54300-260">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="54300-260">deviceBlockNameModification</span></span>|<span data-ttu-id="54300-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-261">Boolean</span></span>|<span data-ttu-id="54300-262">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-262">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="54300-263">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="54300-263">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="54300-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-264">Boolean</span></span>|<span data-ttu-id="54300-265">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="54300-265">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="54300-266">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="54300-266">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="54300-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-267">Boolean</span></span>|<span data-ttu-id="54300-268">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-268">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="54300-269">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="54300-269">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="54300-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-270">Boolean</span></span>|<span data-ttu-id="54300-271">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="54300-271">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="54300-272">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="54300-272">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="54300-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-273">Boolean</span></span>|<span data-ttu-id="54300-274">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="54300-274">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="54300-275">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="54300-275">emailInDomainSuffixes</span></span>|<span data-ttu-id="54300-276">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="54300-276">String collection</span></span>|<span data-ttu-id="54300-277">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="54300-277">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="54300-278">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="54300-278">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="54300-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-279">Boolean</span></span>|<span data-ttu-id="54300-280">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="54300-280">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="54300-281">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="54300-281">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="54300-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-282">Boolean</span></span>|<span data-ttu-id="54300-283">Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="54300-283">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="54300-284">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-284">faceTimeBlocked</span></span>|<span data-ttu-id="54300-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-285">Boolean</span></span>|<span data-ttu-id="54300-286">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="54300-286">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="54300-287">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-287">findMyFriendsBlocked</span></span>|<span data-ttu-id="54300-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-288">Boolean</span></span>|<span data-ttu-id="54300-289">Указывает, следует ли заблокировать функцию "Найти друзей", когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-289">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="54300-290">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="54300-290">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="54300-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-291">Boolean</span></span>|<span data-ttu-id="54300-292">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="54300-292">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="54300-293">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="54300-293">gamingBlockMultiplayer</span></span>|<span data-ttu-id="54300-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-294">Boolean</span></span>|<span data-ttu-id="54300-295">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="54300-295">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="54300-296">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-296">gameCenterBlocked</span></span>|<span data-ttu-id="54300-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-297">Boolean</span></span>|<span data-ttu-id="54300-298">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-298">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="54300-299">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-299">hostPairingBlocked</span></span>|<span data-ttu-id="54300-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-300">Boolean</span></span>|<span data-ttu-id="54300-301">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-301">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="54300-302">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-302">iBooksStoreBlocked</span></span>|<span data-ttu-id="54300-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-303">Boolean</span></span>|<span data-ttu-id="54300-304">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-304">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="54300-305">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="54300-305">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="54300-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-306">Boolean</span></span>|<span data-ttu-id="54300-307">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="54300-307">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="54300-308">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="54300-308">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="54300-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-309">Boolean</span></span>|<span data-ttu-id="54300-310">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="54300-310">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="54300-311">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="54300-311">iCloudBlockBackup</span></span>|<span data-ttu-id="54300-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-312">Boolean</span></span>|<span data-ttu-id="54300-313">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="54300-313">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="54300-314">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="54300-314">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="54300-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-315">Boolean</span></span>|<span data-ttu-id="54300-316">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="54300-316">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="54300-317">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="54300-317">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="54300-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-318">Boolean</span></span>|<span data-ttu-id="54300-319">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="54300-319">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="54300-320">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="54300-320">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="54300-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-321">Boolean</span></span>|<span data-ttu-id="54300-322">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="54300-322">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="54300-323">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="54300-323">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="54300-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-324">Boolean</span></span>|<span data-ttu-id="54300-325">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="54300-325">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="54300-326">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="54300-326">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="54300-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-327">Boolean</span></span>|<span data-ttu-id="54300-328">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="54300-328">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="54300-329">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="54300-329">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="54300-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-330">Boolean</span></span>|<span data-ttu-id="54300-331">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="54300-331">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="54300-332">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="54300-332">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="54300-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-333">Boolean</span></span>|<span data-ttu-id="54300-334">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="54300-334">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="54300-335">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="54300-335">iTunesBlockMusicService</span></span>|<span data-ttu-id="54300-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-336">Boolean</span></span>|<span data-ttu-id="54300-337">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-337">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="54300-338">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="54300-338">iTunesBlockRadio</span></span>|<span data-ttu-id="54300-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-339">Boolean</span></span>|<span data-ttu-id="54300-340">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-340">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="54300-341">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="54300-341">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="54300-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-342">Boolean</span></span>|<span data-ttu-id="54300-343">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-343">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="54300-344">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="54300-344">keyboardBlockDictation</span></span>|<span data-ttu-id="54300-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-345">Boolean</span></span>|<span data-ttu-id="54300-346">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-346">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="54300-347">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="54300-347">keyboardBlockPredictive</span></span>|<span data-ttu-id="54300-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-348">Boolean</span></span>|<span data-ttu-id="54300-349">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-349">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="54300-350">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="54300-350">keyboardBlockShortcuts</span></span>|<span data-ttu-id="54300-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-351">Boolean</span></span>|<span data-ttu-id="54300-352">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-352">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="54300-353">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="54300-353">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="54300-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-354">Boolean</span></span>|<span data-ttu-id="54300-355">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-355">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="54300-356">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="54300-356">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="54300-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-357">Boolean</span></span>|<span data-ttu-id="54300-358">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-358">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-359">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="54300-359">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="54300-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-360">Boolean</span></span>|<span data-ttu-id="54300-361">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-361">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-362">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="54300-362">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="54300-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-363">Boolean</span></span>|<span data-ttu-id="54300-364">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-364">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-365">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="54300-365">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="54300-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-366">Boolean</span></span>|<span data-ttu-id="54300-367">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-367">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-368">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="54300-368">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="54300-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-369">Boolean</span></span>|<span data-ttu-id="54300-370">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-370">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-371">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="54300-371">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="54300-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-372">Boolean</span></span>|<span data-ttu-id="54300-373">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-373">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-374">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="54300-374">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="54300-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-375">Boolean</span></span>|<span data-ttu-id="54300-376">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-376">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-377">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="54300-377">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="54300-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-378">Boolean</span></span>|<span data-ttu-id="54300-379">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-379">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-380">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="54300-380">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="54300-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-381">Boolean</span></span>|<span data-ttu-id="54300-382">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-382">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-383">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="54300-383">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="54300-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-384">Boolean</span></span>|<span data-ttu-id="54300-385">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-385">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-386">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="54300-386">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="54300-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-387">Boolean</span></span>|<span data-ttu-id="54300-388">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-388">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-389">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="54300-389">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="54300-390">String</span><span class="sxs-lookup"><span data-stu-id="54300-390">String</span></span>|<span data-ttu-id="54300-391">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-391">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="54300-392">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="54300-392">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="54300-393">киоскмодебуилтинаппид</span><span class="sxs-lookup"><span data-stu-id="54300-393">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="54300-394">String</span><span class="sxs-lookup"><span data-stu-id="54300-394">String</span></span>|<span data-ttu-id="54300-395">Идентификатор встроенных приложений для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-395">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="54300-396">Используется, когда KioskModeManagedAppId и KioskModeAppStoreUrl не заданы.</span><span class="sxs-lookup"><span data-stu-id="54300-396">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="54300-397">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="54300-397">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="54300-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-398">Boolean</span></span>|<span data-ttu-id="54300-399">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-399">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-400">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="54300-400">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="54300-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-401">Boolean</span></span>|<span data-ttu-id="54300-402">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-402">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-403">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="54300-403">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="54300-404">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-404">Boolean</span></span>|<span data-ttu-id="54300-405">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-405">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-406">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="54300-406">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="54300-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-407">Boolean</span></span>|<span data-ttu-id="54300-408">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-408">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-409">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="54300-409">kioskModeRequireZoom</span></span>|<span data-ttu-id="54300-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-410">Boolean</span></span>|<span data-ttu-id="54300-411">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-411">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="54300-412">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="54300-412">kioskModeManagedAppId</span></span>|<span data-ttu-id="54300-413">String</span><span class="sxs-lookup"><span data-stu-id="54300-413">String</span></span>|<span data-ttu-id="54300-414">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="54300-414">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="54300-415">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="54300-415">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="54300-416">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="54300-416">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="54300-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-417">Boolean</span></span>|<span data-ttu-id="54300-418">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="54300-418">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="54300-419">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="54300-419">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="54300-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-420">Boolean</span></span>|<span data-ttu-id="54300-421">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="54300-421">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="54300-422">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="54300-422">lockScreenBlockPassbook</span></span>|<span data-ttu-id="54300-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-423">Boolean</span></span>|<span data-ttu-id="54300-424">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="54300-424">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="54300-425">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="54300-425">lockScreenBlockTodayView</span></span>|<span data-ttu-id="54300-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-426">Boolean</span></span>|<span data-ttu-id="54300-427">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="54300-427">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="54300-428">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="54300-428">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="54300-429">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="54300-429">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="54300-430">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="54300-430">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="54300-431">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="54300-431">mediaContentRatingCanada</span></span>|[<span data-ttu-id="54300-432">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="54300-432">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="54300-433">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="54300-433">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="54300-434">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="54300-434">mediaContentRatingFrance</span></span>|[<span data-ttu-id="54300-435">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="54300-435">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="54300-436">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="54300-436">Media content rating settings for France</span></span>|
|<span data-ttu-id="54300-437">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="54300-437">mediaContentRatingGermany</span></span>|[<span data-ttu-id="54300-438">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="54300-438">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="54300-439">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="54300-439">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="54300-440">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="54300-440">mediaContentRatingIreland</span></span>|[<span data-ttu-id="54300-441">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="54300-441">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="54300-442">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="54300-442">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="54300-443">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="54300-443">mediaContentRatingJapan</span></span>|[<span data-ttu-id="54300-444">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="54300-444">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="54300-445">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="54300-445">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="54300-446">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="54300-446">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="54300-447">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="54300-447">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="54300-448">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="54300-448">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="54300-449">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="54300-449">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="54300-450">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="54300-450">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="54300-451">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="54300-451">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="54300-452">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="54300-452">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="54300-453">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="54300-453">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="54300-454">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="54300-454">Media content rating settings for United States</span></span>|
|<span data-ttu-id="54300-455">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="54300-455">networkUsageRules</span></span>|<span data-ttu-id="54300-456">Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="54300-456">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="54300-457">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="54300-457">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="54300-458">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="54300-458">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="54300-459">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="54300-459">mediaContentRatingApps</span></span>|[<span data-ttu-id="54300-460">ратингаппстипе</span><span class="sxs-lookup"><span data-stu-id="54300-460">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="54300-461">Параметры оценки контента мультимедиа для приложений.</span><span class="sxs-lookup"><span data-stu-id="54300-461">Media content rating settings for Apps.</span></span> <span data-ttu-id="54300-462">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="54300-462">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="54300-463">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-463">messagesBlocked</span></span>|<span data-ttu-id="54300-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-464">Boolean</span></span>|<span data-ttu-id="54300-465">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="54300-465">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="54300-466">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="54300-466">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="54300-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-467">Boolean</span></span>|<span data-ttu-id="54300-468">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-468">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="54300-469">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="54300-469">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="54300-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-470">Boolean</span></span>|<span data-ttu-id="54300-471">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="54300-471">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="54300-472">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="54300-472">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="54300-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-473">Boolean</span></span>|<span data-ttu-id="54300-474">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-474">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="54300-475">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="54300-475">passcodeBlockModification</span></span>|<span data-ttu-id="54300-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-476">Boolean</span></span>|<span data-ttu-id="54300-477">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-477">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="54300-478">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="54300-478">passcodeBlockSimple</span></span>|<span data-ttu-id="54300-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-479">Boolean</span></span>|<span data-ttu-id="54300-480">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="54300-480">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="54300-481">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="54300-481">passcodeExpirationDays</span></span>|<span data-ttu-id="54300-482">Int32</span><span class="sxs-lookup"><span data-stu-id="54300-482">Int32</span></span>|<span data-ttu-id="54300-483">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="54300-483">Number of days before the passcode expires.</span></span> <span data-ttu-id="54300-484">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="54300-484">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="54300-485">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="54300-485">passcodeMinimumLength</span></span>|<span data-ttu-id="54300-486">Int32</span><span class="sxs-lookup"><span data-stu-id="54300-486">Int32</span></span>|<span data-ttu-id="54300-487">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="54300-487">Minimum length of passcode.</span></span> <span data-ttu-id="54300-488">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="54300-488">Valid values 4 to 14</span></span>|
|<span data-ttu-id="54300-489">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="54300-489">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="54300-490">Int32</span><span class="sxs-lookup"><span data-stu-id="54300-490">Int32</span></span>|<span data-ttu-id="54300-491">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="54300-491">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="54300-492">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="54300-492">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="54300-493">Int32</span><span class="sxs-lookup"><span data-stu-id="54300-493">Int32</span></span>|<span data-ttu-id="54300-494">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="54300-494">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="54300-495">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="54300-495">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="54300-496">Int32</span><span class="sxs-lookup"><span data-stu-id="54300-496">Int32</span></span>|<span data-ttu-id="54300-497">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="54300-497">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="54300-498">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="54300-498">Valid values 0 to 4</span></span>|
|<span data-ttu-id="54300-499">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="54300-499">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="54300-500">Int32</span><span class="sxs-lookup"><span data-stu-id="54300-500">Int32</span></span>|<span data-ttu-id="54300-501">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="54300-501">Number of previous passcodes to block.</span></span> <span data-ttu-id="54300-502">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="54300-502">Valid values 1 to 24</span></span>|
|<span data-ttu-id="54300-503">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="54300-503">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="54300-504">Int32</span><span class="sxs-lookup"><span data-stu-id="54300-504">Int32</span></span>|<span data-ttu-id="54300-505">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="54300-505">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="54300-506">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="54300-506">Valid values 4 to 11</span></span>|
|<span data-ttu-id="54300-507">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="54300-507">passcodeRequiredType</span></span>|[<span data-ttu-id="54300-508">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="54300-508">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="54300-509">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="54300-509">Type of passcode that is required.</span></span> <span data-ttu-id="54300-510">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="54300-510">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="54300-511">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="54300-511">passcodeRequired</span></span>|<span data-ttu-id="54300-512">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-512">Boolean</span></span>|<span data-ttu-id="54300-513">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="54300-513">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="54300-514">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-514">podcastsBlocked</span></span>|<span data-ttu-id="54300-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-515">Boolean</span></span>|<span data-ttu-id="54300-516">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-516">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="54300-517">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="54300-517">safariBlockAutofill</span></span>|<span data-ttu-id="54300-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-518">Boolean</span></span>|<span data-ttu-id="54300-519">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="54300-519">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="54300-520">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="54300-520">safariBlockJavaScript</span></span>|<span data-ttu-id="54300-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-521">Boolean</span></span>|<span data-ttu-id="54300-522">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="54300-522">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="54300-523">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="54300-523">safariBlockPopups</span></span>|<span data-ttu-id="54300-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-524">Boolean</span></span>|<span data-ttu-id="54300-525">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="54300-525">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="54300-526">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-526">safariBlocked</span></span>|<span data-ttu-id="54300-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-527">Boolean</span></span>|<span data-ttu-id="54300-528">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="54300-528">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="54300-529">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="54300-529">safariCookieSettings</span></span>|[<span data-ttu-id="54300-530">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="54300-530">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="54300-531">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="54300-531">Cookie settings for Safari.</span></span> <span data-ttu-id="54300-532">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="54300-532">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="54300-533">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="54300-533">safariManagedDomains</span></span>|<span data-ttu-id="54300-534">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="54300-534">String collection</span></span>|<span data-ttu-id="54300-535">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="54300-535">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="54300-536">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="54300-536">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="54300-537">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="54300-537">String collection</span></span>|<span data-ttu-id="54300-538">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="54300-538">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="54300-539">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-539">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="54300-540">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="54300-540">safariRequireFraudWarning</span></span>|<span data-ttu-id="54300-541">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-541">Boolean</span></span>|<span data-ttu-id="54300-542">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="54300-542">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="54300-543">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-543">screenCaptureBlocked</span></span>|<span data-ttu-id="54300-544">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-544">Boolean</span></span>|<span data-ttu-id="54300-545">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="54300-545">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="54300-546">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-546">siriBlocked</span></span>|<span data-ttu-id="54300-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-547">Boolean</span></span>|<span data-ttu-id="54300-548">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="54300-548">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="54300-549">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="54300-549">siriBlockedWhenLocked</span></span>|<span data-ttu-id="54300-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-550">Boolean</span></span>|<span data-ttu-id="54300-551">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="54300-551">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="54300-552">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="54300-552">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="54300-553">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-553">Boolean</span></span>|<span data-ttu-id="54300-554">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="54300-554">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="54300-555">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="54300-555">siriRequireProfanityFilter</span></span>|<span data-ttu-id="54300-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-556">Boolean</span></span>|<span data-ttu-id="54300-557">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="54300-557">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="54300-558">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="54300-558">spotlightBlockInternetResults</span></span>|<span data-ttu-id="54300-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-559">Boolean</span></span>|<span data-ttu-id="54300-560">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="54300-560">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="54300-561">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="54300-561">voiceDialingBlocked</span></span>|<span data-ttu-id="54300-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-562">Boolean</span></span>|<span data-ttu-id="54300-563">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="54300-563">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="54300-564">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="54300-564">wallpaperBlockModification</span></span>|<span data-ttu-id="54300-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-565">Boolean</span></span>|<span data-ttu-id="54300-566">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="54300-566">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="54300-567">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="54300-567">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="54300-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="54300-568">Boolean</span></span>|<span data-ttu-id="54300-569">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="54300-569">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="54300-570">Ответ</span><span class="sxs-lookup"><span data-stu-id="54300-570">Response</span></span>
<span data-ttu-id="54300-571">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="54300-571">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54300-572">Пример</span><span class="sxs-lookup"><span data-stu-id="54300-572">Example</span></span>

### <a name="request"></a><span data-ttu-id="54300-573">Запрос</span><span class="sxs-lookup"><span data-stu-id="54300-573">Request</span></span>
<span data-ttu-id="54300-574">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54300-574">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 7841

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
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
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```

### <a name="response"></a><span data-ttu-id="54300-575">Отклик</span><span class="sxs-lookup"><span data-stu-id="54300-575">Response</span></span>
<span data-ttu-id="54300-p127">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54300-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 8013

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
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
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```









