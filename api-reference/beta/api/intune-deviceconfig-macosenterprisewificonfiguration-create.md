---
title: Создание macOSEnterpriseWiFiConfiguration
description: Создание нового объекта macOSEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e393861c9e86bb7e91fb45e35c60034c8ee9188
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732995"
---
# <a name="create-macosenterprisewificonfiguration"></a><span data-ttu-id="95492-103">Создание macOSEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="95492-103">Create macOSEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="95492-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95492-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="95492-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95492-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95492-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95492-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95492-107">Создание нового объекта [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="95492-107">Create a new [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95492-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="95492-108">Prerequisites</span></span>
<span data-ttu-id="95492-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95492-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95492-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95492-111">Permission type</span></span>|<span data-ttu-id="95492-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95492-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95492-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95492-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95492-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95492-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95492-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95492-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95492-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95492-116">Not supported.</span></span>|
|<span data-ttu-id="95492-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95492-117">Application</span></span>|<span data-ttu-id="95492-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95492-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95492-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95492-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="95492-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="95492-120">Request headers</span></span>
|<span data-ttu-id="95492-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95492-121">Header</span></span>|<span data-ttu-id="95492-122">Значение</span><span class="sxs-lookup"><span data-stu-id="95492-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95492-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95492-123">Authorization</span></span>|<span data-ttu-id="95492-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95492-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95492-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95492-125">Accept</span></span>|<span data-ttu-id="95492-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95492-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95492-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="95492-127">Request body</span></span>
<span data-ttu-id="95492-128">В тексте запроса добавьте представление объекта macOSEnterpriseWiFiConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95492-128">In the request body, supply a JSON representation for the macOSEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="95492-129">В следующей таблице приведены свойства, необходимые при создании macOSEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="95492-129">The following table shows the properties that are required when you create the macOSEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="95492-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="95492-130">Property</span></span>|<span data-ttu-id="95492-131">Тип</span><span class="sxs-lookup"><span data-stu-id="95492-131">Type</span></span>|<span data-ttu-id="95492-132">Описание</span><span class="sxs-lookup"><span data-stu-id="95492-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95492-133">id</span><span class="sxs-lookup"><span data-stu-id="95492-133">id</span></span>|<span data-ttu-id="95492-134">Строка</span><span class="sxs-lookup"><span data-stu-id="95492-134">String</span></span>|<span data-ttu-id="95492-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="95492-135">Key of the entity.</span></span> <span data-ttu-id="95492-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95492-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95492-137">lastModifiedDateTime</span></span>|<span data-ttu-id="95492-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95492-138">DateTimeOffset</span></span>|<span data-ttu-id="95492-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="95492-139">DateTime the object was last modified.</span></span> <span data-ttu-id="95492-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95492-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95492-141">roleScopeTagIds</span></span>|<span data-ttu-id="95492-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="95492-142">String collection</span></span>|<span data-ttu-id="95492-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="95492-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95492-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95492-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="95492-145">supportsScopeTags</span></span>|<span data-ttu-id="95492-146">Логический</span><span class="sxs-lookup"><span data-stu-id="95492-146">Boolean</span></span>|<span data-ttu-id="95492-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="95492-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95492-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="95492-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95492-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="95492-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95492-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95492-150">This property is read-only.</span></span> <span data-ttu-id="95492-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95492-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="95492-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="95492-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="95492-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="95492-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="95492-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="95492-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95492-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="95492-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="95492-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="95492-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="95492-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="95492-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="95492-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95492-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="95492-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="95492-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="95492-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="95492-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="95492-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="95492-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95492-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95492-164">createdDateTime</span></span>|<span data-ttu-id="95492-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95492-165">DateTimeOffset</span></span>|<span data-ttu-id="95492-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="95492-166">DateTime the object was created.</span></span> <span data-ttu-id="95492-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95492-168">description</span><span class="sxs-lookup"><span data-stu-id="95492-168">description</span></span>|<span data-ttu-id="95492-169">Строка</span><span class="sxs-lookup"><span data-stu-id="95492-169">String</span></span>|<span data-ttu-id="95492-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="95492-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95492-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95492-172">displayName</span><span class="sxs-lookup"><span data-stu-id="95492-172">displayName</span></span>|<span data-ttu-id="95492-173">Строка</span><span class="sxs-lookup"><span data-stu-id="95492-173">String</span></span>|<span data-ttu-id="95492-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="95492-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95492-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95492-176">version</span><span class="sxs-lookup"><span data-stu-id="95492-176">version</span></span>|<span data-ttu-id="95492-177">Int32</span><span class="sxs-lookup"><span data-stu-id="95492-177">Int32</span></span>|<span data-ttu-id="95492-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="95492-178">Version of the device configuration.</span></span> <span data-ttu-id="95492-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95492-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="95492-180">networkName</span></span>|<span data-ttu-id="95492-181">Строка</span><span class="sxs-lookup"><span data-stu-id="95492-181">String</span></span>|<span data-ttu-id="95492-182">Сетевое имя, унаследованное от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95492-182">Network Name Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="95492-183">SSID</span><span class="sxs-lookup"><span data-stu-id="95492-183">ssid</span></span>|<span data-ttu-id="95492-184">Строка</span><span class="sxs-lookup"><span data-stu-id="95492-184">String</span></span>|<span data-ttu-id="95492-185">Это имя Wi-Fiной сети, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="95492-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="95492-186">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95492-186">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="95492-187">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="95492-187">connectAutomatically</span></span>|<span data-ttu-id="95492-188">Логический</span><span class="sxs-lookup"><span data-stu-id="95492-188">Boolean</span></span>|<span data-ttu-id="95492-189">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="95492-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="95492-190">Если задать для этого параметра значение true, запрос пользователя будет пропущен и устройство будет автоматически подключено к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="95492-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="95492-191">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95492-191">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="95492-192">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="95492-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="95492-193">Логический</span><span class="sxs-lookup"><span data-stu-id="95492-193">Boolean</span></span>|<span data-ttu-id="95492-194">Подключаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="95492-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="95492-195">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="95492-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="95492-196">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95492-196">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="95492-197">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="95492-197">wiFiSecurityType</span></span>|[<span data-ttu-id="95492-198">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="95492-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="95492-199">Указывает, использует ли конечная точка Wi-Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="95492-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="95492-200">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-200">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="95492-201">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="95492-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="95492-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="95492-202">proxySettings</span></span>|[<span data-ttu-id="95492-203">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="95492-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="95492-204">Тип прокси-сервера для этого подключения Wi-Fi наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95492-204">Proxy Type for this Wi-Fi connection Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="95492-205">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="95492-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="95492-206">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="95492-206">proxyManualAddress</span></span>|<span data-ttu-id="95492-207">Строка</span><span class="sxs-lookup"><span data-stu-id="95492-207">String</span></span>|<span data-ttu-id="95492-208">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="95492-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="95492-209">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95492-209">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="95492-210">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="95492-210">proxyManualPort</span></span>|<span data-ttu-id="95492-211">Int32</span><span class="sxs-lookup"><span data-stu-id="95492-211">Int32</span></span>|<span data-ttu-id="95492-212">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="95492-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="95492-213">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95492-213">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="95492-214">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="95492-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="95492-215">Строка</span><span class="sxs-lookup"><span data-stu-id="95492-215">String</span></span>|<span data-ttu-id="95492-216">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="95492-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="95492-217">Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="95492-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="95492-218">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95492-218">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="95492-219">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="95492-219">preSharedKey</span></span>|<span data-ttu-id="95492-220">Строка</span><span class="sxs-lookup"><span data-stu-id="95492-220">String</span></span>|<span data-ttu-id="95492-221">Это предварительно общий ключ для сети WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="95492-221">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="95492-222">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95492-222">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="95492-223">еаптипе</span><span class="sxs-lookup"><span data-stu-id="95492-223">eapType</span></span>|[<span data-ttu-id="95492-224">еаптипе</span><span class="sxs-lookup"><span data-stu-id="95492-224">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="95492-225">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="95492-225">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="95492-226">Указывает тип протокола EAP, заданный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="95492-226">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="95492-227">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="95492-227">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="95492-228">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="95492-228">eapFastConfiguration</span></span>|[<span data-ttu-id="95492-229">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="95492-229">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="95492-230">Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="95492-230">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="95492-231">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="95492-231">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="95492-232">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="95492-232">trustedServerCertificateNames</span></span>|<span data-ttu-id="95492-233">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="95492-233">String collection</span></span>|<span data-ttu-id="95492-234">Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="95492-234">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="95492-235">Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="95492-235">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="95492-236">Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к этой сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="95492-236">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="95492-237">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="95492-237">authenticationMethod</span></span>|[<span data-ttu-id="95492-238">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="95492-238">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="95492-239">Метод проверки подлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="95492-239">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="95492-240">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="95492-240">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="95492-241">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="95492-241">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="95492-242">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="95492-242">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="95492-243">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="95492-243">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="95492-244">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="95492-244">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="95492-245">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="95492-245">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="95492-246">Строка</span><span class="sxs-lookup"><span data-stu-id="95492-246">String</span></span>|<span data-ttu-id="95492-247">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="95492-247">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="95492-248">Это свойство маскирует имена пользователей с введенным текстом.</span><span class="sxs-lookup"><span data-stu-id="95492-248">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="95492-249">Например, если вы используете анонимный доступ, каждый пользователь, который проверяет подлинность этого подключения Wi-Fi с помощью действительного имени пользователя, отображается как anonymous.</span><span class="sxs-lookup"><span data-stu-id="95492-249">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="95492-250">Ответ</span><span class="sxs-lookup"><span data-stu-id="95492-250">Response</span></span>
<span data-ttu-id="95492-251">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="95492-251">If successful, this method returns a `201 Created` response code and a [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95492-252">Пример</span><span class="sxs-lookup"><span data-stu-id="95492-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="95492-253">Запрос</span><span class="sxs-lookup"><span data-stu-id="95492-253">Request</span></span>
<span data-ttu-id="95492-254">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95492-254">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1858

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a><span data-ttu-id="95492-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="95492-255">Response</span></span>
<span data-ttu-id="95492-p128">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95492-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2030

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
  "id": "7a6f9a2e-9a2e-7a6f-2e9a-6f7a2e9a6f7a",
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
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





