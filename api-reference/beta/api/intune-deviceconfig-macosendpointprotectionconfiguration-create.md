---
title: Создание Макосендпоинтпротектионконфигуратион
description: Создание нового объекта Макосендпоинтпротектионконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d58b7fe404fa41f2858f1198160b55880323d7a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802340"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="1cd73-103">Создание Макосендпоинтпротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1cd73-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="1cd73-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cd73-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1cd73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cd73-106">Создание нового объекта [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1cd73-106">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cd73-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1cd73-107">Prerequisites</span></span>
<span data-ttu-id="1cd73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cd73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cd73-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1cd73-110">Permission type</span></span>|<span data-ttu-id="1cd73-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1cd73-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cd73-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1cd73-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1cd73-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cd73-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1cd73-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1cd73-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cd73-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd73-115">Not supported.</span></span>|
|<span data-ttu-id="1cd73-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1cd73-116">Application</span></span>|<span data-ttu-id="1cd73-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1cd73-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cd73-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1cd73-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1cd73-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1cd73-119">Request headers</span></span>
|<span data-ttu-id="1cd73-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1cd73-120">Header</span></span>|<span data-ttu-id="1cd73-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1cd73-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cd73-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1cd73-122">Authorization</span></span>|<span data-ttu-id="1cd73-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1cd73-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cd73-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1cd73-124">Accept</span></span>|<span data-ttu-id="1cd73-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1cd73-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cd73-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1cd73-126">Request body</span></span>
<span data-ttu-id="1cd73-127">В тексте запроса добавьте представление объекта Макосендпоинтпротектионконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1cd73-127">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="1cd73-128">В следующей таблице приведены свойства, необходимые при создании Макосендпоинтпротектионконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="1cd73-128">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="1cd73-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1cd73-129">Property</span></span>|<span data-ttu-id="1cd73-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1cd73-130">Type</span></span>|<span data-ttu-id="1cd73-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1cd73-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cd73-132">id</span><span class="sxs-lookup"><span data-stu-id="1cd73-132">id</span></span>|<span data-ttu-id="1cd73-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1cd73-133">String</span></span>|<span data-ttu-id="1cd73-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1cd73-134">Key of the entity.</span></span> <span data-ttu-id="1cd73-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd73-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd73-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd73-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1cd73-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd73-137">DateTimeOffset</span></span>|<span data-ttu-id="1cd73-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1cd73-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1cd73-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd73-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd73-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1cd73-140">roleScopeTagIds</span></span>|<span data-ttu-id="1cd73-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1cd73-141">String collection</span></span>|<span data-ttu-id="1cd73-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="1cd73-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1cd73-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd73-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd73-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="1cd73-144">supportsScopeTags</span></span>|<span data-ttu-id="1cd73-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cd73-145">Boolean</span></span>|<span data-ttu-id="1cd73-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="1cd73-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1cd73-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="1cd73-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1cd73-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1cd73-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1cd73-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1cd73-149">This property is read-only.</span></span> <span data-ttu-id="1cd73-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd73-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd73-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1cd73-151">createdDateTime</span></span>|<span data-ttu-id="1cd73-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cd73-152">DateTimeOffset</span></span>|<span data-ttu-id="1cd73-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1cd73-153">DateTime the object was created.</span></span> <span data-ttu-id="1cd73-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd73-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd73-155">description</span><span class="sxs-lookup"><span data-stu-id="1cd73-155">description</span></span>|<span data-ttu-id="1cd73-156">String</span><span class="sxs-lookup"><span data-stu-id="1cd73-156">String</span></span>|<span data-ttu-id="1cd73-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1cd73-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1cd73-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd73-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd73-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1cd73-159">displayName</span></span>|<span data-ttu-id="1cd73-160">String</span><span class="sxs-lookup"><span data-stu-id="1cd73-160">String</span></span>|<span data-ttu-id="1cd73-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1cd73-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1cd73-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd73-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd73-163">version</span><span class="sxs-lookup"><span data-stu-id="1cd73-163">version</span></span>|<span data-ttu-id="1cd73-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1cd73-164">Int32</span></span>|<span data-ttu-id="1cd73-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1cd73-165">Version of the device configuration.</span></span> <span data-ttu-id="1cd73-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1cd73-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cd73-167">Гатекипералловедаппсаурце</span><span class="sxs-lookup"><span data-stu-id="1cd73-167">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="1cd73-168">Макосгатекипераппсаурцес</span><span class="sxs-lookup"><span data-stu-id="1cd73-168">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="1cd73-169">Параметры системы и конфиденциальности, которые определяют, какие расположения скачивания приложения можно запускать с устройства macOS.</span><span class="sxs-lookup"><span data-stu-id="1cd73-169">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="1cd73-170">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="1cd73-170">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="1cd73-171">Гатекиперблокковерриде</span><span class="sxs-lookup"><span data-stu-id="1cd73-171">gatekeeperBlockOverride</span></span>|<span data-ttu-id="1cd73-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cd73-172">Boolean</span></span>|<span data-ttu-id="1cd73-173">Если задано значение true, переопределение пользователя для привратника будет отключено.</span><span class="sxs-lookup"><span data-stu-id="1cd73-173">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="1cd73-174">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="1cd73-174">firewallEnabled</span></span>|<span data-ttu-id="1cd73-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cd73-175">Boolean</span></span>|<span data-ttu-id="1cd73-176">Указывает, следует ли включить брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="1cd73-176">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="1cd73-177">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="1cd73-177">firewallBlockAllIncoming</span></span>|<span data-ttu-id="1cd73-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cd73-178">Boolean</span></span>|<span data-ttu-id="1cd73-179">Соответствует параметру "блокировать все входящие подключения".</span><span class="sxs-lookup"><span data-stu-id="1cd73-179">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="1cd73-180">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="1cd73-180">firewallEnableStealthMode</span></span>|<span data-ttu-id="1cd73-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cd73-181">Boolean</span></span>|<span data-ttu-id="1cd73-182">Соответствует параметру "включить скрытый режим".</span><span class="sxs-lookup"><span data-stu-id="1cd73-182">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="1cd73-183">Фиреваллаппликатионс</span><span class="sxs-lookup"><span data-stu-id="1cd73-183">firewallApplications</span></span>|<span data-ttu-id="1cd73-184">Коллекция [макосфиреваллаппликатион](../resources/intune-deviceconfig-macosfirewallapplication.md)</span><span class="sxs-lookup"><span data-stu-id="1cd73-184">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="1cd73-185">Список приложений с параметрами брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="1cd73-185">List of applications with firewall settings.</span></span> <span data-ttu-id="1cd73-186">Параметры брандмауэра для приложений, не включенных в этот список, определяются пользователем.</span><span class="sxs-lookup"><span data-stu-id="1cd73-186">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="1cd73-187">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="1cd73-187">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="1cd73-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="1cd73-188">Response</span></span>
<span data-ttu-id="1cd73-189">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосендпоинтпротектионконфигуратион](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1cd73-189">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cd73-190">Пример</span><span class="sxs-lookup"><span data-stu-id="1cd73-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="1cd73-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="1cd73-191">Request</span></span>
<span data-ttu-id="1cd73-192">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1cd73-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 647

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1cd73-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="1cd73-193">Response</span></span>
<span data-ttu-id="1cd73-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1cd73-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 819

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "7bf7f3ca-f3ca-7bf7-caf3-f77bcaf3f77b",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "gatekeeperAllowedAppSource": "macAppStore",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "Bundle Id value",
      "allowsIncomingConnections": true
    }
  ]
}
```





