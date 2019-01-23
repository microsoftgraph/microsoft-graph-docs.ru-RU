---
title: Создание macOSEndpointProtectionConfiguration
description: Создание нового объекта macOSEndpointProtectionConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 31163931fd8f905b2ece59a51ba185211c70c474
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415959"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="e1c3b-103">Создание macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1c3b-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="e1c3b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1c3b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1c3b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1c3b-107">Создание нового объекта [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e1c3b-107">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1c3b-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="e1c3b-108">Prerequisites</span></span>
<span data-ttu-id="e1c3b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e1c3b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1c3b-111">Permission type</span></span>|<span data-ttu-id="e1c3b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1c3b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1c3b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1c3b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1c3b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1c3b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1c3b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1c3b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1c3b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-116">Not supported.</span></span>|
|<span data-ttu-id="e1c3b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1c3b-117">Application</span></span>|<span data-ttu-id="e1c3b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1c3b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1c3b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e1c3b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1c3b-120">Request headers</span></span>
|<span data-ttu-id="e1c3b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1c3b-121">Header</span></span>|<span data-ttu-id="e1c3b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1c3b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1c3b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1c3b-123">Authorization</span></span>|<span data-ttu-id="e1c3b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e1c3b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1c3b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1c3b-125">Accept</span></span>|<span data-ttu-id="e1c3b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1c3b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1c3b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1c3b-127">Request body</span></span>
<span data-ttu-id="e1c3b-128">В тексте запроса укажите представление JSON для объекта macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-128">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="e1c3b-129">В следующей таблице показаны свойства, которые необходимы для создания macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-129">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="e1c3b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1c3b-130">Property</span></span>|<span data-ttu-id="e1c3b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e1c3b-131">Type</span></span>|<span data-ttu-id="e1c3b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e1c3b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1c3b-133">id</span><span class="sxs-lookup"><span data-stu-id="e1c3b-133">id</span></span>|<span data-ttu-id="e1c3b-134">String</span><span class="sxs-lookup"><span data-stu-id="e1c3b-134">String</span></span>|<span data-ttu-id="e1c3b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-135">Key of the entity.</span></span> <span data-ttu-id="e1c3b-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1c3b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1c3b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e1c3b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1c3b-138">DateTimeOffset</span></span>|<span data-ttu-id="e1c3b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e1c3b-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1c3b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e1c3b-141">roleScopeTagIds</span></span>|<span data-ttu-id="e1c3b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e1c3b-142">String collection</span></span>|<span data-ttu-id="e1c3b-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e1c3b-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1c3b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e1c3b-145">supportsScopeTags</span></span>|<span data-ttu-id="e1c3b-146">Логический</span><span class="sxs-lookup"><span data-stu-id="e1c3b-146">Boolean</span></span>|<span data-ttu-id="e1c3b-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e1c3b-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e1c3b-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e1c3b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-150">This property is read-only.</span></span> <span data-ttu-id="e1c3b-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1c3b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1c3b-152">createdDateTime</span></span>|<span data-ttu-id="e1c3b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1c3b-153">DateTimeOffset</span></span>|<span data-ttu-id="e1c3b-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-154">DateTime the object was created.</span></span> <span data-ttu-id="e1c3b-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1c3b-156">description</span><span class="sxs-lookup"><span data-stu-id="e1c3b-156">description</span></span>|<span data-ttu-id="e1c3b-157">String</span><span class="sxs-lookup"><span data-stu-id="e1c3b-157">String</span></span>|<span data-ttu-id="e1c3b-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e1c3b-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1c3b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e1c3b-160">displayName</span></span>|<span data-ttu-id="e1c3b-161">String</span><span class="sxs-lookup"><span data-stu-id="e1c3b-161">String</span></span>|<span data-ttu-id="e1c3b-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e1c3b-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1c3b-164">version</span><span class="sxs-lookup"><span data-stu-id="e1c3b-164">version</span></span>|<span data-ttu-id="e1c3b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e1c3b-165">Int32</span></span>|<span data-ttu-id="e1c3b-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-166">Version of the device configuration.</span></span> <span data-ttu-id="e1c3b-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e1c3b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e1c3b-168">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="e1c3b-168">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="e1c3b-169">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="e1c3b-169">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="e1c3b-170">Система и режим конфиденциальности, который определяет, какие приложения расположений загрузки может выполняться на устройстве macOS.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-170">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="e1c3b-171">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-171">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="e1c3b-172">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="e1c3b-172">gatekeeperBlockOverride</span></span>|<span data-ttu-id="e1c3b-173">Логический</span><span class="sxs-lookup"><span data-stu-id="e1c3b-173">Boolean</span></span>|<span data-ttu-id="e1c3b-174">Если параметр имеет значение true, пользователь переопределяют для Привратник будут отключены.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-174">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="e1c3b-175">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="e1c3b-175">firewallEnabled</span></span>|<span data-ttu-id="e1c3b-176">Логический</span><span class="sxs-lookup"><span data-stu-id="e1c3b-176">Boolean</span></span>|<span data-ttu-id="e1c3b-177">Является ли брандмауэра должна быть включена или нет.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-177">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="e1c3b-178">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="e1c3b-178">firewallBlockAllIncoming</span></span>|<span data-ttu-id="e1c3b-179">Логический</span><span class="sxs-lookup"><span data-stu-id="e1c3b-179">Boolean</span></span>|<span data-ttu-id="e1c3b-180">Соответствующий параметр «Блокировать все входящие подключения».</span><span class="sxs-lookup"><span data-stu-id="e1c3b-180">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="e1c3b-181">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="e1c3b-181">firewallEnableStealthMode</span></span>|<span data-ttu-id="e1c3b-182">Логический</span><span class="sxs-lookup"><span data-stu-id="e1c3b-182">Boolean</span></span>|<span data-ttu-id="e1c3b-183">Соответствует «Включить режим скрытое».</span><span class="sxs-lookup"><span data-stu-id="e1c3b-183">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="e1c3b-184">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="e1c3b-184">firewallApplications</span></span>|<span data-ttu-id="e1c3b-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="e1c3b-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="e1c3b-186">Список приложений с помощью параметров брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-186">List of applications with firewall settings.</span></span> <span data-ttu-id="e1c3b-187">Параметры брандмауэра для приложений не в этом списке определяются пользователем.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-187">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="e1c3b-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-188">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e1c3b-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1c3b-189">Response</span></span>
<span data-ttu-id="e1c3b-190">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-190">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1c3b-191">Пример</span><span class="sxs-lookup"><span data-stu-id="e1c3b-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1c3b-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1c3b-192">Request</span></span>
<span data-ttu-id="e1c3b-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-193">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e1c3b-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1c3b-194">Response</span></span>
<span data-ttu-id="e1c3b-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e1c3b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




