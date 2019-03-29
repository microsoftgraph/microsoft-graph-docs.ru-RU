---
title: Создание androidForWorkVpnConfiguration
description: Создание нового объекта androidForWorkVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4dd7850d909e1dbc5aca5a4c2eac591d21a8fbd8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965657"
---
# <a name="create-androidforworkvpnconfiguration"></a><span data-ttu-id="c2dc9-103">Создание androidForWorkVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="c2dc9-103">Create androidForWorkVpnConfiguration</span></span>

> <span data-ttu-id="c2dc9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2dc9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2dc9-106">Создание нового объекта [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c2dc9-106">Create a new [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2dc9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c2dc9-107">Prerequisites</span></span>
<span data-ttu-id="c2dc9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2dc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2dc9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2dc9-110">Permission type</span></span>|<span data-ttu-id="c2dc9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2dc9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2dc9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2dc9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c2dc9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2dc9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2dc9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2dc9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2dc9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-115">Not supported.</span></span>|
|<span data-ttu-id="c2dc9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2dc9-116">Application</span></span>|<span data-ttu-id="c2dc9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2dc9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2dc9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c2dc9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2dc9-119">Request headers</span></span>
|<span data-ttu-id="c2dc9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2dc9-120">Header</span></span>|<span data-ttu-id="c2dc9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c2dc9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2dc9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2dc9-122">Authorization</span></span>|<span data-ttu-id="c2dc9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2dc9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c2dc9-124">Accept</span></span>|<span data-ttu-id="c2dc9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c2dc9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2dc9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2dc9-126">Request body</span></span>
<span data-ttu-id="c2dc9-127">В тексте запроса добавьте представление объекта androidForWorkVpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-127">In the request body, supply a JSON representation for the androidForWorkVpnConfiguration object.</span></span>

<span data-ttu-id="c2dc9-128">В следующей таблице приведены свойства, необходимые при создании androidForWorkVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-128">The following table shows the properties that are required when you create the androidForWorkVpnConfiguration.</span></span>

|<span data-ttu-id="c2dc9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2dc9-129">Property</span></span>|<span data-ttu-id="c2dc9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c2dc9-130">Type</span></span>|<span data-ttu-id="c2dc9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c2dc9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2dc9-132">id</span><span class="sxs-lookup"><span data-stu-id="c2dc9-132">id</span></span>|<span data-ttu-id="c2dc9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c2dc9-133">String</span></span>|<span data-ttu-id="c2dc9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-134">Key of the entity.</span></span> <span data-ttu-id="c2dc9-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2dc9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2dc9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2dc9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c2dc9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2dc9-137">DateTimeOffset</span></span>|<span data-ttu-id="c2dc9-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c2dc9-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2dc9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2dc9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c2dc9-140">roleScopeTagIds</span></span>|<span data-ttu-id="c2dc9-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c2dc9-141">String collection</span></span>|<span data-ttu-id="c2dc9-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c2dc9-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2dc9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2dc9-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c2dc9-144">supportsScopeTags</span></span>|<span data-ttu-id="c2dc9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2dc9-145">Boolean</span></span>|<span data-ttu-id="c2dc9-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c2dc9-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c2dc9-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c2dc9-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-149">This property is read-only.</span></span> <span data-ttu-id="c2dc9-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2dc9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2dc9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c2dc9-151">createdDateTime</span></span>|<span data-ttu-id="c2dc9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2dc9-152">DateTimeOffset</span></span>|<span data-ttu-id="c2dc9-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-153">DateTime the object was created.</span></span> <span data-ttu-id="c2dc9-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2dc9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2dc9-155">description</span><span class="sxs-lookup"><span data-stu-id="c2dc9-155">description</span></span>|<span data-ttu-id="c2dc9-156">String</span><span class="sxs-lookup"><span data-stu-id="c2dc9-156">String</span></span>|<span data-ttu-id="c2dc9-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c2dc9-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2dc9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2dc9-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c2dc9-159">displayName</span></span>|<span data-ttu-id="c2dc9-160">String</span><span class="sxs-lookup"><span data-stu-id="c2dc9-160">String</span></span>|<span data-ttu-id="c2dc9-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c2dc9-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2dc9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2dc9-163">version</span><span class="sxs-lookup"><span data-stu-id="c2dc9-163">version</span></span>|<span data-ttu-id="c2dc9-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c2dc9-164">Int32</span></span>|<span data-ttu-id="c2dc9-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-165">Version of the device configuration.</span></span> <span data-ttu-id="c2dc9-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c2dc9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c2dc9-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="c2dc9-167">connectionName</span></span>|<span data-ttu-id="c2dc9-168">String</span><span class="sxs-lookup"><span data-stu-id="c2dc9-168">String</span></span>|<span data-ttu-id="c2dc9-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-169">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="c2dc9-170">connectionType</span><span class="sxs-lookup"><span data-stu-id="c2dc9-170">connectionType</span></span>|[<span data-ttu-id="c2dc9-171">Androidforworkvpnconnectiontype.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-171">androidForWorkVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|<span data-ttu-id="c2dc9-172">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-172">Connection type.</span></span> <span data-ttu-id="c2dc9-173">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-173">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`.</span></span>|
|<span data-ttu-id="c2dc9-174">role</span><span class="sxs-lookup"><span data-stu-id="c2dc9-174">role</span></span>|<span data-ttu-id="c2dc9-175">String</span><span class="sxs-lookup"><span data-stu-id="c2dc9-175">String</span></span>|<span data-ttu-id="c2dc9-176">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-176">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="c2dc9-177">область</span><span class="sxs-lookup"><span data-stu-id="c2dc9-177">realm</span></span>|<span data-ttu-id="c2dc9-178">String</span><span class="sxs-lookup"><span data-stu-id="c2dc9-178">String</span></span>|<span data-ttu-id="c2dc9-179">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-179">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="c2dc9-180">серверами</span><span class="sxs-lookup"><span data-stu-id="c2dc9-180">servers</span></span>|<span data-ttu-id="c2dc9-181">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="c2dc9-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="c2dc9-182">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-182">List of VPN Servers on the network.</span></span> <span data-ttu-id="c2dc9-183">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-183">Make sure end users can access these network locations.</span></span> <span data-ttu-id="c2dc9-184">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="c2dc9-185">распознавания</span><span class="sxs-lookup"><span data-stu-id="c2dc9-185">fingerprint</span></span>|<span data-ttu-id="c2dc9-186">String</span><span class="sxs-lookup"><span data-stu-id="c2dc9-186">String</span></span>|<span data-ttu-id="c2dc9-187">ОтПечаток — это строка, которая будет использоваться для проверки доверенности VPN-сервера, который применяется, только если тип подключения — "VPN-метка капсулы".</span><span class="sxs-lookup"><span data-stu-id="c2dc9-187">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="c2dc9-188">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="c2dc9-188">customData</span></span>|<span data-ttu-id="c2dc9-189">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="c2dc9-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="c2dc9-190">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-190">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="c2dc9-191">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-191">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="c2dc9-192">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="c2dc9-192">customKeyValueData</span></span>|<span data-ttu-id="c2dc9-193">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c2dc9-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="c2dc9-194">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-194">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="c2dc9-195">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-195">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="c2dc9-196">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="c2dc9-196">authenticationMethod</span></span>|[<span data-ttu-id="c2dc9-197">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="c2dc9-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="c2dc9-198">Метод проверки поДлинности.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-198">Authentication method.</span></span> <span data-ttu-id="c2dc9-199">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="c2dc9-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2dc9-200">Response</span></span>
<span data-ttu-id="c2dc9-201">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-201">If successful, this method returns a `201 Created` response code and a [androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2dc9-202">Пример</span><span class="sxs-lookup"><span data-stu-id="c2dc9-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2dc9-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2dc9-203">Request</span></span>
<span data-ttu-id="c2dc9-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 985

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="c2dc9-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2dc9-205">Response</span></span>
<span data-ttu-id="c2dc9-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2dc9-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1157

{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
  "id": "2cf4c52c-c52c-2cf4-2cc5-f42c2cc5f42c",
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




