---
title: Create iosGeneralDeviceConfiguration
description: Создание объекта iosGeneralDeviceConfiguration.
ms.openlocfilehash: d6364d07eb9023e8a45afc768003237e962dc893
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079482"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="f0cb6-103">Create iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0cb6-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="f0cb6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0cb6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0cb6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0cb6-107">Создание объекта [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-107">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0cb6-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f0cb6-108">Prerequisites</span></span>
<span data-ttu-id="f0cb6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0cb6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0cb6-111">Permission type</span></span>|<span data-ttu-id="f0cb6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0cb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0cb6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0cb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0cb6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0cb6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0cb6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0cb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0cb6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-116">Not supported.</span></span>|
|<span data-ttu-id="f0cb6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f0cb6-117">Application</span></span>|<span data-ttu-id="f0cb6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0cb6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0cb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f0cb6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f0cb6-120">Request headers</span></span>
|<span data-ttu-id="f0cb6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0cb6-121">Header</span></span>|<span data-ttu-id="f0cb6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0cb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0cb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0cb6-123">Authorization</span></span>|<span data-ttu-id="f0cb6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f0cb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0cb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0cb6-125">Accept</span></span>|<span data-ttu-id="f0cb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0cb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0cb6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f0cb6-127">Request body</span></span>
<span data-ttu-id="f0cb6-128">В теле запроса добавьте представление объекта iosGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-128">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="f0cb6-129">Ниже показаны свойства, которые необходимо указывать при создании объекта iosGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-129">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="f0cb6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0cb6-130">Property</span></span>|<span data-ttu-id="f0cb6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f0cb6-131">Type</span></span>|<span data-ttu-id="f0cb6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f0cb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0cb6-133">id</span><span class="sxs-lookup"><span data-stu-id="f0cb6-133">id</span></span>|<span data-ttu-id="f0cb6-134">String</span><span class="sxs-lookup"><span data-stu-id="f0cb6-134">String</span></span>|<span data-ttu-id="f0cb6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-135">Key of the entity.</span></span> <span data-ttu-id="f0cb6-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cb6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0cb6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f0cb6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0cb6-138">DateTimeOffset</span></span>|<span data-ttu-id="f0cb6-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f0cb6-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cb6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0cb6-141">roleScopeTagIds</span></span>|<span data-ttu-id="f0cb6-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f0cb6-142">String collection</span></span>|<span data-ttu-id="f0cb6-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f0cb6-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cb6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f0cb6-145">supportsScopeTags</span></span>|<span data-ttu-id="f0cb6-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-146">Boolean</span></span>|<span data-ttu-id="f0cb6-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f0cb6-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f0cb6-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f0cb6-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-150">This property is read-only.</span></span> <span data-ttu-id="f0cb6-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cb6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0cb6-152">createdDateTime</span></span>|<span data-ttu-id="f0cb6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0cb6-153">DateTimeOffset</span></span>|<span data-ttu-id="f0cb6-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-154">DateTime the object was created.</span></span> <span data-ttu-id="f0cb6-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cb6-156">описание</span><span class="sxs-lookup"><span data-stu-id="f0cb6-156">description</span></span>|<span data-ttu-id="f0cb6-157">String</span><span class="sxs-lookup"><span data-stu-id="f0cb6-157">String</span></span>|<span data-ttu-id="f0cb6-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f0cb6-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cb6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f0cb6-160">displayName</span></span>|<span data-ttu-id="f0cb6-161">String</span><span class="sxs-lookup"><span data-stu-id="f0cb6-161">String</span></span>|<span data-ttu-id="f0cb6-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f0cb6-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cb6-164">version</span><span class="sxs-lookup"><span data-stu-id="f0cb6-164">version</span></span>|<span data-ttu-id="f0cb6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f0cb6-165">Int32</span></span>|<span data-ttu-id="f0cb6-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-166">Version of the device configuration.</span></span> <span data-ttu-id="f0cb6-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0cb6-168">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="f0cb6-168">accountBlockModification</span></span>|<span data-ttu-id="f0cb6-169">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-169">Boolean</span></span>|<span data-ttu-id="f0cb6-170">Указывает, можно ли изменять учетную запись, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-170">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-171">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="f0cb6-171">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="f0cb6-172">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-172">Boolean</span></span>|<span data-ttu-id="f0cb6-173">Указывает, следует ли запретить блокировку активации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-173">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-174">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-174">airDropBlocked</span></span>|<span data-ttu-id="f0cb6-175">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-175">Boolean</span></span>|<span data-ttu-id="f0cb6-176">Указывает, можно ли передавать файлы через AirDrop, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-176">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-177">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="f0cb6-177">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="f0cb6-178">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-178">Boolean</span></span>|<span data-ttu-id="f0cb6-179">Указывает, следует ли считать AirDrop неуправляемым местом переноса (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-179">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-180">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="f0cb6-180">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="f0cb6-181">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-181">Boolean</span></span>|<span data-ttu-id="f0cb6-182">Указывает, обязательно ли использовать пароль для связывания на всех устройствах, получающих запросы AirPlay с этого устройства.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-182">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="f0cb6-183">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="f0cb6-183">appleWatchBlockPairing</span></span>|<span data-ttu-id="f0cb6-184">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-184">Boolean</span></span>|<span data-ttu-id="f0cb6-185">Указывает, следует ли запретить связывание с Apple Watch, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-185">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-186">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="f0cb6-186">appleWatchForceWristDetection</span></span>|<span data-ttu-id="f0cb6-187">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-187">Boolean</span></span>|<span data-ttu-id="f0cb6-188">Указывает, обязательно ли использовать функцию распознавания запястья на связанном устройстве Apple Watch (iOS 8.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-188">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="f0cb6-189">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-189">appleNewsBlocked</span></span>|<span data-ttu-id="f0cb6-190">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-190">Boolean</span></span>|<span data-ttu-id="f0cb6-191">Указывает, следует ли запретить использовать приложение "Новости", когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-191">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-192">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="f0cb6-192">appsSingleAppModeList</span></span>|<span data-ttu-id="f0cb6-193">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f0cb6-193">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f0cb6-194">Возвращает или задает список приложений iOS, которые могут самостоятельно переходить в режим одной программы.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-194">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="f0cb6-195">Только в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-195">Supervised only.</span></span> <span data-ttu-id="f0cb6-196">iOS 7.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-196">iOS 7.0 and later.</span></span> <span data-ttu-id="f0cb6-197">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f0cb6-198">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="f0cb6-198">appsVisibilityList</span></span>|<span data-ttu-id="f0cb6-199">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f0cb6-199">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f0cb6-200">Список приложений в списке видимых/запускаемых приложений или списке скрытых/незапускаемых приложений (определяется свойством AppsVisibilityListType) (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-200">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="f0cb6-201">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-201">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f0cb6-202">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="f0cb6-202">appsVisibilityListType</span></span>|[<span data-ttu-id="f0cb6-203">appListType</span><span class="sxs-lookup"><span data-stu-id="f0cb6-203">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="f0cb6-204">Тип списка, определенного свойством AppsVisibilityList.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-204">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="f0cb6-205">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-205">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="f0cb6-206">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="f0cb6-206">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="f0cb6-207">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-207">Boolean</span></span>|<span data-ttu-id="f0cb6-208">Указывает, следует ли запретить автоматическое скачивание приложений, приобретенных на других устройствах, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-208">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-209">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-209">appStoreBlocked</span></span>|<span data-ttu-id="f0cb6-210">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-210">Boolean</span></span>|<span data-ttu-id="f0cb6-211">Указывает, следует ли запретить использовать App Store.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-211">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="f0cb6-212">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="f0cb6-212">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="f0cb6-213">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-213">Boolean</span></span>|<span data-ttu-id="f0cb6-214">Указывает, следует ли запретить пользователю совершать покупки из приложения.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-214">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="f0cb6-215">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="f0cb6-215">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="f0cb6-216">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-216">Boolean</span></span>|<span data-ttu-id="f0cb6-217">Указывает, следует ли заблокировать приложение App Store, не ограничивая установку через ведущие приложения.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-217">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="f0cb6-218">Применяется только к защищенному режиму (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-218">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-219">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="f0cb6-219">appStoreRequirePassword</span></span>|<span data-ttu-id="f0cb6-220">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-220">Boolean</span></span>|<span data-ttu-id="f0cb6-221">Указывает, требуется ли пароль, когда вы используете приложение App Store.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-221">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="f0cb6-222">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="f0cb6-222">bluetoothBlockModification</span></span>|<span data-ttu-id="f0cb6-223">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-223">Boolean</span></span>|<span data-ttu-id="f0cb6-224">Указывает, можно ли изменять настройки Bluetooth, когда устройство находится в защищенном режиме (iOS 10.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-224">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-225">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-225">cameraBlocked</span></span>|<span data-ttu-id="f0cb6-226">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-226">Boolean</span></span>|<span data-ttu-id="f0cb6-227">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-227">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="f0cb6-228">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="f0cb6-228">cellularBlockDataRoaming</span></span>|<span data-ttu-id="f0cb6-229">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-229">Boolean</span></span>|<span data-ttu-id="f0cb6-230">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-230">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="f0cb6-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="f0cb6-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="f0cb6-232">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-232">Boolean</span></span>|<span data-ttu-id="f0cb6-233">Указывает, следует ли заблокировать получение фоновых данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-233">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="f0cb6-234">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="f0cb6-234">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="f0cb6-235">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-235">Boolean</span></span>|<span data-ttu-id="f0cb6-236">Указывает, можно ли изменять настройки передачи данных по сотовой сети в приложении, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-236">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-237">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="f0cb6-237">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="f0cb6-238">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-238">Boolean</span></span>|<span data-ttu-id="f0cb6-239">Указывает, следует ли заблокировать личный хот-спот.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-239">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="f0cb6-240">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="f0cb6-240">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="f0cb6-241">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-241">Boolean</span></span>|<span data-ttu-id="f0cb6-242">Указывает, следует ли заблокировать голосовой роуминг.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-242">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="f0cb6-243">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="f0cb6-243">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="f0cb6-244">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-244">Boolean</span></span>|<span data-ttu-id="f0cb6-245">Указывает, следует ли заблокировать ненадежные сертификаты TLS.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-245">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="f0cb6-246">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="f0cb6-246">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="f0cb6-247">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-247">Boolean</span></span>|<span data-ttu-id="f0cb6-248">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "Класс", когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-248">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="f0cb6-249">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="f0cb6-249">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="f0cb6-250">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-250">Boolean</span></span>|<span data-ttu-id="f0cb6-251">Указывает, следует ли предоставлять учителю управляемого курса в приложении "Класс" разрешение на просмотр экрана учащегося автоматически, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-251">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-252">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="f0cb6-252">compliantAppsList</span></span>|<span data-ttu-id="f0cb6-253">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f0cb6-253">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f0cb6-254">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-254">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="f0cb6-255">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-255">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f0cb6-256">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="f0cb6-256">compliantAppListType</span></span>|[<span data-ttu-id="f0cb6-257">appListType</span><span class="sxs-lookup"><span data-stu-id="f0cb6-257">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="f0cb6-258">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-258">List that is in the AppComplianceList.</span></span> <span data-ttu-id="f0cb6-259">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-259">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="f0cb6-260">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="f0cb6-260">configurationProfileBlockChanges</span></span>|<span data-ttu-id="f0cb6-261">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-261">Boolean</span></span>|<span data-ttu-id="f0cb6-262">Указывает, следует ли запретить интерактивную установку профилей и сертификатов конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-262">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-263">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-263">definitionLookupBlocked</span></span>|<span data-ttu-id="f0cb6-264">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-264">Boolean</span></span>|<span data-ttu-id="f0cb6-265">Указывает, следует ли заблокировать поиск определений, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-265">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="f0cb6-266">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="f0cb6-266">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="f0cb6-267">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-267">Boolean</span></span>|<span data-ttu-id="f0cb6-268">Указывает, может ли пользователь включать ограничения в настройках устройства, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-268">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-269">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="f0cb6-269">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="f0cb6-270">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-270">Boolean</span></span>|<span data-ttu-id="f0cb6-271">Указывает, можно ли использовать опцию "Стереть контент и настройки" на устройстве, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-271">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-272">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="f0cb6-272">deviceBlockNameModification</span></span>|<span data-ttu-id="f0cb6-273">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-273">Boolean</span></span>|<span data-ttu-id="f0cb6-274">Указывает, можно ли изменять имя устройства, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-274">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-275">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="f0cb6-275">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="f0cb6-276">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-276">Boolean</span></span>|<span data-ttu-id="f0cb6-277">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-277">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="f0cb6-278">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="f0cb6-278">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="f0cb6-279">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-279">Boolean</span></span>|<span data-ttu-id="f0cb6-280">Указывает, можно ли изменять настройки отправки диагностической информации, когда устройство находится в защищенном режиме (iOS 9.3.2 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-280">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="f0cb6-281">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="f0cb6-281">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="f0cb6-282">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-282">Boolean</span></span>|<span data-ttu-id="f0cb6-283">Указывает, следует ли запретить пользователю просматривать управляемые документы в неуправляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-283">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="f0cb6-284">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="f0cb6-284">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="f0cb6-285">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-285">Boolean</span></span>|<span data-ttu-id="f0cb6-286">Указывает, следует ли запретить пользователю просматривать неуправляемые документы в управляемых приложениях.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-286">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="f0cb6-287">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="f0cb6-287">emailInDomainSuffixes</span></span>|<span data-ttu-id="f0cb6-288">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f0cb6-288">String collection</span></span>|<span data-ttu-id="f0cb6-289">Адрес электронной почты без суффикса, соответствующего одной из этих строк, будет считаться внешним.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-289">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="f0cb6-290">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="f0cb6-290">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="f0cb6-291">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-291">Boolean</span></span>|<span data-ttu-id="f0cb6-292">Указывает, следует ли запретить пользователю подтверждать доверие корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-292">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="f0cb6-293">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="f0cb6-293">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="f0cb6-294">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-294">Boolean</span></span>|<span data-ttu-id="f0cb6-295">Указывает, следует ли запретить пользователю изменять настройки доверия корпоративному приложению.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-295">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="f0cb6-296">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-296">faceTimeBlocked</span></span>|<span data-ttu-id="f0cb6-297">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-297">Boolean</span></span>|<span data-ttu-id="f0cb6-298">Указывает, следует ли запретить использовать FaceTime.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-298">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="f0cb6-299">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-299">findMyFriendsBlocked</span></span>|<span data-ttu-id="f0cb6-300">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-300">Boolean</span></span>|<span data-ttu-id="f0cb6-301">Указывает, следует ли заблокировать функцию "Найти друзей", когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-301">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-302">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="f0cb6-302">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="f0cb6-303">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-303">Boolean</span></span>|<span data-ttu-id="f0cb6-304">Указывает, следует ли запретить пользователю добавлять друзей в Game Center.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-304">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="f0cb6-305">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="f0cb6-305">gamingBlockMultiplayer</span></span>|<span data-ttu-id="f0cb6-306">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-306">Boolean</span></span>|<span data-ttu-id="f0cb6-307">Указывает, следует ли запретить пользователю играть с несколькими игроками.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-307">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="f0cb6-308">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-308">gameCenterBlocked</span></span>|<span data-ttu-id="f0cb6-309">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-309">Boolean</span></span>|<span data-ttu-id="f0cb6-310">Указывает, следует ли запретить использовать Game Center, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-310">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-311">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-311">hostPairingBlocked</span></span>|<span data-ttu-id="f0cb6-312">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-312">Boolean</span></span>|<span data-ttu-id="f0cb6-313">Указывает, следует ли запретить связывание с хостами для определения устройств, к которым может подключаться устройство iOS, когда оно находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-313">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-314">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-314">iBooksStoreBlocked</span></span>|<span data-ttu-id="f0cb6-315">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-315">Boolean</span></span>|<span data-ttu-id="f0cb6-316">Указывает, следует ли запретить использовать iBooks Store, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-316">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-317">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="f0cb6-317">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="f0cb6-318">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-318">Boolean</span></span>|<span data-ttu-id="f0cb6-319">Указывает, следует ли запретить пользователю скачивать материалы из iBooks Store с пометкой "эротика".</span><span class="sxs-lookup"><span data-stu-id="f0cb6-319">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="f0cb6-320">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="f0cb6-320">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="f0cb6-321">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-321">Boolean</span></span>|<span data-ttu-id="f0cb6-322">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве iOS, на другом устройстве с iOS или macOS.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-322">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="f0cb6-323">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="f0cb6-323">iCloudBlockBackup</span></span>|<span data-ttu-id="f0cb6-324">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-324">Boolean</span></span>|<span data-ttu-id="f0cb6-325">Указывает, следует ли заблокировать резервное копирование iCloud.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-325">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="f0cb6-326">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="f0cb6-326">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="f0cb6-327">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-327">Boolean</span></span>|<span data-ttu-id="f0cb6-328">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-328">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="f0cb6-329">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="f0cb6-329">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="f0cb6-330">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-330">Boolean</span></span>|<span data-ttu-id="f0cb6-331">Указывает, следует ли заблокировать облачную синхронизацию управляемых приложений.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-331">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="f0cb6-332">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="f0cb6-332">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="f0cb6-333">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-333">Boolean</span></span>|<span data-ttu-id="f0cb6-334">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-334">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="f0cb6-335">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="f0cb6-335">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="f0cb6-336">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-336">Boolean</span></span>|<span data-ttu-id="f0cb6-337">Указывает, следует ли заблокировать синхронизацию фотопотока iCloud.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-337">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="f0cb6-338">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="f0cb6-338">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="f0cb6-339">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-339">Boolean</span></span>|<span data-ttu-id="f0cb6-340">Указывает, следует ли заблокировать общий фотопоток.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-340">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="f0cb6-341">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="f0cb6-341">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="f0cb6-342">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-342">Boolean</span></span>|<span data-ttu-id="f0cb6-343">Указывает, обязательно ли шифровать резервные копии iCloud.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-343">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="f0cb6-344">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="f0cb6-344">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="f0cb6-345">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-345">Boolean</span></span>|<span data-ttu-id="f0cb6-346">Указывает, следует ли запретить доступ к ненормативному контенту в iTunes и App Store.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-346">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="f0cb6-347">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="f0cb6-347">iTunesBlockMusicService</span></span>|<span data-ttu-id="f0cb6-348">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-348">Boolean</span></span>|<span data-ttu-id="f0cb6-349">Указывает, следует ли заблокировать службу Music и вернуть приложение "Музыка" в классический режим, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий, а также macOS 10.12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-349">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="f0cb6-350">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="f0cb6-350">iTunesBlockRadio</span></span>|<span data-ttu-id="f0cb6-351">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-351">Boolean</span></span>|<span data-ttu-id="f0cb6-352">Указывает, следует ли запретить использовать iTunes Radio, когда устройство находится в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-352">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="f0cb6-353">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="f0cb6-353">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="f0cb6-354">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-354">Boolean</span></span>|<span data-ttu-id="f0cb6-355">Указывает, следует ли заблокировать автокоррекцию, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-355">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="f0cb6-356">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="f0cb6-356">keyboardBlockDictation</span></span>|<span data-ttu-id="f0cb6-357">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-357">Boolean</span></span>|<span data-ttu-id="f0cb6-358">Указывает, следует ли запретить использовать диктофон, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-358">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-359">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="f0cb6-359">keyboardBlockPredictive</span></span>|<span data-ttu-id="f0cb6-360">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-360">Boolean</span></span>|<span data-ttu-id="f0cb6-361">Указывает, следует ли заблокировать предиктивные клавиатуры, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-361">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="f0cb6-362">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="f0cb6-362">keyboardBlockShortcuts</span></span>|<span data-ttu-id="f0cb6-363">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-363">Boolean</span></span>|<span data-ttu-id="f0cb6-364">Указывает, следует ли заблокировать сочетания клавиш, когда устройство находится в защищенном режиме (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-364">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-365">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="f0cb6-365">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="f0cb6-366">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-366">Boolean</span></span>|<span data-ttu-id="f0cb6-367">Указывает, следует ли заблокировать проверку правописания, когда устройство находится в защищенном режиме (iOS 8.1.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-367">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="f0cb6-368">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="f0cb6-368">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="f0cb6-369">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-369">Boolean</span></span>|<span data-ttu-id="f0cb6-370">Указывает, можно ли использовать специальные возможности речеобразования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-370">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-371">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="f0cb6-371">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="f0cb6-372">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-372">Boolean</span></span>|<span data-ttu-id="f0cb6-373">Указывает, следует ли запретить доступ к настройкам сенсорного управления со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-373">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-374">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="f0cb6-374">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="f0cb6-375">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-375">Boolean</span></span>|<span data-ttu-id="f0cb6-376">Указывает, следует ли запретить автоблокировку устройства в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-376">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-377">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="f0cb6-377">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="f0cb6-378">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-378">Boolean</span></span>|<span data-ttu-id="f0cb6-379">Указывает, следует ли запретить доступ к настройкам инверсии цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-379">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-380">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="f0cb6-380">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="f0cb6-381">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-381">Boolean</span></span>|<span data-ttu-id="f0cb6-382">Указывает, можно ли использовать переключатель звонка в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-382">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-383">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="f0cb6-383">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="f0cb6-384">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-384">Boolean</span></span>|<span data-ttu-id="f0cb6-385">Указывает, следует ли запретить поворот экрана в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-385">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-386">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="f0cb6-386">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="f0cb6-387">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-387">Boolean</span></span>|<span data-ttu-id="f0cb6-388">Указывает, можно ли использовать кнопку "Сон" в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-388">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-389">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="f0cb6-389">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="f0cb6-390">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-390">Boolean</span></span>|<span data-ttu-id="f0cb6-391">Указывает, можно ли использовать сенсорный экран в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-391">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-392">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="f0cb6-392">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="f0cb6-393">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-393">Boolean</span></span>|<span data-ttu-id="f0cb6-394">Указывает, следует ли запретить доступ к настройкам VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-394">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-395">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="f0cb6-395">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="f0cb6-396">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-396">Boolean</span></span>|<span data-ttu-id="f0cb6-397">Указывает, можно ли использовать кнопки громкости в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-397">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-398">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="f0cb6-398">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="f0cb6-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0cb6-399">Boolean</span></span>|<span data-ttu-id="f0cb6-400">Указывает, следует ли блокировать кнопки громкости в режиме терминала.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-400">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="f0cb6-401">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="f0cb6-401">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="f0cb6-402">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-402">Boolean</span></span>|<span data-ttu-id="f0cb6-403">Указывает, следует ли запретить доступ к настройкам масштабирования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-403">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-404">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f0cb6-404">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="f0cb6-405">String</span><span class="sxs-lookup"><span data-stu-id="f0cb6-405">String</span></span>|<span data-ttu-id="f0cb6-406">URL-адрес приложения в App Store для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-406">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="f0cb6-407">Используйте, если свойство KioskModeManagedAppId не известно.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-407">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="f0cb6-408">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="f0cb6-408">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="f0cb6-409">String</span><span class="sxs-lookup"><span data-stu-id="f0cb6-409">String</span></span>|<span data-ttu-id="f0cb6-410">КОД для встроенных приложений для использования в полноэкранном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-410">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="f0cb6-411">Используется при KioskModeManagedAppId и KioskModeAppStoreUrl не установлен.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-411">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="f0cb6-412">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="f0cb6-412">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="f0cb6-413">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-413">Boolean</span></span>|<span data-ttu-id="f0cb6-414">Указывает, обязательно ли использовать сенсорное управление со специальными возможностями в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-414">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-415">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="f0cb6-415">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="f0cb6-416">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-416">Boolean</span></span>|<span data-ttu-id="f0cb6-417">Указывает, обязательно ли использовать инверсию цвета в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-417">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-418">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="f0cb6-418">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="f0cb6-419">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-419">Boolean</span></span>|<span data-ttu-id="f0cb6-420">Указывает, обязательно ли использовать монозвук в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-420">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-421">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="f0cb6-421">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="f0cb6-422">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-422">Boolean</span></span>|<span data-ttu-id="f0cb6-423">Указывает, обязательно ли использовать VoiceOver в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-423">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-424">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="f0cb6-424">kioskModeRequireZoom</span></span>|<span data-ttu-id="f0cb6-425">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-425">Boolean</span></span>|<span data-ttu-id="f0cb6-426">Указывает, обязательно ли использовать масштабирование в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-426">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="f0cb6-427">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="f0cb6-427">kioskModeManagedAppId</span></span>|<span data-ttu-id="f0cb6-428">String</span><span class="sxs-lookup"><span data-stu-id="f0cb6-428">String</span></span>|<span data-ttu-id="f0cb6-429">Идентификатор управляемого приложения для использования в режиме киоска.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-429">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="f0cb6-430">Если указано свойство KioskModeManagedAppId, KioskModeAppStoreUrl игнорируется.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-430">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="f0cb6-431">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="f0cb6-431">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="f0cb6-432">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-432">Boolean</span></span>|<span data-ttu-id="f0cb6-433">Указывает, следует ли запретить использовать центр управления на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-433">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="f0cb6-434">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="f0cb6-434">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="f0cb6-435">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-435">Boolean</span></span>|<span data-ttu-id="f0cb6-436">Указывает, следует ли запретить использовать представление уведомлений на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-436">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="f0cb6-437">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="f0cb6-437">lockScreenBlockPassbook</span></span>|<span data-ttu-id="f0cb6-438">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-438">Boolean</span></span>|<span data-ttu-id="f0cb6-439">Указывает, следует ли запретить использовать Passbook, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-439">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="f0cb6-440">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="f0cb6-440">lockScreenBlockTodayView</span></span>|<span data-ttu-id="f0cb6-441">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-441">Boolean</span></span>|<span data-ttu-id="f0cb6-442">Указывает, следует ли запретить использовать представление "Сегодня" на заблокированном экране.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-442">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="f0cb6-443">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="f0cb6-443">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="f0cb6-444">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="f0cb6-444">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="f0cb6-445">Настройки возрастных ограничений для Австралии</span><span class="sxs-lookup"><span data-stu-id="f0cb6-445">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="f0cb6-446">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="f0cb6-446">mediaContentRatingCanada</span></span>|[<span data-ttu-id="f0cb6-447">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="f0cb6-447">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="f0cb6-448">Настройки возрастных ограничений для Канады</span><span class="sxs-lookup"><span data-stu-id="f0cb6-448">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="f0cb6-449">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="f0cb6-449">mediaContentRatingFrance</span></span>|[<span data-ttu-id="f0cb6-450">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="f0cb6-450">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="f0cb6-451">Настройки возрастных ограничений для Франции</span><span class="sxs-lookup"><span data-stu-id="f0cb6-451">Media content rating settings for France</span></span>|
|<span data-ttu-id="f0cb6-452">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="f0cb6-452">mediaContentRatingGermany</span></span>|[<span data-ttu-id="f0cb6-453">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="f0cb6-453">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="f0cb6-454">Настройки возрастных ограничений для Германии</span><span class="sxs-lookup"><span data-stu-id="f0cb6-454">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="f0cb6-455">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="f0cb6-455">mediaContentRatingIreland</span></span>|[<span data-ttu-id="f0cb6-456">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="f0cb6-456">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="f0cb6-457">Настройки возрастных ограничений для Ирландии</span><span class="sxs-lookup"><span data-stu-id="f0cb6-457">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="f0cb6-458">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="f0cb6-458">mediaContentRatingJapan</span></span>|[<span data-ttu-id="f0cb6-459">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="f0cb6-459">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="f0cb6-460">Настройки возрастных ограничений для Японии</span><span class="sxs-lookup"><span data-stu-id="f0cb6-460">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="f0cb6-461">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="f0cb6-461">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="f0cb6-462">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="f0cb6-462">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="f0cb6-463">Настройки возрастных ограничений для Новой Зеландии</span><span class="sxs-lookup"><span data-stu-id="f0cb6-463">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="f0cb6-464">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="f0cb6-464">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="f0cb6-465">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="f0cb6-465">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="f0cb6-466">Настройки возрастных ограничений для Соединенного Королевства</span><span class="sxs-lookup"><span data-stu-id="f0cb6-466">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="f0cb6-467">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="f0cb6-467">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="f0cb6-468">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="f0cb6-468">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="f0cb6-469">Настройки возрастных ограничений для Соединенных Штатов</span><span class="sxs-lookup"><span data-stu-id="f0cb6-469">Media content rating settings for United States</span></span>|
|<span data-ttu-id="f0cb6-470">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="f0cb6-470">networkUsageRules</span></span>|<span data-ttu-id="f0cb6-471">Коллекция [iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md)</span><span class="sxs-lookup"><span data-stu-id="f0cb6-471">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="f0cb6-472">Список управляемых приложений и сетевых правил, которые к ним применяются.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-472">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="f0cb6-473">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-473">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="f0cb6-474">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="f0cb6-474">mediaContentRatingApps</span></span>|[<span data-ttu-id="f0cb6-475">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="f0cb6-475">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="f0cb6-476">Оценка параметры для приложений контента мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-476">Media content rating settings for Apps.</span></span> <span data-ttu-id="f0cb6-477">Возможные значения: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-477">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="f0cb6-478">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-478">messagesBlocked</span></span>|<span data-ttu-id="f0cb6-479">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-479">Boolean</span></span>|<span data-ttu-id="f0cb6-480">Указывает, следует ли запретить использовать приложение "Сообщения" на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-480">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="f0cb6-481">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="f0cb6-481">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="f0cb6-482">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-482">Boolean</span></span>|<span data-ttu-id="f0cb6-483">Указывает, можно ли изменять настройки уведомлений (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-483">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="f0cb6-484">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="f0cb6-484">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="f0cb6-485">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-485">Boolean</span></span>|<span data-ttu-id="f0cb6-486">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-486">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="f0cb6-487">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="f0cb6-487">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="f0cb6-488">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-488">Boolean</span></span>|<span data-ttu-id="f0cb6-489">Позволяет заблокировать изменение зарегистрированных отпечатков пальцев Touch ID в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-489">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-490">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="f0cb6-490">passcodeBlockModification</span></span>|<span data-ttu-id="f0cb6-491">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-491">Boolean</span></span>|<span data-ttu-id="f0cb6-492">Указывает, можно ли изменять секретный код на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-492">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-493">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f0cb6-493">passcodeBlockSimple</span></span>|<span data-ttu-id="f0cb6-494">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-494">Boolean</span></span>|<span data-ttu-id="f0cb6-495">Указывает, следует ли блокировать простые секретные коды.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-495">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="f0cb6-496">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f0cb6-496">passcodeExpirationDays</span></span>|<span data-ttu-id="f0cb6-497">Int32</span><span class="sxs-lookup"><span data-stu-id="f0cb6-497">Int32</span></span>|<span data-ttu-id="f0cb6-498">Количество дней до окончания срока действия секретного кода.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-498">Number of days before the passcode expires.</span></span> <span data-ttu-id="f0cb6-499">Допустимые значения: от 1 до 65 535.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-499">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="f0cb6-500">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f0cb6-500">passcodeMinimumLength</span></span>|<span data-ttu-id="f0cb6-501">Int32</span><span class="sxs-lookup"><span data-stu-id="f0cb6-501">Int32</span></span>|<span data-ttu-id="f0cb6-502">Минимальная длина секретного кода.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-502">Minimum length of passcode.</span></span> <span data-ttu-id="f0cb6-503">Допустимые значения: от 4 до 14.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-503">Valid values 4 to 14</span></span>|
|<span data-ttu-id="f0cb6-504">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f0cb6-504">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f0cb6-505">Int32</span><span class="sxs-lookup"><span data-stu-id="f0cb6-505">Int32</span></span>|<span data-ttu-id="f0cb6-506">Период бездействия (в минутах) до запроса пароля.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-506">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="f0cb6-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f0cb6-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f0cb6-508">Int32</span><span class="sxs-lookup"><span data-stu-id="f0cb6-508">Int32</span></span>|<span data-ttu-id="f0cb6-509">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-509">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f0cb6-510">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f0cb6-510">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="f0cb6-511">Int32</span><span class="sxs-lookup"><span data-stu-id="f0cb6-511">Int32</span></span>|<span data-ttu-id="f0cb6-512">Количество наборов символов, которые должен содержать секретный код.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-512">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="f0cb6-513">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-513">Valid values 0 to 4</span></span>|
|<span data-ttu-id="f0cb6-514">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="f0cb6-514">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="f0cb6-515">Int32</span><span class="sxs-lookup"><span data-stu-id="f0cb6-515">Int32</span></span>|<span data-ttu-id="f0cb6-516">Количество предыдущих секретных кодов, которые следует блокировать.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-516">Number of previous passcodes to block.</span></span> <span data-ttu-id="f0cb6-517">Допустимые значения: от 1 до 24.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-517">Valid values 1 to 24</span></span>|
|<span data-ttu-id="f0cb6-518">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="f0cb6-518">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="f0cb6-519">Int32</span><span class="sxs-lookup"><span data-stu-id="f0cb6-519">Int32</span></span>|<span data-ttu-id="f0cb6-520">Количество неудачных попыток входа до очистки устройства.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-520">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="f0cb6-521">Допустимые значения: от 4 до 11</span><span class="sxs-lookup"><span data-stu-id="f0cb6-521">Valid values 4 to 11</span></span>|
|<span data-ttu-id="f0cb6-522">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="f0cb6-522">passcodeRequiredType</span></span>|[<span data-ttu-id="f0cb6-523">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f0cb6-523">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f0cb6-524">Необходимый тип секретного кода.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-524">Type of passcode that is required.</span></span> <span data-ttu-id="f0cb6-525">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-525">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f0cb6-526">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="f0cb6-526">passcodeRequired</span></span>|<span data-ttu-id="f0cb6-527">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-527">Boolean</span></span>|<span data-ttu-id="f0cb6-528">Указывает, обязательно ли использовать секретный код.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-528">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="f0cb6-529">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-529">podcastsBlocked</span></span>|<span data-ttu-id="f0cb6-530">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-530">Boolean</span></span>|<span data-ttu-id="f0cb6-531">Указывает, следует ли запретить использовать подкасты на защищенном устройстве (iOS 8.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-531">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-532">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="f0cb6-532">safariBlockAutofill</span></span>|<span data-ttu-id="f0cb6-533">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-533">Boolean</span></span>|<span data-ttu-id="f0cb6-534">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-534">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="f0cb6-535">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="f0cb6-535">safariBlockJavaScript</span></span>|<span data-ttu-id="f0cb6-536">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-536">Boolean</span></span>|<span data-ttu-id="f0cb6-537">Указывает, следует ли заблокировать JavaScript в Safari.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-537">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="f0cb6-538">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="f0cb6-538">safariBlockPopups</span></span>|<span data-ttu-id="f0cb6-539">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-539">Boolean</span></span>|<span data-ttu-id="f0cb6-540">Указывает, следует ли блокировать всплывающие окна в Safari.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-540">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="f0cb6-541">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-541">safariBlocked</span></span>|<span data-ttu-id="f0cb6-542">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-542">Boolean</span></span>|<span data-ttu-id="f0cb6-543">Указывает, следует ли запретить использовать Safari.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-543">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="f0cb6-544">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="f0cb6-544">safariCookieSettings</span></span>|[<span data-ttu-id="f0cb6-545">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="f0cb6-545">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="f0cb6-546">Настройки файлов cookie для Safari.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-546">Cookie settings for Safari.</span></span> <span data-ttu-id="f0cb6-547">Возможные значения: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-547">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="f0cb6-548">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="f0cb6-548">safariManagedDomains</span></span>|<span data-ttu-id="f0cb6-549">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f0cb6-549">String collection</span></span>|<span data-ttu-id="f0cb6-550">URL-адреса, соответствующие приведенным здесь шаблонам, будут считаться управляемыми.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-550">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="f0cb6-551">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="f0cb6-551">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="f0cb6-552">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f0cb6-552">String collection</span></span>|<span data-ttu-id="f0cb6-553">Пользователи могут сохранять пароли в Safari только с URL-адресов, соответствующих приведенным здесь шаблонам.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-553">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="f0cb6-554">Применяется к устройствам в защищенном режиме (iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-554">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="f0cb6-555">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="f0cb6-555">safariRequireFraudWarning</span></span>|<span data-ttu-id="f0cb6-556">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-556">Boolean</span></span>|<span data-ttu-id="f0cb6-557">Указывает, обязательно ли предупреждение о мошенничестве в Safari.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-557">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="f0cb6-558">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-558">screenCaptureBlocked</span></span>|<span data-ttu-id="f0cb6-559">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-559">Boolean</span></span>|<span data-ttu-id="f0cb6-560">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-560">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="f0cb6-561">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-561">siriBlocked</span></span>|<span data-ttu-id="f0cb6-562">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-562">Boolean</span></span>|<span data-ttu-id="f0cb6-563">Указывает, следует ли запретить использовать Siri.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-563">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="f0cb6-564">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-564">siriBlockedWhenLocked</span></span>|<span data-ttu-id="f0cb6-565">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-565">Boolean</span></span>|<span data-ttu-id="f0cb6-566">Указывает, следует ли запретить использовать Siri, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-566">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="f0cb6-567">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="f0cb6-567">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="f0cb6-568">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-568">Boolean</span></span>|<span data-ttu-id="f0cb6-569">Указывает, следует ли запретить Siri запрашивать данные о пользовательском контенте на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-569">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="f0cb6-570">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="f0cb6-570">siriRequireProfanityFilter</span></span>|<span data-ttu-id="f0cb6-571">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-571">Boolean</span></span>|<span data-ttu-id="f0cb6-572">Указывает, следует ли запретить Siri записывать или произносить нецензурные выражения на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-572">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="f0cb6-573">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="f0cb6-573">spotlightBlockInternetResults</span></span>|<span data-ttu-id="f0cb6-574">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-574">Boolean</span></span>|<span data-ttu-id="f0cb6-575">Указывает, следует ли запретить показывать результаты из Интернета при поиске полезных сведений на защищенном устройстве.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-575">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="f0cb6-576">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-576">voiceDialingBlocked</span></span>|<span data-ttu-id="f0cb6-577">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-577">Boolean</span></span>|<span data-ttu-id="f0cb6-578">Указывает, следует ли заблокировать голосовой набор.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-578">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="f0cb6-579">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="f0cb6-579">wallpaperBlockModification</span></span>|<span data-ttu-id="f0cb6-580">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-580">Boolean</span></span>|<span data-ttu-id="f0cb6-581">Указывает, можно ли изменять обои на защищенном устройстве (iOS 9.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-581">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="f0cb6-582">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="f0cb6-582">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="f0cb6-583">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-583">Boolean</span></span>|<span data-ttu-id="f0cb6-584">Указывает, обязательно ли использовать только сети Wi-Fi из профилей конфигурации, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-584">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f0cb6-585">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="f0cb6-585">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="f0cb6-586">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-586">Boolean</span></span>|<span data-ttu-id="f0cb6-587">Указывает, будет ли студента участвуют в неуправляемых курс с помощью аудиторий запрашивающих разрешение из преподаватель при попытке оставьте курс (операций ввода-вывода 11.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-587">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="f0cb6-588">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="f0cb6-588">keychainBlockCloudSync</span></span>|<span data-ttu-id="f0cb6-589">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-589">Boolean</span></span>|<span data-ttu-id="f0cb6-590">Указывает, заблокирован ли iCloud ключей синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-590">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="f0cb6-591">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="f0cb6-591">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="f0cb6-592">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-592">Boolean</span></span>|<span data-ttu-id="f0cb6-593">Указывает ли беспроводной PKI заблокированы.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-593">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="f0cb6-594">Задание ограничения значение false, не отключает проверки списка отзыва Сертификатов и OCSP (операций ввода-вывода 7.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-594">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-595">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="f0cb6-595">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="f0cb6-596">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-596">Boolean</span></span>|<span data-ttu-id="f0cb6-597">Указывает, является ли ограниченный ad отслеживания. (операций ввода-вывода 7.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-597">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-598">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="f0cb6-598">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="f0cb6-599">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-599">Boolean</span></span>|<span data-ttu-id="f0cb6-600">Указывает, что заблокирован ли Enterprise книги резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-600">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="f0cb6-601">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="f0cb6-601">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="f0cb6-602">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-602">Boolean</span></span>|<span data-ttu-id="f0cb6-603">Указывает, заблокирован ли Enterprise книги notes и основные сведения о синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-603">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="f0cb6-604">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="f0cb6-604">airPrintBlocked</span></span>|<span data-ttu-id="f0cb6-605">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-605">Boolean</span></span>|<span data-ttu-id="f0cb6-606">Указывает, является ли AirPrint заблокированных (операций ввода-вывода 11.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-606">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-607">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="f0cb6-607">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="f0cb6-608">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-608">Boolean</span></span>|<span data-ttu-id="f0cb6-609">Указывает, является ли хранилища ключей имя пользователя и пароль для Airprint заблокированных (операций ввода-вывода 11.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-609">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-610">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="f0cb6-610">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="f0cb6-611">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-611">Boolean</span></span>|<span data-ttu-id="f0cb6-612">Указывает, являются ли доверенные сертификаты для печати обмена данными TLS (операций ввода-вывода 11.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-612">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-613">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="f0cb6-613">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="f0cb6-614">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-614">Boolean</span></span>|<span data-ttu-id="f0cb6-615">Указывает, заблокирован ли обнаружения iBeacon AirPrint принтеров.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-615">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="f0cb6-616">Это позволяет предотвратить ложных маяки AirPrint Bluetooth от фишинга для сетевого трафика (операций ввода-вывода 11.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-616">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-617">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="f0cb6-617">blockSystemAppRemoval</span></span>|<span data-ttu-id="f0cb6-618">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-618">Boolean</span></span>|<span data-ttu-id="f0cb6-619">Указывает, заблокирован ли удаления приложений системы с устройства на контролируемом устройства (операций ввода-вывода 11.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-619">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="f0cb6-620">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="f0cb6-620">vpnBlockCreation</span></span>|<span data-ttu-id="f0cb6-621">Логический</span><span class="sxs-lookup"><span data-stu-id="f0cb6-621">Boolean</span></span>|<span data-ttu-id="f0cb6-622">Указывает, является ли создание конфигурации VPN заблокированных (операций ввода-вывода 11.0 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="f0cb6-622">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|



## <a name="response"></a><span data-ttu-id="f0cb6-623">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0cb6-623">Response</span></span>
<span data-ttu-id="f0cb6-624">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-624">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0cb6-625">Пример</span><span class="sxs-lookup"><span data-stu-id="f0cb6-625">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0cb6-626">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0cb6-626">Request</span></span>
<span data-ttu-id="f0cb6-627">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0cb6-627">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 8496

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "vpnBlockCreation": true
}
```

### <a name="response"></a><span data-ttu-id="f0cb6-628">Ответ</span><span class="sxs-lookup"><span data-stu-id="f0cb6-628">Response</span></span>
<span data-ttu-id="f0cb6-p132">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f0cb6-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 8604

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
  "vpnBlockCreation": true
}
```





