---
title: Создание macOSEndpointProtectionConfiguration
description: Создание нового объекта macOSEndpointProtectionConfiguration.
author: tfitzmac
ms.openlocfilehash: 49f50856b00229ab6df952847172cda9b7cd19f0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302109"
---
# <a name="create-macosendpointprotectionconfiguration"></a><span data-ttu-id="2472f-103">Создание macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="2472f-103">Create macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="2472f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2472f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2472f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2472f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2472f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2472f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2472f-107">Создание нового объекта [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2472f-107">Create a new [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2472f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2472f-108">Prerequisites</span></span>
<span data-ttu-id="2472f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2472f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2472f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2472f-111">Permission type</span></span>|<span data-ttu-id="2472f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2472f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2472f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2472f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2472f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2472f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2472f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2472f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2472f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2472f-116">Not supported.</span></span>|
|<span data-ttu-id="2472f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2472f-117">Application</span></span>|<span data-ttu-id="2472f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2472f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2472f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2472f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2472f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2472f-120">Request headers</span></span>
|<span data-ttu-id="2472f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2472f-121">Header</span></span>|<span data-ttu-id="2472f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2472f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2472f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2472f-123">Authorization</span></span>|<span data-ttu-id="2472f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2472f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2472f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2472f-125">Accept</span></span>|<span data-ttu-id="2472f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2472f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2472f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2472f-127">Request body</span></span>
<span data-ttu-id="2472f-128">В тексте запроса укажите представление JSON для объекта macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2472f-128">In the request body, supply a JSON representation for the macOSEndpointProtectionConfiguration object.</span></span>

<span data-ttu-id="2472f-129">В следующей таблице показаны свойства, которые необходимы для создания macOSEndpointProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2472f-129">The following table shows the properties that are required when you create the macOSEndpointProtectionConfiguration.</span></span>

|<span data-ttu-id="2472f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2472f-130">Property</span></span>|<span data-ttu-id="2472f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2472f-131">Type</span></span>|<span data-ttu-id="2472f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2472f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2472f-133">id</span><span class="sxs-lookup"><span data-stu-id="2472f-133">id</span></span>|<span data-ttu-id="2472f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2472f-134">String</span></span>|<span data-ttu-id="2472f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2472f-135">Key of the entity.</span></span> <span data-ttu-id="2472f-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2472f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2472f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2472f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2472f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2472f-138">DateTimeOffset</span></span>|<span data-ttu-id="2472f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2472f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2472f-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2472f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2472f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2472f-141">roleScopeTagIds</span></span>|<span data-ttu-id="2472f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2472f-142">String collection</span></span>|<span data-ttu-id="2472f-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2472f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2472f-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2472f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2472f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2472f-145">supportsScopeTags</span></span>|<span data-ttu-id="2472f-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2472f-146">Boolean</span></span>|<span data-ttu-id="2472f-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="2472f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2472f-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="2472f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2472f-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2472f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2472f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2472f-150">This property is read-only.</span></span> <span data-ttu-id="2472f-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2472f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2472f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2472f-152">createdDateTime</span></span>|<span data-ttu-id="2472f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2472f-153">DateTimeOffset</span></span>|<span data-ttu-id="2472f-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2472f-154">DateTime the object was created.</span></span> <span data-ttu-id="2472f-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2472f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2472f-156">описание</span><span class="sxs-lookup"><span data-stu-id="2472f-156">description</span></span>|<span data-ttu-id="2472f-157">Строка</span><span class="sxs-lookup"><span data-stu-id="2472f-157">String</span></span>|<span data-ttu-id="2472f-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2472f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2472f-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2472f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2472f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2472f-160">displayName</span></span>|<span data-ttu-id="2472f-161">Строка</span><span class="sxs-lookup"><span data-stu-id="2472f-161">String</span></span>|<span data-ttu-id="2472f-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2472f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2472f-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2472f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2472f-164">version</span><span class="sxs-lookup"><span data-stu-id="2472f-164">version</span></span>|<span data-ttu-id="2472f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2472f-165">Int32</span></span>|<span data-ttu-id="2472f-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2472f-166">Version of the device configuration.</span></span> <span data-ttu-id="2472f-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2472f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2472f-168">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="2472f-168">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="2472f-169">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="2472f-169">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="2472f-170">Система и режим конфиденциальности, который определяет, какие приложения расположений загрузки может выполняться на устройстве macOS.</span><span class="sxs-lookup"><span data-stu-id="2472f-170">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="2472f-171">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="2472f-171">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="2472f-172">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="2472f-172">gatekeeperBlockOverride</span></span>|<span data-ttu-id="2472f-173">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2472f-173">Boolean</span></span>|<span data-ttu-id="2472f-174">Если параметр имеет значение true, пользователь переопределяют для Привратник будут отключены.</span><span class="sxs-lookup"><span data-stu-id="2472f-174">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="2472f-175">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="2472f-175">firewallEnabled</span></span>|<span data-ttu-id="2472f-176">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2472f-176">Boolean</span></span>|<span data-ttu-id="2472f-177">Является ли брандмауэра должна быть включена или нет.</span><span class="sxs-lookup"><span data-stu-id="2472f-177">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="2472f-178">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="2472f-178">firewallBlockAllIncoming</span></span>|<span data-ttu-id="2472f-179">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2472f-179">Boolean</span></span>|<span data-ttu-id="2472f-180">Соответствующий параметр «Блокировать все входящие подключения».</span><span class="sxs-lookup"><span data-stu-id="2472f-180">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="2472f-181">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="2472f-181">firewallEnableStealthMode</span></span>|<span data-ttu-id="2472f-182">Boolean.</span><span class="sxs-lookup"><span data-stu-id="2472f-182">Boolean</span></span>|<span data-ttu-id="2472f-183">Соответствует «Включить режим скрытое».</span><span class="sxs-lookup"><span data-stu-id="2472f-183">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="2472f-184">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="2472f-184">firewallApplications</span></span>|<span data-ttu-id="2472f-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="2472f-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="2472f-186">Список приложений с помощью параметров брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="2472f-186">List of applications with firewall settings.</span></span> <span data-ttu-id="2472f-187">Параметры брандмауэра для приложений не в этом списке определяются пользователем.</span><span class="sxs-lookup"><span data-stu-id="2472f-187">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="2472f-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="2472f-188">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="2472f-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="2472f-189">Response</span></span>
<span data-ttu-id="2472f-190">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2472f-190">If successful, this method returns a `201 Created` response code and a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2472f-191">Пример</span><span class="sxs-lookup"><span data-stu-id="2472f-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="2472f-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="2472f-192">Request</span></span>
<span data-ttu-id="2472f-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2472f-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 711

{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="2472f-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="2472f-194">Response</span></span>
<span data-ttu-id="2472f-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2472f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





