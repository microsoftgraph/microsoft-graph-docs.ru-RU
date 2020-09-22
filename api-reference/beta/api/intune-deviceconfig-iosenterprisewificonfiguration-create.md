---
title: Создание iosEnterpriseWiFiConfiguration
description: Создание нового объекта iosEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7c29533de12e558c7b51ba2d973d9df0888fff88
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47995480"
---
# <a name="create-iosenterprisewificonfiguration"></a><span data-ttu-id="65f9f-103">Создание iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="65f9f-103">Create iosEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="65f9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65f9f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65f9f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65f9f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65f9f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65f9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65f9f-107">Создание нового объекта [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="65f9f-107">Create a new [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65f9f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="65f9f-108">Prerequisites</span></span>
<span data-ttu-id="65f9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65f9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65f9f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65f9f-111">Permission type</span></span>|<span data-ttu-id="65f9f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="65f9f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65f9f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65f9f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65f9f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65f9f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65f9f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65f9f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65f9f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65f9f-116">Not supported.</span></span>|
|<span data-ttu-id="65f9f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65f9f-117">Application</span></span>|<span data-ttu-id="65f9f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65f9f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65f9f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65f9f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="65f9f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="65f9f-120">Request headers</span></span>
|<span data-ttu-id="65f9f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65f9f-121">Header</span></span>|<span data-ttu-id="65f9f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="65f9f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65f9f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65f9f-123">Authorization</span></span>|<span data-ttu-id="65f9f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65f9f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65f9f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="65f9f-125">Accept</span></span>|<span data-ttu-id="65f9f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65f9f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65f9f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="65f9f-127">Request body</span></span>
<span data-ttu-id="65f9f-128">В тексте запроса добавьте представление объекта iosEnterpriseWiFiConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65f9f-128">In the request body, supply a JSON representation for the iosEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="65f9f-129">В следующей таблице приведены свойства, необходимые при создании iosEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="65f9f-129">The following table shows the properties that are required when you create the iosEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="65f9f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="65f9f-130">Property</span></span>|<span data-ttu-id="65f9f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="65f9f-131">Type</span></span>|<span data-ttu-id="65f9f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="65f9f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65f9f-133">id</span><span class="sxs-lookup"><span data-stu-id="65f9f-133">id</span></span>|<span data-ttu-id="65f9f-134">String</span><span class="sxs-lookup"><span data-stu-id="65f9f-134">String</span></span>|<span data-ttu-id="65f9f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="65f9f-135">Key of the entity.</span></span> <span data-ttu-id="65f9f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="65f9f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="65f9f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65f9f-138">DateTimeOffset</span></span>|<span data-ttu-id="65f9f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="65f9f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="65f9f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="65f9f-141">roleScopeTagIds</span></span>|<span data-ttu-id="65f9f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="65f9f-142">String collection</span></span>|<span data-ttu-id="65f9f-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="65f9f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="65f9f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="65f9f-145">supportsScopeTags</span></span>|<span data-ttu-id="65f9f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="65f9f-146">Boolean</span></span>|<span data-ttu-id="65f9f-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="65f9f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="65f9f-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="65f9f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="65f9f-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="65f9f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="65f9f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="65f9f-150">This property is read-only.</span></span> <span data-ttu-id="65f9f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="65f9f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="65f9f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="65f9f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="65f9f-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="65f9f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="65f9f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="65f9f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="65f9f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="65f9f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="65f9f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="65f9f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="65f9f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="65f9f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="65f9f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="65f9f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="65f9f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="65f9f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="65f9f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="65f9f-164">createdDateTime</span></span>|<span data-ttu-id="65f9f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="65f9f-165">DateTimeOffset</span></span>|<span data-ttu-id="65f9f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="65f9f-166">DateTime the object was created.</span></span> <span data-ttu-id="65f9f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-168">description</span><span class="sxs-lookup"><span data-stu-id="65f9f-168">description</span></span>|<span data-ttu-id="65f9f-169">String</span><span class="sxs-lookup"><span data-stu-id="65f9f-169">String</span></span>|<span data-ttu-id="65f9f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="65f9f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="65f9f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="65f9f-172">displayName</span></span>|<span data-ttu-id="65f9f-173">String</span><span class="sxs-lookup"><span data-stu-id="65f9f-173">String</span></span>|<span data-ttu-id="65f9f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="65f9f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="65f9f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-176">version</span><span class="sxs-lookup"><span data-stu-id="65f9f-176">version</span></span>|<span data-ttu-id="65f9f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="65f9f-177">Int32</span></span>|<span data-ttu-id="65f9f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="65f9f-178">Version of the device configuration.</span></span> <span data-ttu-id="65f9f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="65f9f-180">networkName</span></span>|<span data-ttu-id="65f9f-181">String</span><span class="sxs-lookup"><span data-stu-id="65f9f-181">String</span></span>|<span data-ttu-id="65f9f-182">Сетевое имя, унаследованное от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f9f-182">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-183">SSID</span><span class="sxs-lookup"><span data-stu-id="65f9f-183">ssid</span></span>|<span data-ttu-id="65f9f-184">String</span><span class="sxs-lookup"><span data-stu-id="65f9f-184">String</span></span>|<span data-ttu-id="65f9f-185">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="65f9f-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="65f9f-186">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f9f-186">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-187">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="65f9f-187">connectAutomatically</span></span>|<span data-ttu-id="65f9f-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="65f9f-188">Boolean</span></span>|<span data-ttu-id="65f9f-189">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="65f9f-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="65f9f-190">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="65f9f-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="65f9f-191">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f9f-191">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-192">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="65f9f-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="65f9f-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="65f9f-193">Boolean</span></span>|<span data-ttu-id="65f9f-194">Подключаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="65f9f-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="65f9f-195">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="65f9f-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="65f9f-196">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f9f-196">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-197">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="65f9f-197">wiFiSecurityType</span></span>|[<span data-ttu-id="65f9f-198">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="65f9f-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="65f9f-199">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="65f9f-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="65f9f-200">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-200">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="65f9f-201">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="65f9f-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="65f9f-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="65f9f-202">proxySettings</span></span>|[<span data-ttu-id="65f9f-203">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="65f9f-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="65f9f-204">Тип прокси-сервера для этого подключения Wi-Fi наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="65f9f-204">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="65f9f-205">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="65f9f-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="65f9f-206">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="65f9f-206">proxyManualAddress</span></span>|<span data-ttu-id="65f9f-207">String</span><span class="sxs-lookup"><span data-stu-id="65f9f-207">String</span></span>|<span data-ttu-id="65f9f-208">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="65f9f-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="65f9f-209">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f9f-209">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-210">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="65f9f-210">proxyManualPort</span></span>|<span data-ttu-id="65f9f-211">Int32</span><span class="sxs-lookup"><span data-stu-id="65f9f-211">Int32</span></span>|<span data-ttu-id="65f9f-212">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="65f9f-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="65f9f-213">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f9f-213">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-214">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="65f9f-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="65f9f-215">String</span><span class="sxs-lookup"><span data-stu-id="65f9f-215">String</span></span>|<span data-ttu-id="65f9f-216">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="65f9f-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="65f9f-217">Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="65f9f-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="65f9f-218">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f9f-218">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-219">дисаблемакаддрессрандомизатион</span><span class="sxs-lookup"><span data-stu-id="65f9f-219">disableMacAddressRandomization</span></span>|<span data-ttu-id="65f9f-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="65f9f-220">Boolean</span></span>|<span data-ttu-id="65f9f-221">Если задано значение true, устройства, подключающиеся с помощью этого профиля Wi-Fi, предоставляют свой фактический MAC-адрес Wi-Fi вместо случайного MAC-адреса.</span><span class="sxs-lookup"><span data-stu-id="65f9f-221">If set to true, forces devices connecting using this Wi-Fi profile to present their actual Wi-Fi MAC address instead of a random MAC address.</span></span> <span data-ttu-id="65f9f-222">Применяется к iOS 14 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="65f9f-222">Applies to iOS 14 and later.</span></span> <span data-ttu-id="65f9f-223">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f9f-223">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-224">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="65f9f-224">preSharedKey</span></span>|<span data-ttu-id="65f9f-225">String</span><span class="sxs-lookup"><span data-stu-id="65f9f-225">String</span></span>|<span data-ttu-id="65f9f-226">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="65f9f-226">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="65f9f-227">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="65f9f-227">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="65f9f-228">еаптипе</span><span class="sxs-lookup"><span data-stu-id="65f9f-228">eapType</span></span>|[<span data-ttu-id="65f9f-229">еаптипе</span><span class="sxs-lookup"><span data-stu-id="65f9f-229">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="65f9f-230">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="65f9f-230">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="65f9f-231">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="65f9f-231">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="65f9f-232">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="65f9f-232">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="65f9f-233">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="65f9f-233">eapFastConfiguration</span></span>|[<span data-ttu-id="65f9f-234">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="65f9f-234">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="65f9f-235">Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="65f9f-235">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="65f9f-236">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="65f9f-236">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="65f9f-237">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="65f9f-237">trustedServerCertificateNames</span></span>|<span data-ttu-id="65f9f-238">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="65f9f-238">String collection</span></span>|<span data-ttu-id="65f9f-239">Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="65f9f-239">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="65f9f-240">Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="65f9f-240">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="65f9f-241">Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="65f9f-241">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="65f9f-242">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="65f9f-242">authenticationMethod</span></span>|[<span data-ttu-id="65f9f-243">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="65f9f-243">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="65f9f-244">Метод проверки подлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="65f9f-244">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="65f9f-245">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="65f9f-245">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="65f9f-246">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="65f9f-246">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="65f9f-247">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="65f9f-247">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="65f9f-248">Метод проверки подлинности, отличный от EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="65f9f-248">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="65f9f-249">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="65f9f-249">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="65f9f-250">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="65f9f-250">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="65f9f-251">String</span><span class="sxs-lookup"><span data-stu-id="65f9f-251">String</span></span>|<span data-ttu-id="65f9f-252">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="65f9f-252">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="65f9f-253">Это свойство маскирует имена пользователей с введенным текстом.</span><span class="sxs-lookup"><span data-stu-id="65f9f-253">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="65f9f-254">Например, если вы используете анонимный доступ, все пользователи, которые проходят проверку подлинности с помощью этого подключения Wi-Fi, с помощью действительного имени пользователя отображаются как anonymous.</span><span class="sxs-lookup"><span data-stu-id="65f9f-254">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|
|<span data-ttu-id="65f9f-255">усернамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="65f9f-255">usernameFormatString</span></span>|<span data-ttu-id="65f9f-256">String</span><span class="sxs-lookup"><span data-stu-id="65f9f-256">String</span></span>|<span data-ttu-id="65f9f-257">Строка формата имени пользователя, используемая для построения имени пользователя для подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="65f9f-257">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="65f9f-258">пассвордформатстринг</span><span class="sxs-lookup"><span data-stu-id="65f9f-258">passwordFormatString</span></span>|<span data-ttu-id="65f9f-259">String</span><span class="sxs-lookup"><span data-stu-id="65f9f-259">String</span></span>|<span data-ttu-id="65f9f-260">Строка формата пароля, используемая для создания пароля подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="65f9f-260">Password format string used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="65f9f-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="65f9f-261">Response</span></span>
<span data-ttu-id="65f9f-262">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65f9f-262">If successful, this method returns a `201 Created` response code and a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65f9f-263">Пример</span><span class="sxs-lookup"><span data-stu-id="65f9f-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="65f9f-264">Запрос</span><span class="sxs-lookup"><span data-stu-id="65f9f-264">Request</span></span>
<span data-ttu-id="65f9f-265">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65f9f-265">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2017

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
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
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "disableMacAddressRandomization": true,
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```

### <a name="response"></a><span data-ttu-id="65f9f-266">Отклик</span><span class="sxs-lookup"><span data-stu-id="65f9f-266">Response</span></span>
<span data-ttu-id="65f9f-p129">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65f9f-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2189

{
  "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
  "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
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
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "disableMacAddressRandomization": true,
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "usernameFormatString": "Username Format String value",
  "passwordFormatString": "Password Format String value"
}
```






