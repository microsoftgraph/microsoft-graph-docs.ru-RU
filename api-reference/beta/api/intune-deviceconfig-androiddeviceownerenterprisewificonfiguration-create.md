---
title: Создание Андроиддевицеовнерентерприсевификонфигуратион
description: Создание нового объекта Андроиддевицеовнерентерприсевификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b73cd0fd571b071d0033fd095245acb57fa2287b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444198"
---
# <a name="create-androiddeviceownerenterprisewificonfiguration"></a><span data-ttu-id="54a53-103">Создание Андроиддевицеовнерентерприсевификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="54a53-103">Create androidDeviceOwnerEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="54a53-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="54a53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54a53-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54a53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54a53-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54a53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54a53-107">Создание нового объекта [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="54a53-107">Create a new [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54a53-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="54a53-108">Prerequisites</span></span>
<span data-ttu-id="54a53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54a53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54a53-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54a53-111">Permission type</span></span>|<span data-ttu-id="54a53-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54a53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54a53-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54a53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54a53-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54a53-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="54a53-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54a53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54a53-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54a53-116">Not supported.</span></span>|
|<span data-ttu-id="54a53-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54a53-117">Application</span></span>|<span data-ttu-id="54a53-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54a53-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54a53-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54a53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="54a53-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="54a53-120">Request headers</span></span>
|<span data-ttu-id="54a53-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54a53-121">Header</span></span>|<span data-ttu-id="54a53-122">Значение</span><span class="sxs-lookup"><span data-stu-id="54a53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54a53-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="54a53-123">Authorization</span></span>|<span data-ttu-id="54a53-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54a53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54a53-125">Accept</span><span class="sxs-lookup"><span data-stu-id="54a53-125">Accept</span></span>|<span data-ttu-id="54a53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54a53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54a53-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54a53-127">Request body</span></span>
<span data-ttu-id="54a53-128">В тексте запроса добавьте представление объекта Андроиддевицеовнерентерприсевификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54a53-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="54a53-129">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнерентерприсевификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="54a53-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="54a53-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="54a53-130">Property</span></span>|<span data-ttu-id="54a53-131">Тип</span><span class="sxs-lookup"><span data-stu-id="54a53-131">Type</span></span>|<span data-ttu-id="54a53-132">Описание</span><span class="sxs-lookup"><span data-stu-id="54a53-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54a53-133">id</span><span class="sxs-lookup"><span data-stu-id="54a53-133">id</span></span>|<span data-ttu-id="54a53-134">String</span><span class="sxs-lookup"><span data-stu-id="54a53-134">String</span></span>|<span data-ttu-id="54a53-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="54a53-135">Key of the entity.</span></span> <span data-ttu-id="54a53-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54a53-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54a53-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54a53-137">lastModifiedDateTime</span></span>|<span data-ttu-id="54a53-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54a53-138">DateTimeOffset</span></span>|<span data-ttu-id="54a53-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="54a53-139">DateTime the object was last modified.</span></span> <span data-ttu-id="54a53-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54a53-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54a53-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="54a53-141">roleScopeTagIds</span></span>|<span data-ttu-id="54a53-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="54a53-142">String collection</span></span>|<span data-ttu-id="54a53-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="54a53-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="54a53-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54a53-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54a53-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="54a53-145">supportsScopeTags</span></span>|<span data-ttu-id="54a53-146">Логический</span><span class="sxs-lookup"><span data-stu-id="54a53-146">Boolean</span></span>|<span data-ttu-id="54a53-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="54a53-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="54a53-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="54a53-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="54a53-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="54a53-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="54a53-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="54a53-150">This property is read-only.</span></span> <span data-ttu-id="54a53-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54a53-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54a53-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="54a53-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="54a53-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="54a53-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="54a53-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="54a53-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="54a53-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54a53-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54a53-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="54a53-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="54a53-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="54a53-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="54a53-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="54a53-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="54a53-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54a53-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54a53-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="54a53-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="54a53-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="54a53-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="54a53-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="54a53-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="54a53-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54a53-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54a53-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54a53-164">createdDateTime</span></span>|<span data-ttu-id="54a53-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54a53-165">DateTimeOffset</span></span>|<span data-ttu-id="54a53-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="54a53-166">DateTime the object was created.</span></span> <span data-ttu-id="54a53-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54a53-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54a53-168">description</span><span class="sxs-lookup"><span data-stu-id="54a53-168">description</span></span>|<span data-ttu-id="54a53-169">String</span><span class="sxs-lookup"><span data-stu-id="54a53-169">String</span></span>|<span data-ttu-id="54a53-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54a53-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="54a53-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54a53-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54a53-172">displayName</span><span class="sxs-lookup"><span data-stu-id="54a53-172">displayName</span></span>|<span data-ttu-id="54a53-173">Строка</span><span class="sxs-lookup"><span data-stu-id="54a53-173">String</span></span>|<span data-ttu-id="54a53-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54a53-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="54a53-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54a53-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54a53-176">version</span><span class="sxs-lookup"><span data-stu-id="54a53-176">version</span></span>|<span data-ttu-id="54a53-177">Int32</span><span class="sxs-lookup"><span data-stu-id="54a53-177">Int32</span></span>|<span data-ttu-id="54a53-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="54a53-178">Version of the device configuration.</span></span> <span data-ttu-id="54a53-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54a53-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="54a53-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="54a53-180">networkName</span></span>|<span data-ttu-id="54a53-181">String</span><span class="sxs-lookup"><span data-stu-id="54a53-181">String</span></span>|<span data-ttu-id="54a53-182">Сетевое имя, унаследованное от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54a53-182">Network Name Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="54a53-183">SSID</span><span class="sxs-lookup"><span data-stu-id="54a53-183">ssid</span></span>|<span data-ttu-id="54a53-184">String</span><span class="sxs-lookup"><span data-stu-id="54a53-184">String</span></span>|<span data-ttu-id="54a53-185">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="54a53-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="54a53-186">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54a53-186">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="54a53-187">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="54a53-187">connectAutomatically</span></span>|<span data-ttu-id="54a53-188">Логический</span><span class="sxs-lookup"><span data-stu-id="54a53-188">Boolean</span></span>|<span data-ttu-id="54a53-189">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="54a53-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="54a53-190">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="54a53-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="54a53-191">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54a53-191">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="54a53-192">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="54a53-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="54a53-193">Логический</span><span class="sxs-lookup"><span data-stu-id="54a53-193">Boolean</span></span>|<span data-ttu-id="54a53-194">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="54a53-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="54a53-195">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54a53-195">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="54a53-196">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="54a53-196">wiFiSecurityType</span></span>|[<span data-ttu-id="54a53-197">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="54a53-197">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="54a53-198">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="54a53-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="54a53-199">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="54a53-199">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span> <span data-ttu-id="54a53-200">Возможные значения: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="54a53-200">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="54a53-201">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="54a53-201">preSharedKey</span></span>|<span data-ttu-id="54a53-202">String</span><span class="sxs-lookup"><span data-stu-id="54a53-202">String</span></span>|<span data-ttu-id="54a53-203">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="54a53-203">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="54a53-204">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54a53-204">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="54a53-205">прешаредкэйиссет</span><span class="sxs-lookup"><span data-stu-id="54a53-205">preSharedKeyIsSet</span></span>|<span data-ttu-id="54a53-206">Логический</span><span class="sxs-lookup"><span data-stu-id="54a53-206">Boolean</span></span>|<span data-ttu-id="54a53-207">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="54a53-207">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="54a53-208">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="54a53-208">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="54a53-209">еаптипе</span><span class="sxs-lookup"><span data-stu-id="54a53-209">eapType</span></span>|[<span data-ttu-id="54a53-210">андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="54a53-210">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="54a53-211">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="54a53-211">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="54a53-212">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="54a53-212">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="54a53-213">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="54a53-213">authenticationMethod</span></span>|[<span data-ttu-id="54a53-214">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="54a53-214">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="54a53-215">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="54a53-215">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="54a53-216">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="54a53-216">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="54a53-217">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="54a53-217">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="54a53-218">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="54a53-218">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="54a53-219">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="54a53-219">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="54a53-220">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="54a53-220">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="54a53-221">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="54a53-221">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="54a53-222">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="54a53-222">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="54a53-223">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="54a53-223">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="54a53-224">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="54a53-224">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="54a53-225">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="54a53-225">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="54a53-226">String</span><span class="sxs-lookup"><span data-stu-id="54a53-226">String</span></span>|<span data-ttu-id="54a53-227">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="54a53-227">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="54a53-228">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="54a53-228">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="54a53-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="54a53-229">Response</span></span>
<span data-ttu-id="54a53-230">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="54a53-230">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54a53-231">Пример</span><span class="sxs-lookup"><span data-stu-id="54a53-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="54a53-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="54a53-232">Request</span></span>
<span data-ttu-id="54a53-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54a53-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="54a53-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="54a53-234">Response</span></span>
<span data-ttu-id="54a53-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54a53-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





