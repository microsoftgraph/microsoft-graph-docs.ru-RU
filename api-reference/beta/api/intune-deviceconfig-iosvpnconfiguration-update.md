---
title: Обновление Иосвпнконфигуратион
description: Обновление свойств объекта Иосвпнконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8400613a6f16b2e73ee5c7add7314a1965515417
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923078"
---
# <a name="update-iosvpnconfiguration"></a><span data-ttu-id="e648c-103">Обновление Иосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e648c-103">Update iosVpnConfiguration</span></span>

> <span data-ttu-id="e648c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e648c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e648c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e648c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e648c-106">Обновление свойств объекта [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e648c-106">Update the properties of a [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e648c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e648c-107">Prerequisites</span></span>
<span data-ttu-id="e648c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e648c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e648c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e648c-110">Permission type</span></span>|<span data-ttu-id="e648c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e648c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e648c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e648c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e648c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e648c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e648c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e648c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e648c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e648c-115">Not supported.</span></span>|
|<span data-ttu-id="e648c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e648c-116">Application</span></span>|<span data-ttu-id="e648c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e648c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e648c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e648c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e648c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e648c-119">Request headers</span></span>
|<span data-ttu-id="e648c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e648c-120">Header</span></span>|<span data-ttu-id="e648c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e648c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e648c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e648c-122">Authorization</span></span>|<span data-ttu-id="e648c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e648c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e648c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e648c-124">Accept</span></span>|<span data-ttu-id="e648c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e648c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e648c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e648c-126">Request body</span></span>
<span data-ttu-id="e648c-127">В тексте запроса добавьте представление объекта [Иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e648c-127">In the request body, supply a JSON representation for the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="e648c-128">В следующей таблице приведены свойства, необходимые при создании [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e648c-128">The following table shows the properties that are required when you create the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md).</span></span>

|<span data-ttu-id="e648c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e648c-129">Property</span></span>|<span data-ttu-id="e648c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e648c-130">Type</span></span>|<span data-ttu-id="e648c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e648c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e648c-132">id</span><span class="sxs-lookup"><span data-stu-id="e648c-132">id</span></span>|<span data-ttu-id="e648c-133">String</span><span class="sxs-lookup"><span data-stu-id="e648c-133">String</span></span>|<span data-ttu-id="e648c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e648c-134">Key of the entity.</span></span> <span data-ttu-id="e648c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e648c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e648c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e648c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e648c-137">DateTimeOffset</span></span>|<span data-ttu-id="e648c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e648c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e648c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e648c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e648c-140">roleScopeTagIds</span></span>|<span data-ttu-id="e648c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e648c-141">String collection</span></span>|<span data-ttu-id="e648c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e648c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e648c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e648c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e648c-144">supportsScopeTags</span></span>|<span data-ttu-id="e648c-145">Логический</span><span class="sxs-lookup"><span data-stu-id="e648c-145">Boolean</span></span>|<span data-ttu-id="e648c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e648c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e648c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e648c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e648c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e648c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e648c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e648c-149">This property is read-only.</span></span> <span data-ttu-id="e648c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e648c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e648c-151">createdDateTime</span></span>|<span data-ttu-id="e648c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e648c-152">DateTimeOffset</span></span>|<span data-ttu-id="e648c-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e648c-153">DateTime the object was created.</span></span> <span data-ttu-id="e648c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e648c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-155">description</span><span class="sxs-lookup"><span data-stu-id="e648c-155">description</span></span>|<span data-ttu-id="e648c-156">String</span><span class="sxs-lookup"><span data-stu-id="e648c-156">String</span></span>|<span data-ttu-id="e648c-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e648c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e648c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e648c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e648c-159">displayName</span></span>|<span data-ttu-id="e648c-160">Строка</span><span class="sxs-lookup"><span data-stu-id="e648c-160">String</span></span>|<span data-ttu-id="e648c-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e648c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e648c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e648c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-163">version</span><span class="sxs-lookup"><span data-stu-id="e648c-163">version</span></span>|<span data-ttu-id="e648c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e648c-164">Int32</span></span>|<span data-ttu-id="e648c-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e648c-165">Version of the device configuration.</span></span> <span data-ttu-id="e648c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e648c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="e648c-167">connectionName</span></span>|<span data-ttu-id="e648c-168">Строка</span><span class="sxs-lookup"><span data-stu-id="e648c-168">String</span></span>|<span data-ttu-id="e648c-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e648c-169">Connection name displayed to the user.</span></span> <span data-ttu-id="e648c-170">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="e648c-171">connectionType</span></span>|[<span data-ttu-id="e648c-172">Апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="e648c-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="e648c-173">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="e648c-173">Connection type.</span></span> <span data-ttu-id="e648c-174">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e648c-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="e648c-175">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`,. `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="e648c-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="e648c-176">Логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="e648c-176">loginGroupOrDomain</span></span>|<span data-ttu-id="e648c-177">Строка</span><span class="sxs-lookup"><span data-stu-id="e648c-177">String</span></span>|<span data-ttu-id="e648c-178">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="e648c-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="e648c-179">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-180">role</span><span class="sxs-lookup"><span data-stu-id="e648c-180">role</span></span>|<span data-ttu-id="e648c-181">Строка</span><span class="sxs-lookup"><span data-stu-id="e648c-181">String</span></span>|<span data-ttu-id="e648c-182">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="e648c-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="e648c-183">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-184">область</span><span class="sxs-lookup"><span data-stu-id="e648c-184">realm</span></span>|<span data-ttu-id="e648c-185">Строка</span><span class="sxs-lookup"><span data-stu-id="e648c-185">String</span></span>|<span data-ttu-id="e648c-186">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="e648c-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="e648c-187">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-188">сервер</span><span class="sxs-lookup"><span data-stu-id="e648c-188">server</span></span>|[<span data-ttu-id="e648c-189">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="e648c-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="e648c-190">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="e648c-190">VPN Server on the network.</span></span> <span data-ttu-id="e648c-191">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="e648c-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="e648c-192">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-193">идентификатор</span><span class="sxs-lookup"><span data-stu-id="e648c-193">identifier</span></span>|<span data-ttu-id="e648c-194">Строка</span><span class="sxs-lookup"><span data-stu-id="e648c-194">String</span></span>|<span data-ttu-id="e648c-195">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="e648c-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e648c-196">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наследуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-197">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="e648c-197">customData</span></span>|<span data-ttu-id="e648c-198">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="e648c-199">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="e648c-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e648c-200">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="e648c-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="e648c-201">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="e648c-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="e648c-202">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="e648c-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="e648c-203">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="e648c-204">customKeyValueData</span></span>|<span data-ttu-id="e648c-205">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e648c-206">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="e648c-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e648c-207">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="e648c-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="e648c-208">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="e648c-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="e648c-209">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="e648c-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="e648c-210">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-211">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="e648c-211">enableSplitTunneling</span></span>|<span data-ttu-id="e648c-212">Логический</span><span class="sxs-lookup"><span data-stu-id="e648c-212">Boolean</span></span>|<span data-ttu-id="e648c-213">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="e648c-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="e648c-214">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-215">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="e648c-215">authenticationMethod</span></span>|[<span data-ttu-id="e648c-216">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="e648c-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="e648c-217">Способ проверки подлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="e648c-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="e648c-218">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e648c-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="e648c-219">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="e648c-219">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e648c-220">Енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="e648c-220">enablePerApp</span></span>|<span data-ttu-id="e648c-221">Логический</span><span class="sxs-lookup"><span data-stu-id="e648c-221">Boolean</span></span>|<span data-ttu-id="e648c-222">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту ВИРТУАЛЬную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e648c-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="e648c-223">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-224">Сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="e648c-224">safariDomains</span></span>|<span data-ttu-id="e648c-225">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e648c-225">String collection</span></span>|<span data-ttu-id="e648c-226">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="e648c-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="e648c-227">Кроме приложений, связанных с этой ВИРТУАЛЬНОЙ частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="e648c-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="e648c-228">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-229">Ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="e648c-229">onDemandRules</span></span>|<span data-ttu-id="e648c-230">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="e648c-231">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="e648c-231">On-Demand Rules.</span></span> <span data-ttu-id="e648c-232">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e648c-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e648c-233">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-234">проксисервер</span><span class="sxs-lookup"><span data-stu-id="e648c-234">proxyServer</span></span>|[<span data-ttu-id="e648c-235">Впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="e648c-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="e648c-236">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="e648c-236">Proxy Server.</span></span> <span data-ttu-id="e648c-237">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-238">Оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="e648c-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="e648c-239">Логический</span><span class="sxs-lookup"><span data-stu-id="e648c-239">Boolean</span></span>|<span data-ttu-id="e648c-240">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="e648c-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="e648c-241">Наследуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e648c-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e648c-242">providerType</span><span class="sxs-lookup"><span data-stu-id="e648c-242">providerType</span></span>|[<span data-ttu-id="e648c-243">vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="e648c-243">vpnProviderType</span></span>](../resources/intune-deviceconfig-vpnprovidertype.md)|<span data-ttu-id="e648c-244">Тип поставщика для VPN каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="e648c-244">Provider type for per-app VPN.</span></span> <span data-ttu-id="e648c-245">Возможные значения: `notConfigured`, `appProxy`, `packetTunnel`.</span><span class="sxs-lookup"><span data-stu-id="e648c-245">Possible values are: `notConfigured`, `appProxy`, `packetTunnel`.</span></span>|
|<span data-ttu-id="e648c-246">userDomain</span><span class="sxs-lookup"><span data-stu-id="e648c-246">userDomain</span></span>|<span data-ttu-id="e648c-247">Строка</span><span class="sxs-lookup"><span data-stu-id="e648c-247">String</span></span>|<span data-ttu-id="e648c-248">Только Зскалер.</span><span class="sxs-lookup"><span data-stu-id="e648c-248">Zscaler only.</span></span> <span data-ttu-id="e648c-249">Введите статический домен для предварительного заполнения поля Login в приложении Зскалер.</span><span class="sxs-lookup"><span data-stu-id="e648c-249">Enter a static domain to pre-populate the login field with in the Zscaler app.</span></span> <span data-ttu-id="e648c-250">Если оставить это поле пустым, вместо этого будет использоваться домен Azure Active Directory пользователя.</span><span class="sxs-lookup"><span data-stu-id="e648c-250">If this is left empty, the user's Azure Active Directory domain will be used instead.</span></span>|
|<span data-ttu-id="e648c-251">Стриктенфорцемент</span><span class="sxs-lookup"><span data-stu-id="e648c-251">strictEnforcement</span></span>|<span data-ttu-id="e648c-252">Логический</span><span class="sxs-lookup"><span data-stu-id="e648c-252">Boolean</span></span>|<span data-ttu-id="e648c-253">Только Зскалер.</span><span class="sxs-lookup"><span data-stu-id="e648c-253">Zscaler only.</span></span> <span data-ttu-id="e648c-254">Блокирует сетевой трафик до тех пор, пока пользователь не войдет в приложение Зскалер.</span><span class="sxs-lookup"><span data-stu-id="e648c-254">Blocks network traffic until the user signs into Zscaler app.</span></span> <span data-ttu-id="e648c-255">"True" означает, что трафик блокируется.</span><span class="sxs-lookup"><span data-stu-id="e648c-255">"True" means traffic is blocked.</span></span>|
|<span data-ttu-id="e648c-256">Клауднаме</span><span class="sxs-lookup"><span data-stu-id="e648c-256">cloudName</span></span>|<span data-ttu-id="e648c-257">Строка</span><span class="sxs-lookup"><span data-stu-id="e648c-257">String</span></span>|<span data-ttu-id="e648c-258">Только Зскалер.</span><span class="sxs-lookup"><span data-stu-id="e648c-258">Zscaler only.</span></span> <span data-ttu-id="e648c-259">Облако Зскалер, которому назначен пользователь.</span><span class="sxs-lookup"><span data-stu-id="e648c-259">Zscaler cloud which the user is assigned to.</span></span>|
|<span data-ttu-id="e648c-260">excludeList</span><span class="sxs-lookup"><span data-stu-id="e648c-260">excludeList</span></span>|<span data-ttu-id="e648c-261">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e648c-261">String collection</span></span>|<span data-ttu-id="e648c-262">Только Зскалер.</span><span class="sxs-lookup"><span data-stu-id="e648c-262">Zscaler only.</span></span> <span data-ttu-id="e648c-263">Список сетевых адресов, которые не отправляются через облако Зскалер.</span><span class="sxs-lookup"><span data-stu-id="e648c-263">List of network addresses which are not sent through the Zscaler cloud.</span></span>|



## <a name="response"></a><span data-ttu-id="e648c-264">Отклик</span><span class="sxs-lookup"><span data-stu-id="e648c-264">Response</span></span>
<span data-ttu-id="e648c-265">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосвпнконфигуратион](../resources/intune-deviceconfig-iosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e648c-265">If successful, this method returns a `200 OK` response code and an updated [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e648c-266">Пример</span><span class="sxs-lookup"><span data-stu-id="e648c-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="e648c-267">Запрос</span><span class="sxs-lookup"><span data-stu-id="e648c-267">Request</span></span>
<span data-ttu-id="e648c-268">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e648c-268">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2042

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="e648c-269">Отклик</span><span class="sxs-lookup"><span data-stu-id="e648c-269">Response</span></span>
<span data-ttu-id="e648c-p131">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e648c-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.iosVpnConfiguration",
  "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ]
}
```




