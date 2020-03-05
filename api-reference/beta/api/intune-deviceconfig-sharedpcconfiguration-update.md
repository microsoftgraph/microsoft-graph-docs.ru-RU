---
title: Обновление объекта sharedPCConfiguration
description: Обновляет свойства объекта sharedPCConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 70efa1d7ce0ce07d1281db6a8fdaa0ec83562cc1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42482848"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="22a88-103">Обновление объекта sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="22a88-103">Update sharedPCConfiguration</span></span>

<span data-ttu-id="22a88-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="22a88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22a88-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22a88-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22a88-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22a88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22a88-107">Обновляет свойства объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-107">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22a88-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22a88-108">Prerequisites</span></span>
<span data-ttu-id="22a88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22a88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22a88-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22a88-111">Permission type</span></span>|<span data-ttu-id="22a88-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22a88-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22a88-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22a88-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22a88-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22a88-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="22a88-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22a88-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22a88-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22a88-116">Not supported.</span></span>|
|<span data-ttu-id="22a88-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22a88-117">Application</span></span>|<span data-ttu-id="22a88-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22a88-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22a88-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22a88-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="22a88-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="22a88-120">Request headers</span></span>
|<span data-ttu-id="22a88-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22a88-121">Header</span></span>|<span data-ttu-id="22a88-122">Значение</span><span class="sxs-lookup"><span data-stu-id="22a88-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22a88-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22a88-123">Authorization</span></span>|<span data-ttu-id="22a88-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22a88-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22a88-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22a88-125">Accept</span></span>|<span data-ttu-id="22a88-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22a88-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22a88-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22a88-127">Request body</span></span>
<span data-ttu-id="22a88-128">В теле запроса добавьте представление объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22a88-128">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="22a88-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-129">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="22a88-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="22a88-130">Property</span></span>|<span data-ttu-id="22a88-131">Тип</span><span class="sxs-lookup"><span data-stu-id="22a88-131">Type</span></span>|<span data-ttu-id="22a88-132">Описание</span><span class="sxs-lookup"><span data-stu-id="22a88-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22a88-133">id</span><span class="sxs-lookup"><span data-stu-id="22a88-133">id</span></span>|<span data-ttu-id="22a88-134">String</span><span class="sxs-lookup"><span data-stu-id="22a88-134">String</span></span>|<span data-ttu-id="22a88-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="22a88-135">Key of the entity.</span></span> <span data-ttu-id="22a88-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a88-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22a88-137">lastModifiedDateTime</span></span>|<span data-ttu-id="22a88-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22a88-138">DateTimeOffset</span></span>|<span data-ttu-id="22a88-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="22a88-139">DateTime the object was last modified.</span></span> <span data-ttu-id="22a88-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a88-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="22a88-141">roleScopeTagIds</span></span>|<span data-ttu-id="22a88-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="22a88-142">String collection</span></span>|<span data-ttu-id="22a88-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="22a88-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="22a88-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a88-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="22a88-145">supportsScopeTags</span></span>|<span data-ttu-id="22a88-146">Логический</span><span class="sxs-lookup"><span data-stu-id="22a88-146">Boolean</span></span>|<span data-ttu-id="22a88-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="22a88-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="22a88-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="22a88-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="22a88-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="22a88-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="22a88-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="22a88-150">This property is read-only.</span></span> <span data-ttu-id="22a88-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a88-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22a88-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="22a88-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="22a88-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="22a88-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="22a88-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="22a88-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a88-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22a88-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="22a88-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="22a88-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="22a88-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="22a88-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="22a88-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a88-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22a88-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="22a88-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="22a88-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="22a88-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="22a88-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="22a88-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a88-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22a88-164">createdDateTime</span></span>|<span data-ttu-id="22a88-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22a88-165">DateTimeOffset</span></span>|<span data-ttu-id="22a88-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="22a88-166">DateTime the object was created.</span></span> <span data-ttu-id="22a88-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a88-168">description</span><span class="sxs-lookup"><span data-stu-id="22a88-168">description</span></span>|<span data-ttu-id="22a88-169">String</span><span class="sxs-lookup"><span data-stu-id="22a88-169">String</span></span>|<span data-ttu-id="22a88-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="22a88-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="22a88-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a88-172">displayName</span><span class="sxs-lookup"><span data-stu-id="22a88-172">displayName</span></span>|<span data-ttu-id="22a88-173">Строка</span><span class="sxs-lookup"><span data-stu-id="22a88-173">String</span></span>|<span data-ttu-id="22a88-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="22a88-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="22a88-175">Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a88-176">version</span><span class="sxs-lookup"><span data-stu-id="22a88-176">version</span></span>|<span data-ttu-id="22a88-177">Int32</span><span class="sxs-lookup"><span data-stu-id="22a88-177">Int32</span></span>|<span data-ttu-id="22a88-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="22a88-178">Version of the device configuration.</span></span> <span data-ttu-id="22a88-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="22a88-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="22a88-180">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="22a88-180">accountManagerPolicy</span></span>|[<span data-ttu-id="22a88-181">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="22a88-181">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="22a88-182">Определяет способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="22a88-182">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="22a88-183">Применяется, только если для параметра disableAccountManager установлено значение false.</span><span class="sxs-lookup"><span data-stu-id="22a88-183">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="22a88-184">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="22a88-184">allowedAccounts</span></span>|[<span data-ttu-id="22a88-185">шаредпкалловедаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="22a88-185">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="22a88-186">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="22a88-186">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="22a88-187">Возможные значения: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="22a88-187">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="22a88-188">localStorage</span><span class="sxs-lookup"><span data-stu-id="22a88-188">localStorage</span></span>|[<span data-ttu-id="22a88-189">Включение</span><span class="sxs-lookup"><span data-stu-id="22a88-189">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="22a88-190">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="22a88-190">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="22a88-191">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="22a88-191">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="22a88-192">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="22a88-192">allowLocalStorage</span></span>|<span data-ttu-id="22a88-193">Логический</span><span class="sxs-lookup"><span data-stu-id="22a88-193">Boolean</span></span>|<span data-ttu-id="22a88-194">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="22a88-194">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="22a88-195">сетаккаунтманажер</span><span class="sxs-lookup"><span data-stu-id="22a88-195">setAccountManager</span></span>|[<span data-ttu-id="22a88-196">Включение</span><span class="sxs-lookup"><span data-stu-id="22a88-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="22a88-197">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="22a88-197">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="22a88-198">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="22a88-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="22a88-199">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="22a88-199">disableAccountManager</span></span>|<span data-ttu-id="22a88-200">Логический</span><span class="sxs-lookup"><span data-stu-id="22a88-200">Boolean</span></span>|<span data-ttu-id="22a88-201">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="22a88-201">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="22a88-202">сетедуполиЦиес</span><span class="sxs-lookup"><span data-stu-id="22a88-202">setEduPolicies</span></span>|[<span data-ttu-id="22a88-203">Включение</span><span class="sxs-lookup"><span data-stu-id="22a88-203">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="22a88-204">Указывает, следует ли включать и отключать/не настраивать общие политики среды по умолчанию для образовательных учреждений.</span><span class="sxs-lookup"><span data-stu-id="22a88-204">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="22a88-205">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="22a88-205">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="22a88-206">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="22a88-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="22a88-207">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="22a88-207">disableEduPolicies</span></span>|<span data-ttu-id="22a88-208">Логический</span><span class="sxs-lookup"><span data-stu-id="22a88-208">Boolean</span></span>|<span data-ttu-id="22a88-209">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="22a88-209">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="22a88-210">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="22a88-210">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="22a88-211">сетповерполиЦиес</span><span class="sxs-lookup"><span data-stu-id="22a88-211">setPowerPolicies</span></span>|[<span data-ttu-id="22a88-212">Включение</span><span class="sxs-lookup"><span data-stu-id="22a88-212">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="22a88-213">Указывает, следует ли включать или отключать политики управления питанием общих ПК по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="22a88-213">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="22a88-214">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="22a88-214">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="22a88-215">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="22a88-215">disablePowerPolicies</span></span>|<span data-ttu-id="22a88-216">Логический</span><span class="sxs-lookup"><span data-stu-id="22a88-216">Boolean</span></span>|<span data-ttu-id="22a88-217">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="22a88-217">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="22a88-218">сигнинонресуме</span><span class="sxs-lookup"><span data-stu-id="22a88-218">signInOnResume</span></span>|[<span data-ttu-id="22a88-219">Включение</span><span class="sxs-lookup"><span data-stu-id="22a88-219">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="22a88-220">Задает требование для входа в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="22a88-220">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="22a88-221">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="22a88-221">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="22a88-222">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="22a88-222">disableSignInOnResume</span></span>|<span data-ttu-id="22a88-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a88-223">Boolean</span></span>|<span data-ttu-id="22a88-224">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="22a88-224">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="22a88-225">enabled</span><span class="sxs-lookup"><span data-stu-id="22a88-225">enabled</span></span>|<span data-ttu-id="22a88-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="22a88-226">Boolean</span></span>|<span data-ttu-id="22a88-227">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="22a88-227">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="22a88-228">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="22a88-228">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="22a88-229">Int32</span><span class="sxs-lookup"><span data-stu-id="22a88-229">Int32</span></span>|<span data-ttu-id="22a88-230">Определяет длительность (в секундах) пребывания устройства в режиме бездействия перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="22a88-230">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="22a88-231">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="22a88-231">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="22a88-232">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="22a88-232">kioskAppDisplayName</span></span>|<span data-ttu-id="22a88-233">String</span><span class="sxs-lookup"><span data-stu-id="22a88-233">String</span></span>|<span data-ttu-id="22a88-234">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, определяемого с помощью свойства SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="22a88-234">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="22a88-235">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="22a88-235">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="22a88-236">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="22a88-236">kioskAppUserModelId</span></span>|<span data-ttu-id="22a88-237">String</span><span class="sxs-lookup"><span data-stu-id="22a88-237">String</span></span>|<span data-ttu-id="22a88-238">Определяет идентификатор пользовательской модели для приложения, используемого с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="22a88-238">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="22a88-239">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="22a88-239">maintenanceStartTime</span></span>|<span data-ttu-id="22a88-240">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="22a88-240">TimeOfDay</span></span>|<span data-ttu-id="22a88-241">Указывает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="22a88-241">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="22a88-242">фастфирстсигнин</span><span class="sxs-lookup"><span data-stu-id="22a88-242">fastFirstSignIn</span></span>|[<span data-ttu-id="22a88-243">Включение</span><span class="sxs-lookup"><span data-stu-id="22a88-243">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="22a88-244">Указывает, следует ли автоматически подключать новые учетные записи Azure AD, не являющиеся администраторами, к предварительно настроенным локальным учетным записям кандидатов.</span><span class="sxs-lookup"><span data-stu-id="22a88-244">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="22a88-245">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="22a88-245">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="22a88-246">Отклик</span><span class="sxs-lookup"><span data-stu-id="22a88-246">Response</span></span>
<span data-ttu-id="22a88-247">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="22a88-247">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22a88-248">Пример</span><span class="sxs-lookup"><span data-stu-id="22a88-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="22a88-249">Запрос</span><span class="sxs-lookup"><span data-stu-id="22a88-249">Request</span></span>
<span data-ttu-id="22a88-250">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22a88-250">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1920

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "guest",
  "localStorage": "enabled",
  "allowLocalStorage": true,
  "setAccountManager": "enabled",
  "disableAccountManager": true,
  "setEduPolicies": "enabled",
  "disableEduPolicies": true,
  "setPowerPolicies": "enabled",
  "disablePowerPolicies": true,
  "signInOnResume": "enabled",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000",
  "fastFirstSignIn": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="22a88-251">Отклик</span><span class="sxs-lookup"><span data-stu-id="22a88-251">Response</span></span>
<span data-ttu-id="22a88-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="22a88-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2092

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "guest",
  "localStorage": "enabled",
  "allowLocalStorage": true,
  "setAccountManager": "enabled",
  "disableAccountManager": true,
  "setEduPolicies": "enabled",
  "disableEduPolicies": true,
  "setPowerPolicies": "enabled",
  "disablePowerPolicies": true,
  "signInOnResume": "enabled",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000",
  "fastFirstSignIn": "enabled"
}
```





