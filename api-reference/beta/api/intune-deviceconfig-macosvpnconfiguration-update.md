---
title: Обновление Макосвпнконфигуратион
description: Обновление свойств объекта Макосвпнконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8828cb86ffe3b5f366ce2300a879e06211ee04d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518443"
---
# <a name="update-macosvpnconfiguration"></a><span data-ttu-id="e6406-103">Обновление Макосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="e6406-103">Update macOSVpnConfiguration</span></span>

> <span data-ttu-id="e6406-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6406-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6406-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6406-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6406-106">Обновление свойств объекта [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e6406-106">Update the properties of a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6406-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e6406-107">Prerequisites</span></span>
<span data-ttu-id="e6406-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6406-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6406-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6406-110">Permission type</span></span>|<span data-ttu-id="e6406-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6406-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6406-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6406-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e6406-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6406-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e6406-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6406-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6406-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6406-115">Not supported.</span></span>|
|<span data-ttu-id="e6406-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6406-116">Application</span></span>|<span data-ttu-id="e6406-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6406-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6406-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6406-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e6406-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6406-119">Request headers</span></span>
|<span data-ttu-id="e6406-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6406-120">Header</span></span>|<span data-ttu-id="e6406-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e6406-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6406-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6406-122">Authorization</span></span>|<span data-ttu-id="e6406-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6406-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6406-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e6406-124">Accept</span></span>|<span data-ttu-id="e6406-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e6406-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6406-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e6406-126">Request body</span></span>
<span data-ttu-id="e6406-127">В тексте запроса добавьте представление объекта [Макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6406-127">In the request body, supply a JSON representation for the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

<span data-ttu-id="e6406-128">В следующей таблице приведены свойства, необходимые при создании [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6406-128">The following table shows the properties that are required when you create the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md).</span></span>

|<span data-ttu-id="e6406-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6406-129">Property</span></span>|<span data-ttu-id="e6406-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e6406-130">Type</span></span>|<span data-ttu-id="e6406-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e6406-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6406-132">id</span><span class="sxs-lookup"><span data-stu-id="e6406-132">id</span></span>|<span data-ttu-id="e6406-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e6406-133">String</span></span>|<span data-ttu-id="e6406-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e6406-134">Key of the entity.</span></span> <span data-ttu-id="e6406-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6406-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6406-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e6406-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6406-137">DateTimeOffset</span></span>|<span data-ttu-id="e6406-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e6406-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e6406-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6406-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e6406-140">roleScopeTagIds</span></span>|<span data-ttu-id="e6406-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e6406-141">String collection</span></span>|<span data-ttu-id="e6406-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e6406-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e6406-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6406-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e6406-144">supportsScopeTags</span></span>|<span data-ttu-id="e6406-145">Логический</span><span class="sxs-lookup"><span data-stu-id="e6406-145">Boolean</span></span>|<span data-ttu-id="e6406-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e6406-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e6406-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e6406-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e6406-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e6406-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e6406-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6406-149">This property is read-only.</span></span> <span data-ttu-id="e6406-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6406-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6406-151">createdDateTime</span></span>|<span data-ttu-id="e6406-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6406-152">DateTimeOffset</span></span>|<span data-ttu-id="e6406-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e6406-153">DateTime the object was created.</span></span> <span data-ttu-id="e6406-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6406-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-155">description</span><span class="sxs-lookup"><span data-stu-id="e6406-155">description</span></span>|<span data-ttu-id="e6406-156">String</span><span class="sxs-lookup"><span data-stu-id="e6406-156">String</span></span>|<span data-ttu-id="e6406-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e6406-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e6406-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6406-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e6406-159">displayName</span></span>|<span data-ttu-id="e6406-160">String</span><span class="sxs-lookup"><span data-stu-id="e6406-160">String</span></span>|<span data-ttu-id="e6406-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e6406-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e6406-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6406-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-163">version</span><span class="sxs-lookup"><span data-stu-id="e6406-163">version</span></span>|<span data-ttu-id="e6406-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e6406-164">Int32</span></span>|<span data-ttu-id="e6406-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e6406-165">Version of the device configuration.</span></span> <span data-ttu-id="e6406-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6406-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="e6406-167">connectionName</span></span>|<span data-ttu-id="e6406-168">String</span><span class="sxs-lookup"><span data-stu-id="e6406-168">String</span></span>|<span data-ttu-id="e6406-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="e6406-169">Connection name displayed to the user.</span></span> <span data-ttu-id="e6406-170">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="e6406-171">connectionType</span></span>|[<span data-ttu-id="e6406-172">Апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="e6406-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="e6406-173">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="e6406-173">Connection type.</span></span> <span data-ttu-id="e6406-174">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6406-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="e6406-175">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`,. `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="e6406-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="e6406-176">Логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="e6406-176">loginGroupOrDomain</span></span>|<span data-ttu-id="e6406-177">String</span><span class="sxs-lookup"><span data-stu-id="e6406-177">String</span></span>|<span data-ttu-id="e6406-178">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="e6406-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="e6406-179">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-180">role</span><span class="sxs-lookup"><span data-stu-id="e6406-180">role</span></span>|<span data-ttu-id="e6406-181">String</span><span class="sxs-lookup"><span data-stu-id="e6406-181">String</span></span>|<span data-ttu-id="e6406-182">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="e6406-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="e6406-183">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-184">область</span><span class="sxs-lookup"><span data-stu-id="e6406-184">realm</span></span>|<span data-ttu-id="e6406-185">String</span><span class="sxs-lookup"><span data-stu-id="e6406-185">String</span></span>|<span data-ttu-id="e6406-186">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="e6406-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="e6406-187">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-188">сервер</span><span class="sxs-lookup"><span data-stu-id="e6406-188">server</span></span>|[<span data-ttu-id="e6406-189">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="e6406-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="e6406-190">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="e6406-190">VPN Server on the network.</span></span> <span data-ttu-id="e6406-191">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="e6406-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="e6406-192">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-193">идентификатор</span><span class="sxs-lookup"><span data-stu-id="e6406-193">identifier</span></span>|<span data-ttu-id="e6406-194">String</span><span class="sxs-lookup"><span data-stu-id="e6406-194">String</span></span>|<span data-ttu-id="e6406-195">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="e6406-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e6406-196">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наСледуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-197">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="e6406-197">customData</span></span>|<span data-ttu-id="e6406-198">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="e6406-199">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="e6406-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e6406-200">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="e6406-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="e6406-201">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="e6406-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="e6406-202">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="e6406-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="e6406-203">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="e6406-204">customKeyValueData</span></span>|<span data-ttu-id="e6406-205">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e6406-206">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="e6406-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="e6406-207">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="e6406-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="e6406-208">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="e6406-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="e6406-209">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="e6406-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="e6406-210">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-211">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="e6406-211">enableSplitTunneling</span></span>|<span data-ttu-id="e6406-212">Логический</span><span class="sxs-lookup"><span data-stu-id="e6406-212">Boolean</span></span>|<span data-ttu-id="e6406-213">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="e6406-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="e6406-214">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-215">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="e6406-215">authenticationMethod</span></span>|[<span data-ttu-id="e6406-216">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="e6406-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="e6406-217">Способ проверки поДлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="e6406-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="e6406-218">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e6406-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="e6406-219">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="e6406-219">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="e6406-220">Енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="e6406-220">enablePerApp</span></span>|<span data-ttu-id="e6406-221">Логический</span><span class="sxs-lookup"><span data-stu-id="e6406-221">Boolean</span></span>|<span data-ttu-id="e6406-222">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту ВИРТУАЛЬную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e6406-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="e6406-223">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-224">Сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="e6406-224">safariDomains</span></span>|<span data-ttu-id="e6406-225">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e6406-225">String collection</span></span>|<span data-ttu-id="e6406-226">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="e6406-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="e6406-227">Кроме приложений, связанных с этой ВИРТУАЛЬНОЙ частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="e6406-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="e6406-228">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-229">Ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="e6406-229">onDemandRules</span></span>|<span data-ttu-id="e6406-230">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="e6406-231">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="e6406-231">On-Demand Rules.</span></span> <span data-ttu-id="e6406-232">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e6406-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e6406-233">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-234">проксисервер</span><span class="sxs-lookup"><span data-stu-id="e6406-234">proxyServer</span></span>|[<span data-ttu-id="e6406-235">Впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="e6406-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="e6406-236">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="e6406-236">Proxy Server.</span></span> <span data-ttu-id="e6406-237">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="e6406-238">Оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="e6406-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="e6406-239">Логический</span><span class="sxs-lookup"><span data-stu-id="e6406-239">Boolean</span></span>|<span data-ttu-id="e6406-240">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="e6406-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="e6406-241">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e6406-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e6406-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6406-242">Response</span></span>
<span data-ttu-id="e6406-243">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6406-243">If successful, this method returns a `200 OK` response code and an updated [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6406-244">Пример</span><span class="sxs-lookup"><span data-stu-id="e6406-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6406-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6406-245">Request</span></span>
<span data-ttu-id="e6406-246">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6406-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1857

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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
  "optInToDeviceIdSharing": true
}
```

### <a name="response"></a><span data-ttu-id="e6406-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6406-247">Response</span></span>
<span data-ttu-id="e6406-p126">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e6406-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2029

{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
  "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
  "optInToDeviceIdSharing": true
}
```





