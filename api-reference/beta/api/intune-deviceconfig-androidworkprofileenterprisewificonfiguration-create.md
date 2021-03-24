---
title: Создание androidWorkProfileEnterpriseWiFiConfiguration
description: Создайте новый объект AndroidWorkProfileEnterpriseWiFiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab1c27d72ea671900f177a099806b2e991f2a957
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126579"
---
# <a name="create-androidworkprofileenterprisewificonfiguration"></a><span data-ttu-id="ea42d-103">Создание androidWorkProfileEnterpriseWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea42d-103">Create androidWorkProfileEnterpriseWiFiConfiguration</span></span>

<span data-ttu-id="ea42d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea42d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea42d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea42d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea42d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea42d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea42d-107">Создайте новый [объект AndroidWorkProfileEnterpriseWiFiConfiguration.](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea42d-107">Create a new [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea42d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ea42d-108">Prerequisites</span></span>
<span data-ttu-id="ea42d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea42d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea42d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea42d-111">Permission type</span></span>|<span data-ttu-id="ea42d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea42d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea42d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea42d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea42d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea42d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea42d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea42d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea42d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea42d-116">Not supported.</span></span>|
|<span data-ttu-id="ea42d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ea42d-117">Application</span></span>|<span data-ttu-id="ea42d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea42d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea42d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea42d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ea42d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ea42d-120">Request headers</span></span>
|<span data-ttu-id="ea42d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea42d-121">Header</span></span>|<span data-ttu-id="ea42d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ea42d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea42d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea42d-123">Authorization</span></span>|<span data-ttu-id="ea42d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea42d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea42d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ea42d-125">Accept</span></span>|<span data-ttu-id="ea42d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea42d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea42d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea42d-127">Request body</span></span>
<span data-ttu-id="ea42d-128">В теле запроса предоставляем представление JSON для объекта AndroidWorkProfileEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ea42d-128">In the request body, supply a JSON representation for the androidWorkProfileEnterpriseWiFiConfiguration object.</span></span>

<span data-ttu-id="ea42d-129">В следующей таблице показаны свойства, необходимые при создании androidWorkProfileEnterpriseWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ea42d-129">The following table shows the properties that are required when you create the androidWorkProfileEnterpriseWiFiConfiguration.</span></span>

|<span data-ttu-id="ea42d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea42d-130">Property</span></span>|<span data-ttu-id="ea42d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ea42d-131">Type</span></span>|<span data-ttu-id="ea42d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ea42d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea42d-133">id</span><span class="sxs-lookup"><span data-stu-id="ea42d-133">id</span></span>|<span data-ttu-id="ea42d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ea42d-134">String</span></span>|<span data-ttu-id="ea42d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ea42d-135">Key of the entity.</span></span> <span data-ttu-id="ea42d-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea42d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea42d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ea42d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea42d-138">DateTimeOffset</span></span>|<span data-ttu-id="ea42d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ea42d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ea42d-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea42d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ea42d-141">roleScopeTagIds</span></span>|<span data-ttu-id="ea42d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea42d-142">String collection</span></span>|<span data-ttu-id="ea42d-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="ea42d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ea42d-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea42d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ea42d-145">supportsScopeTags</span></span>|<span data-ttu-id="ea42d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea42d-146">Boolean</span></span>|<span data-ttu-id="ea42d-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="ea42d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ea42d-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="ea42d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ea42d-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ea42d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ea42d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea42d-150">This property is read-only.</span></span> <span data-ttu-id="ea42d-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea42d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ea42d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ea42d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ea42d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ea42d-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ea42d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ea42d-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea42d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ea42d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ea42d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ea42d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ea42d-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ea42d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ea42d-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea42d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ea42d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ea42d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ea42d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ea42d-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="ea42d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ea42d-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea42d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea42d-164">createdDateTime</span></span>|<span data-ttu-id="ea42d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea42d-165">DateTimeOffset</span></span>|<span data-ttu-id="ea42d-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ea42d-166">DateTime the object was created.</span></span> <span data-ttu-id="ea42d-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea42d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-168">description</span><span class="sxs-lookup"><span data-stu-id="ea42d-168">description</span></span>|<span data-ttu-id="ea42d-169">Строка</span><span class="sxs-lookup"><span data-stu-id="ea42d-169">String</span></span>|<span data-ttu-id="ea42d-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ea42d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ea42d-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea42d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ea42d-172">displayName</span></span>|<span data-ttu-id="ea42d-173">Строка</span><span class="sxs-lookup"><span data-stu-id="ea42d-173">String</span></span>|<span data-ttu-id="ea42d-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ea42d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ea42d-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea42d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-176">version</span><span class="sxs-lookup"><span data-stu-id="ea42d-176">version</span></span>|<span data-ttu-id="ea42d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ea42d-177">Int32</span></span>|<span data-ttu-id="ea42d-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ea42d-178">Version of the device configuration.</span></span> <span data-ttu-id="ea42d-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea42d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-180">networkName</span><span class="sxs-lookup"><span data-stu-id="ea42d-180">networkName</span></span>|<span data-ttu-id="ea42d-181">Строка</span><span class="sxs-lookup"><span data-stu-id="ea42d-181">String</span></span>|<span data-ttu-id="ea42d-182">Имя сети, унаследованные от [AndroidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea42d-182">Network Name Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-183">ssid</span><span class="sxs-lookup"><span data-stu-id="ea42d-183">ssid</span></span>|<span data-ttu-id="ea42d-184">Строка</span><span class="sxs-lookup"><span data-stu-id="ea42d-184">String</span></span>|<span data-ttu-id="ea42d-185">Это имя сети Wi-Fi, которая транслируется на все устройства.</span><span class="sxs-lookup"><span data-stu-id="ea42d-185">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span> <span data-ttu-id="ea42d-186">Унаследованный от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea42d-186">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-187">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="ea42d-187">connectAutomatically</span></span>|<span data-ttu-id="ea42d-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea42d-188">Boolean</span></span>|<span data-ttu-id="ea42d-189">Подключение автоматически, когда эта сеть находится в диапазоне.</span><span class="sxs-lookup"><span data-stu-id="ea42d-189">Connect automatically when this network is in range.</span></span> <span data-ttu-id="ea42d-190">Настройка этого параметра будет пропускать запрос пользователя и автоматически подключать устройство к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="ea42d-190">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span> <span data-ttu-id="ea42d-191">Унаследованный от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea42d-191">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-192">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="ea42d-192">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="ea42d-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea42d-193">Boolean</span></span>|<span data-ttu-id="ea42d-194">Если задана истина, этот профиль заставляет устройство подключаться к сети, которая не передает SSID на все устройства.</span><span class="sxs-lookup"><span data-stu-id="ea42d-194">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span> <span data-ttu-id="ea42d-195">Унаследованный от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea42d-195">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)</span></span>|
|<span data-ttu-id="ea42d-196">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="ea42d-196">wiFiSecurityType</span></span>|[<span data-ttu-id="ea42d-197">AndroidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="ea42d-197">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="ea42d-198">Указывает, Wi-Fi конечная точка использует тип безопасности на основе EAP.</span><span class="sxs-lookup"><span data-stu-id="ea42d-198">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="ea42d-199">Унаследовано от [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea42d-199">Inherited from [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md).</span></span> <span data-ttu-id="ea42d-200">Возможные значения: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span><span class="sxs-lookup"><span data-stu-id="ea42d-200">Possible values are: `open`, `wpaEnterprise`, `wpa2Enterprise`.</span></span>|
|<span data-ttu-id="ea42d-201">eapType</span><span class="sxs-lookup"><span data-stu-id="ea42d-201">eapType</span></span>|[<span data-ttu-id="ea42d-202">androidEapType</span><span class="sxs-lookup"><span data-stu-id="ea42d-202">androidEapType</span></span>](../resources/intune-deviceconfig-androideaptype.md)|<span data-ttu-id="ea42d-203">Указывает тип протокола EAP на конечной точке Wi-Fi (маршрутизатор).</span><span class="sxs-lookup"><span data-stu-id="ea42d-203">Indicates the type of EAP protocol set on the Wi-Fi endpoint (router).</span></span> <span data-ttu-id="ea42d-204">Возможные значения: `eapTls`, `eapTtls`, `peap`.</span><span class="sxs-lookup"><span data-stu-id="ea42d-204">Possible values are: `eapTls`, `eapTtls`, `peap`.</span></span>|
|<span data-ttu-id="ea42d-205">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ea42d-205">authenticationMethod</span></span>|[<span data-ttu-id="ea42d-206">wiFiAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ea42d-206">wiFiAuthenticationMethod</span></span>](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|<span data-ttu-id="ea42d-207">Указывает метод проверки подлинности, который клиент (устройство) должен использовать, когда тип EAP настроен на PEAP или EAP-TTLS.</span><span class="sxs-lookup"><span data-stu-id="ea42d-207">Indicates the Authentication Method the client (device) needs to use when the EAP Type is configured to PEAP or EAP-TTLS.</span></span> <span data-ttu-id="ea42d-208">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="ea42d-208">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ea42d-209">innerAuthenticationProtocolForEapTtls</span><span class="sxs-lookup"><span data-stu-id="ea42d-209">innerAuthenticationProtocolForEapTtls</span></span>|[<span data-ttu-id="ea42d-210">nonEapAuthenticationMethodForEapTtlsType</span><span class="sxs-lookup"><span data-stu-id="ea42d-210">nonEapAuthenticationMethodForEapTtlsType</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|<span data-ttu-id="ea42d-211">Метод без EAP для проверки подлинности (внутренняя идентичность), когда тип EAP EAP-TTLS и authenticationmethod — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="ea42d-211">Non-EAP Method for Authentication (Inner Identity) when EAP Type is EAP-TTLS and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="ea42d-212">Возможные значения: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="ea42d-212">Possible values are: `unencryptedPassword`, `challengeHandshakeAuthenticationProtocol`, `microsoftChap`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="ea42d-213">innerAuthenticationProtocolForPeap</span><span class="sxs-lookup"><span data-stu-id="ea42d-213">innerAuthenticationProtocolForPeap</span></span>|[<span data-ttu-id="ea42d-214">nonEapAuthenticationMethodForPeap</span><span class="sxs-lookup"><span data-stu-id="ea42d-214">nonEapAuthenticationMethodForPeap</span></span>](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|<span data-ttu-id="ea42d-215">Метод без EAP для проверки подлинности (внутренняя идентичность), когда тип EAP — PEAP, а проверка подлинности — имя пользователя и пароль.</span><span class="sxs-lookup"><span data-stu-id="ea42d-215">Non-EAP Method for Authentication (Inner Identity) when EAP Type is PEAP and Authenticationmethod is Username and Password.</span></span> <span data-ttu-id="ea42d-216">Возможные значения: `none`, `microsoftChapVersionTwo`.</span><span class="sxs-lookup"><span data-stu-id="ea42d-216">Possible values are: `none`, `microsoftChapVersionTwo`.</span></span>|
|<span data-ttu-id="ea42d-217">outerIdentityPrivacyTemporaryValue</span><span class="sxs-lookup"><span data-stu-id="ea42d-217">outerIdentityPrivacyTemporaryValue</span></span>|<span data-ttu-id="ea42d-218">Строка</span><span class="sxs-lookup"><span data-stu-id="ea42d-218">String</span></span>|<span data-ttu-id="ea42d-219">Введите конфиденциальность удостоверений (внешний идентификатор), если тип EAP настроен на EAP-TTLS или PEAP.</span><span class="sxs-lookup"><span data-stu-id="ea42d-219">Enable identity privacy (Outer Identity) when EAP Type is configured to EAP-TTLS or PEAP.</span></span> <span data-ttu-id="ea42d-220">Строка, представленная здесь, используется для маскировки имени пользователя отдельных пользователей при попытке подключения к Wi-Fi сети.</span><span class="sxs-lookup"><span data-stu-id="ea42d-220">The String provided here is used to mask the username of individual users when they attempt to connect to Wi-Fi network.</span></span>|
|<span data-ttu-id="ea42d-221">proxySettings</span><span class="sxs-lookup"><span data-stu-id="ea42d-221">proxySettings</span></span>|[<span data-ttu-id="ea42d-222">wiFiProxySetting</span><span class="sxs-lookup"><span data-stu-id="ea42d-222">wiFiProxySetting</span></span>](../resources/intune-deviceconfig-wifiproxysetting.md)|<span data-ttu-id="ea42d-223">Тип прокси для Wi-Fi подключения.</span><span class="sxs-lookup"><span data-stu-id="ea42d-223">Proxy Type for this Wi-Fi connection.</span></span> <span data-ttu-id="ea42d-224">Возможные значения: `none`, `manual`, `automatic`.</span><span class="sxs-lookup"><span data-stu-id="ea42d-224">Possible values are: `none`, `manual`, `automatic`.</span></span>|
|<span data-ttu-id="ea42d-225">proxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="ea42d-225">proxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="ea42d-226">Строка</span><span class="sxs-lookup"><span data-stu-id="ea42d-226">String</span></span>|<span data-ttu-id="ea42d-227">URL-адрес сценария автоматической конфигурации прокси-сервера при выборе автоматической конфигурации.</span><span class="sxs-lookup"><span data-stu-id="ea42d-227">URL of the proxy server automatic configuration script when automatic configuration is selected.</span></span> <span data-ttu-id="ea42d-228">Этот URL-адрес обычно является расположением файла PAC (Proxy Auto Configuration).</span><span class="sxs-lookup"><span data-stu-id="ea42d-228">This URL is typically the location of PAC (Proxy Auto Configuration) file.</span></span>|



## <a name="response"></a><span data-ttu-id="ea42d-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea42d-229">Response</span></span>
<span data-ttu-id="ea42d-230">В случае успеха этот метод возвращает код отклика и `201 Created` [объект AndroidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ea42d-230">If successful, this method returns a `201 Created` response code and a [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea42d-231">Пример</span><span class="sxs-lookup"><span data-stu-id="ea42d-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea42d-232">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea42d-232">Request</span></span>
<span data-ttu-id="ea42d-233">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea42d-233">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ea42d-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea42d-234">Response</span></span>
<span data-ttu-id="ea42d-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea42d-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




