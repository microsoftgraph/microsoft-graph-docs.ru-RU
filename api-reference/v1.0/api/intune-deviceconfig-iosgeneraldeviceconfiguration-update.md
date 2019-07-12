---
title: Обновление объекта iosGeneralDeviceConfiguration
description: Обновление свойств объекта iosGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6cd64af8e66e8e1059f975bf0d8e6f9347fab746
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620873"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="6d185-103">Обновление объекта iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6d185-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="6d185-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d185-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d185-105">Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d185-105">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d185-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6d185-106">Prerequisites</span></span>
<span data-ttu-id="6d185-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d185-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d185-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d185-109">Permission type</span></span>|<span data-ttu-id="6d185-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d185-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d185-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d185-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d185-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d185-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6d185-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d185-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d185-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d185-114">Not supported.</span></span>|
|<span data-ttu-id="6d185-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d185-115">Application</span></span>|<span data-ttu-id="6d185-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d185-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d185-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d185-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6d185-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d185-118">Request headers</span></span>
|<span data-ttu-id="6d185-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6d185-119">Header</span></span>|<span data-ttu-id="6d185-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6d185-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d185-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d185-121">Authorization</span></span>|<span data-ttu-id="6d185-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6d185-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d185-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6d185-123">Accept</span></span>|<span data-ttu-id="6d185-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6d185-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d185-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d185-125">Request body</span></span>
<span data-ttu-id="6d185-126">В тексте запроса добавьте представление объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d185-126">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="6d185-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d185-127">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="6d185-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d185-128">Property</span></span>|<span data-ttu-id="6d185-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6d185-129">Type</span></span>|<span data-ttu-id="6d185-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6d185-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d185-131">id</span><span class="sxs-lookup"><span data-stu-id="6d185-131">id</span></span>|<span data-ttu-id="6d185-132">String</span><span class="sxs-lookup"><span data-stu-id="6d185-132">String</span></span>|<span data-ttu-id="6d185-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6d185-133">Key of the entity.</span></span> <span data-ttu-id="6d185-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d185-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d185-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d185-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6d185-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d185-136">DateTimeOffset</span></span>|<span data-ttu-id="6d185-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6d185-137">DateTime the object was last modified.</span></span> <span data-ttu-id="6d185-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d185-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d185-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d185-139">createdDateTime</span></span>|<span data-ttu-id="6d185-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d185-140">DateTimeOffset</span></span>|<span data-ttu-id="6d185-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6d185-141">DateTime the object was created.</span></span> <span data-ttu-id="6d185-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d185-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d185-143">description</span><span class="sxs-lookup"><span data-stu-id="6d185-143">description</span></span>|<span data-ttu-id="6d185-144">String</span><span class="sxs-lookup"><span data-stu-id="6d185-144">String</span></span>|<span data-ttu-id="6d185-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6d185-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6d185-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d185-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d185-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6d185-147">displayName</span></span>|<span data-ttu-id="6d185-148">Строка</span><span class="sxs-lookup"><span data-stu-id="6d185-148">String</span></span>|<span data-ttu-id="6d185-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6d185-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6d185-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6d185-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d185-151">version</span><span class="sxs-lookup"><span data-stu-id="6d185-151">version</span></span>|<span data-ttu-id="6d185-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6d185-152">Int32</span></span>|<span data-ttu-id="6d185-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6d185-153">Version of the device configuration.</span></span> <span data-ttu-id="6d185-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6d185-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6d185-155">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="6d185-155">accountBlockModification</span></span>|<span data-ttu-id="6d185-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-156">Boolean</span></span>|<span data-ttu-id="6d185-157">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-157">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6d185-158">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="6d185-158">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="6d185-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-159">Boolean</span></span>|<span data-ttu-id="6d185-160">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-160">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="6d185-161">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-161">airDropBlocked</span></span>|<span data-ttu-id="6d185-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-162">Boolean</span></span>|<span data-ttu-id="6d185-163">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-163">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6d185-164">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="6d185-164">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="6d185-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-165">Boolean</span></span>|<span data-ttu-id="6d185-166">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-166">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6d185-167">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="6d185-167">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="6d185-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-168">Boolean</span></span>|<span data-ttu-id="6d185-169">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="6d185-169">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="6d185-170">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="6d185-170">appleWatchBlockPairing</span></span>|<span data-ttu-id="6d185-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-171">Boolean</span></span>|<span data-ttu-id="6d185-172">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-172">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6d185-173">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="6d185-173">appleWatchForceWristDetection</span></span>|<span data-ttu-id="6d185-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-174">Boolean</span></span>|<span data-ttu-id="6d185-175">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-175">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="6d185-176">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-176">appleNewsBlocked</span></span>|<span data-ttu-id="6d185-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-177">Boolean</span></span>|<span data-ttu-id="6d185-178">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-178">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6d185-179">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="6d185-179">appsSingleAppModeList</span></span>|<span data-ttu-id="6d185-180">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6d185-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6d185-181">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="6d185-181">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="6d185-182">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-182">Supervised only.</span></span> <span data-ttu-id="6d185-183">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="6d185-183">iOS 7.0 and later.</span></span> <span data-ttu-id="6d185-184">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6d185-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6d185-185">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="6d185-185">appsVisibilityList</span></span>|<span data-ttu-id="6d185-186">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6d185-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6d185-187">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-187">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="6d185-188">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="6d185-188">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6d185-189">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="6d185-189">appsVisibilityListType</span></span>|[<span data-ttu-id="6d185-190">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="6d185-190">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="6d185-191">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="6d185-191">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="6d185-192">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="6d185-192">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="6d185-193">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="6d185-193">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="6d185-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-194">Boolean</span></span>|<span data-ttu-id="6d185-195">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-195">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6d185-196">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-196">appStoreBlocked</span></span>|<span data-ttu-id="6d185-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-197">Boolean</span></span>|<span data-ttu-id="6d185-198">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="6d185-198">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="6d185-199">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="6d185-199">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="6d185-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-200">Boolean</span></span>|<span data-ttu-id="6d185-201">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="6d185-201">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="6d185-202">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="6d185-202">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="6d185-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-203">Boolean</span></span>|<span data-ttu-id="6d185-204">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="6d185-204">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="6d185-205">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-205">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6d185-206">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="6d185-206">appStoreRequirePassword</span></span>|<span data-ttu-id="6d185-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-207">Boolean</span></span>|<span data-ttu-id="6d185-208">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="6d185-208">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="6d185-209">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="6d185-209">bluetoothBlockModification</span></span>|<span data-ttu-id="6d185-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-210">Boolean</span></span>|<span data-ttu-id="6d185-211">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-211">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="6d185-212">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-212">cameraBlocked</span></span>|<span data-ttu-id="6d185-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-213">Boolean</span></span>|<span data-ttu-id="6d185-214">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="6d185-214">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="6d185-215">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="6d185-215">cellularBlockDataRoaming</span></span>|<span data-ttu-id="6d185-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-216">Boolean</span></span>|<span data-ttu-id="6d185-217">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="6d185-217">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="6d185-218">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="6d185-218">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="6d185-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-219">Boolean</span></span>|<span data-ttu-id="6d185-220">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="6d185-220">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="6d185-221">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="6d185-221">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="6d185-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-222">Boolean</span></span>|<span data-ttu-id="6d185-223">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-223">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6d185-224">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="6d185-224">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="6d185-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-225">Boolean</span></span>|<span data-ttu-id="6d185-226">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="6d185-226">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="6d185-227">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="6d185-227">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="6d185-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-228">Boolean</span></span>|<span data-ttu-id="6d185-229">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="6d185-229">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="6d185-230">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="6d185-230">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="6d185-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-231">Boolean</span></span>|<span data-ttu-id="6d185-232">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="6d185-232">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="6d185-233">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="6d185-233">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="6d185-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-234">Boolean</span></span>|<span data-ttu-id="6d185-235">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-235">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6d185-236">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="6d185-236">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="6d185-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-237">Boolean</span></span>|<span data-ttu-id="6d185-238">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-238">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6d185-239">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="6d185-239">compliantAppsList</span></span>|<span data-ttu-id="6d185-240">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="6d185-240">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6d185-241">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="6d185-241">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="6d185-242">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="6d185-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6d185-243">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="6d185-243">compliantAppListType</span></span>|[<span data-ttu-id="6d185-244">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="6d185-244">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="6d185-245">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="6d185-245">List that is in the AppComplianceList.</span></span> <span data-ttu-id="6d185-246">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="6d185-246">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="6d185-247">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="6d185-247">configurationProfileBlockChanges</span></span>|<span data-ttu-id="6d185-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-248">Boolean</span></span>|<span data-ttu-id="6d185-249">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-249">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6d185-250">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-250">definitionLookupBlocked</span></span>|<span data-ttu-id="6d185-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-251">Boolean</span></span>|<span data-ttu-id="6d185-252">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-252">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="6d185-253">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="6d185-253">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="6d185-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-254">Boolean</span></span>|<span data-ttu-id="6d185-255">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-255">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6d185-256">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="6d185-256">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="6d185-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-257">Boolean</span></span>|<span data-ttu-id="6d185-258">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-258">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6d185-259">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="6d185-259">deviceBlockNameModification</span></span>|<span data-ttu-id="6d185-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-260">Boolean</span></span>|<span data-ttu-id="6d185-261">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-261">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6d185-262">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="6d185-262">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="6d185-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-263">Boolean</span></span>|<span data-ttu-id="6d185-264">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="6d185-264">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="6d185-265">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="6d185-265">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="6d185-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-266">Boolean</span></span>|<span data-ttu-id="6d185-267">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-267">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="6d185-268">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="6d185-268">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="6d185-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-269">Boolean</span></span>|<span data-ttu-id="6d185-270">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="6d185-270">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="6d185-271">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="6d185-271">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="6d185-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-272">Boolean</span></span>|<span data-ttu-id="6d185-273">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="6d185-273">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="6d185-274">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="6d185-274">emailInDomainSuffixes</span></span>|<span data-ttu-id="6d185-275">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6d185-275">String collection</span></span>|<span data-ttu-id="6d185-276">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="6d185-276">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="6d185-277">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="6d185-277">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="6d185-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-278">Boolean</span></span>|<span data-ttu-id="6d185-279">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="6d185-279">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="6d185-280">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="6d185-280">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="6d185-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-281">Boolean</span></span>|<span data-ttu-id="6d185-282">Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="6d185-282">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="6d185-283">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-283">faceTimeBlocked</span></span>|<span data-ttu-id="6d185-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-284">Boolean</span></span>|<span data-ttu-id="6d185-285">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="6d185-285">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="6d185-286">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-286">findMyFriendsBlocked</span></span>|<span data-ttu-id="6d185-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-287">Boolean</span></span>|<span data-ttu-id="6d185-288">Указывает, следует ли заблокировать функцию "Найти друзей", когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-288">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6d185-289">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="6d185-289">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="6d185-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-290">Boolean</span></span>|<span data-ttu-id="6d185-291">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="6d185-291">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="6d185-292">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="6d185-292">gamingBlockMultiplayer</span></span>|<span data-ttu-id="6d185-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-293">Boolean</span></span>|<span data-ttu-id="6d185-294">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="6d185-294">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="6d185-295">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-295">gameCenterBlocked</span></span>|<span data-ttu-id="6d185-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-296">Boolean</span></span>|<span data-ttu-id="6d185-297">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-297">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6d185-298">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-298">hostPairingBlocked</span></span>|<span data-ttu-id="6d185-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-299">Boolean</span></span>|<span data-ttu-id="6d185-300">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-300">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="6d185-301">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-301">iBooksStoreBlocked</span></span>|<span data-ttu-id="6d185-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-302">Boolean</span></span>|<span data-ttu-id="6d185-303">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-303">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6d185-304">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="6d185-304">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="6d185-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-305">Boolean</span></span>|<span data-ttu-id="6d185-306">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="6d185-306">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="6d185-307">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="6d185-307">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="6d185-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-308">Boolean</span></span>|<span data-ttu-id="6d185-309">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="6d185-309">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="6d185-310">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="6d185-310">iCloudBlockBackup</span></span>|<span data-ttu-id="6d185-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-311">Boolean</span></span>|<span data-ttu-id="6d185-312">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="6d185-312">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="6d185-313">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="6d185-313">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="6d185-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-314">Boolean</span></span>|<span data-ttu-id="6d185-315">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="6d185-315">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="6d185-316">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="6d185-316">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="6d185-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-317">Boolean</span></span>|<span data-ttu-id="6d185-318">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="6d185-318">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="6d185-319">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="6d185-319">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="6d185-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-320">Boolean</span></span>|<span data-ttu-id="6d185-321">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="6d185-321">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="6d185-322">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="6d185-322">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="6d185-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-323">Boolean</span></span>|<span data-ttu-id="6d185-324">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="6d185-324">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="6d185-325">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="6d185-325">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="6d185-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-326">Boolean</span></span>|<span data-ttu-id="6d185-327">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="6d185-327">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="6d185-328">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="6d185-328">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="6d185-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-329">Boolean</span></span>|<span data-ttu-id="6d185-330">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="6d185-330">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="6d185-331">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="6d185-331">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="6d185-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-332">Boolean</span></span>|<span data-ttu-id="6d185-333">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="6d185-333">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="6d185-334">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="6d185-334">iTunesBlockMusicService</span></span>|<span data-ttu-id="6d185-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-335">Boolean</span></span>|<span data-ttu-id="6d185-336">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-336">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="6d185-337">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="6d185-337">iTunesBlockRadio</span></span>|<span data-ttu-id="6d185-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-338">Boolean</span></span>|<span data-ttu-id="6d185-339">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-339">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6d185-340">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="6d185-340">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="6d185-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-341">Boolean</span></span>|<span data-ttu-id="6d185-342">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-342">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="6d185-343">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="6d185-343">keyboardBlockDictation</span></span>|<span data-ttu-id="6d185-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-344">Boolean</span></span>|<span data-ttu-id="6d185-345">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-345">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6d185-346">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="6d185-346">keyboardBlockPredictive</span></span>|<span data-ttu-id="6d185-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-347">Boolean</span></span>|<span data-ttu-id="6d185-348">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-348">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="6d185-349">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="6d185-349">keyboardBlockShortcuts</span></span>|<span data-ttu-id="6d185-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-350">Boolean</span></span>|<span data-ttu-id="6d185-351">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-351">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6d185-352">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="6d185-352">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="6d185-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-353">Boolean</span></span>|<span data-ttu-id="6d185-354">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-354">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="6d185-355">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="6d185-355">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="6d185-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-356">Boolean</span></span>|<span data-ttu-id="6d185-357">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-357">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-358">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="6d185-358">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="6d185-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-359">Boolean</span></span>|<span data-ttu-id="6d185-360">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-360">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-361">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="6d185-361">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="6d185-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-362">Boolean</span></span>|<span data-ttu-id="6d185-363">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-363">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-364">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="6d185-364">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="6d185-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-365">Boolean</span></span>|<span data-ttu-id="6d185-366">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-366">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-367">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="6d185-367">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="6d185-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-368">Boolean</span></span>|<span data-ttu-id="6d185-369">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-369">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-370">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="6d185-370">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="6d185-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-371">Boolean</span></span>|<span data-ttu-id="6d185-372">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-372">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-373">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="6d185-373">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="6d185-374">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-374">Boolean</span></span>|<span data-ttu-id="6d185-375">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-375">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-376">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="6d185-376">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="6d185-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-377">Boolean</span></span>|<span data-ttu-id="6d185-378">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-378">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-379">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="6d185-379">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="6d185-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-380">Boolean</span></span>|<span data-ttu-id="6d185-381">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-381">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-382">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="6d185-382">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="6d185-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-383">Boolean</span></span>|<span data-ttu-id="6d185-384">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-384">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-385">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="6d185-385">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="6d185-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-386">Boolean</span></span>|<span data-ttu-id="6d185-387">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-387">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-388">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6d185-388">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="6d185-389">String</span><span class="sxs-lookup"><span data-stu-id="6d185-389">String</span></span>|<span data-ttu-id="6d185-390">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-390">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="6d185-391">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="6d185-391">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="6d185-392">Киоскмодебуилтинаппид</span><span class="sxs-lookup"><span data-stu-id="6d185-392">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="6d185-393">String</span><span class="sxs-lookup"><span data-stu-id="6d185-393">String</span></span>|<span data-ttu-id="6d185-394">Идентификатор встроенных приложений для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-394">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="6d185-395">Используется, когда KioskModeManagedAppId и KioskModeAppStoreUrl не заданы.</span><span class="sxs-lookup"><span data-stu-id="6d185-395">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="6d185-396">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="6d185-396">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="6d185-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-397">Boolean</span></span>|<span data-ttu-id="6d185-398">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-398">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-399">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="6d185-399">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="6d185-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-400">Boolean</span></span>|<span data-ttu-id="6d185-401">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-401">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-402">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="6d185-402">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="6d185-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-403">Boolean</span></span>|<span data-ttu-id="6d185-404">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-404">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-405">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="6d185-405">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="6d185-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-406">Boolean</span></span>|<span data-ttu-id="6d185-407">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-407">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-408">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="6d185-408">kioskModeRequireZoom</span></span>|<span data-ttu-id="6d185-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-409">Boolean</span></span>|<span data-ttu-id="6d185-410">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-410">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="6d185-411">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="6d185-411">kioskModeManagedAppId</span></span>|<span data-ttu-id="6d185-412">String</span><span class="sxs-lookup"><span data-stu-id="6d185-412">String</span></span>|<span data-ttu-id="6d185-413">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="6d185-413">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="6d185-414">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="6d185-414">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="6d185-415">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="6d185-415">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="6d185-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-416">Boolean</span></span>|<span data-ttu-id="6d185-417">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="6d185-417">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="6d185-418">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="6d185-418">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="6d185-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-419">Boolean</span></span>|<span data-ttu-id="6d185-420">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="6d185-420">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="6d185-421">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="6d185-421">lockScreenBlockPassbook</span></span>|<span data-ttu-id="6d185-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-422">Boolean</span></span>|<span data-ttu-id="6d185-423">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="6d185-423">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="6d185-424">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="6d185-424">lockScreenBlockTodayView</span></span>|<span data-ttu-id="6d185-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-425">Boolean</span></span>|<span data-ttu-id="6d185-426">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="6d185-426">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="6d185-427">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="6d185-427">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="6d185-428">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="6d185-428">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="6d185-429">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="6d185-429">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="6d185-430">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="6d185-430">mediaContentRatingCanada</span></span>|[<span data-ttu-id="6d185-431">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="6d185-431">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="6d185-432">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="6d185-432">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="6d185-433">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="6d185-433">mediaContentRatingFrance</span></span>|[<span data-ttu-id="6d185-434">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="6d185-434">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="6d185-435">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="6d185-435">Media content rating settings for France</span></span>|
|<span data-ttu-id="6d185-436">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="6d185-436">mediaContentRatingGermany</span></span>|[<span data-ttu-id="6d185-437">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="6d185-437">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="6d185-438">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="6d185-438">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="6d185-439">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="6d185-439">mediaContentRatingIreland</span></span>|[<span data-ttu-id="6d185-440">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="6d185-440">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="6d185-441">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="6d185-441">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="6d185-442">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="6d185-442">mediaContentRatingJapan</span></span>|[<span data-ttu-id="6d185-443">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="6d185-443">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="6d185-444">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="6d185-444">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="6d185-445">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="6d185-445">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="6d185-446">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="6d185-446">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="6d185-447">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="6d185-447">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="6d185-448">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="6d185-448">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="6d185-449">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="6d185-449">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="6d185-450">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="6d185-450">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="6d185-451">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="6d185-451">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="6d185-452">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="6d185-452">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="6d185-453">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="6d185-453">Media content rating settings for United States</span></span>|
|<span data-ttu-id="6d185-454">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="6d185-454">networkUsageRules</span></span>|<span data-ttu-id="6d185-455">Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="6d185-455">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="6d185-456">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="6d185-456">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="6d185-457">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="6d185-457">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6d185-458">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="6d185-458">mediaContentRatingApps</span></span>|[<span data-ttu-id="6d185-459">Ратингаппстипе</span><span class="sxs-lookup"><span data-stu-id="6d185-459">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="6d185-460">Параметры оценки контента мультимедиа для приложений.</span><span class="sxs-lookup"><span data-stu-id="6d185-460">Media content rating settings for Apps.</span></span> <span data-ttu-id="6d185-461">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="6d185-461">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="6d185-462">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-462">messagesBlocked</span></span>|<span data-ttu-id="6d185-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-463">Boolean</span></span>|<span data-ttu-id="6d185-464">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="6d185-464">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="6d185-465">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="6d185-465">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="6d185-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-466">Boolean</span></span>|<span data-ttu-id="6d185-467">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-467">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6d185-468">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6d185-468">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="6d185-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-469">Boolean</span></span>|<span data-ttu-id="6d185-470">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="6d185-470">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6d185-471">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="6d185-471">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="6d185-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-472">Boolean</span></span>|<span data-ttu-id="6d185-473">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-473">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="6d185-474">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="6d185-474">passcodeBlockModification</span></span>|<span data-ttu-id="6d185-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-475">Boolean</span></span>|<span data-ttu-id="6d185-476">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-476">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6d185-477">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6d185-477">passcodeBlockSimple</span></span>|<span data-ttu-id="6d185-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-478">Boolean</span></span>|<span data-ttu-id="6d185-479">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="6d185-479">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="6d185-480">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6d185-480">passcodeExpirationDays</span></span>|<span data-ttu-id="6d185-481">Int32</span><span class="sxs-lookup"><span data-stu-id="6d185-481">Int32</span></span>|<span data-ttu-id="6d185-482">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="6d185-482">Number of days before the passcode expires.</span></span> <span data-ttu-id="6d185-483">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="6d185-483">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6d185-484">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6d185-484">passcodeMinimumLength</span></span>|<span data-ttu-id="6d185-485">Int32</span><span class="sxs-lookup"><span data-stu-id="6d185-485">Int32</span></span>|<span data-ttu-id="6d185-486">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="6d185-486">Minimum length of passcode.</span></span> <span data-ttu-id="6d185-487">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="6d185-487">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6d185-488">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6d185-488">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6d185-489">Int32</span><span class="sxs-lookup"><span data-stu-id="6d185-489">Int32</span></span>|<span data-ttu-id="6d185-490">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="6d185-490">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="6d185-491">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6d185-491">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6d185-492">Int32</span><span class="sxs-lookup"><span data-stu-id="6d185-492">Int32</span></span>|<span data-ttu-id="6d185-493">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="6d185-493">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6d185-494">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6d185-494">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="6d185-495">Int32</span><span class="sxs-lookup"><span data-stu-id="6d185-495">Int32</span></span>|<span data-ttu-id="6d185-496">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="6d185-496">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="6d185-497">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="6d185-497">Valid values 0 to 4</span></span>|
|<span data-ttu-id="6d185-498">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="6d185-498">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="6d185-499">Int32</span><span class="sxs-lookup"><span data-stu-id="6d185-499">Int32</span></span>|<span data-ttu-id="6d185-500">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="6d185-500">Number of previous passcodes to block.</span></span> <span data-ttu-id="6d185-501">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="6d185-501">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6d185-502">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="6d185-502">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="6d185-503">Int32</span><span class="sxs-lookup"><span data-stu-id="6d185-503">Int32</span></span>|<span data-ttu-id="6d185-504">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="6d185-504">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="6d185-505">Допустимые значения: от 4 до 11.</span><span class="sxs-lookup"><span data-stu-id="6d185-505">Valid values 4 to 11</span></span>|
|<span data-ttu-id="6d185-506">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="6d185-506">passcodeRequiredType</span></span>|[<span data-ttu-id="6d185-507">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="6d185-507">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6d185-508">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="6d185-508">Type of passcode that is required.</span></span> <span data-ttu-id="6d185-509">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="6d185-509">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6d185-510">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="6d185-510">passcodeRequired</span></span>|<span data-ttu-id="6d185-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-511">Boolean</span></span>|<span data-ttu-id="6d185-512">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="6d185-512">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="6d185-513">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-513">podcastsBlocked</span></span>|<span data-ttu-id="6d185-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-514">Boolean</span></span>|<span data-ttu-id="6d185-515">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-515">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="6d185-516">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="6d185-516">safariBlockAutofill</span></span>|<span data-ttu-id="6d185-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-517">Boolean</span></span>|<span data-ttu-id="6d185-518">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="6d185-518">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="6d185-519">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="6d185-519">safariBlockJavaScript</span></span>|<span data-ttu-id="6d185-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-520">Boolean</span></span>|<span data-ttu-id="6d185-521">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="6d185-521">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="6d185-522">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="6d185-522">safariBlockPopups</span></span>|<span data-ttu-id="6d185-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-523">Boolean</span></span>|<span data-ttu-id="6d185-524">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="6d185-524">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="6d185-525">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-525">safariBlocked</span></span>|<span data-ttu-id="6d185-526">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-526">Boolean</span></span>|<span data-ttu-id="6d185-527">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="6d185-527">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="6d185-528">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="6d185-528">safariCookieSettings</span></span>|[<span data-ttu-id="6d185-529">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="6d185-529">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="6d185-530">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="6d185-530">Cookie settings for Safari.</span></span> <span data-ttu-id="6d185-531">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="6d185-531">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="6d185-532">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="6d185-532">safariManagedDomains</span></span>|<span data-ttu-id="6d185-533">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6d185-533">String collection</span></span>|<span data-ttu-id="6d185-534">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="6d185-534">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="6d185-535">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="6d185-535">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="6d185-536">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6d185-536">String collection</span></span>|<span data-ttu-id="6d185-537">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="6d185-537">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="6d185-538">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-538">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6d185-539">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="6d185-539">safariRequireFraudWarning</span></span>|<span data-ttu-id="6d185-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-540">Boolean</span></span>|<span data-ttu-id="6d185-541">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="6d185-541">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="6d185-542">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-542">screenCaptureBlocked</span></span>|<span data-ttu-id="6d185-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-543">Boolean</span></span>|<span data-ttu-id="6d185-544">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="6d185-544">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="6d185-545">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-545">siriBlocked</span></span>|<span data-ttu-id="6d185-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-546">Boolean</span></span>|<span data-ttu-id="6d185-547">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="6d185-547">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="6d185-548">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="6d185-548">siriBlockedWhenLocked</span></span>|<span data-ttu-id="6d185-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-549">Boolean</span></span>|<span data-ttu-id="6d185-550">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="6d185-550">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="6d185-551">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="6d185-551">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="6d185-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-552">Boolean</span></span>|<span data-ttu-id="6d185-553">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="6d185-553">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="6d185-554">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="6d185-554">siriRequireProfanityFilter</span></span>|<span data-ttu-id="6d185-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-555">Boolean</span></span>|<span data-ttu-id="6d185-556">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="6d185-556">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="6d185-557">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="6d185-557">spotlightBlockInternetResults</span></span>|<span data-ttu-id="6d185-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-558">Boolean</span></span>|<span data-ttu-id="6d185-559">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="6d185-559">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="6d185-560">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="6d185-560">voiceDialingBlocked</span></span>|<span data-ttu-id="6d185-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-561">Boolean</span></span>|<span data-ttu-id="6d185-562">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="6d185-562">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="6d185-563">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="6d185-563">wallpaperBlockModification</span></span>|<span data-ttu-id="6d185-564">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-564">Boolean</span></span>|<span data-ttu-id="6d185-565">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6d185-565">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="6d185-566">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="6d185-566">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="6d185-567">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d185-567">Boolean</span></span>|<span data-ttu-id="6d185-568">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="6d185-568">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="6d185-569">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d185-569">Response</span></span>
<span data-ttu-id="6d185-570">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d185-570">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d185-571">Пример</span><span class="sxs-lookup"><span data-stu-id="6d185-571">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d185-572">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d185-572">Request</span></span>
<span data-ttu-id="6d185-573">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d185-573">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="6d185-574">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d185-574">Response</span></span>
<span data-ttu-id="6d185-p127">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d185-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



