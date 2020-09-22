---
title: Создание Андроидворкпрофилинтерприсевификонфигуратион
description: Создание нового объекта Андроидворкпрофилинтерприсевификонфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fe2148a77661c4691ca9dc22510344128cae7107
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024985"
---
# <a name="create-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="f3d74-103">Создание Андроидворкпрофилинтерприсевификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="f3d74-103">Create androidWorkProfileEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="f3d74-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3d74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3d74-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3d74-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3d74-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f3d74-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3d74-107">Создание нового объекта [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f3d74-107">Create a new [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3d74-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f3d74-108">Prerequisites</span></span>
<span data-ttu-id="f3d74-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3d74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3d74-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3d74-111">Permission type</span></span>|<span data-ttu-id="f3d74-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3d74-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3d74-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3d74-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3d74-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3d74-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3d74-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3d74-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3d74-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3d74-116">Not supported.</span></span>|
|<span data-ttu-id="f3d74-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3d74-117">Application</span></span>|<span data-ttu-id="f3d74-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3d74-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3d74-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3d74-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f3d74-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f3d74-120">Request headers</span></span>
|<span data-ttu-id="f3d74-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3d74-121">Header</span></span>|<span data-ttu-id="f3d74-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3d74-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3d74-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3d74-123">Authorization</span></span>|<span data-ttu-id="f3d74-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3d74-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3d74-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3d74-125">Accept</span></span>|<span data-ttu-id="f3d74-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3d74-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3d74-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f3d74-127">Request body</span></span>
<span data-ttu-id="f3d74-128">В тексте запроса добавьте представление объекта Андроидворкпрофилинтерприсевификонфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3d74-128">In the request body, supply a JSON representation for the androidWorkProfileEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="f3d74-129">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилинтерприсевификонфигуратион.</span><span class="sxs-lookup"><span data-stu-id="f3d74-129">The following table shows the properties that are required when you create the androidWorkProfileEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="f3d74-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3d74-130">Property</span></span>|<span data-ttu-id="f3d74-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f3d74-131">Type</span></span>|<span data-ttu-id="f3d74-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f3d74-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3d74-133">id</span><span class="sxs-lookup"><span data-stu-id="f3d74-133">id</span></span>|<span data-ttu-id="f3d74-134">String</span><span class="sxs-lookup"><span data-stu-id="f3d74-134">String</span></span>|<span data-ttu-id="f3d74-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f3d74-135">Key of the entity.</span></span> <span data-ttu-id="f3d74-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3d74-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3d74-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f3d74-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3d74-138">DateTimeOffset</span></span>|<span data-ttu-id="f3d74-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f3d74-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f3d74-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3d74-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f3d74-141">roleScopeTagIds</span></span>|<span data-ttu-id="f3d74-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f3d74-142">String collection</span></span>|<span data-ttu-id="f3d74-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f3d74-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f3d74-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3d74-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f3d74-145">supportsScopeTags</span></span>|<span data-ttu-id="f3d74-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3d74-146">Boolean</span></span>|<span data-ttu-id="f3d74-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f3d74-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f3d74-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f3d74-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f3d74-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f3d74-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f3d74-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f3d74-150">This property is read-only.</span></span> <span data-ttu-id="f3d74-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3d74-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f3d74-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f3d74-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f3d74-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f3d74-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f3d74-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f3d74-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3d74-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f3d74-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f3d74-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f3d74-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f3d74-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f3d74-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f3d74-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3d74-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f3d74-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f3d74-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f3d74-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f3d74-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f3d74-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f3d74-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3d74-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3d74-164">createdDateTime</span></span>|<span data-ttu-id="f3d74-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3d74-165">DateTimeOffset</span></span>|<span data-ttu-id="f3d74-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f3d74-166">DateTime the object was created.</span></span> <span data-ttu-id="f3d74-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3d74-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-168">description</span><span class="sxs-lookup"><span data-stu-id="f3d74-168">description</span></span>|<span data-ttu-id="f3d74-169">String</span><span class="sxs-lookup"><span data-stu-id="f3d74-169">String</span></span>|<span data-ttu-id="f3d74-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f3d74-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f3d74-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3d74-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f3d74-172">displayName</span></span>|<span data-ttu-id="f3d74-173">String</span><span class="sxs-lookup"><span data-stu-id="f3d74-173">String</span></span>|<span data-ttu-id="f3d74-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f3d74-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f3d74-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3d74-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-176">version</span><span class="sxs-lookup"><span data-stu-id="f3d74-176">version</span></span>|<span data-ttu-id="f3d74-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f3d74-177">Int32</span></span>|<span data-ttu-id="f3d74-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f3d74-178">Version of the device configuration.</span></span> <span data-ttu-id="f3d74-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3d74-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="f3d74-180">networkName</span></span>|<span data-ttu-id="f3d74-181">String</span><span class="sxs-lookup"><span data-stu-id="f3d74-181">String</span></span>|<span data-ttu-id="f3d74-182">Сетевое имя, унаследованное от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d74-182">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-183">SSID</span><span class="sxs-lookup"><span data-stu-id="f3d74-183">ssid</span></span>|<span data-ttu-id="f3d74-184">String</span><span class="sxs-lookup"><span data-stu-id="f3d74-184">String</span></span>|<span data-ttu-id="f3d74-185">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="f3d74-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="f3d74-186">Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d74-186">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-187">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="f3d74-187">connectAutomatically</span></span>|<span data-ttu-id="f3d74-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3d74-188">Boolean</span></span>|<span data-ttu-id="f3d74-189">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="f3d74-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f3d74-190">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="f3d74-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="f3d74-191">Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d74-191">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-192">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="f3d74-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f3d74-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3d74-193">Boolean</span></span>|<span data-ttu-id="f3d74-194">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="f3d74-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="f3d74-195">Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3d74-195">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="f3d74-196">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="f3d74-196">wiFiSecurityType</span></span>|[<span data-ttu-id="f3d74-197">андроидвифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="f3d74-197">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="f3d74-198">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="f3d74-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f3d74-199">Наследуется от [андроидворкпрофилевификонфигуратион](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f3d74-199">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="f3d74-200">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="f3d74-200">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="f3d74-201">еаптипе</span><span class="sxs-lookup"><span data-stu-id="f3d74-201">eapType</span></span>|[<span data-ttu-id="f3d74-202">андроидеаптипе</span><span class="sxs-lookup"><span data-stu-id="f3d74-202">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="f3d74-203">Указывает тип протокола EAP, установленный для конечной точки Wi-Fi (маршрутизатора).</span><span class="sxs-lookup"><span data-stu-id="f3d74-203">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="f3d74-204">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="f3d74-204">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="f3d74-205">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="f3d74-205">authenticationMethod</span></span>|[<span data-ttu-id="f3d74-206">вифиаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="f3d74-206">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="f3d74-207">Указывает метод проверки подлинности, который должен использоваться клиентом (устройством), если тип EAP настроен для протокола PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="f3d74-207">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="f3d74-208">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="f3d74-208">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="f3d74-209">Свойства innerauthenticationprotocolforeapttls</span><span class="sxs-lookup"><span data-stu-id="f3d74-209">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="f3d74-210">нонеапаусентикатионмесодфореапттлстипе</span><span class="sxs-lookup"><span data-stu-id="f3d74-210">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="f3d74-211">Метод проверки подлинности (внутреннее удостоверение), не относящийся к EAP, если тип EAP — EAP-TTLS, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="f3d74-211">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="f3d74-212">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="f3d74-212">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="f3d74-213">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="f3d74-213">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="f3d74-214">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="f3d74-214">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="f3d74-215">Метод проверки подлинности, отличный от EAP (внутреннее удостоверение), если тип EAP — PEAP, а параметр authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="f3d74-215">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="f3d74-216">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="f3d74-216">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="f3d74-217">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="f3d74-217">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="f3d74-218">String</span><span class="sxs-lookup"><span data-stu-id="f3d74-218">String</span></span>|<span data-ttu-id="f3d74-219">Включите конфиденциальность удостоверений (внешнее удостоверение), если тип EAP настроен для EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="f3d74-219">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="f3d74-220">Приведенная здесь строка используется для маскирования имени пользователя отдельных пользователей при попытке подключения к сети Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f3d74-220">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="f3d74-221">proxySettings</span><span class="sxs-lookup"><span data-stu-id="f3d74-221">proxySettings</span></span>|[<span data-ttu-id="f3d74-222">вифипроксисеттинг</span><span class="sxs-lookup"><span data-stu-id="f3d74-222">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="f3d74-223">Тип прокси-сервера для этого подключения Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f3d74-223">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="f3d74-224">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="f3d74-224">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="f3d74-225">проксяутоматикконфигуратионурл</span><span class="sxs-lookup"><span data-stu-id="f3d74-225">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="f3d74-226">String</span><span class="sxs-lookup"><span data-stu-id="f3d74-226">String</span></span>|<span data-ttu-id="f3d74-227">URL-адрес скрипта автоматической настройки прокси-сервера при выборе параметра Автоматическая настройка.</span><span class="sxs-lookup"><span data-stu-id="f3d74-227">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="f3d74-228">Обычно это URL-адрес файла PAC (Автонастройка прокси-сервера).</span><span class="sxs-lookup"><span data-stu-id="f3d74-228">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|



## <a name="response"></a><span data-ttu-id="f3d74-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3d74-229">Response</span></span>
<span data-ttu-id="f3d74-230">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилинтерприсевификонфигуратион](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f3d74-230">If successful, this method returns a `201 Created` response code and a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3d74-231">Пример</span><span class="sxs-lookup"><span data-stu-id="f3d74-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3d74-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3d74-232">Request</span></span>
<span data-ttu-id="f3d74-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3d74-233">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1671

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "proxySettings": "manual",
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/"
}
```

### <a name="response"></a><span data-ttu-id="f3d74-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3d74-234">Response</span></span>
<span data-ttu-id="f3d74-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f3d74-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1843

{
  "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
  "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
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
  "wiFiSecurityType": "wpaEnterprise",
  "eapType": "eapTtls",
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
  "proxySettings": "manual",
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/"
}
```






