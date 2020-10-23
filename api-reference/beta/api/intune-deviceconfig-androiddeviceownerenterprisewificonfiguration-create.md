---
title: Создание Андроиддевицеовнерентерприсевификонфигуратион
description: Создание нового объекта Андроиддевицеовнерентерприсевификонфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c8a7ec1a8aa5cb7d818f9faa58f474f0bc4170c1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733904"
---
# <a name="create-androiddeviceownerenterprisewificonfiguration"></a><span data-ttu-id="6f8ce-103">Создание Андроиддевицеовнерентерприсевификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="6f8ce-103">Create androidDeviceOwnerEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="6f8ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f8ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f8ce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f8ce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f8ce-107">Создание нового объекта [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6f8ce-107">Create a new [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f8ce-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6f8ce-108">Prerequisites</span></span>
<span data-ttu-id="6f8ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f8ce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f8ce-111">Permission type</span></span>|<span data-ttu-id="6f8ce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f8ce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f8ce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f8ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f8ce-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f8ce-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f8ce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f8ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f8ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-116">Not supported.</span></span>|
|<span data-ttu-id="6f8ce-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f8ce-117">Application</span></span>|<span data-ttu-id="6f8ce-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f8ce-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f8ce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f8ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6f8ce-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6f8ce-120">Request headers</span></span>
|<span data-ttu-id="6f8ce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f8ce-121">Header</span></span>|<span data-ttu-id="6f8ce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6f8ce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f8ce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f8ce-123">Authorization</span></span>|<span data-ttu-id="6f8ce-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f8ce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f8ce-125">Accept</span></span>|<span data-ttu-id="6f8ce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f8ce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f8ce-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f8ce-127">Request body</span></span>
<span data-ttu-id="6f8ce-128">В тексте запроса добавьте представление объекта Андроиддевицеовнерентерприсевификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-128">In the request body, supply a JSON representation for the androidDeviceOwnerEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="6f8ce-129">В следующей таблице приведены свойства, необходимые при создании Андроиддевицеовнерентерприсевификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-129">The following table shows the properties that are required when you create the androidDeviceOwnerEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="6f8ce-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f8ce-130">Property</span></span>|<span data-ttu-id="6f8ce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6f8ce-131">Type</span></span>|<span data-ttu-id="6f8ce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6f8ce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f8ce-133">id</span><span class="sxs-lookup"><span data-stu-id="6f8ce-133">id</span></span>|<span data-ttu-id="6f8ce-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6f8ce-134">String</span></span>|<span data-ttu-id="6f8ce-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-135">Key of the entity.</span></span> <span data-ttu-id="6f8ce-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f8ce-137">lastModifiedDateTime</span></span>|<span data-ttu-id="6f8ce-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f8ce-138">DateTimeOffset</span></span>|<span data-ttu-id="6f8ce-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-139">DateTime the object was last modified.</span></span> <span data-ttu-id="6f8ce-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6f8ce-141">roleScopeTagIds</span></span>|<span data-ttu-id="6f8ce-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6f8ce-142">String collection</span></span>|<span data-ttu-id="6f8ce-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6f8ce-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="6f8ce-145">supportsScopeTags</span></span>|<span data-ttu-id="6f8ce-146">Логический</span><span class="sxs-lookup"><span data-stu-id="6f8ce-146">Boolean</span></span>|<span data-ttu-id="6f8ce-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6f8ce-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6f8ce-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6f8ce-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-150">This property is read-only.</span></span> <span data-ttu-id="6f8ce-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6f8ce-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6f8ce-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6f8ce-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6f8ce-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6f8ce-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6f8ce-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6f8ce-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6f8ce-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6f8ce-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6f8ce-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6f8ce-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6f8ce-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="6f8ce-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6f8ce-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6f8ce-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f8ce-164">createdDateTime</span></span>|<span data-ttu-id="6f8ce-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f8ce-165">DateTimeOffset</span></span>|<span data-ttu-id="6f8ce-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-166">DateTime the object was created.</span></span> <span data-ttu-id="6f8ce-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-168">description</span><span class="sxs-lookup"><span data-stu-id="6f8ce-168">description</span></span>|<span data-ttu-id="6f8ce-169">Строка</span><span class="sxs-lookup"><span data-stu-id="6f8ce-169">String</span></span>|<span data-ttu-id="6f8ce-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6f8ce-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-172">displayName</span><span class="sxs-lookup"><span data-stu-id="6f8ce-172">displayName</span></span>|<span data-ttu-id="6f8ce-173">Строка</span><span class="sxs-lookup"><span data-stu-id="6f8ce-173">String</span></span>|<span data-ttu-id="6f8ce-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6f8ce-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-176">version</span><span class="sxs-lookup"><span data-stu-id="6f8ce-176">version</span></span>|<span data-ttu-id="6f8ce-177">Int32</span><span class="sxs-lookup"><span data-stu-id="6f8ce-177">Int32</span></span>|<span data-ttu-id="6f8ce-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-178">Version of the device configuration.</span></span> <span data-ttu-id="6f8ce-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="6f8ce-180">networkName</span></span>|<span data-ttu-id="6f8ce-181">Строка</span><span class="sxs-lookup"><span data-stu-id="6f8ce-181">String</span></span>|<span data-ttu-id="6f8ce-182">Сетевое имя, унаследованное от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f8ce-182">Network Name Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-183">SSID</span><span class="sxs-lookup"><span data-stu-id="6f8ce-183">ssid</span></span>|<span data-ttu-id="6f8ce-184">Строка</span><span class="sxs-lookup"><span data-stu-id="6f8ce-184">String</span></span>|<span data-ttu-id="6f8ce-185">Это имя Wi-Fiной сети, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="6f8ce-186">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f8ce-186">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-187">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="6f8ce-187">connectAutomatically</span></span>|<span data-ttu-id="6f8ce-188">Логический</span><span class="sxs-lookup"><span data-stu-id="6f8ce-188">Boolean</span></span>|<span data-ttu-id="6f8ce-189">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="6f8ce-190">Если задать для этого параметра значение true, запрос пользователя будет пропущен и устройство будет автоматически подключено к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="6f8ce-191">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f8ce-191">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-192">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="6f8ce-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="6f8ce-193">Логический</span><span class="sxs-lookup"><span data-stu-id="6f8ce-193">Boolean</span></span>|<span data-ttu-id="6f8ce-194">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="6f8ce-195">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f8ce-195">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-196">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="6f8ce-196">wiFiSecurityType</span></span>|[<span data-ttu-id="6f8ce-197">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="6f8ce-197">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="6f8ce-198">Указывает, использует ли конечная точка Wi-Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="6f8ce-199">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-199">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span> <span data-ttu-id="6f8ce-200">Возможные значения: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-200">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="6f8ce-201">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="6f8ce-201">preSharedKey</span></span>|<span data-ttu-id="6f8ce-202">Строка</span><span class="sxs-lookup"><span data-stu-id="6f8ce-202">String</span></span>|<span data-ttu-id="6f8ce-203">Это предварительно общий ключ для сети WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-203">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="6f8ce-204">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f8ce-204">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-205">прешаредкэйиссет</span><span class="sxs-lookup"><span data-stu-id="6f8ce-205">preSharedKeyIsSet</span></span>|<span data-ttu-id="6f8ce-206">Логический</span><span class="sxs-lookup"><span data-stu-id="6f8ce-206">Boolean</span></span>|<span data-ttu-id="6f8ce-207">Это предварительно общий ключ для сети WPA Personal Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-207">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span> <span data-ttu-id="6f8ce-208">Наследуется от [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6f8ce-208">Inherited from [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)</span></span>|
|<span data-ttu-id="6f8ce-209">еаптипе</span><span class="sxs-lookup"><span data-stu-id="6f8ce-209">eapType</span></span>|[<span data-ttu-id="6f8ce-210">андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="6f8ce-210">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="6f8ce-211">Указывает тип протокола EAP, заданный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="6f8ce-211">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="6f8ce-212">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-212">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="6f8ce-213">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="6f8ce-213">authenticationMethod</span></span>|[<span data-ttu-id="6f8ce-214">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="6f8ce-214">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="6f8ce-215">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-215">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="6f8ce-216">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-216">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="6f8ce-217">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="6f8ce-217">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="6f8ce-218">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="6f8ce-218">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="6f8ce-219">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-219">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="6f8ce-220">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-220">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6f8ce-221">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="6f8ce-221">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="6f8ce-222">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="6f8ce-222">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="6f8ce-223">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-223">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="6f8ce-224">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-224">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="6f8ce-225">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="6f8ce-225">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="6f8ce-226">Строка</span><span class="sxs-lookup"><span data-stu-id="6f8ce-226">String</span></span>|<span data-ttu-id="6f8ce-227">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-227">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="6f8ce-228">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-228">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="6f8ce-229">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f8ce-229">Response</span></span>
<span data-ttu-id="6f8ce-230">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроиддевицеовнерентерприсевификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-230">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f8ce-231">Пример</span><span class="sxs-lookup"><span data-stu-id="6f8ce-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f8ce-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f8ce-232">Request</span></span>
<span data-ttu-id="6f8ce-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6f8ce-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f8ce-234">Response</span></span>
<span data-ttu-id="6f8ce-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f8ce-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





