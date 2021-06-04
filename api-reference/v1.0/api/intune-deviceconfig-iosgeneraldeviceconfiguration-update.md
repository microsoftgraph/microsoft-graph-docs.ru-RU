---
title: Обновление объекта iosGeneralDeviceConfiguration
description: Обновление свойств объекта iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 679996c701f076c98047b71e5d57fae479e5751b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753869"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="9f077-103">Обновление объекта iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f077-103">Update iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="9f077-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f077-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f077-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f077-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f077-106">Обновление свойств объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f077-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f077-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f077-107">Prerequisites</span></span>
<span data-ttu-id="9f077-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f077-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f077-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f077-110">Permission type</span></span>|<span data-ttu-id="9f077-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f077-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f077-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f077-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f077-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f077-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f077-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f077-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f077-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f077-115">Not supported.</span></span>|
|<span data-ttu-id="9f077-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f077-116">Application</span></span>|<span data-ttu-id="9f077-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f077-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f077-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f077-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9f077-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f077-119">Request headers</span></span>
|<span data-ttu-id="9f077-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f077-120">Header</span></span>|<span data-ttu-id="9f077-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9f077-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f077-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f077-122">Authorization</span></span>|<span data-ttu-id="9f077-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f077-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f077-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9f077-124">Accept</span></span>|<span data-ttu-id="9f077-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f077-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f077-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f077-126">Request body</span></span>
<span data-ttu-id="9f077-127">В тексте запроса добавьте представление объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f077-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="9f077-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f077-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="9f077-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f077-129">Property</span></span>|<span data-ttu-id="9f077-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9f077-130">Type</span></span>|<span data-ttu-id="9f077-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9f077-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f077-132">id</span><span class="sxs-lookup"><span data-stu-id="9f077-132">id</span></span>|<span data-ttu-id="9f077-133">String</span><span class="sxs-lookup"><span data-stu-id="9f077-133">String</span></span>|<span data-ttu-id="9f077-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9f077-134">Key of the entity.</span></span> <span data-ttu-id="9f077-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f077-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f077-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f077-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9f077-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f077-137">DateTimeOffset</span></span>|<span data-ttu-id="9f077-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9f077-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9f077-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f077-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f077-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f077-140">createdDateTime</span></span>|<span data-ttu-id="9f077-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f077-141">DateTimeOffset</span></span>|<span data-ttu-id="9f077-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9f077-142">DateTime the object was created.</span></span> <span data-ttu-id="9f077-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f077-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f077-144">description</span><span class="sxs-lookup"><span data-stu-id="9f077-144">description</span></span>|<span data-ttu-id="9f077-145">String</span><span class="sxs-lookup"><span data-stu-id="9f077-145">String</span></span>|<span data-ttu-id="9f077-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f077-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9f077-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f077-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f077-148">displayName</span><span class="sxs-lookup"><span data-stu-id="9f077-148">displayName</span></span>|<span data-ttu-id="9f077-149">String</span><span class="sxs-lookup"><span data-stu-id="9f077-149">String</span></span>|<span data-ttu-id="9f077-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f077-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9f077-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f077-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f077-152">version</span><span class="sxs-lookup"><span data-stu-id="9f077-152">version</span></span>|<span data-ttu-id="9f077-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9f077-153">Int32</span></span>|<span data-ttu-id="9f077-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f077-154">Version of the device configuration.</span></span> <span data-ttu-id="9f077-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f077-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f077-156">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="9f077-156">accountBlockModification</span></span>|<span data-ttu-id="9f077-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-157">Boolean</span></span>|<span data-ttu-id="9f077-158">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-158">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9f077-159">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="9f077-159">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="9f077-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-160">Boolean</span></span>|<span data-ttu-id="9f077-161">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-161">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="9f077-162">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-162">airDropBlocked</span></span>|<span data-ttu-id="9f077-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-163">Boolean</span></span>|<span data-ttu-id="9f077-164">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-164">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9f077-165">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="9f077-165">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="9f077-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-166">Boolean</span></span>|<span data-ttu-id="9f077-167">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-167">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9f077-168">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="9f077-168">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="9f077-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-169">Boolean</span></span>|<span data-ttu-id="9f077-170">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="9f077-170">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="9f077-171">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="9f077-171">appleWatchBlockPairing</span></span>|<span data-ttu-id="9f077-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-172">Boolean</span></span>|<span data-ttu-id="9f077-173">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-173">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9f077-174">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="9f077-174">appleWatchForceWristDetection</span></span>|<span data-ttu-id="9f077-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-175">Boolean</span></span>|<span data-ttu-id="9f077-176">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-176">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="9f077-177">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-177">appleNewsBlocked</span></span>|<span data-ttu-id="9f077-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-178">Boolean</span></span>|<span data-ttu-id="9f077-179">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-179">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9f077-180">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="9f077-180">appsSingleAppModeList</span></span>|<span data-ttu-id="9f077-181">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="9f077-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9f077-182">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="9f077-182">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="9f077-183">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-183">Supervised only.</span></span> <span data-ttu-id="9f077-184">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="9f077-184">iOS 7.0 and later.</span></span> <span data-ttu-id="9f077-185">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="9f077-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="9f077-186">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="9f077-186">appsVisibilityList</span></span>|<span data-ttu-id="9f077-187">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="9f077-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9f077-188">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-188">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="9f077-189">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="9f077-189">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="9f077-190">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="9f077-190">appsVisibilityListType</span></span>|[<span data-ttu-id="9f077-191">appListType</span><span class="sxs-lookup"><span data-stu-id="9f077-191">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="9f077-192">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="9f077-192">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="9f077-193">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="9f077-193">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="9f077-194">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="9f077-194">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="9f077-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-195">Boolean</span></span>|<span data-ttu-id="9f077-196">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-196">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9f077-197">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-197">appStoreBlocked</span></span>|<span data-ttu-id="9f077-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-198">Boolean</span></span>|<span data-ttu-id="9f077-199">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="9f077-199">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="9f077-200">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="9f077-200">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="9f077-201">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="9f077-201">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="9f077-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-202">Boolean</span></span>|<span data-ttu-id="9f077-203">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="9f077-203">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="9f077-204">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="9f077-204">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="9f077-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-205">Boolean</span></span>|<span data-ttu-id="9f077-206">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="9f077-206">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="9f077-207">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-207">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9f077-208">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="9f077-208">appStoreRequirePassword</span></span>|<span data-ttu-id="9f077-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-209">Boolean</span></span>|<span data-ttu-id="9f077-210">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="9f077-210">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="9f077-211">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="9f077-211">bluetoothBlockModification</span></span>|<span data-ttu-id="9f077-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-212">Boolean</span></span>|<span data-ttu-id="9f077-213">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-213">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="9f077-214">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-214">cameraBlocked</span></span>|<span data-ttu-id="9f077-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-215">Boolean</span></span>|<span data-ttu-id="9f077-216">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="9f077-216">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="9f077-217">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="9f077-217">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="9f077-218">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="9f077-218">cellularBlockDataRoaming</span></span>|<span data-ttu-id="9f077-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-219">Boolean</span></span>|<span data-ttu-id="9f077-220">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="9f077-220">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="9f077-221">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="9f077-221">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="9f077-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-222">Boolean</span></span>|<span data-ttu-id="9f077-223">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="9f077-223">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="9f077-224">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="9f077-224">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="9f077-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-225">Boolean</span></span>|<span data-ttu-id="9f077-226">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-226">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9f077-227">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="9f077-227">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="9f077-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-228">Boolean</span></span>|<span data-ttu-id="9f077-229">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="9f077-229">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="9f077-230">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="9f077-230">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="9f077-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-231">Boolean</span></span>|<span data-ttu-id="9f077-232">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="9f077-232">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="9f077-233">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="9f077-233">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="9f077-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-234">Boolean</span></span>|<span data-ttu-id="9f077-235">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="9f077-235">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="9f077-236">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="9f077-236">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="9f077-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-237">Boolean</span></span>|<span data-ttu-id="9f077-238">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-238">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="9f077-239">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="9f077-239">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="9f077-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-240">Boolean</span></span>|<span data-ttu-id="9f077-241">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-241">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9f077-242">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="9f077-242">compliantAppsList</span></span>|<span data-ttu-id="9f077-243">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="9f077-243">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9f077-244">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="9f077-244">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="9f077-245">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="9f077-245">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="9f077-246">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="9f077-246">compliantAppListType</span></span>|[<span data-ttu-id="9f077-247">appListType</span><span class="sxs-lookup"><span data-stu-id="9f077-247">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="9f077-248">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="9f077-248">List that is in the AppComplianceList.</span></span> <span data-ttu-id="9f077-249">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="9f077-249">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="9f077-250">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="9f077-250">configurationProfileBlockChanges</span></span>|<span data-ttu-id="9f077-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-251">Boolean</span></span>|<span data-ttu-id="9f077-252">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-252">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9f077-253">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-253">definitionLookupBlocked</span></span>|<span data-ttu-id="9f077-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-254">Boolean</span></span>|<span data-ttu-id="9f077-255">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-255">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="9f077-256">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="9f077-256">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="9f077-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-257">Boolean</span></span>|<span data-ttu-id="9f077-258">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-258">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9f077-259">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="9f077-259">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="9f077-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-260">Boolean</span></span>|<span data-ttu-id="9f077-261">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-261">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9f077-262">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="9f077-262">deviceBlockNameModification</span></span>|<span data-ttu-id="9f077-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-263">Boolean</span></span>|<span data-ttu-id="9f077-264">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-264">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9f077-265">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="9f077-265">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="9f077-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-266">Boolean</span></span>|<span data-ttu-id="9f077-267">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="9f077-267">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="9f077-268">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="9f077-268">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="9f077-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-269">Boolean</span></span>|<span data-ttu-id="9f077-270">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-270">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="9f077-271">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="9f077-271">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="9f077-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-272">Boolean</span></span>|<span data-ttu-id="9f077-273">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="9f077-273">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="9f077-274">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="9f077-274">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="9f077-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-275">Boolean</span></span>|<span data-ttu-id="9f077-276">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="9f077-276">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="9f077-277">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="9f077-277">emailInDomainSuffixes</span></span>|<span data-ttu-id="9f077-278">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9f077-278">String collection</span></span>|<span data-ttu-id="9f077-279">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="9f077-279">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="9f077-280">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="9f077-280">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="9f077-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-281">Boolean</span></span>|<span data-ttu-id="9f077-282">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="9f077-282">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="9f077-283">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="9f077-283">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="9f077-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-284">Boolean</span></span>|<span data-ttu-id="9f077-285">\[Неоконфигурированная настройка этого параметра и установка значения "true" не влияет \] на устройство.</span><span class="sxs-lookup"><span data-stu-id="9f077-285">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="9f077-286">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-286">faceTimeBlocked</span></span>|<span data-ttu-id="9f077-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-287">Boolean</span></span>|<span data-ttu-id="9f077-288">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="9f077-288">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="9f077-289">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="9f077-289">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="9f077-290">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-290">findMyFriendsBlocked</span></span>|<span data-ttu-id="9f077-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-291">Boolean</span></span>|<span data-ttu-id="9f077-292">Указывает, следует ли блокировать изменения в "Найти друзей", когда устройство находится в режиме контроля.</span><span class="sxs-lookup"><span data-stu-id="9f077-292">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9f077-293">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="9f077-293">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="9f077-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-294">Boolean</span></span>|<span data-ttu-id="9f077-295">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="9f077-295">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="9f077-296">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="9f077-296">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="9f077-297">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="9f077-297">gamingBlockMultiplayer</span></span>|<span data-ttu-id="9f077-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-298">Boolean</span></span>|<span data-ttu-id="9f077-299">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="9f077-299">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="9f077-300">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="9f077-300">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="9f077-301">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-301">gameCenterBlocked</span></span>|<span data-ttu-id="9f077-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-302">Boolean</span></span>|<span data-ttu-id="9f077-303">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-303">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9f077-304">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-304">hostPairingBlocked</span></span>|<span data-ttu-id="9f077-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-305">Boolean</span></span>|<span data-ttu-id="9f077-306">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-306">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="9f077-307">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-307">iBooksStoreBlocked</span></span>|<span data-ttu-id="9f077-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-308">Boolean</span></span>|<span data-ttu-id="9f077-309">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-309">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9f077-310">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="9f077-310">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="9f077-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-311">Boolean</span></span>|<span data-ttu-id="9f077-312">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="9f077-312">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="9f077-313">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="9f077-313">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="9f077-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-314">Boolean</span></span>|<span data-ttu-id="9f077-315">Указывает, следует ли блокировать пользователю продолжение работы, начатой на устройстве iOS, на другое устройство iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="9f077-315">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="9f077-316">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="9f077-316">iCloudBlockBackup</span></span>|<span data-ttu-id="9f077-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-317">Boolean</span></span>|<span data-ttu-id="9f077-318">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="9f077-318">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="9f077-319">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="9f077-319">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="9f077-320">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="9f077-320">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="9f077-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-321">Boolean</span></span>|<span data-ttu-id="9f077-322">Указывает, следует ли блокировать синхронизацию документов iCloud. Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="9f077-322">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="9f077-323">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="9f077-323">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="9f077-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-324">Boolean</span></span>|<span data-ttu-id="9f077-325">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="9f077-325">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="9f077-326">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="9f077-326">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="9f077-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-327">Boolean</span></span>|<span data-ttu-id="9f077-328">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="9f077-328">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="9f077-329">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="9f077-329">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="9f077-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-330">Boolean</span></span>|<span data-ttu-id="9f077-331">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="9f077-331">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="9f077-332">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="9f077-332">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="9f077-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-333">Boolean</span></span>|<span data-ttu-id="9f077-334">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="9f077-334">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="9f077-335">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="9f077-335">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="9f077-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-336">Boolean</span></span>|<span data-ttu-id="9f077-337">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="9f077-337">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="9f077-338">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="9f077-338">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="9f077-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-339">Boolean</span></span>|<span data-ttu-id="9f077-340">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="9f077-340">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="9f077-341">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="9f077-341">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="9f077-342">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="9f077-342">iTunesBlockMusicService</span></span>|<span data-ttu-id="9f077-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-343">Boolean</span></span>|<span data-ttu-id="9f077-344">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-344">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="9f077-345">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="9f077-345">iTunesBlockRadio</span></span>|<span data-ttu-id="9f077-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-346">Boolean</span></span>|<span data-ttu-id="9f077-347">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-347">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="9f077-348">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="9f077-348">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="9f077-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-349">Boolean</span></span>|<span data-ttu-id="9f077-350">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-350">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="9f077-351">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="9f077-351">keyboardBlockDictation</span></span>|<span data-ttu-id="9f077-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-352">Boolean</span></span>|<span data-ttu-id="9f077-353">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-353">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="9f077-354">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="9f077-354">keyboardBlockPredictive</span></span>|<span data-ttu-id="9f077-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-355">Boolean</span></span>|<span data-ttu-id="9f077-356">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-356">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="9f077-357">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="9f077-357">keyboardBlockShortcuts</span></span>|<span data-ttu-id="9f077-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-358">Boolean</span></span>|<span data-ttu-id="9f077-359">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-359">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9f077-360">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="9f077-360">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="9f077-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-361">Boolean</span></span>|<span data-ttu-id="9f077-362">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-362">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="9f077-363">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="9f077-363">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="9f077-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-364">Boolean</span></span>|<span data-ttu-id="9f077-365">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-365">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="9f077-366">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="9f077-366">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="9f077-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-367">Boolean</span></span>|<span data-ttu-id="9f077-368">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-368">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="9f077-369">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="9f077-369">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="9f077-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-370">Boolean</span></span>|<span data-ttu-id="9f077-371">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-371">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="9f077-372">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="9f077-372">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="9f077-373">Вместо этого используйте KioskModeBlockAutoLock.</span><span class="sxs-lookup"><span data-stu-id="9f077-373">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="9f077-374">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="9f077-374">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="9f077-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-375">Boolean</span></span>|<span data-ttu-id="9f077-376">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-376">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="9f077-377">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="9f077-377">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="9f077-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-378">Boolean</span></span>|<span data-ttu-id="9f077-379">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-379">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="9f077-380">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="9f077-380">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="9f077-381">Вместо этого используйте KioskModeBlockRingerSwitch.</span><span class="sxs-lookup"><span data-stu-id="9f077-381">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="9f077-382">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="9f077-382">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="9f077-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-383">Boolean</span></span>|<span data-ttu-id="9f077-384">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-384">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="9f077-385">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="9f077-385">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="9f077-386">Вместо этого используйте kioskModeBlockScreenRotation.</span><span class="sxs-lookup"><span data-stu-id="9f077-386">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="9f077-387">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="9f077-387">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="9f077-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-388">Boolean</span></span>|<span data-ttu-id="9f077-389">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-389">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="9f077-390">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="9f077-390">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="9f077-391">Вместо этого используйте kioskModeBlockSleepButton.</span><span class="sxs-lookup"><span data-stu-id="9f077-391">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="9f077-392">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="9f077-392">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="9f077-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-393">Boolean</span></span>|<span data-ttu-id="9f077-394">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-394">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="9f077-395">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="9f077-395">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="9f077-396">Вместо этого используйте kioskModeBlockTouchscreen.</span><span class="sxs-lookup"><span data-stu-id="9f077-396">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="9f077-397">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="9f077-397">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="9f077-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-398">Boolean</span></span>|<span data-ttu-id="9f077-399">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-399">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="9f077-400">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="9f077-400">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="9f077-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-401">Boolean</span></span>|<span data-ttu-id="9f077-402">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-402">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="9f077-403">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="9f077-403">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="9f077-404">Вместо этого используйте kioskModeBlockVolumeButtons.</span><span class="sxs-lookup"><span data-stu-id="9f077-404">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="9f077-405">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="9f077-405">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="9f077-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-406">Boolean</span></span>|<span data-ttu-id="9f077-407">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-407">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="9f077-408">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9f077-408">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="9f077-409">String</span><span class="sxs-lookup"><span data-stu-id="9f077-409">String</span></span>|<span data-ttu-id="9f077-410">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-410">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="9f077-411">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="9f077-411">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="9f077-412">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="9f077-412">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="9f077-413">String</span><span class="sxs-lookup"><span data-stu-id="9f077-413">String</span></span>|<span data-ttu-id="9f077-414">ID для встроенных приложений, которые можно использовать для режима киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-414">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="9f077-415">Используется, когда не заданы KioskModeManagedAppId и KioskModeAppStoreUrl.</span><span class="sxs-lookup"><span data-stu-id="9f077-415">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="9f077-416">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="9f077-416">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="9f077-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-417">Boolean</span></span>|<span data-ttu-id="9f077-418">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-418">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="9f077-419">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="9f077-419">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="9f077-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-420">Boolean</span></span>|<span data-ttu-id="9f077-421">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-421">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="9f077-422">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="9f077-422">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="9f077-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-423">Boolean</span></span>|<span data-ttu-id="9f077-424">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-424">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="9f077-425">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="9f077-425">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="9f077-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-426">Boolean</span></span>|<span data-ttu-id="9f077-427">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-427">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="9f077-428">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="9f077-428">kioskModeRequireZoom</span></span>|<span data-ttu-id="9f077-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-429">Boolean</span></span>|<span data-ttu-id="9f077-430">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-430">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="9f077-431">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="9f077-431">kioskModeManagedAppId</span></span>|<span data-ttu-id="9f077-432">String</span><span class="sxs-lookup"><span data-stu-id="9f077-432">String</span></span>|<span data-ttu-id="9f077-433">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="9f077-433">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="9f077-434">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="9f077-434">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="9f077-435">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="9f077-435">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="9f077-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-436">Boolean</span></span>|<span data-ttu-id="9f077-437">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="9f077-437">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="9f077-438">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="9f077-438">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="9f077-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-439">Boolean</span></span>|<span data-ttu-id="9f077-440">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="9f077-440">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="9f077-441">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="9f077-441">lockScreenBlockPassbook</span></span>|<span data-ttu-id="9f077-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-442">Boolean</span></span>|<span data-ttu-id="9f077-443">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="9f077-443">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="9f077-444">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="9f077-444">lockScreenBlockTodayView</span></span>|<span data-ttu-id="9f077-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-445">Boolean</span></span>|<span data-ttu-id="9f077-446">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="9f077-446">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="9f077-447">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="9f077-447">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="9f077-448">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="9f077-448">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="9f077-449">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="9f077-449">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="9f077-450">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="9f077-450">mediaContentRatingCanada</span></span>|[<span data-ttu-id="9f077-451">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="9f077-451">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="9f077-452">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="9f077-452">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="9f077-453">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="9f077-453">mediaContentRatingFrance</span></span>|[<span data-ttu-id="9f077-454">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="9f077-454">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="9f077-455">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="9f077-455">Media content rating settings for France</span></span>|
|<span data-ttu-id="9f077-456">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="9f077-456">mediaContentRatingGermany</span></span>|[<span data-ttu-id="9f077-457">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="9f077-457">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="9f077-458">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="9f077-458">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="9f077-459">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="9f077-459">mediaContentRatingIreland</span></span>|[<span data-ttu-id="9f077-460">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="9f077-460">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="9f077-461">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="9f077-461">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="9f077-462">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="9f077-462">mediaContentRatingJapan</span></span>|[<span data-ttu-id="9f077-463">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="9f077-463">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="9f077-464">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="9f077-464">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="9f077-465">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="9f077-465">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="9f077-466">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="9f077-466">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="9f077-467">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="9f077-467">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="9f077-468">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="9f077-468">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="9f077-469">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="9f077-469">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="9f077-470">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="9f077-470">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="9f077-471">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="9f077-471">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="9f077-472">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="9f077-472">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="9f077-473">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="9f077-473">Media content rating settings for United States</span></span>|
|<span data-ttu-id="9f077-474">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="9f077-474">networkUsageRules</span></span>|<span data-ttu-id="9f077-475">Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="9f077-475">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="9f077-476">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="9f077-476">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="9f077-477">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="9f077-477">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="9f077-478">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="9f077-478">mediaContentRatingApps</span></span>|[<span data-ttu-id="9f077-479">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="9f077-479">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="9f077-480">Параметры оценки контента мультимедиа для приложений.</span><span class="sxs-lookup"><span data-stu-id="9f077-480">Media content rating settings for Apps.</span></span> <span data-ttu-id="9f077-481">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="9f077-481">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="9f077-482">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-482">messagesBlocked</span></span>|<span data-ttu-id="9f077-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-483">Boolean</span></span>|<span data-ttu-id="9f077-484">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="9f077-484">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="9f077-485">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="9f077-485">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="9f077-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-486">Boolean</span></span>|<span data-ttu-id="9f077-487">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-487">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="9f077-488">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="9f077-488">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="9f077-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-489">Boolean</span></span>|<span data-ttu-id="9f077-490">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="9f077-490">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="9f077-491">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="9f077-491">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="9f077-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-492">Boolean</span></span>|<span data-ttu-id="9f077-493">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-493">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="9f077-494">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="9f077-494">passcodeBlockModification</span></span>|<span data-ttu-id="9f077-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-495">Boolean</span></span>|<span data-ttu-id="9f077-496">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-496">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="9f077-497">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9f077-497">passcodeBlockSimple</span></span>|<span data-ttu-id="9f077-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-498">Boolean</span></span>|<span data-ttu-id="9f077-499">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="9f077-499">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="9f077-500">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9f077-500">passcodeExpirationDays</span></span>|<span data-ttu-id="9f077-501">Int32</span><span class="sxs-lookup"><span data-stu-id="9f077-501">Int32</span></span>|<span data-ttu-id="9f077-502">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="9f077-502">Number of days before the passcode expires.</span></span> <span data-ttu-id="9f077-503">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="9f077-503">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="9f077-504">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9f077-504">passcodeMinimumLength</span></span>|<span data-ttu-id="9f077-505">Int32</span><span class="sxs-lookup"><span data-stu-id="9f077-505">Int32</span></span>|<span data-ttu-id="9f077-506">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="9f077-506">Minimum length of passcode.</span></span> <span data-ttu-id="9f077-507">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="9f077-507">Valid values 4 to 14</span></span>|
|<span data-ttu-id="9f077-508">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="9f077-508">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="9f077-509">Int32</span><span class="sxs-lookup"><span data-stu-id="9f077-509">Int32</span></span>|<span data-ttu-id="9f077-510">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="9f077-510">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="9f077-511">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9f077-511">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9f077-512">Int32</span><span class="sxs-lookup"><span data-stu-id="9f077-512">Int32</span></span>|<span data-ttu-id="9f077-513">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="9f077-513">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="9f077-514">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9f077-514">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="9f077-515">Int32</span><span class="sxs-lookup"><span data-stu-id="9f077-515">Int32</span></span>|<span data-ttu-id="9f077-516">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="9f077-516">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="9f077-517">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="9f077-517">Valid values 0 to 4</span></span>|
|<span data-ttu-id="9f077-518">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="9f077-518">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="9f077-519">Int32</span><span class="sxs-lookup"><span data-stu-id="9f077-519">Int32</span></span>|<span data-ttu-id="9f077-520">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="9f077-520">Number of previous passcodes to block.</span></span> <span data-ttu-id="9f077-521">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="9f077-521">Valid values 1 to 24</span></span>|
|<span data-ttu-id="9f077-522">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="9f077-522">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="9f077-523">Int32</span><span class="sxs-lookup"><span data-stu-id="9f077-523">Int32</span></span>|<span data-ttu-id="9f077-524">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="9f077-524">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="9f077-525">Допустимые значения от 2 до 11</span><span class="sxs-lookup"><span data-stu-id="9f077-525">Valid values 2 to 11</span></span>|
|<span data-ttu-id="9f077-526">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="9f077-526">passcodeRequiredType</span></span>|[<span data-ttu-id="9f077-527">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9f077-527">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9f077-528">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="9f077-528">Type of passcode that is required.</span></span> <span data-ttu-id="9f077-529">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="9f077-529">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9f077-530">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="9f077-530">passcodeRequired</span></span>|<span data-ttu-id="9f077-531">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-531">Boolean</span></span>|<span data-ttu-id="9f077-532">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="9f077-532">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="9f077-533">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-533">podcastsBlocked</span></span>|<span data-ttu-id="9f077-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-534">Boolean</span></span>|<span data-ttu-id="9f077-535">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-535">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="9f077-536">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="9f077-536">safariBlockAutofill</span></span>|<span data-ttu-id="9f077-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-537">Boolean</span></span>|<span data-ttu-id="9f077-538">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="9f077-538">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="9f077-539">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="9f077-539">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="9f077-540">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="9f077-540">safariBlockJavaScript</span></span>|<span data-ttu-id="9f077-541">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-541">Boolean</span></span>|<span data-ttu-id="9f077-542">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="9f077-542">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="9f077-543">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="9f077-543">safariBlockPopups</span></span>|<span data-ttu-id="9f077-544">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-544">Boolean</span></span>|<span data-ttu-id="9f077-545">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="9f077-545">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="9f077-546">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-546">safariBlocked</span></span>|<span data-ttu-id="9f077-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-547">Boolean</span></span>|<span data-ttu-id="9f077-548">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="9f077-548">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="9f077-549">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="9f077-549">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="9f077-550">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="9f077-550">safariCookieSettings</span></span>|[<span data-ttu-id="9f077-551">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="9f077-551">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="9f077-552">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="9f077-552">Cookie settings for Safari.</span></span> <span data-ttu-id="9f077-553">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="9f077-553">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="9f077-554">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="9f077-554">safariManagedDomains</span></span>|<span data-ttu-id="9f077-555">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9f077-555">String collection</span></span>|<span data-ttu-id="9f077-556">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="9f077-556">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="9f077-557">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="9f077-557">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="9f077-558">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9f077-558">String collection</span></span>|<span data-ttu-id="9f077-559">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="9f077-559">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="9f077-560">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-560">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="9f077-561">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="9f077-561">safariRequireFraudWarning</span></span>|<span data-ttu-id="9f077-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-562">Boolean</span></span>|<span data-ttu-id="9f077-563">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="9f077-563">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="9f077-564">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-564">screenCaptureBlocked</span></span>|<span data-ttu-id="9f077-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-565">Boolean</span></span>|<span data-ttu-id="9f077-566">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="9f077-566">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="9f077-567">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-567">siriBlocked</span></span>|<span data-ttu-id="9f077-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-568">Boolean</span></span>|<span data-ttu-id="9f077-569">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="9f077-569">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="9f077-570">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="9f077-570">siriBlockedWhenLocked</span></span>|<span data-ttu-id="9f077-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-571">Boolean</span></span>|<span data-ttu-id="9f077-572">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="9f077-572">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="9f077-573">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="9f077-573">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="9f077-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-574">Boolean</span></span>|<span data-ttu-id="9f077-575">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="9f077-575">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="9f077-576">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="9f077-576">siriRequireProfanityFilter</span></span>|<span data-ttu-id="9f077-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-577">Boolean</span></span>|<span data-ttu-id="9f077-578">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="9f077-578">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="9f077-579">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="9f077-579">spotlightBlockInternetResults</span></span>|<span data-ttu-id="9f077-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-580">Boolean</span></span>|<span data-ttu-id="9f077-581">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="9f077-581">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="9f077-582">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="9f077-582">voiceDialingBlocked</span></span>|<span data-ttu-id="9f077-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-583">Boolean</span></span>|<span data-ttu-id="9f077-584">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="9f077-584">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="9f077-585">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="9f077-585">wallpaperBlockModification</span></span>|<span data-ttu-id="9f077-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-586">Boolean</span></span>|<span data-ttu-id="9f077-587">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="9f077-587">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="9f077-588">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="9f077-588">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="9f077-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f077-589">Boolean</span></span>|<span data-ttu-id="9f077-590">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="9f077-590">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span> <span data-ttu-id="9f077-591">Доступно для устройств с версиями iOS и iPadOS 14.4 и более ранних версий.</span><span class="sxs-lookup"><span data-stu-id="9f077-591">Available for devices running iOS and iPadOS versions 14.4 and earlier.</span></span> <span data-ttu-id="9f077-592">Устройства с 14.5+ должны использовать параметр "WiFiConnectToAllowedNetworksOnlyForced.</span><span class="sxs-lookup"><span data-stu-id="9f077-592">Devices running 14.5+ should use the setting, “WiFiConnectToAllowedNetworksOnlyForced.</span></span>|



## <a name="response"></a><span data-ttu-id="9f077-593">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f077-593">Response</span></span>
<span data-ttu-id="9f077-594">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f077-594">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f077-595">Пример</span><span class="sxs-lookup"><span data-stu-id="9f077-595">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f077-596">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f077-596">Request</span></span>
<span data-ttu-id="9f077-597">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f077-597">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f077-598">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f077-598">Response</span></span>
<span data-ttu-id="9f077-p143">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f077-p143">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




