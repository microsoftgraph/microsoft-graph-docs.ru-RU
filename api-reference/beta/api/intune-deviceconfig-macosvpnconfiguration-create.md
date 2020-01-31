---
title: Создание Макосвпнконфигуратион
description: Создание нового объекта Макосвпнконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c0340c5e9b5e985e5311562ff6eb374262e15540
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635820"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="4f4d1-103">Создание Макосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4f4d1-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="4f4d1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f4d1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f4d1-106">Создание нового объекта [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4f4d1-106">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f4d1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4f4d1-107">Prerequisites</span></span>
<span data-ttu-id="4f4d1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f4d1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f4d1-110">Permission type</span></span>|<span data-ttu-id="4f4d1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f4d1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f4d1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f4d1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f4d1-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f4d1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-115">Not supported.</span></span>|
|<span data-ttu-id="4f4d1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f4d1-116">Application</span></span>|<span data-ttu-id="4f4d1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f4d1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f4d1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f4d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4f4d1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4f4d1-119">Request headers</span></span>
|<span data-ttu-id="4f4d1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f4d1-120">Header</span></span>|<span data-ttu-id="4f4d1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4f4d1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f4d1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f4d1-122">Authorization</span></span>|<span data-ttu-id="4f4d1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f4d1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4f4d1-124">Accept</span></span>|<span data-ttu-id="4f4d1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f4d1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f4d1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f4d1-126">Request body</span></span>
<span data-ttu-id="4f4d1-127">В тексте запроса добавьте представление объекта Макосвпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-127">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="4f4d1-128">В следующей таблице приведены свойства, необходимые при создании Макосвпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-128">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="4f4d1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f4d1-129">Property</span></span>|<span data-ttu-id="4f4d1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4f4d1-130">Type</span></span>|<span data-ttu-id="4f4d1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4f4d1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f4d1-132">id</span><span class="sxs-lookup"><span data-stu-id="4f4d1-132">id</span></span>|<span data-ttu-id="4f4d1-133">String</span><span class="sxs-lookup"><span data-stu-id="4f4d1-133">String</span></span>|<span data-ttu-id="4f4d1-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-134">Key of the entity.</span></span> <span data-ttu-id="4f4d1-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f4d1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4f4d1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f4d1-137">DateTimeOffset</span></span>|<span data-ttu-id="4f4d1-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4f4d1-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f4d1-140">roleScopeTagIds</span></span>|<span data-ttu-id="4f4d1-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4f4d1-141">String collection</span></span>|<span data-ttu-id="4f4d1-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4f4d1-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4f4d1-144">supportsScopeTags</span></span>|<span data-ttu-id="4f4d1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f4d1-145">Boolean</span></span>|<span data-ttu-id="4f4d1-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4f4d1-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4f4d1-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4f4d1-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-149">This property is read-only.</span></span> <span data-ttu-id="4f4d1-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4f4d1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4f4d1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4f4d1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4f4d1-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4f4d1-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4f4d1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4f4d1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4f4d1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4f4d1-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4f4d1-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4f4d1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4f4d1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4f4d1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4f4d1-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4f4d1-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f4d1-163">createdDateTime</span></span>|<span data-ttu-id="4f4d1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f4d1-164">DateTimeOffset</span></span>|<span data-ttu-id="4f4d1-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-165">DateTime the object was created.</span></span> <span data-ttu-id="4f4d1-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-167">description</span><span class="sxs-lookup"><span data-stu-id="4f4d1-167">description</span></span>|<span data-ttu-id="4f4d1-168">String</span><span class="sxs-lookup"><span data-stu-id="4f4d1-168">String</span></span>|<span data-ttu-id="4f4d1-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4f4d1-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4f4d1-171">displayName</span></span>|<span data-ttu-id="4f4d1-172">Строка</span><span class="sxs-lookup"><span data-stu-id="4f4d1-172">String</span></span>|<span data-ttu-id="4f4d1-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4f4d1-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-175">version</span><span class="sxs-lookup"><span data-stu-id="4f4d1-175">version</span></span>|<span data-ttu-id="4f4d1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4f4d1-176">Int32</span></span>|<span data-ttu-id="4f4d1-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-177">Version of the device configuration.</span></span> <span data-ttu-id="4f4d1-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-179">коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="4f4d1-179">connectionName</span></span>|<span data-ttu-id="4f4d1-180">Строка</span><span class="sxs-lookup"><span data-stu-id="4f4d1-180">String</span></span>|<span data-ttu-id="4f4d1-181">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-181">Connection name displayed to the user.</span></span> <span data-ttu-id="4f4d1-182">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-182">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-183">connectionType</span><span class="sxs-lookup"><span data-stu-id="4f4d1-183">connectionType</span></span>|[<span data-ttu-id="4f4d1-184">апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="4f4d1-184">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="4f4d1-185">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-185">Connection type.</span></span> <span data-ttu-id="4f4d1-186">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-186">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="4f4d1-187">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-187">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`, `ikEv2`, `alwaysOn`.</span></span>|
|<span data-ttu-id="4f4d1-188">логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="4f4d1-188">loginGroupOrDomain</span></span>|<span data-ttu-id="4f4d1-189">Строка</span><span class="sxs-lookup"><span data-stu-id="4f4d1-189">String</span></span>|<span data-ttu-id="4f4d1-190">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-190">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="4f4d1-191">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-191">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-192">role</span><span class="sxs-lookup"><span data-stu-id="4f4d1-192">role</span></span>|<span data-ttu-id="4f4d1-193">Строка</span><span class="sxs-lookup"><span data-stu-id="4f4d1-193">String</span></span>|<span data-ttu-id="4f4d1-194">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-194">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="4f4d1-195">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-195">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-196">область</span><span class="sxs-lookup"><span data-stu-id="4f4d1-196">realm</span></span>|<span data-ttu-id="4f4d1-197">Строка</span><span class="sxs-lookup"><span data-stu-id="4f4d1-197">String</span></span>|<span data-ttu-id="4f4d1-198">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-198">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="4f4d1-199">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-199">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-200">сервер</span><span class="sxs-lookup"><span data-stu-id="4f4d1-200">server</span></span>|[<span data-ttu-id="4f4d1-201">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-201">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="4f4d1-202">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-202">VPN Server on the network.</span></span> <span data-ttu-id="4f4d1-203">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-203">Make sure end users can access this network location.</span></span> <span data-ttu-id="4f4d1-204">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-204">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-205">идентификатор</span><span class="sxs-lookup"><span data-stu-id="4f4d1-205">identifier</span></span>|<span data-ttu-id="4f4d1-206">Строка</span><span class="sxs-lookup"><span data-stu-id="4f4d1-206">String</span></span>|<span data-ttu-id="4f4d1-207">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-207">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="4f4d1-208">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-208">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-209">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="4f4d1-209">customData</span></span>|<span data-ttu-id="4f4d1-210">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-210">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="4f4d1-211">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-211">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="4f4d1-212">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-212">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="4f4d1-213">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="4f4d1-213">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="4f4d1-214">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-214">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="4f4d1-215">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-215">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-216">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="4f4d1-216">customKeyValueData</span></span>|<span data-ttu-id="4f4d1-217">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-217">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4f4d1-218">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-218">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="4f4d1-219">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-219">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="4f4d1-220">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="4f4d1-220">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="4f4d1-221">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-221">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="4f4d1-222">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-222">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-223">енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="4f4d1-223">enableSplitTunneling</span></span>|<span data-ttu-id="4f4d1-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f4d1-224">Boolean</span></span>|<span data-ttu-id="4f4d1-225">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-225">Send all network traffic through VPN.</span></span> <span data-ttu-id="4f4d1-226">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-226">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-227">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="4f4d1-227">authenticationMethod</span></span>|[<span data-ttu-id="4f4d1-228">впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="4f4d1-228">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="4f4d1-229">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-229">Authentication method for this VPN connection.</span></span> <span data-ttu-id="4f4d1-230">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f4d1-230">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="4f4d1-231">Возможные значения: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-231">Possible values are: `certificate`, `usernameAndPassword`, `sharedSecret`, `derivedCredential`.</span></span>|
|<span data-ttu-id="4f4d1-232">енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="4f4d1-232">enablePerApp</span></span>|<span data-ttu-id="4f4d1-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f4d1-233">Boolean</span></span>|<span data-ttu-id="4f4d1-234">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту виртуальную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-234">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="4f4d1-235">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-235">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-236">сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="4f4d1-236">safariDomains</span></span>|<span data-ttu-id="4f4d1-237">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4f4d1-237">String collection</span></span>|<span data-ttu-id="4f4d1-238">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-238">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="4f4d1-239">Кроме приложений, связанных с этой виртуальной частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-239">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="4f4d1-240">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-240">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-241">ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="4f4d1-241">onDemandRules</span></span>|<span data-ttu-id="4f4d1-242">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-242">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="4f4d1-243">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-243">On-Demand Rules.</span></span> <span data-ttu-id="4f4d1-244">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-244">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="4f4d1-245">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-245">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-246">проксисервер</span><span class="sxs-lookup"><span data-stu-id="4f4d1-246">proxyServer</span></span>|[<span data-ttu-id="4f4d1-247">впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="4f4d1-247">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="4f4d1-248">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-248">Proxy Server.</span></span> <span data-ttu-id="4f4d1-249">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-249">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="4f4d1-250">оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="4f4d1-250">optInToDeviceIdSharing</span></span>|<span data-ttu-id="4f4d1-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f4d1-251">Boolean</span></span>|<span data-ttu-id="4f4d1-252">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-252">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="4f4d1-253">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f4d1-253">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="4f4d1-254">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f4d1-254">Response</span></span>
<span data-ttu-id="4f4d1-255">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-255">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f4d1-256">Пример</span><span class="sxs-lookup"><span data-stu-id="4f4d1-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f4d1-257">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f4d1-257">Request</span></span>
<span data-ttu-id="4f4d1-258">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2630

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="4f4d1-259">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f4d1-259">Response</span></span>
<span data-ttu-id="4f4d1-p129">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f4d1-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2802

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true
}
```





