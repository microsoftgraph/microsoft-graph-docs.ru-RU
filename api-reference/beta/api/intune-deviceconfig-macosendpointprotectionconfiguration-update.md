---
title: Обновление macOSEndpointProtectionConfiguration
description: Обновление свойства объекта macOSEndpointProtectionConfiguration.
author: tfitzmac
ms.openlocfilehash: 27860f298f6b0e2de12af33c8137df07a6fa16f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338607"
---
# <a name="update-macosendpointprotectionconfiguration"></a><span data-ttu-id="7a282-103">Обновление macOSEndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="7a282-103">Update macOSEndpointProtectionConfiguration</span></span>

> <span data-ttu-id="7a282-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7a282-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a282-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a282-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a282-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7a282-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7a282-107">Обновление свойства объекта [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7a282-107">Update the properties of a [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7a282-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7a282-108">Prerequisites</span></span>
<span data-ttu-id="7a282-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a282-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a282-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a282-111">Permission type</span></span>|<span data-ttu-id="7a282-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a282-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7a282-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a282-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7a282-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a282-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7a282-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a282-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7a282-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a282-116">Not supported.</span></span>|
|<span data-ttu-id="7a282-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a282-117">Application</span></span>|<span data-ttu-id="7a282-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a282-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7a282-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a282-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7a282-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a282-120">Request headers</span></span>
|<span data-ttu-id="7a282-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7a282-121">Header</span></span>|<span data-ttu-id="7a282-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7a282-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7a282-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7a282-123">Authorization</span></span>|<span data-ttu-id="7a282-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7a282-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7a282-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7a282-125">Accept</span></span>|<span data-ttu-id="7a282-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7a282-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7a282-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a282-127">Request body</span></span>
<span data-ttu-id="7a282-128">В тексте запроса укажите представление JSON для объекта [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="7a282-128">In the request body, supply a JSON representation for the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="7a282-129">В следующей таблице показаны свойства, которые необходимы для создания [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a282-129">The following table shows the properties that are required when you create the [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md).</span></span>

|<span data-ttu-id="7a282-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a282-130">Property</span></span>|<span data-ttu-id="7a282-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7a282-131">Type</span></span>|<span data-ttu-id="7a282-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7a282-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a282-133">id</span><span class="sxs-lookup"><span data-stu-id="7a282-133">id</span></span>|<span data-ttu-id="7a282-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7a282-134">String</span></span>|<span data-ttu-id="7a282-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7a282-135">Key of the entity.</span></span> <span data-ttu-id="7a282-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a282-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a282-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7a282-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7a282-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a282-138">DateTimeOffset</span></span>|<span data-ttu-id="7a282-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7a282-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7a282-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a282-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a282-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7a282-141">roleScopeTagIds</span></span>|<span data-ttu-id="7a282-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7a282-142">String collection</span></span>|<span data-ttu-id="7a282-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7a282-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7a282-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a282-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a282-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7a282-145">supportsScopeTags</span></span>|<span data-ttu-id="7a282-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="7a282-146">Boolean</span></span>|<span data-ttu-id="7a282-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="7a282-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7a282-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="7a282-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7a282-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7a282-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7a282-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a282-150">This property is read-only.</span></span> <span data-ttu-id="7a282-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a282-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a282-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7a282-152">createdDateTime</span></span>|<span data-ttu-id="7a282-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a282-153">DateTimeOffset</span></span>|<span data-ttu-id="7a282-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7a282-154">DateTime the object was created.</span></span> <span data-ttu-id="7a282-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a282-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a282-156">описание</span><span class="sxs-lookup"><span data-stu-id="7a282-156">description</span></span>|<span data-ttu-id="7a282-157">Строка</span><span class="sxs-lookup"><span data-stu-id="7a282-157">String</span></span>|<span data-ttu-id="7a282-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7a282-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7a282-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a282-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a282-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7a282-160">displayName</span></span>|<span data-ttu-id="7a282-161">Строка</span><span class="sxs-lookup"><span data-stu-id="7a282-161">String</span></span>|<span data-ttu-id="7a282-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7a282-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7a282-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a282-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a282-164">version</span><span class="sxs-lookup"><span data-stu-id="7a282-164">version</span></span>|<span data-ttu-id="7a282-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7a282-165">Int32</span></span>|<span data-ttu-id="7a282-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7a282-166">Version of the device configuration.</span></span> <span data-ttu-id="7a282-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7a282-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7a282-168">gatekeeperAllowedAppSource</span><span class="sxs-lookup"><span data-stu-id="7a282-168">gatekeeperAllowedAppSource</span></span>|[<span data-ttu-id="7a282-169">macOSGatekeeperAppSources</span><span class="sxs-lookup"><span data-stu-id="7a282-169">macOSGatekeeperAppSources</span></span>](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|<span data-ttu-id="7a282-170">Система и режим конфиденциальности, который определяет, какие приложения расположений загрузки может выполняться на устройстве macOS.</span><span class="sxs-lookup"><span data-stu-id="7a282-170">System and Privacy setting that determines which download locations apps can be run from on a macOS device.</span></span> <span data-ttu-id="7a282-171">Возможные значения: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span><span class="sxs-lookup"><span data-stu-id="7a282-171">Possible values are: `notConfigured`, `macAppStore`, `macAppStoreAndIdentifiedDevelopers`, `anywhere`.</span></span>|
|<span data-ttu-id="7a282-172">gatekeeperBlockOverride</span><span class="sxs-lookup"><span data-stu-id="7a282-172">gatekeeperBlockOverride</span></span>|<span data-ttu-id="7a282-173">Boolean.</span><span class="sxs-lookup"><span data-stu-id="7a282-173">Boolean</span></span>|<span data-ttu-id="7a282-174">Если параметр имеет значение true, пользователь переопределяют для Привратник будут отключены.</span><span class="sxs-lookup"><span data-stu-id="7a282-174">If set to true, the user override for Gatekeeper will be disabled.</span></span>|
|<span data-ttu-id="7a282-175">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="7a282-175">firewallEnabled</span></span>|<span data-ttu-id="7a282-176">Boolean.</span><span class="sxs-lookup"><span data-stu-id="7a282-176">Boolean</span></span>|<span data-ttu-id="7a282-177">Является ли брандмауэра должна быть включена или нет.</span><span class="sxs-lookup"><span data-stu-id="7a282-177">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="7a282-178">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="7a282-178">firewallBlockAllIncoming</span></span>|<span data-ttu-id="7a282-179">Boolean.</span><span class="sxs-lookup"><span data-stu-id="7a282-179">Boolean</span></span>|<span data-ttu-id="7a282-180">Соответствующий параметр «Блокировать все входящие подключения».</span><span class="sxs-lookup"><span data-stu-id="7a282-180">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="7a282-181">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="7a282-181">firewallEnableStealthMode</span></span>|<span data-ttu-id="7a282-182">Boolean.</span><span class="sxs-lookup"><span data-stu-id="7a282-182">Boolean</span></span>|<span data-ttu-id="7a282-183">Соответствует «Включить режим скрытое».</span><span class="sxs-lookup"><span data-stu-id="7a282-183">Corresponds to “Enable stealth mode.”</span></span>|
|<span data-ttu-id="7a282-184">firewallApplications</span><span class="sxs-lookup"><span data-stu-id="7a282-184">firewallApplications</span></span>|<span data-ttu-id="7a282-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="7a282-185">[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md) collection</span></span>|<span data-ttu-id="7a282-186">Список приложений с помощью параметров брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="7a282-186">List of applications with firewall settings.</span></span> <span data-ttu-id="7a282-187">Параметры брандмауэра для приложений не в этом списке определяются пользователем.</span><span class="sxs-lookup"><span data-stu-id="7a282-187">Firewall settings for applications not on this list are determined by the user.</span></span> <span data-ttu-id="7a282-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="7a282-188">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="7a282-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a282-189">Response</span></span>
<span data-ttu-id="7a282-190">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7a282-190">If successful, this method returns a `200 OK` response code and an updated [macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a282-191">Пример</span><span class="sxs-lookup"><span data-stu-id="7a282-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="7a282-192">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a282-192">Request</span></span>
<span data-ttu-id="7a282-193">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a282-193">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 636

{
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

### <a name="response"></a><span data-ttu-id="7a282-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="7a282-194">Response</span></span>
<span data-ttu-id="7a282-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7a282-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





