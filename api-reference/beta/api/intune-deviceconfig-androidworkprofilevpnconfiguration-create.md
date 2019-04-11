---
title: Создание Андроидворкпрофилевпнконфигуратион
description: Создание нового объекта Андроидворкпрофилевпнконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 861311c0ccd008ad137a5c5f49e1f1ba96c6bb21
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775662"
---
# <a name="create-androidworkprofilevpnconfiguration"></a><span data-ttu-id="4b9cb-103">Создание Андроидворкпрофилевпнконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4b9cb-103">Create androidWorkProfileVpnConfiguration</span></span>

> <span data-ttu-id="4b9cb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b9cb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b9cb-106">Создание нового объекта [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4b9cb-106">Create a new [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b9cb-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4b9cb-107">Prerequisites</span></span>
<span data-ttu-id="4b9cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b9cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b9cb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b9cb-110">Permission type</span></span>|<span data-ttu-id="4b9cb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b9cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b9cb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b9cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b9cb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b9cb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b9cb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b9cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b9cb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-115">Not supported.</span></span>|
|<span data-ttu-id="4b9cb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b9cb-116">Application</span></span>|<span data-ttu-id="4b9cb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b9cb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b9cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4b9cb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4b9cb-119">Request headers</span></span>
|<span data-ttu-id="4b9cb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b9cb-120">Header</span></span>|<span data-ttu-id="4b9cb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4b9cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b9cb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4b9cb-122">Authorization</span></span>|<span data-ttu-id="4b9cb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b9cb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4b9cb-124">Accept</span></span>|<span data-ttu-id="4b9cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b9cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b9cb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4b9cb-126">Request body</span></span>
<span data-ttu-id="4b9cb-127">В тексте запроса добавьте представление объекта Андроидворкпрофилевпнконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-127">In the request body, supply a JSON representation for the androidWorkProfileVpnConfiguration object.</span></span>

<span data-ttu-id="4b9cb-128">В следующей таблице приведены свойства, необходимые при создании Андроидворкпрофилевпнконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-128">The following table shows the properties that are required when you create the androidWorkProfileVpnConfiguration.</span></span>

|<span data-ttu-id="4b9cb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b9cb-129">Property</span></span>|<span data-ttu-id="4b9cb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4b9cb-130">Type</span></span>|<span data-ttu-id="4b9cb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4b9cb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b9cb-132">id</span><span class="sxs-lookup"><span data-stu-id="4b9cb-132">id</span></span>|<span data-ttu-id="4b9cb-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4b9cb-133">String</span></span>|<span data-ttu-id="4b9cb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-134">Key of the entity.</span></span> <span data-ttu-id="4b9cb-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b9cb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b9cb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b9cb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4b9cb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b9cb-137">DateTimeOffset</span></span>|<span data-ttu-id="4b9cb-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4b9cb-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b9cb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b9cb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b9cb-140">roleScopeTagIds</span></span>|<span data-ttu-id="4b9cb-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4b9cb-141">String collection</span></span>|<span data-ttu-id="4b9cb-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4b9cb-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b9cb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b9cb-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4b9cb-144">supportsScopeTags</span></span>|<span data-ttu-id="4b9cb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b9cb-145">Boolean</span></span>|<span data-ttu-id="4b9cb-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4b9cb-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4b9cb-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4b9cb-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-149">This property is read-only.</span></span> <span data-ttu-id="4b9cb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b9cb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b9cb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b9cb-151">createdDateTime</span></span>|<span data-ttu-id="4b9cb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b9cb-152">DateTimeOffset</span></span>|<span data-ttu-id="4b9cb-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-153">DateTime the object was created.</span></span> <span data-ttu-id="4b9cb-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b9cb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b9cb-155">description</span><span class="sxs-lookup"><span data-stu-id="4b9cb-155">description</span></span>|<span data-ttu-id="4b9cb-156">String</span><span class="sxs-lookup"><span data-stu-id="4b9cb-156">String</span></span>|<span data-ttu-id="4b9cb-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b9cb-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b9cb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b9cb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4b9cb-159">displayName</span></span>|<span data-ttu-id="4b9cb-160">String</span><span class="sxs-lookup"><span data-stu-id="4b9cb-160">String</span></span>|<span data-ttu-id="4b9cb-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b9cb-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b9cb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b9cb-163">version</span><span class="sxs-lookup"><span data-stu-id="4b9cb-163">version</span></span>|<span data-ttu-id="4b9cb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4b9cb-164">Int32</span></span>|<span data-ttu-id="4b9cb-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-165">Version of the device configuration.</span></span> <span data-ttu-id="4b9cb-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b9cb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b9cb-167">Коннектионнаме</span><span class="sxs-lookup"><span data-stu-id="4b9cb-167">connectionName</span></span>|<span data-ttu-id="4b9cb-168">String</span><span class="sxs-lookup"><span data-stu-id="4b9cb-168">String</span></span>|<span data-ttu-id="4b9cb-169">Имя подключения, отображаемое для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-169">Connection name displayed to the user.</span></span>|
|<span data-ttu-id="4b9cb-170">connectionType</span><span class="sxs-lookup"><span data-stu-id="4b9cb-170">connectionType</span></span>|[<span data-ttu-id="4b9cb-171">androidWorkProfileVpnConnectionType</span><span class="sxs-lookup"><span data-stu-id="4b9cb-171">androidWorkProfileVpnConnectionType</span></span>](../resources/intune-deviceconfig-androidworkprofilevpnconnectiontype.md)|<span data-ttu-id="4b9cb-172">Тип подключения.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-172">Connection type.</span></span> <span data-ttu-id="4b9cb-173">Возможные значения: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-173">Possible values are: `ciscoAnyConnect`, `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`, `citrix`, `paloAltoGlobalProtect`.</span></span>|
|<span data-ttu-id="4b9cb-174">role</span><span class="sxs-lookup"><span data-stu-id="4b9cb-174">role</span></span>|<span data-ttu-id="4b9cb-175">String</span><span class="sxs-lookup"><span data-stu-id="4b9cb-175">String</span></span>|<span data-ttu-id="4b9cb-176">Роль, когда для типа подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-176">Role when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="4b9cb-177">область</span><span class="sxs-lookup"><span data-stu-id="4b9cb-177">realm</span></span>|<span data-ttu-id="4b9cb-178">String</span><span class="sxs-lookup"><span data-stu-id="4b9cb-178">String</span></span>|<span data-ttu-id="4b9cb-179">Область, когда для параметра Тип подключения задано значение Secure Pulse.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-179">Realm when connection type is set to Pulse Secure.</span></span>|
|<span data-ttu-id="4b9cb-180">серверами</span><span class="sxs-lookup"><span data-stu-id="4b9cb-180">servers</span></span>|<span data-ttu-id="4b9cb-181">Коллекция [vpnserver.](../resources/intune-deviceconfig-vpnserver.md)</span><span class="sxs-lookup"><span data-stu-id="4b9cb-181">[vpnServer](../resources/intune-deviceconfig-vpnserver.md) collection</span></span>|<span data-ttu-id="4b9cb-182">Список VPN-серверов в сети.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-182">List of VPN Servers on the network.</span></span> <span data-ttu-id="4b9cb-183">Убедитесь, что конечные пользователи могут получать доступ к этим сетевым расположениям.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-183">Make sure end users can access these network locations.</span></span> <span data-ttu-id="4b9cb-184">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="4b9cb-185">распознавания</span><span class="sxs-lookup"><span data-stu-id="4b9cb-185">fingerprint</span></span>|<span data-ttu-id="4b9cb-186">String</span><span class="sxs-lookup"><span data-stu-id="4b9cb-186">String</span></span>|<span data-ttu-id="4b9cb-187">ОтПечаток — это строка, которая будет использоваться для проверки доверенности VPN-сервера, который применяется, только если тип подключения — "VPN-метка капсулы".</span><span class="sxs-lookup"><span data-stu-id="4b9cb-187">Fingerprint is a string that will be used to verify the VPN server can be trusted, which is only applicable when connection type is Check Point Capsule VPN.</span></span>|
|<span data-ttu-id="4b9cb-188">Пользовательские</span><span class="sxs-lookup"><span data-stu-id="4b9cb-188">customData</span></span>|<span data-ttu-id="4b9cb-189">Коллекция [keyValue](../resources/intune-deviceconfig-keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="4b9cb-189">[keyValue](../resources/intune-deviceconfig-keyvalue.md) collection</span></span>|<span data-ttu-id="4b9cb-190">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-190">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="4b9cb-191">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-191">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="4b9cb-192">customKeyValueData</span><span class="sxs-lookup"><span data-stu-id="4b9cb-192">customKeyValueData</span></span>|<span data-ttu-id="4b9cb-193">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4b9cb-193">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4b9cb-194">Пользовательские данные, если для параметра Тип подключения задано значение Citrix.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-194">Custom data when connection type is set to Citrix.</span></span> <span data-ttu-id="4b9cb-195">Эта коллекция может содержать не более 25 элементов.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-195">This collection can contain a maximum of 25 elements.</span></span>|
|<span data-ttu-id="4b9cb-196">Параметр authenticationmethod</span><span class="sxs-lookup"><span data-stu-id="4b9cb-196">authenticationMethod</span></span>|[<span data-ttu-id="4b9cb-197">Впнаусентикатионмесод</span><span class="sxs-lookup"><span data-stu-id="4b9cb-197">vpnAuthenticationMethod</span></span>](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|<span data-ttu-id="4b9cb-198">Метод проверки поДлинности.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-198">Authentication method.</span></span> <span data-ttu-id="4b9cb-199">Возможные значения: `certificate`, `usernameAndPassword`.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-199">Possible values are: `certificate`, `usernameAndPassword`.</span></span>|



## <a name="response"></a><span data-ttu-id="4b9cb-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b9cb-200">Response</span></span>
<span data-ttu-id="4b9cb-201">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидворкпрофилевпнконфигуратион](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-201">If successful, this method returns a `201 Created` response code and a [androidWorkProfileVpnConfiguration](../resources/intune-deviceconfig-androidworkprofilevpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b9cb-202">Пример</span><span class="sxs-lookup"><span data-stu-id="4b9cb-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b9cb-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b9cb-203">Request</span></span>
<span data-ttu-id="4b9cb-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4b9cb-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b9cb-205">Response</span></span>
<span data-ttu-id="4b9cb-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b9cb-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





