---
title: Create iosGeneralDeviceConfiguration
description: Создание объекта iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4e8649b945c6f57b1968c067798ac5141b28a089
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757082"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="dca2e-103">Create iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="dca2e-103">Create iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="dca2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dca2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dca2e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dca2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dca2e-106">Создание объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca2e-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dca2e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="dca2e-107">Prerequisites</span></span>
<span data-ttu-id="dca2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dca2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dca2e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dca2e-110">Permission type</span></span>|<span data-ttu-id="dca2e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dca2e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dca2e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dca2e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dca2e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dca2e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dca2e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dca2e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dca2e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dca2e-115">Not supported.</span></span>|
|<span data-ttu-id="dca2e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="dca2e-116">Application</span></span>|<span data-ttu-id="dca2e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dca2e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dca2e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dca2e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dca2e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dca2e-119">Request headers</span></span>
|<span data-ttu-id="dca2e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dca2e-120">Header</span></span>|<span data-ttu-id="dca2e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dca2e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dca2e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dca2e-122">Authorization</span></span>|<span data-ttu-id="dca2e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dca2e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dca2e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dca2e-124">Accept</span></span>|<span data-ttu-id="dca2e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dca2e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dca2e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dca2e-126">Request body</span></span>
<span data-ttu-id="dca2e-127">В теле запроса добавьте представление объекта iosGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dca2e-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="dca2e-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="dca2e-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="dca2e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dca2e-129">Property</span></span>|<span data-ttu-id="dca2e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dca2e-130">Type</span></span>|<span data-ttu-id="dca2e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dca2e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dca2e-132">id</span><span class="sxs-lookup"><span data-stu-id="dca2e-132">id</span></span>|<span data-ttu-id="dca2e-133">String</span><span class="sxs-lookup"><span data-stu-id="dca2e-133">String</span></span>|<span data-ttu-id="dca2e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dca2e-134">Key of the entity.</span></span> <span data-ttu-id="dca2e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca2e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca2e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dca2e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="dca2e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dca2e-137">DateTimeOffset</span></span>|<span data-ttu-id="dca2e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="dca2e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="dca2e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca2e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca2e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dca2e-140">createdDateTime</span></span>|<span data-ttu-id="dca2e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dca2e-141">DateTimeOffset</span></span>|<span data-ttu-id="dca2e-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="dca2e-142">DateTime the object was created.</span></span> <span data-ttu-id="dca2e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca2e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca2e-144">description</span><span class="sxs-lookup"><span data-stu-id="dca2e-144">description</span></span>|<span data-ttu-id="dca2e-145">String</span><span class="sxs-lookup"><span data-stu-id="dca2e-145">String</span></span>|<span data-ttu-id="dca2e-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dca2e-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dca2e-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca2e-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca2e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="dca2e-148">displayName</span></span>|<span data-ttu-id="dca2e-149">String</span><span class="sxs-lookup"><span data-stu-id="dca2e-149">String</span></span>|<span data-ttu-id="dca2e-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dca2e-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dca2e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca2e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca2e-152">version</span><span class="sxs-lookup"><span data-stu-id="dca2e-152">version</span></span>|<span data-ttu-id="dca2e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="dca2e-153">Int32</span></span>|<span data-ttu-id="dca2e-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dca2e-154">Version of the device configuration.</span></span> <span data-ttu-id="dca2e-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dca2e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dca2e-156">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="dca2e-156">accountBlockModification</span></span>|<span data-ttu-id="dca2e-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-157">Boolean</span></span>|<span data-ttu-id="dca2e-158">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-158">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-159">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="dca2e-159">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="dca2e-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-160">Boolean</span></span>|<span data-ttu-id="dca2e-161">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-161">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="dca2e-162">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-162">airDropBlocked</span></span>|<span data-ttu-id="dca2e-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-163">Boolean</span></span>|<span data-ttu-id="dca2e-164">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-164">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-165">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="dca2e-165">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="dca2e-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-166">Boolean</span></span>|<span data-ttu-id="dca2e-167">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-167">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dca2e-168">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="dca2e-168">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="dca2e-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-169">Boolean</span></span>|<span data-ttu-id="dca2e-170">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="dca2e-170">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="dca2e-171">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="dca2e-171">appleWatchBlockPairing</span></span>|<span data-ttu-id="dca2e-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-172">Boolean</span></span>|<span data-ttu-id="dca2e-173">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-173">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dca2e-174">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="dca2e-174">appleWatchForceWristDetection</span></span>|<span data-ttu-id="dca2e-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-175">Boolean</span></span>|<span data-ttu-id="dca2e-176">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-176">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="dca2e-177">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-177">appleNewsBlocked</span></span>|<span data-ttu-id="dca2e-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-178">Boolean</span></span>|<span data-ttu-id="dca2e-179">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-179">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dca2e-180">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="dca2e-180">appsSingleAppModeList</span></span>|<span data-ttu-id="dca2e-181">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="dca2e-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="dca2e-182">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="dca2e-182">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="dca2e-183">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-183">Supervised only.</span></span> <span data-ttu-id="dca2e-184">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="dca2e-184">iOS 7.0 and later.</span></span> <span data-ttu-id="dca2e-185">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="dca2e-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="dca2e-186">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="dca2e-186">appsVisibilityList</span></span>|<span data-ttu-id="dca2e-187">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="dca2e-187">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="dca2e-188">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-188">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="dca2e-189">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="dca2e-189">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="dca2e-190">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="dca2e-190">appsVisibilityListType</span></span>|[<span data-ttu-id="dca2e-191">appListType</span><span class="sxs-lookup"><span data-stu-id="dca2e-191">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="dca2e-192">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="dca2e-192">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="dca2e-193">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="dca2e-193">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="dca2e-194">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="dca2e-194">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="dca2e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-195">Boolean</span></span>|<span data-ttu-id="dca2e-196">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-196">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dca2e-197">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-197">appStoreBlocked</span></span>|<span data-ttu-id="dca2e-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-198">Boolean</span></span>|<span data-ttu-id="dca2e-199">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="dca2e-199">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="dca2e-200">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="dca2e-200">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="dca2e-201">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="dca2e-201">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="dca2e-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-202">Boolean</span></span>|<span data-ttu-id="dca2e-203">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="dca2e-203">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="dca2e-204">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="dca2e-204">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="dca2e-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-205">Boolean</span></span>|<span data-ttu-id="dca2e-206">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="dca2e-206">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="dca2e-207">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-207">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dca2e-208">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="dca2e-208">appStoreRequirePassword</span></span>|<span data-ttu-id="dca2e-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-209">Boolean</span></span>|<span data-ttu-id="dca2e-210">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="dca2e-210">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="dca2e-211">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="dca2e-211">bluetoothBlockModification</span></span>|<span data-ttu-id="dca2e-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-212">Boolean</span></span>|<span data-ttu-id="dca2e-213">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-213">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="dca2e-214">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-214">cameraBlocked</span></span>|<span data-ttu-id="dca2e-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-215">Boolean</span></span>|<span data-ttu-id="dca2e-216">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="dca2e-216">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="dca2e-217">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="dca2e-217">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="dca2e-218">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="dca2e-218">cellularBlockDataRoaming</span></span>|<span data-ttu-id="dca2e-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-219">Boolean</span></span>|<span data-ttu-id="dca2e-220">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="dca2e-220">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="dca2e-221">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="dca2e-221">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="dca2e-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-222">Boolean</span></span>|<span data-ttu-id="dca2e-223">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="dca2e-223">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="dca2e-224">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="dca2e-224">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="dca2e-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-225">Boolean</span></span>|<span data-ttu-id="dca2e-226">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-226">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-227">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="dca2e-227">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="dca2e-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-228">Boolean</span></span>|<span data-ttu-id="dca2e-229">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="dca2e-229">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="dca2e-230">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="dca2e-230">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="dca2e-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-231">Boolean</span></span>|<span data-ttu-id="dca2e-232">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="dca2e-232">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="dca2e-233">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="dca2e-233">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="dca2e-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-234">Boolean</span></span>|<span data-ttu-id="dca2e-235">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="dca2e-235">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="dca2e-236">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="dca2e-236">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="dca2e-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-237">Boolean</span></span>|<span data-ttu-id="dca2e-238">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-238">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="dca2e-239">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="dca2e-239">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="dca2e-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-240">Boolean</span></span>|<span data-ttu-id="dca2e-241">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-241">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-242">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="dca2e-242">compliantAppsList</span></span>|<span data-ttu-id="dca2e-243">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="dca2e-243">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="dca2e-244">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="dca2e-244">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="dca2e-245">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="dca2e-245">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="dca2e-246">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="dca2e-246">compliantAppListType</span></span>|[<span data-ttu-id="dca2e-247">appListType</span><span class="sxs-lookup"><span data-stu-id="dca2e-247">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="dca2e-248">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="dca2e-248">List that is in the AppComplianceList.</span></span> <span data-ttu-id="dca2e-249">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="dca2e-249">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="dca2e-250">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="dca2e-250">configurationProfileBlockChanges</span></span>|<span data-ttu-id="dca2e-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-251">Boolean</span></span>|<span data-ttu-id="dca2e-252">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-252">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-253">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-253">definitionLookupBlocked</span></span>|<span data-ttu-id="dca2e-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-254">Boolean</span></span>|<span data-ttu-id="dca2e-255">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-255">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="dca2e-256">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="dca2e-256">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="dca2e-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-257">Boolean</span></span>|<span data-ttu-id="dca2e-258">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-258">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-259">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="dca2e-259">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="dca2e-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-260">Boolean</span></span>|<span data-ttu-id="dca2e-261">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-261">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-262">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="dca2e-262">deviceBlockNameModification</span></span>|<span data-ttu-id="dca2e-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-263">Boolean</span></span>|<span data-ttu-id="dca2e-264">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-264">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dca2e-265">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="dca2e-265">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="dca2e-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-266">Boolean</span></span>|<span data-ttu-id="dca2e-267">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="dca2e-267">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="dca2e-268">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="dca2e-268">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="dca2e-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-269">Boolean</span></span>|<span data-ttu-id="dca2e-270">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-270">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="dca2e-271">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="dca2e-271">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="dca2e-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-272">Boolean</span></span>|<span data-ttu-id="dca2e-273">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="dca2e-273">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="dca2e-274">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="dca2e-274">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="dca2e-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-275">Boolean</span></span>|<span data-ttu-id="dca2e-276">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="dca2e-276">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="dca2e-277">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="dca2e-277">emailInDomainSuffixes</span></span>|<span data-ttu-id="dca2e-278">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dca2e-278">String collection</span></span>|<span data-ttu-id="dca2e-279">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="dca2e-279">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="dca2e-280">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="dca2e-280">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="dca2e-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-281">Boolean</span></span>|<span data-ttu-id="dca2e-282">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="dca2e-282">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="dca2e-283">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="dca2e-283">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="dca2e-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-284">Boolean</span></span>|<span data-ttu-id="dca2e-285">\[Неоконфигурированная настройка этого параметра и установка значения "true" не влияет \] на устройство.</span><span class="sxs-lookup"><span data-stu-id="dca2e-285">\[Deprecated\] Configuring this setting and setting the value to 'true' has no effect on the device.</span></span>|
|<span data-ttu-id="dca2e-286">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-286">faceTimeBlocked</span></span>|<span data-ttu-id="dca2e-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-287">Boolean</span></span>|<span data-ttu-id="dca2e-288">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="dca2e-288">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="dca2e-289">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="dca2e-289">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="dca2e-290">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-290">findMyFriendsBlocked</span></span>|<span data-ttu-id="dca2e-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-291">Boolean</span></span>|<span data-ttu-id="dca2e-292">Указывает, следует ли блокировать изменения в "Найти друзей", когда устройство находится в режиме контроля.</span><span class="sxs-lookup"><span data-stu-id="dca2e-292">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-293">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="dca2e-293">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="dca2e-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-294">Boolean</span></span>|<span data-ttu-id="dca2e-295">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="dca2e-295">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="dca2e-296">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="dca2e-296">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="dca2e-297">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="dca2e-297">gamingBlockMultiplayer</span></span>|<span data-ttu-id="dca2e-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-298">Boolean</span></span>|<span data-ttu-id="dca2e-299">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="dca2e-299">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="dca2e-300">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="dca2e-300">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="dca2e-301">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-301">gameCenterBlocked</span></span>|<span data-ttu-id="dca2e-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-302">Boolean</span></span>|<span data-ttu-id="dca2e-303">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-303">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-304">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-304">hostPairingBlocked</span></span>|<span data-ttu-id="dca2e-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-305">Boolean</span></span>|<span data-ttu-id="dca2e-306">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-306">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-307">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-307">iBooksStoreBlocked</span></span>|<span data-ttu-id="dca2e-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-308">Boolean</span></span>|<span data-ttu-id="dca2e-309">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-309">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-310">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="dca2e-310">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="dca2e-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-311">Boolean</span></span>|<span data-ttu-id="dca2e-312">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="dca2e-312">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="dca2e-313">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="dca2e-313">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="dca2e-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-314">Boolean</span></span>|<span data-ttu-id="dca2e-315">Указывает, следует ли блокировать пользователю продолжение работы, начатой на устройстве iOS, на другое устройство iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="dca2e-315">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="dca2e-316">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="dca2e-316">iCloudBlockBackup</span></span>|<span data-ttu-id="dca2e-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-317">Boolean</span></span>|<span data-ttu-id="dca2e-318">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="dca2e-318">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="dca2e-319">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="dca2e-319">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="dca2e-320">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="dca2e-320">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="dca2e-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-321">Boolean</span></span>|<span data-ttu-id="dca2e-322">Указывает, следует ли блокировать синхронизацию документов iCloud. Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="dca2e-322">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="dca2e-323">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="dca2e-323">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="dca2e-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-324">Boolean</span></span>|<span data-ttu-id="dca2e-325">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="dca2e-325">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="dca2e-326">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="dca2e-326">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="dca2e-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-327">Boolean</span></span>|<span data-ttu-id="dca2e-328">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="dca2e-328">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="dca2e-329">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="dca2e-329">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="dca2e-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-330">Boolean</span></span>|<span data-ttu-id="dca2e-331">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="dca2e-331">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="dca2e-332">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="dca2e-332">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="dca2e-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-333">Boolean</span></span>|<span data-ttu-id="dca2e-334">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="dca2e-334">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="dca2e-335">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="dca2e-335">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="dca2e-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-336">Boolean</span></span>|<span data-ttu-id="dca2e-337">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="dca2e-337">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="dca2e-338">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="dca2e-338">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="dca2e-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-339">Boolean</span></span>|<span data-ttu-id="dca2e-340">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="dca2e-340">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="dca2e-341">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="dca2e-341">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="dca2e-342">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="dca2e-342">iTunesBlockMusicService</span></span>|<span data-ttu-id="dca2e-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-343">Boolean</span></span>|<span data-ttu-id="dca2e-344">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-344">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="dca2e-345">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="dca2e-345">iTunesBlockRadio</span></span>|<span data-ttu-id="dca2e-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-346">Boolean</span></span>|<span data-ttu-id="dca2e-347">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-347">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="dca2e-348">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="dca2e-348">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="dca2e-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-349">Boolean</span></span>|<span data-ttu-id="dca2e-350">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-350">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="dca2e-351">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="dca2e-351">keyboardBlockDictation</span></span>|<span data-ttu-id="dca2e-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-352">Boolean</span></span>|<span data-ttu-id="dca2e-353">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-353">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-354">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="dca2e-354">keyboardBlockPredictive</span></span>|<span data-ttu-id="dca2e-355">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-355">Boolean</span></span>|<span data-ttu-id="dca2e-356">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-356">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="dca2e-357">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="dca2e-357">keyboardBlockShortcuts</span></span>|<span data-ttu-id="dca2e-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-358">Boolean</span></span>|<span data-ttu-id="dca2e-359">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-359">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dca2e-360">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="dca2e-360">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="dca2e-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-361">Boolean</span></span>|<span data-ttu-id="dca2e-362">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-362">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="dca2e-363">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="dca2e-363">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="dca2e-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-364">Boolean</span></span>|<span data-ttu-id="dca2e-365">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-365">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="dca2e-366">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="dca2e-366">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="dca2e-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-367">Boolean</span></span>|<span data-ttu-id="dca2e-368">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-368">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="dca2e-369">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="dca2e-369">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="dca2e-370">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-370">Boolean</span></span>|<span data-ttu-id="dca2e-371">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-371">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="dca2e-372">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="dca2e-372">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="dca2e-373">Вместо этого используйте KioskModeBlockAutoLock.</span><span class="sxs-lookup"><span data-stu-id="dca2e-373">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="dca2e-374">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="dca2e-374">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="dca2e-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-375">Boolean</span></span>|<span data-ttu-id="dca2e-376">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-376">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="dca2e-377">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="dca2e-377">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="dca2e-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-378">Boolean</span></span>|<span data-ttu-id="dca2e-379">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-379">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="dca2e-380">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="dca2e-380">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="dca2e-381">Вместо этого используйте KioskModeBlockRingerSwitch.</span><span class="sxs-lookup"><span data-stu-id="dca2e-381">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="dca2e-382">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="dca2e-382">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="dca2e-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-383">Boolean</span></span>|<span data-ttu-id="dca2e-384">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-384">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="dca2e-385">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="dca2e-385">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="dca2e-386">Вместо этого используйте kioskModeBlockScreenRotation.</span><span class="sxs-lookup"><span data-stu-id="dca2e-386">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="dca2e-387">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="dca2e-387">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="dca2e-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-388">Boolean</span></span>|<span data-ttu-id="dca2e-389">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-389">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="dca2e-390">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="dca2e-390">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="dca2e-391">Вместо этого используйте kioskModeBlockSleepButton.</span><span class="sxs-lookup"><span data-stu-id="dca2e-391">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="dca2e-392">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="dca2e-392">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="dca2e-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-393">Boolean</span></span>|<span data-ttu-id="dca2e-394">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-394">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="dca2e-395">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="dca2e-395">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="dca2e-396">Вместо этого используйте kioskModeBlockTouchscreen.</span><span class="sxs-lookup"><span data-stu-id="dca2e-396">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="dca2e-397">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="dca2e-397">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="dca2e-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-398">Boolean</span></span>|<span data-ttu-id="dca2e-399">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-399">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="dca2e-400">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="dca2e-400">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="dca2e-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-401">Boolean</span></span>|<span data-ttu-id="dca2e-402">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-402">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="dca2e-403">Функциональность этого свойства является избыточной с помощью оси по умолчанию и обесценяется.</span><span class="sxs-lookup"><span data-stu-id="dca2e-403">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="dca2e-404">Вместо этого используйте kioskModeBlockVolumeButtons.</span><span class="sxs-lookup"><span data-stu-id="dca2e-404">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="dca2e-405">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="dca2e-405">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="dca2e-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-406">Boolean</span></span>|<span data-ttu-id="dca2e-407">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-407">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="dca2e-408">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="dca2e-408">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="dca2e-409">String</span><span class="sxs-lookup"><span data-stu-id="dca2e-409">String</span></span>|<span data-ttu-id="dca2e-410">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-410">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="dca2e-411">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="dca2e-411">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="dca2e-412">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="dca2e-412">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="dca2e-413">String</span><span class="sxs-lookup"><span data-stu-id="dca2e-413">String</span></span>|<span data-ttu-id="dca2e-414">ID для встроенных приложений, которые можно использовать для режима киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-414">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="dca2e-415">Используется, когда не заданы KioskModeManagedAppId и KioskModeAppStoreUrl.</span><span class="sxs-lookup"><span data-stu-id="dca2e-415">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="dca2e-416">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="dca2e-416">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="dca2e-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-417">Boolean</span></span>|<span data-ttu-id="dca2e-418">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-418">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="dca2e-419">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="dca2e-419">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="dca2e-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-420">Boolean</span></span>|<span data-ttu-id="dca2e-421">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-421">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="dca2e-422">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="dca2e-422">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="dca2e-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-423">Boolean</span></span>|<span data-ttu-id="dca2e-424">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-424">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="dca2e-425">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="dca2e-425">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="dca2e-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-426">Boolean</span></span>|<span data-ttu-id="dca2e-427">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-427">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="dca2e-428">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="dca2e-428">kioskModeRequireZoom</span></span>|<span data-ttu-id="dca2e-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-429">Boolean</span></span>|<span data-ttu-id="dca2e-430">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-430">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="dca2e-431">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="dca2e-431">kioskModeManagedAppId</span></span>|<span data-ttu-id="dca2e-432">String</span><span class="sxs-lookup"><span data-stu-id="dca2e-432">String</span></span>|<span data-ttu-id="dca2e-433">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="dca2e-433">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="dca2e-434">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="dca2e-434">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="dca2e-435">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="dca2e-435">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="dca2e-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-436">Boolean</span></span>|<span data-ttu-id="dca2e-437">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="dca2e-437">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="dca2e-438">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="dca2e-438">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="dca2e-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-439">Boolean</span></span>|<span data-ttu-id="dca2e-440">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="dca2e-440">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="dca2e-441">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="dca2e-441">lockScreenBlockPassbook</span></span>|<span data-ttu-id="dca2e-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-442">Boolean</span></span>|<span data-ttu-id="dca2e-443">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="dca2e-443">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="dca2e-444">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="dca2e-444">lockScreenBlockTodayView</span></span>|<span data-ttu-id="dca2e-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-445">Boolean</span></span>|<span data-ttu-id="dca2e-446">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="dca2e-446">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="dca2e-447">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="dca2e-447">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="dca2e-448">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="dca2e-448">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="dca2e-449">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="dca2e-449">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="dca2e-450">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="dca2e-450">mediaContentRatingCanada</span></span>|[<span data-ttu-id="dca2e-451">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="dca2e-451">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="dca2e-452">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="dca2e-452">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="dca2e-453">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="dca2e-453">mediaContentRatingFrance</span></span>|[<span data-ttu-id="dca2e-454">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="dca2e-454">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="dca2e-455">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="dca2e-455">Media content rating settings for France</span></span>|
|<span data-ttu-id="dca2e-456">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="dca2e-456">mediaContentRatingGermany</span></span>|[<span data-ttu-id="dca2e-457">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="dca2e-457">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="dca2e-458">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="dca2e-458">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="dca2e-459">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="dca2e-459">mediaContentRatingIreland</span></span>|[<span data-ttu-id="dca2e-460">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="dca2e-460">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="dca2e-461">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="dca2e-461">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="dca2e-462">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="dca2e-462">mediaContentRatingJapan</span></span>|[<span data-ttu-id="dca2e-463">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="dca2e-463">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="dca2e-464">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="dca2e-464">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="dca2e-465">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="dca2e-465">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="dca2e-466">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="dca2e-466">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="dca2e-467">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="dca2e-467">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="dca2e-468">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="dca2e-468">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="dca2e-469">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="dca2e-469">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="dca2e-470">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="dca2e-470">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="dca2e-471">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="dca2e-471">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="dca2e-472">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="dca2e-472">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="dca2e-473">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="dca2e-473">Media content rating settings for United States</span></span>|
|<span data-ttu-id="dca2e-474">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="dca2e-474">networkUsageRules</span></span>|<span data-ttu-id="dca2e-475">Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="dca2e-475">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="dca2e-476">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="dca2e-476">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="dca2e-477">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="dca2e-477">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="dca2e-478">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="dca2e-478">mediaContentRatingApps</span></span>|[<span data-ttu-id="dca2e-479">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="dca2e-479">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="dca2e-480">Параметры оценки контента мультимедиа для приложений.</span><span class="sxs-lookup"><span data-stu-id="dca2e-480">Media content rating settings for Apps.</span></span> <span data-ttu-id="dca2e-481">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="dca2e-481">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="dca2e-482">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-482">messagesBlocked</span></span>|<span data-ttu-id="dca2e-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-483">Boolean</span></span>|<span data-ttu-id="dca2e-484">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="dca2e-484">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="dca2e-485">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="dca2e-485">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="dca2e-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-486">Boolean</span></span>|<span data-ttu-id="dca2e-487">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-487">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="dca2e-488">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="dca2e-488">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="dca2e-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-489">Boolean</span></span>|<span data-ttu-id="dca2e-490">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="dca2e-490">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="dca2e-491">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="dca2e-491">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="dca2e-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-492">Boolean</span></span>|<span data-ttu-id="dca2e-493">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-493">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="dca2e-494">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="dca2e-494">passcodeBlockModification</span></span>|<span data-ttu-id="dca2e-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-495">Boolean</span></span>|<span data-ttu-id="dca2e-496">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-496">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dca2e-497">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="dca2e-497">passcodeBlockSimple</span></span>|<span data-ttu-id="dca2e-498">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-498">Boolean</span></span>|<span data-ttu-id="dca2e-499">Указывает, следует ли заблокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="dca2e-499">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="dca2e-500">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dca2e-500">passcodeExpirationDays</span></span>|<span data-ttu-id="dca2e-501">Int32</span><span class="sxs-lookup"><span data-stu-id="dca2e-501">Int32</span></span>|<span data-ttu-id="dca2e-502">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="dca2e-502">Number of days before the passcode expires.</span></span> <span data-ttu-id="dca2e-503">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="dca2e-503">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="dca2e-504">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dca2e-504">passcodeMinimumLength</span></span>|<span data-ttu-id="dca2e-505">Int32</span><span class="sxs-lookup"><span data-stu-id="dca2e-505">Int32</span></span>|<span data-ttu-id="dca2e-506">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="dca2e-506">Minimum length of passcode.</span></span> <span data-ttu-id="dca2e-507">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="dca2e-507">Valid values 4 to 14</span></span>|
|<span data-ttu-id="dca2e-508">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="dca2e-508">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="dca2e-509">Int32</span><span class="sxs-lookup"><span data-stu-id="dca2e-509">Int32</span></span>|<span data-ttu-id="dca2e-510">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="dca2e-510">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="dca2e-511">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="dca2e-511">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="dca2e-512">Int32</span><span class="sxs-lookup"><span data-stu-id="dca2e-512">Int32</span></span>|<span data-ttu-id="dca2e-513">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="dca2e-513">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="dca2e-514">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="dca2e-514">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="dca2e-515">Int32</span><span class="sxs-lookup"><span data-stu-id="dca2e-515">Int32</span></span>|<span data-ttu-id="dca2e-516">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="dca2e-516">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="dca2e-517">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="dca2e-517">Valid values 0 to 4</span></span>|
|<span data-ttu-id="dca2e-518">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="dca2e-518">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="dca2e-519">Int32</span><span class="sxs-lookup"><span data-stu-id="dca2e-519">Int32</span></span>|<span data-ttu-id="dca2e-520">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="dca2e-520">Number of previous passcodes to block.</span></span> <span data-ttu-id="dca2e-521">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="dca2e-521">Valid values 1 to 24</span></span>|
|<span data-ttu-id="dca2e-522">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="dca2e-522">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="dca2e-523">Int32</span><span class="sxs-lookup"><span data-stu-id="dca2e-523">Int32</span></span>|<span data-ttu-id="dca2e-524">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="dca2e-524">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="dca2e-525">Допустимые значения от 2 до 11</span><span class="sxs-lookup"><span data-stu-id="dca2e-525">Valid values 2 to 11</span></span>|
|<span data-ttu-id="dca2e-526">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="dca2e-526">passcodeRequiredType</span></span>|[<span data-ttu-id="dca2e-527">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dca2e-527">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="dca2e-528">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="dca2e-528">Type of passcode that is required.</span></span> <span data-ttu-id="dca2e-529">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="dca2e-529">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="dca2e-530">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="dca2e-530">passcodeRequired</span></span>|<span data-ttu-id="dca2e-531">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-531">Boolean</span></span>|<span data-ttu-id="dca2e-532">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="dca2e-532">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="dca2e-533">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-533">podcastsBlocked</span></span>|<span data-ttu-id="dca2e-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-534">Boolean</span></span>|<span data-ttu-id="dca2e-535">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-535">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="dca2e-536">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="dca2e-536">safariBlockAutofill</span></span>|<span data-ttu-id="dca2e-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-537">Boolean</span></span>|<span data-ttu-id="dca2e-538">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="dca2e-538">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="dca2e-539">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="dca2e-539">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="dca2e-540">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="dca2e-540">safariBlockJavaScript</span></span>|<span data-ttu-id="dca2e-541">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-541">Boolean</span></span>|<span data-ttu-id="dca2e-542">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="dca2e-542">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="dca2e-543">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="dca2e-543">safariBlockPopups</span></span>|<span data-ttu-id="dca2e-544">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-544">Boolean</span></span>|<span data-ttu-id="dca2e-545">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="dca2e-545">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="dca2e-546">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-546">safariBlocked</span></span>|<span data-ttu-id="dca2e-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-547">Boolean</span></span>|<span data-ttu-id="dca2e-548">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="dca2e-548">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="dca2e-549">Требуется контролируемое устройство для iOS 13 и более поздней.</span><span class="sxs-lookup"><span data-stu-id="dca2e-549">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="dca2e-550">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="dca2e-550">safariCookieSettings</span></span>|[<span data-ttu-id="dca2e-551">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="dca2e-551">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="dca2e-552">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="dca2e-552">Cookie settings for Safari.</span></span> <span data-ttu-id="dca2e-553">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="dca2e-553">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="dca2e-554">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="dca2e-554">safariManagedDomains</span></span>|<span data-ttu-id="dca2e-555">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dca2e-555">String collection</span></span>|<span data-ttu-id="dca2e-556">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="dca2e-556">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="dca2e-557">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="dca2e-557">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="dca2e-558">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dca2e-558">String collection</span></span>|<span data-ttu-id="dca2e-559">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="dca2e-559">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="dca2e-560">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-560">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="dca2e-561">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="dca2e-561">safariRequireFraudWarning</span></span>|<span data-ttu-id="dca2e-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-562">Boolean</span></span>|<span data-ttu-id="dca2e-563">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="dca2e-563">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="dca2e-564">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-564">screenCaptureBlocked</span></span>|<span data-ttu-id="dca2e-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-565">Boolean</span></span>|<span data-ttu-id="dca2e-566">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="dca2e-566">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="dca2e-567">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-567">siriBlocked</span></span>|<span data-ttu-id="dca2e-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-568">Boolean</span></span>|<span data-ttu-id="dca2e-569">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="dca2e-569">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="dca2e-570">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-570">siriBlockedWhenLocked</span></span>|<span data-ttu-id="dca2e-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-571">Boolean</span></span>|<span data-ttu-id="dca2e-572">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="dca2e-572">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="dca2e-573">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="dca2e-573">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="dca2e-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-574">Boolean</span></span>|<span data-ttu-id="dca2e-575">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="dca2e-575">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="dca2e-576">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="dca2e-576">siriRequireProfanityFilter</span></span>|<span data-ttu-id="dca2e-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-577">Boolean</span></span>|<span data-ttu-id="dca2e-578">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="dca2e-578">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="dca2e-579">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="dca2e-579">spotlightBlockInternetResults</span></span>|<span data-ttu-id="dca2e-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-580">Boolean</span></span>|<span data-ttu-id="dca2e-581">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="dca2e-581">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="dca2e-582">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="dca2e-582">voiceDialingBlocked</span></span>|<span data-ttu-id="dca2e-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-583">Boolean</span></span>|<span data-ttu-id="dca2e-584">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="dca2e-584">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="dca2e-585">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="dca2e-585">wallpaperBlockModification</span></span>|<span data-ttu-id="dca2e-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-586">Boolean</span></span>|<span data-ttu-id="dca2e-587">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="dca2e-587">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="dca2e-588">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="dca2e-588">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="dca2e-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca2e-589">Boolean</span></span>|<span data-ttu-id="dca2e-590">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="dca2e-590">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span> <span data-ttu-id="dca2e-591">Доступно для устройств с версиями iOS и iPadOS 14.4 и более ранних версий.</span><span class="sxs-lookup"><span data-stu-id="dca2e-591">Available for devices running iOS and iPadOS versions 14.4 and earlier.</span></span> <span data-ttu-id="dca2e-592">Устройства с 14.5+ должны использовать параметр "WiFiConnectToAllowedNetworksOnlyForced.</span><span class="sxs-lookup"><span data-stu-id="dca2e-592">Devices running 14.5+ should use the setting, “WiFiConnectToAllowedNetworksOnlyForced.</span></span>|



## <a name="response"></a><span data-ttu-id="dca2e-593">Ответ</span><span class="sxs-lookup"><span data-stu-id="dca2e-593">Response</span></span>
<span data-ttu-id="dca2e-594">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="dca2e-594">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dca2e-595">Пример</span><span class="sxs-lookup"><span data-stu-id="dca2e-595">Example</span></span>

### <a name="request"></a><span data-ttu-id="dca2e-596">Запрос</span><span class="sxs-lookup"><span data-stu-id="dca2e-596">Request</span></span>
<span data-ttu-id="dca2e-597">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dca2e-597">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dca2e-598">Отклик</span><span class="sxs-lookup"><span data-stu-id="dca2e-598">Response</span></span>
<span data-ttu-id="dca2e-p143">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dca2e-p143">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




