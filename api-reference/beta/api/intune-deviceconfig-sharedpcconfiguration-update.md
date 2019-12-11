---
title: Обновление объекта sharedPCConfiguration
description: Обновляет свойства объекта sharedPCConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3120f042cb82a613ee0712782190433a0f22ab1
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947759"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="7728f-103">Обновление объекта sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="7728f-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="7728f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7728f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7728f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7728f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7728f-106">Обновляет свойства объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-106">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7728f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7728f-107">Prerequisites</span></span>
<span data-ttu-id="7728f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7728f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7728f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7728f-110">Permission type</span></span>|<span data-ttu-id="7728f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7728f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7728f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7728f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7728f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7728f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7728f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7728f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7728f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7728f-115">Not supported.</span></span>|
|<span data-ttu-id="7728f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7728f-116">Application</span></span>|<span data-ttu-id="7728f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7728f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7728f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7728f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7728f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7728f-119">Request headers</span></span>
|<span data-ttu-id="7728f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7728f-120">Header</span></span>|<span data-ttu-id="7728f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7728f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7728f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7728f-122">Authorization</span></span>|<span data-ttu-id="7728f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7728f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7728f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7728f-124">Accept</span></span>|<span data-ttu-id="7728f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7728f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7728f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7728f-126">Request body</span></span>
<span data-ttu-id="7728f-127">В теле запроса добавьте представление объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7728f-127">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="7728f-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-128">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="7728f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7728f-129">Property</span></span>|<span data-ttu-id="7728f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7728f-130">Type</span></span>|<span data-ttu-id="7728f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7728f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7728f-132">id</span><span class="sxs-lookup"><span data-stu-id="7728f-132">id</span></span>|<span data-ttu-id="7728f-133">String</span><span class="sxs-lookup"><span data-stu-id="7728f-133">String</span></span>|<span data-ttu-id="7728f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7728f-134">Key of the entity.</span></span> <span data-ttu-id="7728f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7728f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7728f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7728f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7728f-137">DateTimeOffset</span></span>|<span data-ttu-id="7728f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="7728f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="7728f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7728f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7728f-140">roleScopeTagIds</span></span>|<span data-ttu-id="7728f-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7728f-141">String collection</span></span>|<span data-ttu-id="7728f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="7728f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7728f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7728f-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="7728f-144">supportsScopeTags</span></span>|<span data-ttu-id="7728f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="7728f-145">Boolean</span></span>|<span data-ttu-id="7728f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="7728f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7728f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="7728f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7728f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="7728f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7728f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7728f-149">This property is read-only.</span></span> <span data-ttu-id="7728f-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7728f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7728f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="7728f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="7728f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="7728f-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7728f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="7728f-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7728f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7728f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="7728f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="7728f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="7728f-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7728f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="7728f-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7728f-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7728f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="7728f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="7728f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="7728f-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="7728f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="7728f-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7728f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7728f-163">createdDateTime</span></span>|<span data-ttu-id="7728f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7728f-164">DateTimeOffset</span></span>|<span data-ttu-id="7728f-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="7728f-165">DateTime the object was created.</span></span> <span data-ttu-id="7728f-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7728f-167">description</span><span class="sxs-lookup"><span data-stu-id="7728f-167">description</span></span>|<span data-ttu-id="7728f-168">String</span><span class="sxs-lookup"><span data-stu-id="7728f-168">String</span></span>|<span data-ttu-id="7728f-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7728f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7728f-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7728f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="7728f-171">displayName</span></span>|<span data-ttu-id="7728f-172">Строка</span><span class="sxs-lookup"><span data-stu-id="7728f-172">String</span></span>|<span data-ttu-id="7728f-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7728f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7728f-174">Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7728f-175">version</span><span class="sxs-lookup"><span data-stu-id="7728f-175">version</span></span>|<span data-ttu-id="7728f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7728f-176">Int32</span></span>|<span data-ttu-id="7728f-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="7728f-177">Version of the device configuration.</span></span> <span data-ttu-id="7728f-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7728f-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7728f-179">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="7728f-179">accountManagerPolicy</span></span>|[<span data-ttu-id="7728f-180">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="7728f-180">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="7728f-181">Определяет способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="7728f-181">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="7728f-182">Применяется, только если для параметра disableAccountManager установлено значение false.</span><span class="sxs-lookup"><span data-stu-id="7728f-182">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="7728f-183">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="7728f-183">allowedAccounts</span></span>|[<span data-ttu-id="7728f-184">шаредпкалловедаккаунттипе</span><span class="sxs-lookup"><span data-stu-id="7728f-184">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="7728f-185">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="7728f-185">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="7728f-186">Возможные значения: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="7728f-186">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="7728f-187">localStorage</span><span class="sxs-lookup"><span data-stu-id="7728f-187">localStorage</span></span>|[<span data-ttu-id="7728f-188">Включение</span><span class="sxs-lookup"><span data-stu-id="7728f-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7728f-189">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="7728f-189">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="7728f-190">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7728f-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7728f-191">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="7728f-191">allowLocalStorage</span></span>|<span data-ttu-id="7728f-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="7728f-192">Boolean</span></span>|<span data-ttu-id="7728f-193">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="7728f-193">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="7728f-194">сетаккаунтманажер</span><span class="sxs-lookup"><span data-stu-id="7728f-194">setAccountManager</span></span>|[<span data-ttu-id="7728f-195">Включение</span><span class="sxs-lookup"><span data-stu-id="7728f-195">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7728f-196">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="7728f-196">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="7728f-197">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7728f-197">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7728f-198">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="7728f-198">disableAccountManager</span></span>|<span data-ttu-id="7728f-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="7728f-199">Boolean</span></span>|<span data-ttu-id="7728f-200">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="7728f-200">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="7728f-201">сетедуполиЦиес</span><span class="sxs-lookup"><span data-stu-id="7728f-201">setEduPolicies</span></span>|[<span data-ttu-id="7728f-202">Включение</span><span class="sxs-lookup"><span data-stu-id="7728f-202">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7728f-203">Указывает, следует ли включать и отключать/не настраивать общие политики среды по умолчанию для образовательных учреждений.</span><span class="sxs-lookup"><span data-stu-id="7728f-203">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="7728f-204">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="7728f-204">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="7728f-205">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7728f-205">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7728f-206">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="7728f-206">disableEduPolicies</span></span>|<span data-ttu-id="7728f-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="7728f-207">Boolean</span></span>|<span data-ttu-id="7728f-208">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="7728f-208">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="7728f-209">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="7728f-209">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="7728f-210">сетповерполиЦиес</span><span class="sxs-lookup"><span data-stu-id="7728f-210">setPowerPolicies</span></span>|[<span data-ttu-id="7728f-211">Включение</span><span class="sxs-lookup"><span data-stu-id="7728f-211">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7728f-212">Указывает, следует ли включать или отключать политики управления питанием общих ПК по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7728f-212">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="7728f-213">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7728f-213">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7728f-214">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="7728f-214">disablePowerPolicies</span></span>|<span data-ttu-id="7728f-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="7728f-215">Boolean</span></span>|<span data-ttu-id="7728f-216">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="7728f-216">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="7728f-217">сигнинонресуме</span><span class="sxs-lookup"><span data-stu-id="7728f-217">signInOnResume</span></span>|[<span data-ttu-id="7728f-218">Включение</span><span class="sxs-lookup"><span data-stu-id="7728f-218">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7728f-219">Задает требование для входа в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="7728f-219">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="7728f-220">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7728f-220">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="7728f-221">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="7728f-221">disableSignInOnResume</span></span>|<span data-ttu-id="7728f-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="7728f-222">Boolean</span></span>|<span data-ttu-id="7728f-223">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="7728f-223">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="7728f-224">enabled</span><span class="sxs-lookup"><span data-stu-id="7728f-224">enabled</span></span>|<span data-ttu-id="7728f-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="7728f-225">Boolean</span></span>|<span data-ttu-id="7728f-226">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="7728f-226">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="7728f-227">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="7728f-227">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="7728f-228">Int32</span><span class="sxs-lookup"><span data-stu-id="7728f-228">Int32</span></span>|<span data-ttu-id="7728f-229">Определяет длительность (в секундах) пребывания устройства в режиме бездействия перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="7728f-229">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="7728f-230">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="7728f-230">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="7728f-231">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="7728f-231">kioskAppDisplayName</span></span>|<span data-ttu-id="7728f-232">Строка</span><span class="sxs-lookup"><span data-stu-id="7728f-232">String</span></span>|<span data-ttu-id="7728f-233">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, определяемого с помощью свойства SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="7728f-233">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="7728f-234">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="7728f-234">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="7728f-235">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="7728f-235">kioskAppUserModelId</span></span>|<span data-ttu-id="7728f-236">String</span><span class="sxs-lookup"><span data-stu-id="7728f-236">String</span></span>|<span data-ttu-id="7728f-237">Определяет идентификатор пользовательской модели для приложения, используемого с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="7728f-237">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="7728f-238">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="7728f-238">maintenanceStartTime</span></span>|<span data-ttu-id="7728f-239">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7728f-239">TimeOfDay</span></span>|<span data-ttu-id="7728f-240">Указывает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="7728f-240">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="7728f-241">фастфирстсигнин</span><span class="sxs-lookup"><span data-stu-id="7728f-241">fastFirstSignIn</span></span>|[<span data-ttu-id="7728f-242">Включение</span><span class="sxs-lookup"><span data-stu-id="7728f-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="7728f-243">Указывает, следует ли автоматически подключать новые учетные записи Azure AD, не являющиеся администраторами, к предварительно настроенным локальным учетным записям кандидатов.</span><span class="sxs-lookup"><span data-stu-id="7728f-243">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="7728f-244">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="7728f-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="7728f-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="7728f-245">Response</span></span>
<span data-ttu-id="7728f-246">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7728f-246">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7728f-247">Пример</span><span class="sxs-lookup"><span data-stu-id="7728f-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="7728f-248">Запрос</span><span class="sxs-lookup"><span data-stu-id="7728f-248">Request</span></span>
<span data-ttu-id="7728f-249">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7728f-249">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7728f-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="7728f-250">Response</span></span>
<span data-ttu-id="7728f-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7728f-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





