---
title: Обновление Андроиддевицеовнервификонфигуратион
description: Обновление свойств объекта Андроиддевицеовнервификонфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 71690f873cff0526a125cb05f94621d067e5554a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43349728"
---
# <a name="update-androiddeviceownerwificonfiguration"></a><span data-ttu-id="8b56a-103">Обновление Андроиддевицеовнервификонфигуратион</span><span class="sxs-lookup"><span data-stu-id="8b56a-103">Update androidDeviceOwnerWiFiConfiguration</span></span>

<span data-ttu-id="8b56a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b56a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b56a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b56a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b56a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b56a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b56a-107">Обновление свойств объекта [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8b56a-107">Update the properties of a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b56a-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8b56a-108">Prerequisites</span></span>
<span data-ttu-id="8b56a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b56a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b56a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b56a-111">Permission type</span></span>|<span data-ttu-id="8b56a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b56a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b56a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b56a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b56a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b56a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8b56a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b56a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b56a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b56a-116">Not supported.</span></span>|
|<span data-ttu-id="8b56a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b56a-117">Application</span></span>|<span data-ttu-id="8b56a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b56a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b56a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b56a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8b56a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8b56a-120">Request headers</span></span>
|<span data-ttu-id="8b56a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b56a-121">Header</span></span>|<span data-ttu-id="8b56a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8b56a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b56a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b56a-123">Authorization</span></span>|<span data-ttu-id="8b56a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b56a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b56a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8b56a-125">Accept</span></span>|<span data-ttu-id="8b56a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b56a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b56a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b56a-127">Request body</span></span>
<span data-ttu-id="8b56a-128">В тексте запроса добавьте представление объекта [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b56a-128">In the request body, supply a JSON representation for the [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

<span data-ttu-id="8b56a-129">В следующей таблице приведены свойства, необходимые при создании [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b56a-129">The following table shows the properties that are required when you create the [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).</span></span>

|<span data-ttu-id="8b56a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b56a-130">Property</span></span>|<span data-ttu-id="8b56a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8b56a-131">Type</span></span>|<span data-ttu-id="8b56a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8b56a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b56a-133">id</span><span class="sxs-lookup"><span data-stu-id="8b56a-133">id</span></span>|<span data-ttu-id="8b56a-134">String</span><span class="sxs-lookup"><span data-stu-id="8b56a-134">String</span></span>|<span data-ttu-id="8b56a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8b56a-135">Key of the entity.</span></span> <span data-ttu-id="8b56a-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b56a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b56a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b56a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8b56a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b56a-138">DateTimeOffset</span></span>|<span data-ttu-id="8b56a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8b56a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8b56a-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b56a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b56a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8b56a-141">roleScopeTagIds</span></span>|<span data-ttu-id="8b56a-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="8b56a-142">String collection</span></span>|<span data-ttu-id="8b56a-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8b56a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8b56a-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b56a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b56a-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8b56a-145">supportsScopeTags</span></span>|<span data-ttu-id="8b56a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b56a-146">Boolean</span></span>|<span data-ttu-id="8b56a-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8b56a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8b56a-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8b56a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8b56a-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8b56a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8b56a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8b56a-150">This property is read-only.</span></span> <span data-ttu-id="8b56a-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b56a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b56a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8b56a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8b56a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8b56a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8b56a-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8b56a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8b56a-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b56a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b56a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8b56a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8b56a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8b56a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8b56a-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8b56a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8b56a-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b56a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b56a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8b56a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8b56a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8b56a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8b56a-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8b56a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8b56a-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b56a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b56a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b56a-164">createdDateTime</span></span>|<span data-ttu-id="8b56a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b56a-165">DateTimeOffset</span></span>|<span data-ttu-id="8b56a-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8b56a-166">DateTime the object was created.</span></span> <span data-ttu-id="8b56a-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b56a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b56a-168">description</span><span class="sxs-lookup"><span data-stu-id="8b56a-168">description</span></span>|<span data-ttu-id="8b56a-169">String</span><span class="sxs-lookup"><span data-stu-id="8b56a-169">String</span></span>|<span data-ttu-id="8b56a-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8b56a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8b56a-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b56a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b56a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="8b56a-172">displayName</span></span>|<span data-ttu-id="8b56a-173">Строка</span><span class="sxs-lookup"><span data-stu-id="8b56a-173">String</span></span>|<span data-ttu-id="8b56a-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8b56a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8b56a-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b56a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b56a-176">version</span><span class="sxs-lookup"><span data-stu-id="8b56a-176">version</span></span>|<span data-ttu-id="8b56a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="8b56a-177">Int32</span></span>|<span data-ttu-id="8b56a-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8b56a-178">Version of the device configuration.</span></span> <span data-ttu-id="8b56a-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8b56a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b56a-180">нетворкнаме</span><span class="sxs-lookup"><span data-stu-id="8b56a-180">networkName</span></span>|<span data-ttu-id="8b56a-181">String</span><span class="sxs-lookup"><span data-stu-id="8b56a-181">String</span></span>|<span data-ttu-id="8b56a-182">Сетевое имя</span><span class="sxs-lookup"><span data-stu-id="8b56a-182">Network Name</span></span>|
|<span data-ttu-id="8b56a-183">SSID</span><span class="sxs-lookup"><span data-stu-id="8b56a-183">ssid</span></span>|<span data-ttu-id="8b56a-184">String</span><span class="sxs-lookup"><span data-stu-id="8b56a-184">String</span></span>|<span data-ttu-id="8b56a-185">Это имя сети Wi-Fi, которая отправляется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="8b56a-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="8b56a-186">коннектаутоматикалли</span><span class="sxs-lookup"><span data-stu-id="8b56a-186">connectAutomatically</span></span>|<span data-ttu-id="8b56a-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b56a-187">Boolean</span></span>|<span data-ttu-id="8b56a-188">Подключаться автоматически, если сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="8b56a-188">Connect automatically when this network is in range.</span></span> <span data-ttu-id="8b56a-189">Если задать для этого параметра значение true, запрос пользователя будет пропущен и автоматически подключено устройство к сети Wi/Fi.</span><span class="sxs-lookup"><span data-stu-id="8b56a-189">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="8b56a-190">коннектвхеннетворкнамеишидден</span><span class="sxs-lookup"><span data-stu-id="8b56a-190">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="8b56a-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b56a-191">Boolean</span></span>|<span data-ttu-id="8b56a-192">Если задано значение true, этот профиль заставляет устройство подключаться к сети, на которой не выполняется трансляция идентификатора SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="8b56a-192">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="8b56a-193">вифисекурититипе</span><span class="sxs-lookup"><span data-stu-id="8b56a-193">wiFiSecurityType</span></span>|[<span data-ttu-id="8b56a-194">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="8b56a-194">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="8b56a-195">Указывает, использует ли конечная точка Wi/Fi тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="8b56a-195">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="8b56a-196">Возможные значения: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="8b56a-196">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="8b56a-197">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="8b56a-197">preSharedKey</span></span>|<span data-ttu-id="8b56a-198">String</span><span class="sxs-lookup"><span data-stu-id="8b56a-198">String</span></span>|<span data-ttu-id="8b56a-199">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="8b56a-199">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="8b56a-200">прешаредкэйиссет</span><span class="sxs-lookup"><span data-stu-id="8b56a-200">preSharedKeyIsSet</span></span>|<span data-ttu-id="8b56a-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b56a-201">Boolean</span></span>|<span data-ttu-id="8b56a-202">Это предварительно общий ключ для частной сети Wi-Fi WPA.</span><span class="sxs-lookup"><span data-stu-id="8b56a-202">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="8b56a-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b56a-203">Response</span></span>
<span data-ttu-id="8b56a-204">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроиддевицеовнервификонфигуратион](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b56a-204">If successful, this method returns a `200 OK` response code and an updated [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b56a-205">Пример</span><span class="sxs-lookup"><span data-stu-id="8b56a-205">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b56a-206">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b56a-206">Request</span></span>
<span data-ttu-id="8b56a-207">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b56a-207">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1282

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
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
  "preSharedKeyIsSet": true
}
```

### <a name="response"></a><span data-ttu-id="8b56a-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b56a-208">Response</span></span>
<span data-ttu-id="8b56a-p115">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b56a-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1454

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "id": "8d25beba-beba-8d25-babe-258dbabe258d",
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
  "preSharedKeyIsSet": true
}
```



