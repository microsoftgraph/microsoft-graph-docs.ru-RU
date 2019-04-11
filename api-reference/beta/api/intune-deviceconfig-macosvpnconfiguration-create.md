---
title: Создание Макосвпнконфигуратион
description: Создание нового объекта Макосвпнконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a19d53fdc4307d7dae8dca6c07f77420bb4711a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779022"
---
# <a name="create-macosvpnconfiguration"></a><span data-ttu-id="31beb-103">Создание Макосвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="31beb-103">Create macOSVpnConfiguration</span></span>

> <span data-ttu-id="31beb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31beb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31beb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31beb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31beb-106">Создание нового объекта [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="31beb-106">Create a new [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31beb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="31beb-107">Prerequisites</span></span>
<span data-ttu-id="31beb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="31beb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31beb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="31beb-110">Permission type</span></span>|<span data-ttu-id="31beb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="31beb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31beb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="31beb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31beb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31beb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="31beb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="31beb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31beb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31beb-115">Not supported.</span></span>|
|<span data-ttu-id="31beb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="31beb-116">Application</span></span>|<span data-ttu-id="31beb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31beb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31beb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="31beb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="31beb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="31beb-119">Request headers</span></span>
|<span data-ttu-id="31beb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="31beb-120">Header</span></span>|<span data-ttu-id="31beb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="31beb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31beb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="31beb-122">Authorization</span></span>|<span data-ttu-id="31beb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="31beb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31beb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="31beb-124">Accept</span></span>|<span data-ttu-id="31beb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31beb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31beb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="31beb-126">Request body</span></span>
<span data-ttu-id="31beb-127">В тексте запроса добавьте представление объекта Макосвпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31beb-127">In the request body, supply a JSON representation for the macOSVpnConfiguration object.</span></span>

<span data-ttu-id="31beb-128">В следующей таблице приведены свойства, необходимые при создании Макосвпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="31beb-128">The following table shows the properties that are required when you create the macOSVpnConfiguration.</span></span>

|<span data-ttu-id="31beb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="31beb-129">Property</span></span>|<span data-ttu-id="31beb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="31beb-130">Type</span></span>|<span data-ttu-id="31beb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="31beb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31beb-132">id</span><span class="sxs-lookup"><span data-stu-id="31beb-132">id</span></span>|<span data-ttu-id="31beb-133">Строка</span><span class="sxs-lookup"><span data-stu-id="31beb-133">String</span></span>|<span data-ttu-id="31beb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="31beb-134">Key of the entity.</span></span> <span data-ttu-id="31beb-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31beb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31beb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="31beb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31beb-137">DateTimeOffset</span></span>|<span data-ttu-id="31beb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="31beb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="31beb-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31beb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="31beb-140">roleScopeTagIds</span></span>|<span data-ttu-id="31beb-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="31beb-141">String collection</span></span>|<span data-ttu-id="31beb-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="31beb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="31beb-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31beb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="31beb-144">supportsScopeTags</span></span>|<span data-ttu-id="31beb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="31beb-145">Boolean</span></span>|<span data-ttu-id="31beb-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="31beb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="31beb-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="31beb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="31beb-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="31beb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="31beb-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="31beb-149">This property is read-only.</span></span> <span data-ttu-id="31beb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31beb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31beb-151">createdDateTime</span></span>|<span data-ttu-id="31beb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31beb-152">DateTimeOffset</span></span>|<span data-ttu-id="31beb-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="31beb-153">DateTime the object was created.</span></span> <span data-ttu-id="31beb-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31beb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-155">description</span><span class="sxs-lookup"><span data-stu-id="31beb-155">description</span></span>|<span data-ttu-id="31beb-156">String</span><span class="sxs-lookup"><span data-stu-id="31beb-156">String</span></span>|<span data-ttu-id="31beb-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="31beb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="31beb-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31beb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="31beb-159">displayName</span></span>|<span data-ttu-id="31beb-160">String</span><span class="sxs-lookup"><span data-stu-id="31beb-160">String</span></span>|<span data-ttu-id="31beb-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="31beb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="31beb-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31beb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-163">version</span><span class="sxs-lookup"><span data-stu-id="31beb-163">version</span></span>|<span data-ttu-id="31beb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="31beb-164">Int32</span></span>|<span data-ttu-id="31beb-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="31beb-165">Version of the device configuration.</span></span> <span data-ttu-id="31beb-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31beb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="31beb-167">connectionName</span></span>|<span data-ttu-id="31beb-168">String</span><span class="sxs-lookup"><span data-stu-id="31beb-168">String</span></span>|<span data-ttu-id="31beb-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="31beb-169">Connection name displayed to the user.</span></span> <span data-ttu-id="31beb-170">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-170">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-171">connectionType</span><span class="sxs-lookup"><span data-stu-id="31beb-171">connectionType</span></span>|[<span data-ttu-id="31beb-172">Апплевпнконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="31beb-172">appleVpnConnectionType</span></span>](../resources/intune-deviceconfig-applevpnconnectiontype.md)|<span data-ttu-id="31beb-173">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="31beb-173">Connection type.</span></span> <span data-ttu-id="31beb-174">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31beb-174">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="31beb-175">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`,. `paloAltoGlobalProtectV2`</span><span class="sxs-lookup"><span data-stu-id="31beb-175">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `customVpn`, `ciscoIPSec`, `citrix`, `ciscoAnyConnectV2`, `paloAltoGlobalProtect`, `zscalerPrivateAccess`, `f5Access2018`, `citrixSso`, `paloAltoGlobalProtectV2`.</span></span>|
|<span data-ttu-id="31beb-176">Логинграупордомаин</span><span class="sxs-lookup"><span data-stu-id="31beb-176">loginGroupOrDomain</span></span>|<span data-ttu-id="31beb-177">String</span><span class="sxs-lookup"><span data-stu-id="31beb-177">String</span></span>|<span data-ttu-id="31beb-178">Группа входа или домен, когда для параметра Тип подключения установлено мобильное подключение Dell Сониквалл.</span><span class="sxs-lookup"><span data-stu-id="31beb-178">Login group or domain when connection type is set to Dell SonicWALL Mobile Connection.</span></span> <span data-ttu-id="31beb-179">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-179">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-180">role</span><span class="sxs-lookup"><span data-stu-id="31beb-180">role</span></span>|<span data-ttu-id="31beb-181">String</span><span class="sxs-lookup"><span data-stu-id="31beb-181">String</span></span>|<span data-ttu-id="31beb-182">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="31beb-182">Role when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="31beb-183">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-183">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-184">область</span><span class="sxs-lookup"><span data-stu-id="31beb-184">realm</span></span>|<span data-ttu-id="31beb-185">String</span><span class="sxs-lookup"><span data-stu-id="31beb-185">String</span></span>|<span data-ttu-id="31beb-186">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="31beb-186">Realm when connection type is set to Pulse Secure.</span></span> <span data-ttu-id="31beb-187">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-187">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-188">сервер</span><span class="sxs-lookup"><span data-stu-id="31beb-188">server</span></span>|[<span data-ttu-id="31beb-189">Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="31beb-189">vpnServer</span></span>](../resources/intune-deviceconfig-vpnserver.md)|<span data-ttu-id="31beb-190">VPN-сервер в сети.</span><span class="sxs-lookup"><span data-stu-id="31beb-190">VPN Server on the network.</span></span> <span data-ttu-id="31beb-191">Убедитесь, что конечные пользователи имеют доступ к этому сетевому расположению.</span><span class="sxs-lookup"><span data-stu-id="31beb-191">Make sure end users can access this network location.</span></span> <span data-ttu-id="31beb-192">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-192">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-193">идентификатор</span><span class="sxs-lookup"><span data-stu-id="31beb-193">identifier</span></span>|<span data-ttu-id="31beb-194">String</span><span class="sxs-lookup"><span data-stu-id="31beb-194">String</span></span>|<span data-ttu-id="31beb-195">Идентификатор, предоставленный поставщиком VPN, если для параметра Тип подключения задано значение пользовательская сеть VPN.</span><span class="sxs-lookup"><span data-stu-id="31beb-195">Identifier provided by VPN vendor when connection type is set to Custom VPN.</span></span> <span data-ttu-id="31beb-196">Например: Cisco Аниконнект использует идентификатор формы com. Cisco. аниконнект. апплевпн. подключаемый модуль, наСледуемый от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-196">For example: Cisco AnyConnect uses an identifier of the form com.cisco.anyconnect.applevpn.plugin Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-197">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="31beb-197">customData</span></span>|<span data-ttu-id="31beb-198">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-198">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="31beb-199">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="31beb-199">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="31beb-200">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="31beb-200">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="31beb-201">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="31beb-201">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="31beb-202">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="31beb-202">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="31beb-203">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-203">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-204">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="31beb-204">customKeyValueData</span></span>|<span data-ttu-id="31beb-205">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-205">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="31beb-206">Пользовательские данные, когда для параметра Тип подключения задано значение Custom VPN.</span><span class="sxs-lookup"><span data-stu-id="31beb-206">Custom data when connection type is set to Custom VPN.</span></span> <span data-ttu-id="31beb-207">Используйте это поле, чтобы включить функции, не поддерживаемые Intune, но доступные в решении VPN.</span><span class="sxs-lookup"><span data-stu-id="31beb-207">Use this field to enable functionality not supported by Intune, but available in your VPN solution.</span></span> <span data-ttu-id="31beb-208">Обратитесь к поставщику услуг VPN, чтобы узнать, как добавить эти пары "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="31beb-208">Contact your VPN vendor to learn how to add these key/value pairs.</span></span> <span data-ttu-id="31beb-209">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="31beb-209">This collection can contain a maximum of 25 elements.</span></span> <span data-ttu-id="31beb-210">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-210">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-211">Енаблесплиттуннелинг</span><span class="sxs-lookup"><span data-stu-id="31beb-211">enableSplitTunneling</span></span>|<span data-ttu-id="31beb-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="31beb-212">Boolean</span></span>|<span data-ttu-id="31beb-213">Отправлять весь сетевой трафик через VPN.</span><span class="sxs-lookup"><span data-stu-id="31beb-213">Send all network traffic through VPN.</span></span> <span data-ttu-id="31beb-214">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-214">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-215">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="31beb-215">authenticationMethod</span></span>|[<span data-ttu-id="31beb-216">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="31beb-216">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="31beb-217">Способ проверки поДлинности для этого VPN-подключения.</span><span class="sxs-lookup"><span data-stu-id="31beb-217">Authentication method for this VPN connection.</span></span> <span data-ttu-id="31beb-218">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="31beb-218">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md).</span></span> <span data-ttu-id="31beb-219">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="31beb-219">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|
|<span data-ttu-id="31beb-220">Енаблеперапп</span><span class="sxs-lookup"><span data-stu-id="31beb-220">enablePerApp</span></span>|<span data-ttu-id="31beb-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="31beb-221">Boolean</span></span>|<span data-ttu-id="31beb-222">Если задать для этого параметра значение true, будут создаваться полезные данные VPN для каждого приложения, которые позже могут быть связаны с приложениями, которые могут активировать эту ВИРТУАЛЬную сеть VPN коннеЦитон на устройстве iOS конечного пользователя.</span><span class="sxs-lookup"><span data-stu-id="31beb-222">Setting this to true creates Per-App VPN payload which can later be associated with Apps that can trigger this VPN conneciton on the end user's iOS device.</span></span> <span data-ttu-id="31beb-223">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-223">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-224">Сафаридомаинс</span><span class="sxs-lookup"><span data-stu-id="31beb-224">safariDomains</span></span>|<span data-ttu-id="31beb-225">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="31beb-225">String collection</span></span>|<span data-ttu-id="31beb-226">Домены Safari при включении этого параметра VPN для каждого приложения.</span><span class="sxs-lookup"><span data-stu-id="31beb-226">Safari domains when this VPN per App setting is enabled.</span></span> <span data-ttu-id="31beb-227">Кроме приложений, связанных с этой ВИРТУАЛЬНОЙ частной сети, домены Safari, указанные здесь, также смогут инициировать это VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="31beb-227">In addition to the apps associated with this VPN, Safari domains specified here will also be able to trigger this VPN connection.</span></span> <span data-ttu-id="31beb-228">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-228">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-229">Ондемандрулес</span><span class="sxs-lookup"><span data-stu-id="31beb-229">onDemandRules</span></span>|<span data-ttu-id="31beb-230">Коллекция [впнондемандруле](../resources/intune-deviceconfig-vpnondemandrule.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-230">[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md) collection</span></span>|<span data-ttu-id="31beb-231">Правила по запросу.</span><span class="sxs-lookup"><span data-stu-id="31beb-231">On-Demand Rules.</span></span> <span data-ttu-id="31beb-232">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="31beb-232">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="31beb-233">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-233">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-234">проксисервер</span><span class="sxs-lookup"><span data-stu-id="31beb-234">proxyServer</span></span>|[<span data-ttu-id="31beb-235">Впнпроксисервер</span><span class="sxs-lookup"><span data-stu-id="31beb-235">vpnProxyServer</span></span>](../resources/intune-deviceconfig-vpnproxyserver.md)|<span data-ttu-id="31beb-236">Прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="31beb-236">Proxy Server.</span></span> <span data-ttu-id="31beb-237">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-237">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|
|<span data-ttu-id="31beb-238">Оптинтодевицеидшаринг</span><span class="sxs-lookup"><span data-stu-id="31beb-238">optInToDeviceIdSharing</span></span>|<span data-ttu-id="31beb-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="31beb-239">Boolean</span></span>|<span data-ttu-id="31beb-240">Предоставление доступа к идентификатору устройства сторонним VPN-клиентам для использования во время проверки управления доступом к сети.</span><span class="sxs-lookup"><span data-stu-id="31beb-240">Opt-In to sharing the device's Id to third-party vpn clients for use during network access control validation.</span></span> <span data-ttu-id="31beb-241">НаСледуется от [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="31beb-241">Inherited from [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="31beb-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="31beb-242">Response</span></span>
<span data-ttu-id="31beb-243">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвпнконфигуратион](../resources/intune-deviceconfig-macosvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="31beb-243">If successful, this method returns a `201 Created` response code and a [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31beb-244">Пример</span><span class="sxs-lookup"><span data-stu-id="31beb-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="31beb-245">Запрос</span><span class="sxs-lookup"><span data-stu-id="31beb-245">Request</span></span>
<span data-ttu-id="31beb-246">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="31beb-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="31beb-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="31beb-247">Response</span></span>
<span data-ttu-id="31beb-p126">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="31beb-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





