---
title: Создание iosEnterpriseWiFiConfiguration
description: Создание нового объекта iosEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 243fd70da27535d3a19d2e271d0346abeab13742
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442798"
---
# <a name="create-iosenterprisewificonfiguration"></a><span data-ttu-id="f865e-103">Создание iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="f865e-103">Create iosEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="f865e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f865e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f865e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f865e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f865e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f865e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f865e-107">Создание нового объекта [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f865e-107">Create a new [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f865e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f865e-108">Prerequisites</span></span>
<span data-ttu-id="f865e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f865e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f865e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f865e-111">Permission type</span></span>|<span data-ttu-id="f865e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f865e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f865e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f865e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f865e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f865e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f865e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f865e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f865e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f865e-116">Not supported.</span></span>|
|<span data-ttu-id="f865e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f865e-117">Application</span></span>|<span data-ttu-id="f865e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f865e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f865e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f865e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f865e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f865e-120">Request headers</span></span>
|<span data-ttu-id="f865e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f865e-121">Header</span></span>|<span data-ttu-id="f865e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f865e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f865e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f865e-123">Authorization</span></span>|<span data-ttu-id="f865e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f865e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f865e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f865e-125">Accept</span></span>|<span data-ttu-id="f865e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f865e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f865e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f865e-127">Request body</span></span>
<span data-ttu-id="f865e-128">В тексте запроса добавьте представление объекта iosEnterpriseWiFiConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f865e-128">In the request body, supply a JSON representation for the iosEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="f865e-129">В следующей таблице приведены свойства, необходимые при создании iosEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f865e-129">The following table shows the properties that are required when you create the iosEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="f865e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f865e-130">Property</span></span>|<span data-ttu-id="f865e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f865e-131">Type</span></span>|<span data-ttu-id="f865e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f865e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f865e-133">id</span><span class="sxs-lookup"><span data-stu-id="f865e-133">id</span></span>|<span data-ttu-id="f865e-134">String</span><span class="sxs-lookup"><span data-stu-id="f865e-134">String</span></span>|<span data-ttu-id="f865e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f865e-135">Key of the entity.</span></span> <span data-ttu-id="f865e-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f865e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f865e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f865e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f865e-138">DateTimeOffset</span></span>|<span data-ttu-id="f865e-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f865e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f865e-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f865e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f865e-141">roleScopeTagIds</span></span>|<span data-ttu-id="f865e-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f865e-142">String collection</span></span>|<span data-ttu-id="f865e-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f865e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f865e-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f865e-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f865e-145">supportsScopeTags</span></span>|<span data-ttu-id="f865e-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f865e-146">Boolean</span></span>|<span data-ttu-id="f865e-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f865e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f865e-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f865e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f865e-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f865e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f865e-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f865e-150">This property is read-only.</span></span> <span data-ttu-id="f865e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f865e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f865e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f865e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f865e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f865e-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f865e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f865e-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f865e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f865e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f865e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f865e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f865e-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f865e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f865e-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f865e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f865e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f865e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f865e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f865e-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f865e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f865e-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f865e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f865e-164">createdDateTime</span></span>|<span data-ttu-id="f865e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f865e-165">DateTimeOffset</span></span>|<span data-ttu-id="f865e-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f865e-166">DateTime the object was created.</span></span> <span data-ttu-id="f865e-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f865e-168">description</span><span class="sxs-lookup"><span data-stu-id="f865e-168">description</span></span>|<span data-ttu-id="f865e-169">String</span><span class="sxs-lookup"><span data-stu-id="f865e-169">String</span></span>|<span data-ttu-id="f865e-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f865e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f865e-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f865e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f865e-172">displayName</span></span>|<span data-ttu-id="f865e-173">Строка</span><span class="sxs-lookup"><span data-stu-id="f865e-173">String</span></span>|<span data-ttu-id="f865e-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f865e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f865e-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f865e-176">version</span><span class="sxs-lookup"><span data-stu-id="f865e-176">version</span></span>|<span data-ttu-id="f865e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f865e-177">Int32</span></span>|<span data-ttu-id="f865e-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f865e-178">Version of the device configuration.</span></span> <span data-ttu-id="f865e-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f865e-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="f865e-180">networkName</span></span>|<span data-ttu-id="f865e-181">String</span><span class="sxs-lookup"><span data-stu-id="f865e-181">String</span></span>|<span data-ttu-id="f865e-182">Сетевое имя, унаследованное от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f865e-182">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="f865e-183">SSID</span><span class="sxs-lookup"><span data-stu-id="f865e-183">ssid</span></span>|<span data-ttu-id="f865e-184">String</span><span class="sxs-lookup"><span data-stu-id="f865e-184">String</span></span>|<span data-ttu-id="f865e-185">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="f865e-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="f865e-186">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f865e-186">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="f865e-187">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="f865e-187">connectAutomatically</span></span>|<span data-ttu-id="f865e-188">Логический</span><span class="sxs-lookup"><span data-stu-id="f865e-188">Boolean</span></span>|<span data-ttu-id="f865e-189">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="f865e-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f865e-190">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="f865e-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="f865e-191">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f865e-191">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="f865e-192">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="f865e-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f865e-193">Логический</span><span class="sxs-lookup"><span data-stu-id="f865e-193">Boolean</span></span>|<span data-ttu-id="f865e-194">Подключаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="f865e-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="f865e-195">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="f865e-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="f865e-196">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f865e-196">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="f865e-197">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="f865e-197">wiFiSecurityType</span></span>|[<span data-ttu-id="f865e-198">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="f865e-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="f865e-199">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="f865e-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f865e-200">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-200">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="f865e-201">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="f865e-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="f865e-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="f865e-202">proxySettings</span></span>|[<span data-ttu-id="f865e-203">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="f865e-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="f865e-204">Тип прокси-сервера для этого подключения Wi-Fi наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f865e-204">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="f865e-205">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="f865e-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="f865e-206">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="f865e-206">proxyManualAddress</span></span>|<span data-ttu-id="f865e-207">String</span><span class="sxs-lookup"><span data-stu-id="f865e-207">String</span></span>|<span data-ttu-id="f865e-208">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="f865e-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="f865e-209">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f865e-209">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="f865e-210">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="f865e-210">proxyManualPort</span></span>|<span data-ttu-id="f865e-211">Int32</span><span class="sxs-lookup"><span data-stu-id="f865e-211">Int32</span></span>|<span data-ttu-id="f865e-212">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="f865e-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="f865e-213">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f865e-213">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="f865e-214">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="f865e-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="f865e-215">String</span><span class="sxs-lookup"><span data-stu-id="f865e-215">String</span></span>|<span data-ttu-id="f865e-216">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="f865e-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="f865e-217">Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="f865e-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="f865e-218">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f865e-218">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="f865e-219">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="f865e-219">preSharedKey</span></span>|<span data-ttu-id="f865e-220">String</span><span class="sxs-lookup"><span data-stu-id="f865e-220">String</span></span>|<span data-ttu-id="f865e-221">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="f865e-221">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="f865e-222">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f865e-222">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="f865e-223">еаптипе</span><span class="sxs-lookup"><span data-stu-id="f865e-223">eapType</span></span>|[<span data-ttu-id="f865e-224">еаптипе</span><span class="sxs-lookup"><span data-stu-id="f865e-224">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="f865e-225">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="f865e-225">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="f865e-226">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="f865e-226">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="f865e-227">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="f865e-227">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="f865e-228">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f865e-228">eapFastConfiguration</span></span>|[<span data-ttu-id="f865e-229">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f865e-229">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="f865e-230">Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="f865e-230">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="f865e-231">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="f865e-231">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="f865e-232">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="f865e-232">trustedServerCertificateNames</span></span>|<span data-ttu-id="f865e-233">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f865e-233">String collection</span></span>|<span data-ttu-id="f865e-234">Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="f865e-234">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="f865e-235">Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="f865e-235">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="f865e-236">Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f865e-236">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="f865e-237">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="f865e-237">authenticationMethod</span></span>|[<span data-ttu-id="f865e-238">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="f865e-238">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="f865e-239">Метод проверки подлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="f865e-239">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="f865e-240">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="f865e-240">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="f865e-241">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="f865e-241">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="f865e-242">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="f865e-242">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="f865e-243">Метод проверки подлинности, отличный от EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="f865e-243">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="f865e-244">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="f865e-244">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="f865e-245">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="f865e-245">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="f865e-246">String</span><span class="sxs-lookup"><span data-stu-id="f865e-246">String</span></span>|<span data-ttu-id="f865e-247">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="f865e-247">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="f865e-248">Это свойство маскирует имена пользователей с введенным текстом.</span><span class="sxs-lookup"><span data-stu-id="f865e-248">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="f865e-249">Например, если вы используете анонимный доступ, все пользователи, которые проходят проверку подлинности с помощью этого подключения Wi-Fi, с помощью действительного имени пользователя отображаются как anonymous.</span><span class="sxs-lookup"><span data-stu-id="f865e-249">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|
|<span data-ttu-id="f865e-250">усернамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="f865e-250">usernameFormatString</span></span>|<span data-ttu-id="f865e-251">String</span><span class="sxs-lookup"><span data-stu-id="f865e-251">String</span></span>|<span data-ttu-id="f865e-252">Строка формата имени пользователя, используемая для построения имени пользователя для подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="f865e-252">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="f865e-253">пассвордформатстринг</span><span class="sxs-lookup"><span data-stu-id="f865e-253">passwordFormatString</span></span>|<span data-ttu-id="f865e-254">String</span><span class="sxs-lookup"><span data-stu-id="f865e-254">String</span></span>|<span data-ttu-id="f865e-255">Строка формата пароля, используемая для создания пароля подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="f865e-255">Password format string used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="f865e-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="f865e-256">Response</span></span>
<span data-ttu-id="f865e-257">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f865e-257">If successful, this method returns a `201 Created` response code and a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f865e-258">Пример</span><span class="sxs-lookup"><span data-stu-id="f865e-258">Example</span></span>

### <a name="request"></a><span data-ttu-id="f865e-259">Запрос</span><span class="sxs-lookup"><span data-stu-id="f865e-259">Request</span></span>
<span data-ttu-id="f865e-260">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f865e-260">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1974

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

### <a name="response"></a><span data-ttu-id="f865e-261">Отклик</span><span class="sxs-lookup"><span data-stu-id="f865e-261">Response</span></span>
<span data-ttu-id="f865e-p128">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f865e-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2146

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





