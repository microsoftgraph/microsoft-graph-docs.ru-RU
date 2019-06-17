---
title: Обновление iosEnterpriseWiFiConfiguration
description: Обновление свойств объекта iosEnterpriseWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e48a9dafd287594d56236cb93809a2137a6b285
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966735"
---
# <a name="update-iosenterprisewificonfiguration"></a><span data-ttu-id="363fb-103">Обновление iosEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="363fb-103">Update iosEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="363fb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="363fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="363fb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="363fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="363fb-106">Обновление свойств объекта [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="363fb-106">Update the properties of a [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="363fb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="363fb-107">Prerequisites</span></span>
<span data-ttu-id="363fb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="363fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="363fb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="363fb-110">Permission type</span></span>|<span data-ttu-id="363fb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="363fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="363fb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="363fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="363fb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="363fb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="363fb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="363fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="363fb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="363fb-115">Not supported.</span></span>|
|<span data-ttu-id="363fb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="363fb-116">Application</span></span>|<span data-ttu-id="363fb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="363fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="363fb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="363fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="363fb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="363fb-119">Request headers</span></span>
|<span data-ttu-id="363fb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="363fb-120">Header</span></span>|<span data-ttu-id="363fb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="363fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="363fb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="363fb-122">Authorization</span></span>|<span data-ttu-id="363fb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="363fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="363fb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="363fb-124">Accept</span></span>|<span data-ttu-id="363fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="363fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="363fb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="363fb-126">Request body</span></span>
<span data-ttu-id="363fb-127">В тексте запроса добавьте представление объекта [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="363fb-127">In the request body, supply a JSON representation for the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

<span data-ttu-id="363fb-128">В следующей таблице приведены свойства, необходимые при создании [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-128">The following table shows the properties that are required when you create the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md).</span></span>

|<span data-ttu-id="363fb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="363fb-129">Property</span></span>|<span data-ttu-id="363fb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="363fb-130">Type</span></span>|<span data-ttu-id="363fb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="363fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="363fb-132">id</span><span class="sxs-lookup"><span data-stu-id="363fb-132">id</span></span>|<span data-ttu-id="363fb-133">String</span><span class="sxs-lookup"><span data-stu-id="363fb-133">String</span></span>|<span data-ttu-id="363fb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="363fb-134">Key of the entity.</span></span> <span data-ttu-id="363fb-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="363fb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="363fb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="363fb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="363fb-137">DateTimeOffset</span></span>|<span data-ttu-id="363fb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="363fb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="363fb-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="363fb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="363fb-140">roleScopeTagIds</span></span>|<span data-ttu-id="363fb-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="363fb-141">String collection</span></span>|<span data-ttu-id="363fb-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="363fb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="363fb-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="363fb-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="363fb-144">supportsScopeTags</span></span>|<span data-ttu-id="363fb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="363fb-145">Boolean</span></span>|<span data-ttu-id="363fb-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="363fb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="363fb-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="363fb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="363fb-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="363fb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="363fb-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="363fb-149">This property is read-only.</span></span> <span data-ttu-id="363fb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="363fb-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="363fb-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="363fb-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="363fb-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="363fb-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="363fb-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="363fb-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="363fb-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="363fb-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="363fb-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="363fb-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="363fb-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="363fb-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="363fb-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="363fb-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="363fb-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="363fb-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="363fb-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="363fb-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="363fb-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="363fb-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="363fb-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="363fb-163">createdDateTime</span></span>|<span data-ttu-id="363fb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="363fb-164">DateTimeOffset</span></span>|<span data-ttu-id="363fb-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="363fb-165">DateTime the object was created.</span></span> <span data-ttu-id="363fb-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="363fb-167">description</span><span class="sxs-lookup"><span data-stu-id="363fb-167">description</span></span>|<span data-ttu-id="363fb-168">String</span><span class="sxs-lookup"><span data-stu-id="363fb-168">String</span></span>|<span data-ttu-id="363fb-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="363fb-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="363fb-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="363fb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="363fb-171">displayName</span></span>|<span data-ttu-id="363fb-172">Строка</span><span class="sxs-lookup"><span data-stu-id="363fb-172">String</span></span>|<span data-ttu-id="363fb-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="363fb-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="363fb-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="363fb-175">version</span><span class="sxs-lookup"><span data-stu-id="363fb-175">version</span></span>|<span data-ttu-id="363fb-176">Int32</span><span class="sxs-lookup"><span data-stu-id="363fb-176">Int32</span></span>|<span data-ttu-id="363fb-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="363fb-177">Version of the device configuration.</span></span> <span data-ttu-id="363fb-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="363fb-179">Нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="363fb-179">networkName</span></span>|<span data-ttu-id="363fb-180">String</span><span class="sxs-lookup"><span data-stu-id="363fb-180">String</span></span>|<span data-ttu-id="363fb-181">Сетевое имя, унаследованное от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="363fb-181">Network Name Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="363fb-182">SSID</span><span class="sxs-lookup"><span data-stu-id="363fb-182">ssid</span></span>|<span data-ttu-id="363fb-183">String</span><span class="sxs-lookup"><span data-stu-id="363fb-183">String</span></span>|<span data-ttu-id="363fb-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="363fb-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="363fb-185">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="363fb-185">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="363fb-186">Коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="363fb-186">connectAutomatically</span></span>|<span data-ttu-id="363fb-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="363fb-187">Boolean</span></span>|<span data-ttu-id="363fb-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="363fb-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="363fb-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="363fb-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="363fb-190">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="363fb-190">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="363fb-191">Коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="363fb-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="363fb-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="363fb-192">Boolean</span></span>|<span data-ttu-id="363fb-193">Подключаться, если сеть не ведет вещание своего имени (SSID).</span><span class="sxs-lookup"><span data-stu-id="363fb-193">Connect when the network is not broadcasting its name (SSID).</span></span> <span data-ttu-id="363fb-194">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="363fb-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="363fb-195">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="363fb-195">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="363fb-196">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="363fb-196">wiFiSecurityType</span></span>|[<span data-ttu-id="363fb-197">Вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="363fb-197">wiFiSecurityType</span></span>](../resources/intune-deviceconfig-wifisecuritytype.md)|<span data-ttu-id="363fb-198">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="363fb-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="363fb-199">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-199">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="363fb-200">Возможные значения: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="363fb-200">Possible values are: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="363fb-201">proxySettings</span><span class="sxs-lookup"><span data-stu-id="363fb-201">proxySettings</span></span>|[<span data-ttu-id="363fb-202">Вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="363fb-202">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="363fb-203">Тип прокси-сервера для этого подключения Wi-Fi наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="363fb-203">Proxy Type for this Wi-Fi connection Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).</span></span> <span data-ttu-id="363fb-204">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="363fb-204">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="363fb-205">Проксимануаладдресс</span><span class="sxs-lookup"><span data-stu-id="363fb-205">proxyManualAddress</span></span>|<span data-ttu-id="363fb-206">String</span><span class="sxs-lookup"><span data-stu-id="363fb-206">String</span></span>|<span data-ttu-id="363fb-207">IP-адрес или DNS-имя узла прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="363fb-207">IP Address or DNS hostname of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="363fb-208">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="363fb-208">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="363fb-209">Проксимануалпорт</span><span class="sxs-lookup"><span data-stu-id="363fb-209">proxyManualPort</span></span>|<span data-ttu-id="363fb-210">Int32</span><span class="sxs-lookup"><span data-stu-id="363fb-210">Int32</span></span>|<span data-ttu-id="363fb-211">Порт прокси-сервера при выборе конфигурации вручную.</span><span class="sxs-lookup"><span data-stu-id="363fb-211">Port of the proxy server when manual configuration is selected.</span></span> <span data-ttu-id="363fb-212">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="363fb-212">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="363fb-213">Проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="363fb-213">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="363fb-214">String</span><span class="sxs-lookup"><span data-stu-id="363fb-214">String</span></span>|<span data-ttu-id="363fb-215">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="363fb-215">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="363fb-216">Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="363fb-216">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span> <span data-ttu-id="363fb-217">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="363fb-217">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="363fb-218">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="363fb-218">preSharedKey</span></span>|<span data-ttu-id="363fb-219">String</span><span class="sxs-lookup"><span data-stu-id="363fb-219">String</span></span>|<span data-ttu-id="363fb-220">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="363fb-220">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="363fb-221">Наследуется от [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="363fb-221">Inherited from [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)</span></span>|
|<span data-ttu-id="363fb-222">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="363fb-222">eapType</span></span>|[<span data-ttu-id="363fb-223">Еаптипе</span><span class="sxs-lookup"><span data-stu-id="363fb-223">eapType</span></span>](../resources/intune-deviceconfig-eaptype.md)|<span data-ttu-id="363fb-224">Протокол расширенной проверки подлинности (EAP).</span><span class="sxs-lookup"><span data-stu-id="363fb-224">Extensible Authentication Protocol (EAP).</span></span> <span data-ttu-id="363fb-225">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="363fb-225">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="363fb-226">Возможные значения: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span><span class="sxs-lookup"><span data-stu-id="363fb-226">Possible values are: `eapTls`, `leap`, `eapSim`, `eapTtls`, `peap`, `eapFast`.</span></span>|
|<span data-ttu-id="363fb-227">Еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="363fb-227">eapFastConfiguration</span></span>|[<span data-ttu-id="363fb-228">Еапфастконфигуратион</span><span class="sxs-lookup"><span data-stu-id="363fb-228">eapFastConfiguration</span></span>](../resources/intune-deviceconfig-eapfastconfiguration.md)|<span data-ttu-id="363fb-229">Параметр конфигурации EAP-FAST, когда EAP-FAST выбран тип EAP.</span><span class="sxs-lookup"><span data-stu-id="363fb-229">EAP-FAST Configuration Option when EAP-FAST is the selected EAP Type.</span></span> <span data-ttu-id="363fb-230">Возможные значения: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span><span class="sxs-lookup"><span data-stu-id="363fb-230">Possible values are: `noProtectedAccessCredential`, `useProtectedAccessCredential`, `useProtectedAccessCredentialAndProvision`, `useProtectedAccessCredentialAndProvisionAnonymously`.</span></span>|
|<span data-ttu-id="363fb-231">Трустедсерверцертификатенамес</span><span class="sxs-lookup"><span data-stu-id="363fb-231">trustedServerCertificateNames</span></span>|<span data-ttu-id="363fb-232">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="363fb-232">String collection</span></span>|<span data-ttu-id="363fb-233">Имена сертификатов доверенных серверов, когда тип EAP настроен для EAP-TLS/TTLS/FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="363fb-233">Trusted server certificate names when EAP Type is configured to EAP-TLS/TTLS/FAST or PEAP.</span></span> <span data-ttu-id="363fb-234">Это общее имя, используемое в сертификатах, выдаваемых доверенным центром сертификации (CA).</span><span class="sxs-lookup"><span data-stu-id="363fb-234">This is the common name used in the certificates issued by your trusted certificate authority (CA).</span></span> <span data-ttu-id="363fb-235">Если вы предоставляете эти сведения, вы можете обходить диалоговое окно динамического доверия, отображаемое на устройствах конечных пользователей, когда они подключаются к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="363fb-235">If you provide this information, you can bypass the dynamic trust dialog that is displayed on end users' devices when they connect to this Wi-Fi network.</span></span>|
|<span data-ttu-id="363fb-236">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="363fb-236">authenticationMethod</span></span>|[<span data-ttu-id="363fb-237">Вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="363fb-237">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="363fb-238">Метод проверки подлинности, когда тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="363fb-238">Authentication Method when EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="363fb-239">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="363fb-239">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="363fb-240">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="363fb-240">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="363fb-241">Нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="363fb-241">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="363fb-242">Метод проверки подлинности, отличный от EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="363fb-242">Non-EAP Method for Authentication when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="363fb-243">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="363fb-243">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="363fb-244">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="363fb-244">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="363fb-245">String</span><span class="sxs-lookup"><span data-stu-id="363fb-245">String</span></span>|<span data-ttu-id="363fb-246">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS, EAP-FAST или PEAP.</span><span class="sxs-lookup"><span data-stu-id="363fb-246">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP - TTLS, EAP - FAST or PEAP.</span></span> <span data-ttu-id="363fb-247">Это свойство маскирует имена пользователей с введенным текстом.</span><span class="sxs-lookup"><span data-stu-id="363fb-247">This property masks usernames with the text you enter.</span></span> <span data-ttu-id="363fb-248">Например, если вы используете анонимный доступ, все пользователи, которые проходят проверку подлинности с помощью этого подключения Wi-Fi, с помощью действительного имени пользователя отображаются как anonymous.</span><span class="sxs-lookup"><span data-stu-id="363fb-248">For example, if you use 'anonymous', each user that authenticates with this Wi-Fi connection using their real username is displayed as 'anonymous'.</span></span>|
|<span data-ttu-id="363fb-249">Усернамеформатстринг</span><span class="sxs-lookup"><span data-stu-id="363fb-249">usernameFormatString</span></span>|<span data-ttu-id="363fb-250">String</span><span class="sxs-lookup"><span data-stu-id="363fb-250">String</span></span>|<span data-ttu-id="363fb-251">Строка формата имени пользователя, используемая для построения имени пользователя для подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="363fb-251">Username format string used to build the username to connect to wifi</span></span>|
|<span data-ttu-id="363fb-252">Пассвордформатстринг</span><span class="sxs-lookup"><span data-stu-id="363fb-252">passwordFormatString</span></span>|<span data-ttu-id="363fb-253">String</span><span class="sxs-lookup"><span data-stu-id="363fb-253">String</span></span>|<span data-ttu-id="363fb-254">Строка формата пароля, используемая для создания пароля подключения к Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="363fb-254">Password format string used to build the password to connect to wifi</span></span>|



## <a name="response"></a><span data-ttu-id="363fb-255">Отклик</span><span class="sxs-lookup"><span data-stu-id="363fb-255">Response</span></span>
<span data-ttu-id="363fb-256">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="363fb-256">If successful, this method returns a `200 OK` response code and an updated [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="363fb-257">Пример</span><span class="sxs-lookup"><span data-stu-id="363fb-257">Example</span></span>

### <a name="request"></a><span data-ttu-id="363fb-258">Запрос</span><span class="sxs-lookup"><span data-stu-id="363fb-258">Request</span></span>
<span data-ttu-id="363fb-259">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="363fb-259">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="363fb-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="363fb-260">Response</span></span>
<span data-ttu-id="363fb-p128">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="363fb-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





