---
title: Обновление Андроидвпнконфигуратион
description: Обновление свойств объекта Андроидвпнконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 82fe083a59ff35858e6cf56b4c941851a10d852f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928790"
---
# <a name="update-androidvpnconfiguration"></a><span data-ttu-id="5c7ae-103">Обновление Андроидвпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5c7ae-103">Update androidVpnConfiguration</span></span>

> <span data-ttu-id="5c7ae-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c7ae-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c7ae-106">Обновление свойств объекта [андроидвпнконфигуратион](../resources/intune-deviceconfig-androidvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5c7ae-106">Update the properties of a [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c7ae-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5c7ae-107">Prerequisites</span></span>
<span data-ttu-id="5c7ae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c7ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c7ae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c7ae-110">Permission type</span></span>|<span data-ttu-id="5c7ae-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c7ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c7ae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c7ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c7ae-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c7ae-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c7ae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c7ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c7ae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-115">Not supported.</span></span>|
|<span data-ttu-id="5c7ae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5c7ae-116">Application</span></span>|<span data-ttu-id="5c7ae-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c7ae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c7ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5c7ae-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c7ae-119">Request headers</span></span>
|<span data-ttu-id="5c7ae-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c7ae-120">Header</span></span>|<span data-ttu-id="5c7ae-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5c7ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c7ae-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c7ae-122">Authorization</span></span>|<span data-ttu-id="5c7ae-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c7ae-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5c7ae-124">Accept</span></span>|<span data-ttu-id="5c7ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c7ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c7ae-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5c7ae-126">Request body</span></span>
<span data-ttu-id="5c7ae-127">В тексте запроса добавьте представление объекта [Андроидвпнконфигуратион](../resources/intune-deviceconfig-androidvpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-127">In the request body, supply a JSON representation for the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object.</span></span>

<span data-ttu-id="5c7ae-128">В следующей таблице приведены свойства, необходимые при создании [андроидвпнконфигуратион](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c7ae-128">The following table shows the properties that are required when you create the [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md).</span></span>

|<span data-ttu-id="5c7ae-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c7ae-129">Property</span></span>|<span data-ttu-id="5c7ae-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5c7ae-130">Type</span></span>|<span data-ttu-id="5c7ae-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5c7ae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c7ae-132">id</span><span class="sxs-lookup"><span data-stu-id="5c7ae-132">id</span></span>|<span data-ttu-id="5c7ae-133">String</span><span class="sxs-lookup"><span data-stu-id="5c7ae-133">String</span></span>|<span data-ttu-id="5c7ae-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-134">Key of the entity.</span></span> <span data-ttu-id="5c7ae-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c7ae-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c7ae-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c7ae-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5c7ae-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c7ae-137">DateTimeOffset</span></span>|<span data-ttu-id="5c7ae-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5c7ae-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c7ae-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c7ae-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5c7ae-140">roleScopeTagIds</span></span>|<span data-ttu-id="5c7ae-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5c7ae-141">String collection</span></span>|<span data-ttu-id="5c7ae-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5c7ae-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c7ae-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c7ae-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="5c7ae-144">supportsScopeTags</span></span>|<span data-ttu-id="5c7ae-145">Логический</span><span class="sxs-lookup"><span data-stu-id="5c7ae-145">Boolean</span></span>|<span data-ttu-id="5c7ae-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5c7ae-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5c7ae-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5c7ae-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-149">This property is read-only.</span></span> <span data-ttu-id="5c7ae-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c7ae-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c7ae-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c7ae-151">createdDateTime</span></span>|<span data-ttu-id="5c7ae-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c7ae-152">DateTimeOffset</span></span>|<span data-ttu-id="5c7ae-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-153">DateTime the object was created.</span></span> <span data-ttu-id="5c7ae-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c7ae-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c7ae-155">description</span><span class="sxs-lookup"><span data-stu-id="5c7ae-155">description</span></span>|<span data-ttu-id="5c7ae-156">String</span><span class="sxs-lookup"><span data-stu-id="5c7ae-156">String</span></span>|<span data-ttu-id="5c7ae-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5c7ae-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c7ae-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c7ae-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5c7ae-159">displayName</span></span>|<span data-ttu-id="5c7ae-160">Строка</span><span class="sxs-lookup"><span data-stu-id="5c7ae-160">String</span></span>|<span data-ttu-id="5c7ae-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5c7ae-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c7ae-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c7ae-163">version</span><span class="sxs-lookup"><span data-stu-id="5c7ae-163">version</span></span>|<span data-ttu-id="5c7ae-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5c7ae-164">Int32</span></span>|<span data-ttu-id="5c7ae-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-165">Version of the device configuration.</span></span> <span data-ttu-id="5c7ae-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5c7ae-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5c7ae-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="5c7ae-167">connectionName</span></span>|<span data-ttu-id="5c7ae-168">Строка</span><span class="sxs-lookup"><span data-stu-id="5c7ae-168">String</span></span>|<span data-ttu-id="5c7ae-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-169">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="5c7ae-170">connectionType</span><span class="sxs-lookup"><span data-stu-id="5c7ae-170">connectionType</span></span>|[<span data-ttu-id="5c7ae-171">Androidvpnconnectiontype.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-171">androidVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidvpnconnectiontype.md)|<span data-ttu-id="5c7ae-172">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-172">Connection type.</span></span> <span data-ttu-id="5c7ae-173">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-173">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="5c7ae-174">role</span><span class="sxs-lookup"><span data-stu-id="5c7ae-174">role</span></span>|<span data-ttu-id="5c7ae-175">Строка</span><span class="sxs-lookup"><span data-stu-id="5c7ae-175">String</span></span>|<span data-ttu-id="5c7ae-176">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-176">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="5c7ae-177">область</span><span class="sxs-lookup"><span data-stu-id="5c7ae-177">realm</span></span>|<span data-ttu-id="5c7ae-178">Строка</span><span class="sxs-lookup"><span data-stu-id="5c7ae-178">String</span></span>|<span data-ttu-id="5c7ae-179">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-179">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="5c7ae-180">серверами</span><span class="sxs-lookup"><span data-stu-id="5c7ae-180">servers</span></span>|<span data-ttu-id="5c7ae-181">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="5c7ae-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="5c7ae-182">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-182">List of VPN Servers on the network.</span></span> <span data-ttu-id="5c7ae-183">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-183">Make sure end users can access these network locations.</span></span> <span data-ttu-id="5c7ae-184">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5c7ae-185">распознавания</span><span class="sxs-lookup"><span data-stu-id="5c7ae-185">fingerprint</span></span>|<span data-ttu-id="5c7ae-186">Строка</span><span class="sxs-lookup"><span data-stu-id="5c7ae-186">String</span></span>|<span data-ttu-id="5c7ae-187">Отпечаток — это строка, которая будет использоваться для проверки доверенности VPN-сервера, который применяется, только если тип подключения — "VPN-метка капсулы".</span><span class="sxs-lookup"><span data-stu-id="5c7ae-187">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="5c7ae-188">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="5c7ae-188">customData</span></span>|<span data-ttu-id="5c7ae-189">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="5c7ae-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="5c7ae-190">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-190">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="5c7ae-191">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-191">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="5c7ae-192">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="5c7ae-192">customKeyValueData</span></span>|<span data-ttu-id="5c7ae-193">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="5c7ae-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="5c7ae-194">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-194">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="5c7ae-195">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-195">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="5c7ae-196">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="5c7ae-196">authenticationMethod</span></span>|[<span data-ttu-id="5c7ae-197">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="5c7ae-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="5c7ae-198">Метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-198">Authentication method.</span></span> <span data-ttu-id="5c7ae-199">Возможные значения: `certificate`, `usernameAndPassword`, `derivedCredential`.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-199">Possible values are: `certificate`, `usernameAndPassword`, `derivedCredential`.</span></span>|



## <a name="response"></a><span data-ttu-id="5c7ae-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c7ae-200">Response</span></span>
<span data-ttu-id="5c7ae-201">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидвпнконфигуратион](../resources/intune-deviceconfig-androidvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-201">If successful, this method returns a `200 OK` response code and an updated [androidVpnConfiguration](../resources/intune-deviceconfig-androidvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c7ae-202">Пример</span><span class="sxs-lookup"><span data-stu-id="5c7ae-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c7ae-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c7ae-203">Request</span></span>
<span data-ttu-id="5c7ae-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 978

{
  "@odata.type": "#microsoft.graph.androidVpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
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
  "authenticationMethod": "usernameAndPassword"
}
```

### <a name="response"></a><span data-ttu-id="5c7ae-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c7ae-205">Response</span></span>
<span data-ttu-id="5c7ae-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1150

{
  "@odata.type": "#microsoft.graph.androidVpnConfiguration",
  "id": "d4c48852-8852-d4c4-5288-c4d45288c4d4",
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
  "role": "Role value",
  "realm": "Realm value",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "Description value",
      "address": "Address value",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "Fingerprint value",
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
  "authenticationMethod": "usernameAndPassword"
}
```




