---
title: Обновление macOSEnterpriseWiFiConfiguration
description: Обновление свойств объекта macOSEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9f49f8de366eb80c2a19d9673c9a551b6529b477
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306626"
---
# <a name="update-macosenterprisewificonfiguration"></a><span data-ttu-id="9f53a-103">Обновление macOSEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f53a-103">Update macOSEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="9f53a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f53a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f53a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f53a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f53a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f53a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f53a-107">Обновление свойств объекта [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9f53a-107">Update the properties of a [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f53a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9f53a-108">Prerequisites</span></span>
<span data-ttu-id="9f53a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f53a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f53a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f53a-111">Permission type</span></span>|<span data-ttu-id="9f53a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f53a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f53a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f53a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f53a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f53a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9f53a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f53a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f53a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f53a-116">Not supported.</span></span>|
|<span data-ttu-id="9f53a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f53a-117">Application</span></span>|<span data-ttu-id="9f53a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f53a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f53a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f53a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9f53a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9f53a-120">Request headers</span></span>
|<span data-ttu-id="9f53a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f53a-121">Header</span></span>|<span data-ttu-id="9f53a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9f53a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f53a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f53a-123">Authorization</span></span>|<span data-ttu-id="9f53a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f53a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f53a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f53a-125">Accept</span></span>|<span data-ttu-id="9f53a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f53a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f53a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f53a-127">Request body</span></span>
<span data-ttu-id="9f53a-128">В тексте запроса добавьте представление объекта [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f53a-128">In the request body, supply a JSON representation for the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="9f53a-129">В следующей таблице приведены свойства, необходимые при создании [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-129">The following table shows the properties that are required when you create the [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="9f53a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f53a-130">Property</span></span>|<span data-ttu-id="9f53a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f53a-131">Type</span></span>|<span data-ttu-id="9f53a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f53a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f53a-133">id</span><span class="sxs-lookup"><span data-stu-id="9f53a-133">id</span></span>|<span data-ttu-id="9f53a-134">String</span><span class="sxs-lookup"><span data-stu-id="9f53a-134">String</span></span>|<span data-ttu-id="9f53a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9f53a-135">Key of the entity.</span></span> <span data-ttu-id="9f53a-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f53a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9f53a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f53a-138">DateTimeOffset</span></span>|<span data-ttu-id="9f53a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9f53a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9f53a-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f53a-141">roleScopeTagIds</span></span>|<span data-ttu-id="9f53a-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9f53a-142">String collection</span></span>|<span data-ttu-id="9f53a-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="9f53a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9f53a-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="9f53a-145">supportsScopeTags</span></span>|<span data-ttu-id="9f53a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f53a-146">Boolean</span></span>|<span data-ttu-id="9f53a-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9f53a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9f53a-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="9f53a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9f53a-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9f53a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9f53a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9f53a-150">This property is read-only.</span></span> <span data-ttu-id="9f53a-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9f53a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9f53a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9f53a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9f53a-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9f53a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9f53a-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9f53a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9f53a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9f53a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9f53a-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9f53a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9f53a-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9f53a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9f53a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9f53a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9f53a-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9f53a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9f53a-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f53a-164">createdDateTime</span></span>|<span data-ttu-id="9f53a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f53a-165">DateTimeOffset</span></span>|<span data-ttu-id="9f53a-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9f53a-166">DateTime the object was created.</span></span> <span data-ttu-id="9f53a-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-168">description</span><span class="sxs-lookup"><span data-stu-id="9f53a-168">description</span></span>|<span data-ttu-id="9f53a-169">String</span><span class="sxs-lookup"><span data-stu-id="9f53a-169">String</span></span>|<span data-ttu-id="9f53a-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f53a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9f53a-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9f53a-172">displayName</span></span>|<span data-ttu-id="9f53a-173">String</span><span class="sxs-lookup"><span data-stu-id="9f53a-173">String</span></span>|<span data-ttu-id="9f53a-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f53a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9f53a-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-176">version</span><span class="sxs-lookup"><span data-stu-id="9f53a-176">version</span></span>|<span data-ttu-id="9f53a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9f53a-177">Int32</span></span>|<span data-ttu-id="9f53a-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f53a-178">Version of the device configuration.</span></span> <span data-ttu-id="9f53a-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="9f53a-180">networkName</span></span>|<span data-ttu-id="9f53a-181">String</span><span class="sxs-lookup"><span data-stu-id="9f53a-181">String</span></span>|<span data-ttu-id="9f53a-182">Сетевое имя, унаследованное от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f53a-182">Network Name Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-183">SSID</span><span class="sxs-lookup"><span data-stu-id="9f53a-183">ssid</span></span>|<span data-ttu-id="9f53a-184">String</span><span class="sxs-lookup"><span data-stu-id="9f53a-184">String</span></span>|<span data-ttu-id="9f53a-185">Это имя Wi-Fiной сети, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="9f53a-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="9f53a-186">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f53a-186">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-187">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="9f53a-187">connectAutomatically</span></span>|<span data-ttu-id="9f53a-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f53a-188">Boolean</span></span>|<span data-ttu-id="9f53a-189">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="9f53a-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="9f53a-190">Если задать для этого параметра значение true, запрос пользователя будет пропущен и устройство будет автоматически подключено к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="9f53a-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="9f53a-191">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f53a-191">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-192">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="9f53a-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="9f53a-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f53a-193">Boolean</span></span>|<span data-ttu-id="9f53a-194">Подключаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="9f53a-194">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="9f53a-195">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="9f53a-195">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="9f53a-196">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f53a-196">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-197">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="9f53a-197">wiFiSecurityType</span></span>|[<span data-ttu-id="9f53a-198">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="9f53a-198">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="9f53a-199">Указывает, использует ли конечная точка Wi-Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="9f53a-199">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="9f53a-200">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-200">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="9f53a-201">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="9f53a-201">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="9f53a-202">proxySettings</span><span class="sxs-lookup"><span data-stu-id="9f53a-202">proxySettings</span></span>|[<span data-ttu-id="9f53a-203">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="9f53a-203">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="9f53a-204">Тип прокси-сервера для этого подключения Wi-Fi наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f53a-204">Proxy Type for this Wi-Fi connection Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md).</span></span> <span data-ttu-id="9f53a-205">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="9f53a-205">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="9f53a-206">проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="9f53a-206">proxyManualAddress</span></span>|<span data-ttu-id="9f53a-207">String</span><span class="sxs-lookup"><span data-stu-id="9f53a-207">String</span></span>|<span data-ttu-id="9f53a-208">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="9f53a-208">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="9f53a-209">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f53a-209">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-210">проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="9f53a-210">proxyManualPort</span></span>|<span data-ttu-id="9f53a-211">Int32</span><span class="sxs-lookup"><span data-stu-id="9f53a-211">Int32</span></span>|<span data-ttu-id="9f53a-212">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="9f53a-212">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="9f53a-213">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f53a-213">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-214">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="9f53a-214">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="9f53a-215">String</span><span class="sxs-lookup"><span data-stu-id="9f53a-215">String</span></span>|<span data-ttu-id="9f53a-216">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="9f53a-216">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="9f53a-217">Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="9f53a-217">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="9f53a-218">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f53a-218">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-219">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="9f53a-219">preSharedKey</span></span>|<span data-ttu-id="9f53a-220">String</span><span class="sxs-lookup"><span data-stu-id="9f53a-220">String</span></span>|<span data-ttu-id="9f53a-221">Это предварительно общий ключ для сети WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="9f53a-221">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="9f53a-222">Наследуется от [макосвификонфигуратион](../resources/intune-deviceconfig-macoswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f53a-222">Inherited from [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)</span></span>|
|<span data-ttu-id="9f53a-223">еаптипе</span><span class="sxs-lookup"><span data-stu-id="9f53a-223">eapType</span></span>|[<span data-ttu-id="9f53a-224">еаптипе</span><span class="sxs-lookup"><span data-stu-id="9f53a-224">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="9f53a-225">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="9f53a-225">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="9f53a-226">Указывает тип протокола EAP, заданный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="9f53a-226">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="9f53a-227">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="9f53a-227">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="9f53a-228">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9f53a-228">eapFastConfiguration</span></span>|[<span data-ttu-id="9f53a-229">еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9f53a-229">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="9f53a-230">Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="9f53a-230">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="9f53a-231">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="9f53a-231">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="9f53a-232">трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="9f53a-232">trustedServerCertificateNames</span></span>|<span data-ttu-id="9f53a-233">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9f53a-233">String collection</span></span>|<span data-ttu-id="9f53a-234">Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="9f53a-234">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="9f53a-235">Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="9f53a-235">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="9f53a-236">Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к этой сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="9f53a-236">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="9f53a-237">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="9f53a-237">authenticationMethod</span></span>|[<span data-ttu-id="9f53a-238">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="9f53a-238">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="9f53a-239">Метод проверки подлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="9f53a-239">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="9f53a-240">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="9f53a-240">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="9f53a-241">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="9f53a-241">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="9f53a-242">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="9f53a-242">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="9f53a-243">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="9f53a-243">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="9f53a-244">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="9f53a-244">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="9f53a-245">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="9f53a-245">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="9f53a-246">String</span><span class="sxs-lookup"><span data-stu-id="9f53a-246">String</span></span>|<span data-ttu-id="9f53a-247">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="9f53a-247">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS, EAP-FAST or PEAP.</span></span> <span data-ttu-id="9f53a-248">Это свойство маскирует имена пользователей с введенным текстом.</span><span class="sxs-lookup"><span data-stu-id="9f53a-248">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="9f53a-249">Например, если вы используете анонимный доступ, каждый пользователь, который проверяет подлинность этого подключения Wi-Fi с помощью действительного имени пользователя, отображается как anonymous.</span><span class="sxs-lookup"><span data-stu-id="9f53a-249">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|



## <a name="response"></a><span data-ttu-id="9f53a-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f53a-250">Response</span></span>
<span data-ttu-id="9f53a-251">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f53a-251">If successful, this method returns a `200 OK` response code and an updated [macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f53a-252">Пример</span><span class="sxs-lookup"><span data-stu-id="9f53a-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f53a-253">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f53a-253">Request</span></span>
<span data-ttu-id="9f53a-254">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f53a-254">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="9f53a-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f53a-255">Response</span></span>
<span data-ttu-id="9f53a-p128">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f53a-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




