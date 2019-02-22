---
title: Обновление Андроидворкпрофилевпнконфигуратион
description: Обновление свойств объекта Андроидворкпрофилевпнконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61ea061f5e6a1d1e9f9900ceb5de5ec8cabfd6da
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164108"
---
# <a name="update-androidworkprofilevpnconfiguration"></a><span data-ttu-id="82717-103">Обновление Андроидворкпрофилевпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="82717-103">Update androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="82717-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82717-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82717-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82717-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82717-106">Обновление свойств объекта [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="82717-106">Update the properties of a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82717-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="82717-107">Prerequisites</span></span>
<span data-ttu-id="82717-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="82717-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="82717-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82717-110">Permission type</span></span>|<span data-ttu-id="82717-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82717-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82717-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82717-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82717-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82717-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82717-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82717-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82717-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82717-115">Not supported.</span></span>|
|<span data-ttu-id="82717-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82717-116">Application</span></span>|<span data-ttu-id="82717-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82717-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82717-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82717-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="82717-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82717-119">Request headers</span></span>
|<span data-ttu-id="82717-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82717-120">Header</span></span>|<span data-ttu-id="82717-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82717-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82717-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82717-122">Authorization</span></span>|<span data-ttu-id="82717-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="82717-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82717-124">Accept</span><span class="sxs-lookup"><span data-stu-id="82717-124">Accept</span></span>|<span data-ttu-id="82717-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82717-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82717-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82717-126">Request body</span></span>
<span data-ttu-id="82717-127">В тексте запроса добавьте представление объекта [Андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82717-127">In the request body, supply a JSON representation for the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

<span data-ttu-id="82717-128">В следующей таблице приведены свойства, необходимые при создании [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82717-128">The following table shows the properties that are required when you create the [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md).</span></span>

|<span data-ttu-id="82717-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="82717-129">Property</span></span>|<span data-ttu-id="82717-130">Тип</span><span class="sxs-lookup"><span data-stu-id="82717-130">Type</span></span>|<span data-ttu-id="82717-131">Описание</span><span class="sxs-lookup"><span data-stu-id="82717-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82717-132">id</span><span class="sxs-lookup"><span data-stu-id="82717-132">id</span></span>|<span data-ttu-id="82717-133">String</span><span class="sxs-lookup"><span data-stu-id="82717-133">String</span></span>|<span data-ttu-id="82717-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="82717-134">Key of the entity.</span></span> <span data-ttu-id="82717-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82717-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82717-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82717-136">lastModifiedDateTime</span></span>|<span data-ttu-id="82717-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82717-137">DateTimeOffset</span></span>|<span data-ttu-id="82717-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="82717-138">DateTime the object was last modified.</span></span> <span data-ttu-id="82717-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82717-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82717-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82717-140">roleScopeTagIds</span></span>|<span data-ttu-id="82717-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="82717-141">String collection</span></span>|<span data-ttu-id="82717-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="82717-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="82717-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82717-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82717-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="82717-144">supportsScopeTags</span></span>|<span data-ttu-id="82717-145">Логический</span><span class="sxs-lookup"><span data-stu-id="82717-145">Boolean</span></span>|<span data-ttu-id="82717-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="82717-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="82717-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="82717-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="82717-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="82717-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="82717-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="82717-149">This property is read-only.</span></span> <span data-ttu-id="82717-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82717-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82717-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82717-151">createdDateTime</span></span>|<span data-ttu-id="82717-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82717-152">DateTimeOffset</span></span>|<span data-ttu-id="82717-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="82717-153">DateTime the object was created.</span></span> <span data-ttu-id="82717-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82717-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82717-155">description</span><span class="sxs-lookup"><span data-stu-id="82717-155">description</span></span>|<span data-ttu-id="82717-156">String</span><span class="sxs-lookup"><span data-stu-id="82717-156">String</span></span>|<span data-ttu-id="82717-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82717-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82717-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82717-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82717-159">displayName</span><span class="sxs-lookup"><span data-stu-id="82717-159">displayName</span></span>|<span data-ttu-id="82717-160">String</span><span class="sxs-lookup"><span data-stu-id="82717-160">String</span></span>|<span data-ttu-id="82717-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82717-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82717-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82717-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82717-163">version</span><span class="sxs-lookup"><span data-stu-id="82717-163">version</span></span>|<span data-ttu-id="82717-164">Int32</span><span class="sxs-lookup"><span data-stu-id="82717-164">Int32</span></span>|<span data-ttu-id="82717-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="82717-165">Version of the device configuration.</span></span> <span data-ttu-id="82717-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="82717-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82717-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="82717-167">connectionName</span></span>|<span data-ttu-id="82717-168">String</span><span class="sxs-lookup"><span data-stu-id="82717-168">String</span></span>|<span data-ttu-id="82717-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="82717-169">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="82717-170">connectionType</span><span class="sxs-lookup"><span data-stu-id="82717-170">connectionType</span></span>|[<span data-ttu-id="82717-171">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="82717-171">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="82717-172">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="82717-172">Connection type.</span></span> <span data-ttu-id="82717-173">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="82717-173">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="82717-174">role</span><span class="sxs-lookup"><span data-stu-id="82717-174">role</span></span>|<span data-ttu-id="82717-175">String</span><span class="sxs-lookup"><span data-stu-id="82717-175">String</span></span>|<span data-ttu-id="82717-176">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="82717-176">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="82717-177">область</span><span class="sxs-lookup"><span data-stu-id="82717-177">realm</span></span>|<span data-ttu-id="82717-178">String</span><span class="sxs-lookup"><span data-stu-id="82717-178">String</span></span>|<span data-ttu-id="82717-179">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="82717-179">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="82717-180">серверы</span><span class="sxs-lookup"><span data-stu-id="82717-180">servers</span></span>|<span data-ttu-id="82717-181">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="82717-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="82717-182">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="82717-182">List of VPN Servers on the network.</span></span> <span data-ttu-id="82717-183">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="82717-183">Make sure end users can access these network locations.</span></span> <span data-ttu-id="82717-184">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="82717-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="82717-185">распознавания</span><span class="sxs-lookup"><span data-stu-id="82717-185">fingerprint</span></span>|<span data-ttu-id="82717-186">String</span><span class="sxs-lookup"><span data-stu-id="82717-186">String</span></span>|<span data-ttu-id="82717-187">ОтПечаток — это строка, которая будет использоваться для проверки доверенности VPN-сервера, который применяется, только если тип подключения — "VPN-метка капсулы".</span><span class="sxs-lookup"><span data-stu-id="82717-187">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="82717-188">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="82717-188">customData</span></span>|<span data-ttu-id="82717-189">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="82717-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="82717-190">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="82717-190">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="82717-191">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="82717-191">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="82717-192">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="82717-192">customKeyValueData</span></span>|<span data-ttu-id="82717-193">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="82717-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="82717-194">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="82717-194">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="82717-195">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="82717-195">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="82717-196">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="82717-196">authenticationMethod</span></span>|[<span data-ttu-id="82717-197">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="82717-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="82717-198">Метод проверки поДлинности.</span><span class="sxs-lookup"><span data-stu-id="82717-198">Authentication method.</span></span> <span data-ttu-id="82717-199">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="82717-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="82717-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="82717-200">Response</span></span>
<span data-ttu-id="82717-201">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82717-201">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82717-202">Пример</span><span class="sxs-lookup"><span data-stu-id="82717-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="82717-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="82717-203">Request</span></span>
<span data-ttu-id="82717-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82717-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 989

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="82717-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="82717-205">Response</span></span>
<span data-ttu-id="82717-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82717-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1161

{
  "@odata.type": "#microsoft.graph.androidWorkProfileVpnConfiguration",
  "id": "32910378-0378-3291-7803-913278039132",
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




