---
title: Создание Макосвификонфигуратион
description: Создание нового объекта Макосвификонфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0bd592f91f25637493e295919cc0bf477518bf5d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432235"
---
# <a name="create-macoswificonfiguration"></a><span data-ttu-id="fdc98-103">Создание Макосвификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="fdc98-103">Create macOSWiFiConfiguration</span></span>

<span data-ttu-id="fdc98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fdc98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdc98-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdc98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdc98-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdc98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdc98-107">Создание нового объекта [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="fdc98-107">Create a new [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdc98-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fdc98-108">Prerequisites</span></span>
<span data-ttu-id="fdc98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdc98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdc98-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdc98-111">Permission type</span></span>|<span data-ttu-id="fdc98-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdc98-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdc98-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdc98-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdc98-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdc98-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fdc98-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdc98-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdc98-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdc98-116">Not supported.</span></span>|
|<span data-ttu-id="fdc98-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdc98-117">Application</span></span>|<span data-ttu-id="fdc98-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdc98-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdc98-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdc98-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fdc98-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fdc98-120">Request headers</span></span>
|<span data-ttu-id="fdc98-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdc98-121">Header</span></span>|<span data-ttu-id="fdc98-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fdc98-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdc98-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fdc98-123">Authorization</span></span>|<span data-ttu-id="fdc98-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdc98-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdc98-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fdc98-125">Accept</span></span>|<span data-ttu-id="fdc98-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdc98-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdc98-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fdc98-127">Request body</span></span>
<span data-ttu-id="fdc98-128">В тексте запроса добавьте представление объекта Макосвификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdc98-128">In the request body, supply a JSON representation for the macOSWiFiConfiguration object.</span></span>

<span data-ttu-id="fdc98-129">В следующей таблице приведены свойства, необходимые при создании Макосвификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="fdc98-129">The following table shows the properties that are required when you create the macOSWiFiConfiguration.</span></span>

|<span data-ttu-id="fdc98-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdc98-130">Property</span></span>|<span data-ttu-id="fdc98-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fdc98-131">Type</span></span>|<span data-ttu-id="fdc98-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fdc98-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdc98-133">id</span><span class="sxs-lookup"><span data-stu-id="fdc98-133">id</span></span>|<span data-ttu-id="fdc98-134">String</span><span class="sxs-lookup"><span data-stu-id="fdc98-134">String</span></span>|<span data-ttu-id="fdc98-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fdc98-135">Key of the entity.</span></span> <span data-ttu-id="fdc98-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdc98-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdc98-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fdc98-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fdc98-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdc98-138">DateTimeOffset</span></span>|<span data-ttu-id="fdc98-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fdc98-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fdc98-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdc98-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdc98-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fdc98-141">roleScopeTagIds</span></span>|<span data-ttu-id="fdc98-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="fdc98-142">String collection</span></span>|<span data-ttu-id="fdc98-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fdc98-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fdc98-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdc98-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdc98-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="fdc98-145">supportsScopeTags</span></span>|<span data-ttu-id="fdc98-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc98-146">Boolean</span></span>|<span data-ttu-id="fdc98-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="fdc98-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fdc98-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="fdc98-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fdc98-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fdc98-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fdc98-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fdc98-150">This property is read-only.</span></span> <span data-ttu-id="fdc98-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdc98-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdc98-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fdc98-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fdc98-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fdc98-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fdc98-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fdc98-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fdc98-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdc98-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdc98-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fdc98-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fdc98-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fdc98-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fdc98-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fdc98-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fdc98-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdc98-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdc98-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fdc98-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fdc98-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fdc98-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fdc98-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fdc98-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fdc98-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdc98-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdc98-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fdc98-164">createdDateTime</span></span>|<span data-ttu-id="fdc98-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdc98-165">DateTimeOffset</span></span>|<span data-ttu-id="fdc98-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fdc98-166">DateTime the object was created.</span></span> <span data-ttu-id="fdc98-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdc98-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdc98-168">description</span><span class="sxs-lookup"><span data-stu-id="fdc98-168">description</span></span>|<span data-ttu-id="fdc98-169">String</span><span class="sxs-lookup"><span data-stu-id="fdc98-169">String</span></span>|<span data-ttu-id="fdc98-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fdc98-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fdc98-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdc98-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdc98-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fdc98-172">displayName</span></span>|<span data-ttu-id="fdc98-173">Строка</span><span class="sxs-lookup"><span data-stu-id="fdc98-173">String</span></span>|<span data-ttu-id="fdc98-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fdc98-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fdc98-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdc98-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdc98-176">version</span><span class="sxs-lookup"><span data-stu-id="fdc98-176">version</span></span>|<span data-ttu-id="fdc98-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fdc98-177">Int32</span></span>|<span data-ttu-id="fdc98-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fdc98-178">Version of the device configuration.</span></span> <span data-ttu-id="fdc98-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fdc98-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fdc98-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="fdc98-180">networkName</span></span>|<span data-ttu-id="fdc98-181">String</span><span class="sxs-lookup"><span data-stu-id="fdc98-181">String</span></span>|<span data-ttu-id="fdc98-182">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="fdc98-182">Network Name</span></span>|
|<span data-ttu-id="fdc98-183">SSID</span><span class="sxs-lookup"><span data-stu-id="fdc98-183">ssid</span></span>|<span data-ttu-id="fdc98-184">String</span><span class="sxs-lookup"><span data-stu-id="fdc98-184">String</span></span>|<span data-ttu-id="fdc98-185">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="fdc98-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="fdc98-186">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="fdc98-186">connectAutomatically</span></span>|<span data-ttu-id="fdc98-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc98-187">Boolean</span></span>|<span data-ttu-id="fdc98-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="fdc98-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="fdc98-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="fdc98-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="fdc98-190">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="fdc98-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="fdc98-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc98-191">Boolean</span></span>|<span data-ttu-id="fdc98-192">Подключаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="fdc98-192">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="fdc98-193">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="fdc98-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="fdc98-194">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="fdc98-194">wiFiSecurityType</span></span>|[<span data-ttu-id="fdc98-195">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="fdc98-195">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="fdc98-196">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="fdc98-196">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="fdc98-197">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="fdc98-197">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="fdc98-198">proxySettings</span><span class="sxs-lookup"><span data-stu-id="fdc98-198">proxySettings</span></span>|[<span data-ttu-id="fdc98-199">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="fdc98-199">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="fdc98-200">Тип прокси-сервера для этого подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="fdc98-200">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="fdc98-201">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="fdc98-201">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="fdc98-202">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="fdc98-202">proxyManualAddress</span></span>|<span data-ttu-id="fdc98-203">String</span><span class="sxs-lookup"><span data-stu-id="fdc98-203">String</span></span>|<span data-ttu-id="fdc98-204">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="fdc98-204">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="fdc98-205">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="fdc98-205">proxyManualPort</span></span>|<span data-ttu-id="fdc98-206">Int32</span><span class="sxs-lookup"><span data-stu-id="fdc98-206">Int32</span></span>|<span data-ttu-id="fdc98-207">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="fdc98-207">Port of the proxy server when manual configuration is selected.</span></span>|
|<span data-ttu-id="fdc98-208">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="fdc98-208">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="fdc98-209">String</span><span class="sxs-lookup"><span data-stu-id="fdc98-209">String</span></span>|<span data-ttu-id="fdc98-210">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="fdc98-210">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="fdc98-211">Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="fdc98-211">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|
|<span data-ttu-id="fdc98-212">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="fdc98-212">preSharedKey</span></span>|<span data-ttu-id="fdc98-213">String</span><span class="sxs-lookup"><span data-stu-id="fdc98-213">String</span></span>|<span data-ttu-id="fdc98-214">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="fdc98-214">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="fdc98-215">Ответ</span><span class="sxs-lookup"><span data-stu-id="fdc98-215">Response</span></span>
<span data-ttu-id="fdc98-216">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fdc98-216">If successful, this method returns a `201 Created` response code and a [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdc98-217">Пример</span><span class="sxs-lookup"><span data-stu-id="fdc98-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdc98-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdc98-218">Request</span></span>
<span data-ttu-id="fdc98-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdc98-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1450

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="fdc98-220">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdc98-220">Response</span></span>
<span data-ttu-id="fdc98-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdc98-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1622

{
  "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
  "id": "471203fb-03fb-4712-fb03-1247fb031247",
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



