---
title: Создание Андроиддевицеовнерентерприсевификонфигуратион
description: Создание нового объекта Андроиддевицеовнерентерприсевификонфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a8feef3038fd397ce3dfd51cab45226dbdb3dce1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36317045"
---
# <a name="create-androiddeviceownerenterprisewificonfiguration"></a><span data-ttu-id="25c29-103">Создание Андроиддевицеовнерентерприсевификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="25c29-103">Create androidDeviceOwnerEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="25c29-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25c29-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25c29-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25c29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25c29-106">Создание нового объекта [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="25c29-106">Create a new [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25c29-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="25c29-107">Prerequisites</span></span>
<span data-ttu-id="25c29-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25c29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25c29-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25c29-110">Permission type</span></span>|<span data-ttu-id="25c29-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25c29-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25c29-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25c29-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25c29-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c29-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25c29-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25c29-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25c29-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25c29-115">Not supported.</span></span>|
|<span data-ttu-id="25c29-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25c29-116">Application</span></span>|<span data-ttu-id="25c29-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c29-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="25c29-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25c29-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="25c29-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="25c29-119">Request headers</span></span>
|<span data-ttu-id="25c29-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25c29-120">Header</span></span>|<span data-ttu-id="25c29-121">Значение</span><span class="sxs-lookup"><span data-stu-id="25c29-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25c29-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="25c29-122">Authorization</span></span>|<span data-ttu-id="25c29-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25c29-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25c29-124">Accept</span><span class="sxs-lookup"><span data-stu-id="25c29-124">Accept</span></span>|<span data-ttu-id="25c29-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25c29-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25c29-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="25c29-126">Request body</span></span>
<span data-ttu-id="25c29-127">В тексте запроса добавьте представление объекта Андроиддевицеовнерентерприсевификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25c29-127">In the request body, supply a JSON representation for the androidDeviceOwnerEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="25c29-128">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнерентерприсевификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="25c29-128">The following table shows the properties that are required when you create the androidDeviceOwnerEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="25c29-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="25c29-129">Property</span></span>|<span data-ttu-id="25c29-130">Тип</span><span class="sxs-lookup"><span data-stu-id="25c29-130">Type</span></span>|<span data-ttu-id="25c29-131">Описание</span><span class="sxs-lookup"><span data-stu-id="25c29-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25c29-132">id</span><span class="sxs-lookup"><span data-stu-id="25c29-132">id</span></span>|<span data-ttu-id="25c29-133">String</span><span class="sxs-lookup"><span data-stu-id="25c29-133">String</span></span>|<span data-ttu-id="25c29-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="25c29-134">Key of the entity.</span></span> <span data-ttu-id="25c29-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25c29-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25c29-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25c29-136">lastModifiedDateTime</span></span>|<span data-ttu-id="25c29-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25c29-137">DateTimeOffset</span></span>|<span data-ttu-id="25c29-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="25c29-138">DateTime the object was last modified.</span></span> <span data-ttu-id="25c29-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25c29-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25c29-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="25c29-140">roleScopeTagIds</span></span>|<span data-ttu-id="25c29-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="25c29-141">String collection</span></span>|<span data-ttu-id="25c29-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="25c29-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="25c29-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25c29-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25c29-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="25c29-144">supportsScopeTags</span></span>|<span data-ttu-id="25c29-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="25c29-145">Boolean</span></span>|<span data-ttu-id="25c29-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="25c29-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="25c29-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="25c29-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="25c29-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="25c29-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="25c29-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="25c29-149">This property is read-only.</span></span> <span data-ttu-id="25c29-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25c29-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25c29-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="25c29-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="25c29-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="25c29-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="25c29-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="25c29-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="25c29-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25c29-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25c29-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="25c29-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="25c29-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="25c29-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="25c29-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="25c29-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="25c29-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25c29-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25c29-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="25c29-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="25c29-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="25c29-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="25c29-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="25c29-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="25c29-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25c29-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25c29-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25c29-163">createdDateTime</span></span>|<span data-ttu-id="25c29-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25c29-164">DateTimeOffset</span></span>|<span data-ttu-id="25c29-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="25c29-165">DateTime the object was created.</span></span> <span data-ttu-id="25c29-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25c29-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25c29-167">description</span><span class="sxs-lookup"><span data-stu-id="25c29-167">description</span></span>|<span data-ttu-id="25c29-168">String</span><span class="sxs-lookup"><span data-stu-id="25c29-168">String</span></span>|<span data-ttu-id="25c29-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="25c29-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="25c29-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25c29-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25c29-171">displayName</span><span class="sxs-lookup"><span data-stu-id="25c29-171">displayName</span></span>|<span data-ttu-id="25c29-172">Строка</span><span class="sxs-lookup"><span data-stu-id="25c29-172">String</span></span>|<span data-ttu-id="25c29-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="25c29-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="25c29-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25c29-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25c29-175">version</span><span class="sxs-lookup"><span data-stu-id="25c29-175">version</span></span>|<span data-ttu-id="25c29-176">Int32</span><span class="sxs-lookup"><span data-stu-id="25c29-176">Int32</span></span>|<span data-ttu-id="25c29-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="25c29-177">Version of the device configuration.</span></span> <span data-ttu-id="25c29-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25c29-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25c29-179">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="25c29-179">networkName</span></span>|<span data-ttu-id="25c29-180">String</span><span class="sxs-lookup"><span data-stu-id="25c29-180">String</span></span>|<span data-ttu-id="25c29-181">Сетевое имя, унаследованное от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c29-181">Network Name Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="25c29-182">SSID</span><span class="sxs-lookup"><span data-stu-id="25c29-182">ssid</span></span>|<span data-ttu-id="25c29-183">String</span><span class="sxs-lookup"><span data-stu-id="25c29-183">String</span></span>|<span data-ttu-id="25c29-184">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="25c29-184">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="25c29-185">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c29-185">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="25c29-186">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="25c29-186">connectAutomatically</span></span>|<span data-ttu-id="25c29-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="25c29-187">Boolean</span></span>|<span data-ttu-id="25c29-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="25c29-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="25c29-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="25c29-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="25c29-190">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c29-190">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="25c29-191">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="25c29-191">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="25c29-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="25c29-192">Boolean</span></span>|<span data-ttu-id="25c29-193">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="25c29-193">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="25c29-194">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c29-194">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="25c29-195">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="25c29-195">wiFiSecurityType</span></span>|[<span data-ttu-id="25c29-196">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="25c29-196">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="25c29-197">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="25c29-197">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="25c29-198">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25c29-198">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span> <span data-ttu-id="25c29-199">Возможные значения: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="25c29-199">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="25c29-200">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="25c29-200">preSharedKey</span></span>|<span data-ttu-id="25c29-201">String</span><span class="sxs-lookup"><span data-stu-id="25c29-201">String</span></span>|<span data-ttu-id="25c29-202">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="25c29-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="25c29-203">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c29-203">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="25c29-204">прешаредкэйиссет</span><span class="sxs-lookup"><span data-stu-id="25c29-204">preSharedKeyIsSet</span></span>|<span data-ttu-id="25c29-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="25c29-205">Boolean</span></span>|<span data-ttu-id="25c29-206">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="25c29-206">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="25c29-207">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25c29-207">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="25c29-208">еаптипе</span><span class="sxs-lookup"><span data-stu-id="25c29-208">eapType</span></span>|[<span data-ttu-id="25c29-209">андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="25c29-209">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="25c29-210">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="25c29-210">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="25c29-211">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="25c29-211">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="25c29-212">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="25c29-212">authenticationMethod</span></span>|[<span data-ttu-id="25c29-213">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="25c29-213">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="25c29-214">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="25c29-214">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="25c29-215">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="25c29-215">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="25c29-216">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="25c29-216">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="25c29-217">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="25c29-217">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="25c29-218">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="25c29-218">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="25c29-219">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="25c29-219">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="25c29-220">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="25c29-220">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="25c29-221">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="25c29-221">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="25c29-222">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="25c29-222">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="25c29-223">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="25c29-223">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="25c29-224">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="25c29-224">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="25c29-225">String</span><span class="sxs-lookup"><span data-stu-id="25c29-225">String</span></span>|<span data-ttu-id="25c29-226">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="25c29-226">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="25c29-227">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="25c29-227">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="25c29-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="25c29-228">Response</span></span>
<span data-ttu-id="25c29-229">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="25c29-229">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25c29-230">Пример</span><span class="sxs-lookup"><span data-stu-id="25c29-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="25c29-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="25c29-231">Request</span></span>
<span data-ttu-id="25c29-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25c29-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="25c29-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="25c29-233">Response</span></span>
<span data-ttu-id="25c29-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25c29-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






