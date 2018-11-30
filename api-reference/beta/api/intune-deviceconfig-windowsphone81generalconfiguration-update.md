---
title: Обновление windowsPhone81GeneralConfiguration
description: Обновление свойств объекта windowsPhone81GeneralConfiguration.
ms.openlocfilehash: b6789ea8dcf7ebeb1a36b705256af27857c93970
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082683"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="b4fb6-103">Обновление windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="b4fb6-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="b4fb6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4fb6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4fb6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4fb6-107">Обновление свойств объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-107">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4fb6-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b4fb6-108">Prerequisites</span></span>
<span data-ttu-id="b4fb6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4fb6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4fb6-111">Permission type</span></span>|<span data-ttu-id="b4fb6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4fb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4fb6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4fb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4fb6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4fb6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4fb6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4fb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4fb6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-116">Not supported.</span></span>|
|<span data-ttu-id="b4fb6-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4fb6-117">Application</span></span>|<span data-ttu-id="b4fb6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4fb6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4fb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b4fb6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4fb6-120">Request headers</span></span>
|<span data-ttu-id="b4fb6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4fb6-121">Header</span></span>|<span data-ttu-id="b4fb6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b4fb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4fb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4fb6-123">Authorization</span></span>|<span data-ttu-id="b4fb6-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="b4fb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4fb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b4fb6-125">Accept</span></span>|<span data-ttu-id="b4fb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4fb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4fb6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4fb6-127">Request body</span></span>
<span data-ttu-id="b4fb6-128">В теле запроса добавьте представление объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-128">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="b4fb6-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-129">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="b4fb6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4fb6-130">Property</span></span>|<span data-ttu-id="b4fb6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b4fb6-131">Type</span></span>|<span data-ttu-id="b4fb6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b4fb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4fb6-133">id</span><span class="sxs-lookup"><span data-stu-id="b4fb6-133">id</span></span>|<span data-ttu-id="b4fb6-134">String</span><span class="sxs-lookup"><span data-stu-id="b4fb6-134">String</span></span>|<span data-ttu-id="b4fb6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-135">Key of the entity.</span></span> <span data-ttu-id="b4fb6-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4fb6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4fb6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b4fb6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4fb6-138">DateTimeOffset</span></span>|<span data-ttu-id="b4fb6-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b4fb6-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4fb6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b4fb6-141">roleScopeTagIds</span></span>|<span data-ttu-id="b4fb6-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b4fb6-142">String collection</span></span>|<span data-ttu-id="b4fb6-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b4fb6-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4fb6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b4fb6-145">supportsScopeTags</span></span>|<span data-ttu-id="b4fb6-146">Логический</span><span class="sxs-lookup"><span data-stu-id="b4fb6-146">Boolean</span></span>|<span data-ttu-id="b4fb6-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b4fb6-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b4fb6-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b4fb6-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-150">This property is read-only.</span></span> <span data-ttu-id="b4fb6-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4fb6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4fb6-152">createdDateTime</span></span>|<span data-ttu-id="b4fb6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4fb6-153">DateTimeOffset</span></span>|<span data-ttu-id="b4fb6-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-154">DateTime the object was created.</span></span> <span data-ttu-id="b4fb6-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4fb6-156">описание</span><span class="sxs-lookup"><span data-stu-id="b4fb6-156">description</span></span>|<span data-ttu-id="b4fb6-157">String</span><span class="sxs-lookup"><span data-stu-id="b4fb6-157">String</span></span>|<span data-ttu-id="b4fb6-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b4fb6-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4fb6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b4fb6-160">displayName</span></span>|<span data-ttu-id="b4fb6-161">String</span><span class="sxs-lookup"><span data-stu-id="b4fb6-161">String</span></span>|<span data-ttu-id="b4fb6-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b4fb6-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4fb6-164">version</span><span class="sxs-lookup"><span data-stu-id="b4fb6-164">version</span></span>|<span data-ttu-id="b4fb6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b4fb6-165">Int32</span></span>|<span data-ttu-id="b4fb6-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-166">Version of the device configuration.</span></span> <span data-ttu-id="b4fb6-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4fb6-168">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="b4fb6-168">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="b4fb6-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-169">Boolean</span></span>|<span data-ttu-id="b4fb6-170">Указывает, применяется ли эта политика только к Windows Phone 8.1.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-170">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="b4fb6-171">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-171">This property is read-only.</span></span>|
|<span data-ttu-id="b4fb6-172">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="b4fb6-172">appsBlockCopyPaste</span></span>|<span data-ttu-id="b4fb6-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-173">Boolean</span></span>|<span data-ttu-id="b4fb6-174">Указывает, следует ли заблокировать копирование данных.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-174">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="b4fb6-175">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="b4fb6-175">bluetoothBlocked</span></span>|<span data-ttu-id="b4fb6-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-176">Boolean</span></span>|<span data-ttu-id="b4fb6-177">Указывает, следует ли заблокировать Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-177">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="b4fb6-178">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b4fb6-178">cameraBlocked</span></span>|<span data-ttu-id="b4fb6-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-179">Boolean</span></span>|<span data-ttu-id="b4fb6-180">Указывает, следует ли заблокировать камеру.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-180">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="b4fb6-181">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="b4fb6-181">cellularBlockWifiTethering</span></span>|<span data-ttu-id="b4fb6-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-182">Boolean</span></span>|<span data-ttu-id="b4fb6-183">Указывает, следует ли заблокировать модем Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-183">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="b4fb6-184">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-184">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="b4fb6-185">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="b4fb6-185">compliantAppsList</span></span>|<span data-ttu-id="b4fb6-186">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4fb6-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b4fb6-187">Список приложений (разрешенных или заблокированных в зависимости от значения свойства CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-187">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="b4fb6-188">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-188">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b4fb6-189">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="b4fb6-189">compliantAppListType</span></span>|[<span data-ttu-id="b4fb6-190">appListType</span><span class="sxs-lookup"><span data-stu-id="b4fb6-190">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="b4fb6-191">Список, указанный с помощью свойства AppComplianceList.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-191">List that is in the AppComplianceList.</span></span> <span data-ttu-id="b4fb6-192">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-192">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b4fb6-193">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="b4fb6-193">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="b4fb6-194">Логический</span><span class="sxs-lookup"><span data-stu-id="b4fb6-194">Boolean</span></span>|<span data-ttu-id="b4fb6-195">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-195">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b4fb6-196">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="b4fb6-196">emailBlockAddingAccounts</span></span>|<span data-ttu-id="b4fb6-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-197">Boolean</span></span>|<span data-ttu-id="b4fb6-198">Указывает, следует ли заблокировать пользовательские учетные записи электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-198">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="b4fb6-199">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="b4fb6-199">locationServicesBlocked</span></span>|<span data-ttu-id="b4fb6-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-200">Boolean</span></span>|<span data-ttu-id="b4fb6-201">Указывает, следует ли заблокировать службы определения местоположения.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-201">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="b4fb6-202">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="b4fb6-202">microsoftAccountBlocked</span></span>|<span data-ttu-id="b4fb6-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-203">Boolean</span></span>|<span data-ttu-id="b4fb6-204">Указывает, следует ли запретить использовать учетную запись Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-204">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="b4fb6-205">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="b4fb6-205">nfcBlocked</span></span>|<span data-ttu-id="b4fb6-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-206">Boolean</span></span>|<span data-ttu-id="b4fb6-207">Указывает, следует ли заблокировать NFC.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-207">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="b4fb6-208">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b4fb6-208">passwordBlockSimple</span></span>|<span data-ttu-id="b4fb6-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-209">Boolean</span></span>|<span data-ttu-id="b4fb6-210">Указывает, следует ли заблокировать синхронизацию календаря.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-210">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="b4fb6-211">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b4fb6-211">passwordExpirationDays</span></span>|<span data-ttu-id="b4fb6-212">Int32</span><span class="sxs-lookup"><span data-stu-id="b4fb6-212">Int32</span></span>|<span data-ttu-id="b4fb6-213">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-213">Number of days before the password expires.</span></span>|
|<span data-ttu-id="b4fb6-214">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b4fb6-214">passwordMinimumLength</span></span>|<span data-ttu-id="b4fb6-215">Int32</span><span class="sxs-lookup"><span data-stu-id="b4fb6-215">Int32</span></span>|<span data-ttu-id="b4fb6-216">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-216">Minimum length of passwords.</span></span>|
|<span data-ttu-id="b4fb6-217">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b4fb6-217">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b4fb6-218">Int32</span><span class="sxs-lookup"><span data-stu-id="b4fb6-218">Int32</span></span>|<span data-ttu-id="b4fb6-219">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="b4fb6-219">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="b4fb6-220">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b4fb6-220">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b4fb6-221">Int32</span><span class="sxs-lookup"><span data-stu-id="b4fb6-221">Int32</span></span>|<span data-ttu-id="b4fb6-222">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-222">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="b4fb6-223">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b4fb6-223">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b4fb6-224">Int32</span><span class="sxs-lookup"><span data-stu-id="b4fb6-224">Int32</span></span>|<span data-ttu-id="b4fb6-225">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-225">Number of previous passwords to block.</span></span> <span data-ttu-id="b4fb6-226">Допустимые значения: от 0 до 24</span><span class="sxs-lookup"><span data-stu-id="b4fb6-226">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b4fb6-227">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b4fb6-227">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b4fb6-228">Int32</span><span class="sxs-lookup"><span data-stu-id="b4fb6-228">Int32</span></span>|<span data-ttu-id="b4fb6-229">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-229">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="b4fb6-230">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b4fb6-230">passwordRequiredType</span></span>|[<span data-ttu-id="b4fb6-231">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b4fb6-231">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b4fb6-232">Необходимый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-232">Password type that is required.</span></span> <span data-ttu-id="b4fb6-233">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-233">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b4fb6-234">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b4fb6-234">passwordRequired</span></span>|<span data-ttu-id="b4fb6-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-235">Boolean</span></span>|<span data-ttu-id="b4fb6-236">Указывает, обязательно ли использовать пароль.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-236">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="b4fb6-237">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b4fb6-237">screenCaptureBlocked</span></span>|<span data-ttu-id="b4fb6-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-238">Boolean</span></span>|<span data-ttu-id="b4fb6-239">Указывает, следует ли запретить делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-239">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="b4fb6-240">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="b4fb6-240">storageBlockRemovableStorage</span></span>|<span data-ttu-id="b4fb6-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-241">Boolean</span></span>|<span data-ttu-id="b4fb6-242">Указывает, следует ли запретить использовать съемные носители.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-242">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="b4fb6-243">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="b4fb6-243">storageRequireEncryption</span></span>|<span data-ttu-id="b4fb6-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-244">Boolean</span></span>|<span data-ttu-id="b4fb6-245">Указывает, обязательно ли шифрование.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-245">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="b4fb6-246">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="b4fb6-246">webBrowserBlocked</span></span>|<span data-ttu-id="b4fb6-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-247">Boolean</span></span>|<span data-ttu-id="b4fb6-248">Указывает, следует ли заблокировать веб-браузер.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-248">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="b4fb6-249">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="b4fb6-249">wifiBlocked</span></span>|<span data-ttu-id="b4fb6-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-250">Boolean</span></span>|<span data-ttu-id="b4fb6-251">Указывает, следует ли заблокировать Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-251">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="b4fb6-252">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="b4fb6-252">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="b4fb6-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-253">Boolean</span></span>|<span data-ttu-id="b4fb6-254">Указывает, следует ли заблокировать автоматическое подключение к хот-спотам Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-254">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="b4fb6-255">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-255">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="b4fb6-256">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="b4fb6-256">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="b4fb6-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-257">Boolean</span></span>|<span data-ttu-id="b4fb6-258">Указывает, следует ли запретить устройству сообщать об обнаруженных хот-спотах Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-258">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="b4fb6-259">Ни на что не влияет, если Wi-Fi заблокирован.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-259">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="b4fb6-260">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b4fb6-260">windowsStoreBlocked</span></span>|<span data-ttu-id="b4fb6-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4fb6-261">Boolean</span></span>|<span data-ttu-id="b4fb6-262">Указывает, следует ли заблокировать Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-262">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="b4fb6-263">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4fb6-263">Response</span></span>
<span data-ttu-id="b4fb6-264">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-264">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4fb6-265">Пример</span><span class="sxs-lookup"><span data-stu-id="b4fb6-265">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4fb6-266">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4fb6-266">Request</span></span>
<span data-ttu-id="b4fb6-267">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4fb6-267">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1544

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="b4fb6-268">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4fb6-268">Response</span></span>
<span data-ttu-id="b4fb6-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="b4fb6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1725

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```





