---
title: Обновление iosWiFiConfiguration
description: Обновление свойств объекта iosWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9d0a2fd1a5a73a942ea3cef382a36275fed10684
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438409"
---
# <a name="update-ioswificonfiguration"></a><span data-ttu-id="babde-103">Обновление iosWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="babde-103">Update iosWiFiConfiguration</span></span>

<span data-ttu-id="babde-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="babde-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="babde-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="babde-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="babde-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="babde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="babde-107">Обновление свойств объекта [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="babde-107">Update the properties of a [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="babde-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="babde-108">Prerequisites</span></span>
<span data-ttu-id="babde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="babde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="babde-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="babde-111">Permission type</span></span>|<span data-ttu-id="babde-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="babde-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="babde-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="babde-113">Delegated (work or school account)</span></span>|<span data-ttu-id="babde-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="babde-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="babde-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="babde-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="babde-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="babde-116">Not supported.</span></span>|
|<span data-ttu-id="babde-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="babde-117">Application</span></span>|<span data-ttu-id="babde-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="babde-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="babde-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="babde-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="babde-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="babde-120">Request headers</span></span>
|<span data-ttu-id="babde-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="babde-121">Header</span></span>|<span data-ttu-id="babde-122">Значение</span><span class="sxs-lookup"><span data-stu-id="babde-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="babde-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="babde-123">Authorization</span></span>|<span data-ttu-id="babde-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="babde-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="babde-125">Accept</span><span class="sxs-lookup"><span data-stu-id="babde-125">Accept</span></span>|<span data-ttu-id="babde-126">application/json</span><span class="sxs-lookup"><span data-stu-id="babde-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="babde-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="babde-127">Request body</span></span>
<span data-ttu-id="babde-128">В тексте запроса добавьте представление объекта [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="babde-128">In the request body, supply a JSON representation for the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

<span data-ttu-id="babde-129">В следующей таблице приведены свойства, необходимые при создании [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="babde-129">The following table shows the properties that are required when you create the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span>

|<span data-ttu-id="babde-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="babde-130">Property</span></span>|<span data-ttu-id="babde-131">Тип</span><span class="sxs-lookup"><span data-stu-id="babde-131">Type</span></span>|<span data-ttu-id="babde-132">Описание</span><span class="sxs-lookup"><span data-stu-id="babde-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="babde-133">id</span><span class="sxs-lookup"><span data-stu-id="babde-133">id</span></span>|<span data-ttu-id="babde-134">String</span><span class="sxs-lookup"><span data-stu-id="babde-134">String</span></span>|<span data-ttu-id="babde-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="babde-135">Key of the entity.</span></span> <span data-ttu-id="babde-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="babde-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="babde-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="babde-137">lastModifiedDateTime</span></span>|<span data-ttu-id="babde-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="babde-138">DateTimeOffset</span></span>|<span data-ttu-id="babde-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="babde-139">DateTime the object was last modified.</span></span> <span data-ttu-id="babde-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="babde-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="babde-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="babde-141">roleScopeTagIds</span></span>|<span data-ttu-id="babde-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="babde-142">String collection</span></span>|<span data-ttu-id="babde-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="babde-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="babde-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="babde-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="babde-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="babde-145">supportsScopeTags</span></span>|<span data-ttu-id="babde-146">Логическое</span><span class="sxs-lookup"><span data-stu-id="babde-146">Boolean</span></span>|<span data-ttu-id="babde-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="babde-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="babde-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="babde-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="babde-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="babde-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="babde-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="babde-150">This property is read-only.</span></span> <span data-ttu-id="babde-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="babde-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="babde-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="babde-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="babde-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="babde-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="babde-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="babde-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="babde-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="babde-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="babde-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="babde-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="babde-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="babde-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="babde-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="babde-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="babde-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="babde-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="babde-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="babde-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="babde-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="babde-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="babde-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="babde-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="babde-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="babde-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="babde-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="babde-164">createdDateTime</span></span>|<span data-ttu-id="babde-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="babde-165">DateTimeOffset</span></span>|<span data-ttu-id="babde-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="babde-166">DateTime the object was created.</span></span> <span data-ttu-id="babde-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="babde-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="babde-168">description</span><span class="sxs-lookup"><span data-stu-id="babde-168">description</span></span>|<span data-ttu-id="babde-169">String</span><span class="sxs-lookup"><span data-stu-id="babde-169">String</span></span>|<span data-ttu-id="babde-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="babde-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="babde-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="babde-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="babde-172">displayName</span><span class="sxs-lookup"><span data-stu-id="babde-172">displayName</span></span>|<span data-ttu-id="babde-173">Строка</span><span class="sxs-lookup"><span data-stu-id="babde-173">String</span></span>|<span data-ttu-id="babde-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="babde-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="babde-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="babde-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="babde-176">version</span><span class="sxs-lookup"><span data-stu-id="babde-176">version</span></span>|<span data-ttu-id="babde-177">Int32</span><span class="sxs-lookup"><span data-stu-id="babde-177">Int32</span></span>|<span data-ttu-id="babde-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="babde-178">Version of the device configuration.</span></span> <span data-ttu-id="babde-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="babde-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="babde-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="babde-180">networkName</span></span>|<span data-ttu-id="babde-181">String</span><span class="sxs-lookup"><span data-stu-id="babde-181">String</span></span>|<span data-ttu-id="babde-182">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="babde-182">Network Name</span></span>|
|<span data-ttu-id="babde-183">SSID</span><span class="sxs-lookup"><span data-stu-id="babde-183">ssid</span></span>|<span data-ttu-id="babde-184">String</span><span class="sxs-lookup"><span data-stu-id="babde-184">String</span></span>|<span data-ttu-id="babde-185">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="babde-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="babde-186">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="babde-186">connectAutomatically</span></span>|<span data-ttu-id="babde-187">Логическое</span><span class="sxs-lookup"><span data-stu-id="babde-187">Boolean</span></span>|<span data-ttu-id="babde-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="babde-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="babde-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="babde-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="babde-190">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="babde-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="babde-191">Логическое</span><span class="sxs-lookup"><span data-stu-id="babde-191">Boolean</span></span>|<span data-ttu-id="babde-192">Подключаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="babde-192">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="babde-193">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="babde-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="babde-194">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="babde-194">wiFiSecurityType</span></span>|[<span data-ttu-id="babde-195">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="babde-195">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="babde-196">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="babde-196">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="babde-197">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="babde-197">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="babde-198">proxySettings</span><span class="sxs-lookup"><span data-stu-id="babde-198">proxySettings</span></span>|[<span data-ttu-id="babde-199">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="babde-199">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="babde-200">Тип прокси-сервера для этого подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="babde-200">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="babde-201">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="babde-201">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="babde-202">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="babde-202">proxyManualAddress</span></span>|<span data-ttu-id="babde-203">String</span><span class="sxs-lookup"><span data-stu-id="babde-203">String</span></span>|<span data-ttu-id="babde-204">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="babde-204">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="babde-205">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="babde-205">proxyManualPort</span></span>|<span data-ttu-id="babde-206">Int32</span><span class="sxs-lookup"><span data-stu-id="babde-206">Int32</span></span>|<span data-ttu-id="babde-207">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="babde-207">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="babde-208">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="babde-208">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="babde-209">String</span><span class="sxs-lookup"><span data-stu-id="babde-209">String</span></span>|<span data-ttu-id="babde-210">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="babde-210">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="babde-211">Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="babde-211">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="babde-212">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="babde-212">preSharedKey</span></span>|<span data-ttu-id="babde-213">String</span><span class="sxs-lookup"><span data-stu-id="babde-213">String</span></span>|<span data-ttu-id="babde-214">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="babde-214">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="babde-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="babde-215">Response</span></span>
<span data-ttu-id="babde-216">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="babde-216">If successful, this method returns a `200 OK` response code and an updated [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="babde-217">Пример</span><span class="sxs-lookup"><span data-stu-id="babde-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="babde-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="babde-218">Request</span></span>
<span data-ttu-id="babde-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="babde-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1448

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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
  "preSharedKey": "Pre Shared Key value"
}
```

### <a name="response"></a><span data-ttu-id="babde-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="babde-220">Response</span></span>
<span data-ttu-id="babde-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="babde-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1620

{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
  "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
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
  "preSharedKey": "Pre Shared Key value"
}
```



