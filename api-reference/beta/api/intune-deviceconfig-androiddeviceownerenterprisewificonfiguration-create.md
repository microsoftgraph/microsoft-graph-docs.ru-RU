---
title: Создание Андроиддевицеовнерентерприсевификонфигуратион
description: Создание нового объекта Андроиддевицеовнерентерприсевификонфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 185da4ca4e06485c642cd59ffa6d205f95c136c3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42759859"
---
# <a name="create-androiddeviceownerenterprisewificonfiguration"></a><span data-ttu-id="f03d6-103">Создание Андроиддевицеовнерентерприсевификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="f03d6-103">Create androidDeviceOwnerEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="f03d6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f03d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f03d6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f03d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f03d6-106">Создание нового объекта [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f03d6-106">Create a new [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f03d6-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f03d6-107">Prerequisites</span></span>
<span data-ttu-id="f03d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f03d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f03d6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f03d6-110">Permission type</span></span>|<span data-ttu-id="f03d6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f03d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f03d6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f03d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f03d6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f03d6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f03d6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f03d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f03d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f03d6-115">Not supported.</span></span>|
|<span data-ttu-id="f03d6-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="f03d6-116">Application</span></span>|<span data-ttu-id="f03d6-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f03d6-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f03d6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f03d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f03d6-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f03d6-119">Request headers</span></span>
|<span data-ttu-id="f03d6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f03d6-120">Header</span></span>|<span data-ttu-id="f03d6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f03d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f03d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f03d6-122">Authorization</span></span>|<span data-ttu-id="f03d6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f03d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f03d6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f03d6-124">Accept</span></span>|<span data-ttu-id="f03d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f03d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f03d6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f03d6-126">Request body</span></span>
<span data-ttu-id="f03d6-127">В тексте запроса добавьте представление объекта Андроиддевицеовнерентерприсевификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f03d6-127">In the request body, supply a JSON representation for the androidDeviceOwnerEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="f03d6-128">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнерентерприсевификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="f03d6-128">The following table shows the properties that are required when you create the androidDeviceOwnerEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="f03d6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f03d6-129">Property</span></span>|<span data-ttu-id="f03d6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f03d6-130">Type</span></span>|<span data-ttu-id="f03d6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f03d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f03d6-132">id</span><span class="sxs-lookup"><span data-stu-id="f03d6-132">id</span></span>|<span data-ttu-id="f03d6-133">String</span><span class="sxs-lookup"><span data-stu-id="f03d6-133">String</span></span>|<span data-ttu-id="f03d6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f03d6-134">Key of the entity.</span></span> <span data-ttu-id="f03d6-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f03d6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f03d6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f03d6-137">DateTimeOffset</span></span>|<span data-ttu-id="f03d6-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f03d6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f03d6-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f03d6-140">roleScopeTagIds</span></span>|<span data-ttu-id="f03d6-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f03d6-141">String collection</span></span>|<span data-ttu-id="f03d6-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f03d6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f03d6-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f03d6-144">supportsScopeTags</span></span>|<span data-ttu-id="f03d6-145">Логический</span><span class="sxs-lookup"><span data-stu-id="f03d6-145">Boolean</span></span>|<span data-ttu-id="f03d6-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f03d6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f03d6-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f03d6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f03d6-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f03d6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f03d6-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f03d6-149">This property is read-only.</span></span> <span data-ttu-id="f03d6-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f03d6-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f03d6-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f03d6-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f03d6-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f03d6-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f03d6-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f03d6-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f03d6-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f03d6-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f03d6-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f03d6-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f03d6-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f03d6-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f03d6-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f03d6-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f03d6-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f03d6-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f03d6-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f03d6-163">createdDateTime</span></span>|<span data-ttu-id="f03d6-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f03d6-164">DateTimeOffset</span></span>|<span data-ttu-id="f03d6-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f03d6-165">DateTime the object was created.</span></span> <span data-ttu-id="f03d6-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-167">description</span><span class="sxs-lookup"><span data-stu-id="f03d6-167">description</span></span>|<span data-ttu-id="f03d6-168">String</span><span class="sxs-lookup"><span data-stu-id="f03d6-168">String</span></span>|<span data-ttu-id="f03d6-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f03d6-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f03d6-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f03d6-171">displayName</span></span>|<span data-ttu-id="f03d6-172">Строка</span><span class="sxs-lookup"><span data-stu-id="f03d6-172">String</span></span>|<span data-ttu-id="f03d6-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f03d6-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f03d6-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-175">version</span><span class="sxs-lookup"><span data-stu-id="f03d6-175">version</span></span>|<span data-ttu-id="f03d6-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f03d6-176">Int32</span></span>|<span data-ttu-id="f03d6-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f03d6-177">Version of the device configuration.</span></span> <span data-ttu-id="f03d6-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="f03d6-179">networkName</span></span>|<span data-ttu-id="f03d6-180">String</span><span class="sxs-lookup"><span data-stu-id="f03d6-180">String</span></span>|<span data-ttu-id="f03d6-181">Сетевое имя, унаследованное от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03d6-181">Network Name Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-182">SSID</span><span class="sxs-lookup"><span data-stu-id="f03d6-182">ssid</span></span>|<span data-ttu-id="f03d6-183">String</span><span class="sxs-lookup"><span data-stu-id="f03d6-183">String</span></span>|<span data-ttu-id="f03d6-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="f03d6-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="f03d6-185">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03d6-185">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-186">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="f03d6-186">connectAutomatically</span></span>|<span data-ttu-id="f03d6-187">Логический</span><span class="sxs-lookup"><span data-stu-id="f03d6-187">Boolean</span></span>|<span data-ttu-id="f03d6-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="f03d6-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f03d6-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="f03d6-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="f03d6-190">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03d6-190">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-191">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="f03d6-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f03d6-192">Логический</span><span class="sxs-lookup"><span data-stu-id="f03d6-192">Boolean</span></span>|<span data-ttu-id="f03d6-193">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="f03d6-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="f03d6-194">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03d6-194">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-195">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="f03d6-195">wiFiSecurityType</span></span>|[<span data-ttu-id="f03d6-196">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f03d6-196">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="f03d6-197">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="f03d6-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f03d6-198">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f03d6-198">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span> <span data-ttu-id="f03d6-199">Возможные значения: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="f03d6-199">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="f03d6-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="f03d6-200">preSharedKey</span></span>|<span data-ttu-id="f03d6-201">String</span><span class="sxs-lookup"><span data-stu-id="f03d6-201">String</span></span>|<span data-ttu-id="f03d6-202">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="f03d6-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="f03d6-203">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03d6-203">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-204">прешаредкэйиссет</span><span class="sxs-lookup"><span data-stu-id="f03d6-204">preSharedKeyIsSet</span></span>|<span data-ttu-id="f03d6-205">Логический</span><span class="sxs-lookup"><span data-stu-id="f03d6-205">Boolean</span></span>|<span data-ttu-id="f03d6-206">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="f03d6-206">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="f03d6-207">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f03d6-207">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="f03d6-208">еаптипе</span><span class="sxs-lookup"><span data-stu-id="f03d6-208">eapType</span></span>|[<span data-ttu-id="f03d6-209">андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="f03d6-209">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="f03d6-210">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="f03d6-210">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="f03d6-211">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="f03d6-211">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="f03d6-212">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="f03d6-212">authenticationMethod</span></span>|[<span data-ttu-id="f03d6-213">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="f03d6-213">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="f03d6-214">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="f03d6-214">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="f03d6-215">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="f03d6-215">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="f03d6-216">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="f03d6-216">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="f03d6-217">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="f03d6-217">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="f03d6-218">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="f03d6-218">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="f03d6-219">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="f03d6-219">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="f03d6-220">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="f03d6-220">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="f03d6-221">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="f03d6-221">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="f03d6-222">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="f03d6-222">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="f03d6-223">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="f03d6-223">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="f03d6-224">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="f03d6-224">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="f03d6-225">String</span><span class="sxs-lookup"><span data-stu-id="f03d6-225">String</span></span>|<span data-ttu-id="f03d6-226">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="f03d6-226">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="f03d6-227">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f03d6-227">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="f03d6-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="f03d6-228">Response</span></span>
<span data-ttu-id="f03d6-229">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f03d6-229">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f03d6-230">Пример</span><span class="sxs-lookup"><span data-stu-id="f03d6-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="f03d6-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="f03d6-231">Request</span></span>
<span data-ttu-id="f03d6-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f03d6-232">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1612

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true,
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="f03d6-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="f03d6-233">Response</span></span>
<span data-ttu-id="f03d6-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f03d6-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1784

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration",
  "id": "7ef0d9c3-d9c3-7ef0-c3d9-f07ec3d9f07e",
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
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true,
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




