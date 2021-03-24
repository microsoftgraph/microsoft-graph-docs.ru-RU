---
title: Обновление объекта sharedPCConfiguration
description: Обновляет свойства объекта sharedPCConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ed8402d459a750f120754a5e33a087656de958b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137086"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="4428c-103">Обновление объекта sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="4428c-103">Update sharedPCConfiguration</span></span>

<span data-ttu-id="4428c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4428c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4428c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4428c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4428c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4428c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4428c-107">Обновляет свойства объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-107">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4428c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4428c-108">Prerequisites</span></span>
<span data-ttu-id="4428c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4428c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4428c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4428c-111">Permission type</span></span>|<span data-ttu-id="4428c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4428c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4428c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4428c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4428c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4428c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4428c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4428c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4428c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4428c-116">Not supported.</span></span>|
|<span data-ttu-id="4428c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4428c-117">Application</span></span>|<span data-ttu-id="4428c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4428c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4428c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4428c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4428c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4428c-120">Request headers</span></span>
|<span data-ttu-id="4428c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4428c-121">Header</span></span>|<span data-ttu-id="4428c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4428c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4428c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4428c-123">Authorization</span></span>|<span data-ttu-id="4428c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4428c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4428c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4428c-125">Accept</span></span>|<span data-ttu-id="4428c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4428c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4428c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4428c-127">Request body</span></span>
<span data-ttu-id="4428c-128">В теле запроса добавьте представление объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4428c-128">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="4428c-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-129">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="4428c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4428c-130">Property</span></span>|<span data-ttu-id="4428c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4428c-131">Type</span></span>|<span data-ttu-id="4428c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4428c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4428c-133">id</span><span class="sxs-lookup"><span data-stu-id="4428c-133">id</span></span>|<span data-ttu-id="4428c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4428c-134">String</span></span>|<span data-ttu-id="4428c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4428c-135">Key of the entity.</span></span> <span data-ttu-id="4428c-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4428c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4428c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4428c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4428c-138">DateTimeOffset</span></span>|<span data-ttu-id="4428c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4428c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4428c-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4428c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4428c-141">roleScopeTagIds</span></span>|<span data-ttu-id="4428c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4428c-142">String collection</span></span>|<span data-ttu-id="4428c-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="4428c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4428c-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4428c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4428c-145">supportsScopeTags</span></span>|<span data-ttu-id="4428c-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4428c-146">Boolean</span></span>|<span data-ttu-id="4428c-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4428c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4428c-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="4428c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4428c-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4428c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4428c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4428c-150">This property is read-only.</span></span> <span data-ttu-id="4428c-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4428c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4428c-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4428c-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4428c-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4428c-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4428c-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4428c-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4428c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4428c-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4428c-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4428c-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4428c-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4428c-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4428c-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4428c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4428c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4428c-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4428c-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4428c-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4428c-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4428c-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4428c-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4428c-164">createdDateTime</span></span>|<span data-ttu-id="4428c-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4428c-165">DateTimeOffset</span></span>|<span data-ttu-id="4428c-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4428c-166">DateTime the object was created.</span></span> <span data-ttu-id="4428c-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4428c-168">description</span><span class="sxs-lookup"><span data-stu-id="4428c-168">description</span></span>|<span data-ttu-id="4428c-169">Строка</span><span class="sxs-lookup"><span data-stu-id="4428c-169">String</span></span>|<span data-ttu-id="4428c-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4428c-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4428c-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4428c-172">displayName</span><span class="sxs-lookup"><span data-stu-id="4428c-172">displayName</span></span>|<span data-ttu-id="4428c-173">Строка</span><span class="sxs-lookup"><span data-stu-id="4428c-173">String</span></span>|<span data-ttu-id="4428c-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4428c-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4428c-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4428c-176">version</span><span class="sxs-lookup"><span data-stu-id="4428c-176">version</span></span>|<span data-ttu-id="4428c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="4428c-177">Int32</span></span>|<span data-ttu-id="4428c-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4428c-178">Version of the device configuration.</span></span> <span data-ttu-id="4428c-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4428c-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4428c-180">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="4428c-180">accountManagerPolicy</span></span>|[<span data-ttu-id="4428c-181">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="4428c-181">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="4428c-182">Определяет способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="4428c-182">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="4428c-183">Применяется, только если для параметра disableAccountManager установлено значение false.</span><span class="sxs-lookup"><span data-stu-id="4428c-183">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="4428c-184">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="4428c-184">allowedAccounts</span></span>|[<span data-ttu-id="4428c-185">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="4428c-185">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="4428c-186">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="4428c-186">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="4428c-187">Возможные значения: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="4428c-187">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="4428c-188">localStorage</span><span class="sxs-lookup"><span data-stu-id="4428c-188">localStorage</span></span>|[<span data-ttu-id="4428c-189">включить</span><span class="sxs-lookup"><span data-stu-id="4428c-189">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4428c-190">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="4428c-190">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="4428c-191">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4428c-191">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4428c-192">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="4428c-192">allowLocalStorage</span></span>|<span data-ttu-id="4428c-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="4428c-193">Boolean</span></span>|<span data-ttu-id="4428c-194">Определяет, разрешено ли на общем компьютере локальное хранилище.</span><span class="sxs-lookup"><span data-stu-id="4428c-194">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="4428c-195">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="4428c-195">setAccountManager</span></span>|[<span data-ttu-id="4428c-196">включить</span><span class="sxs-lookup"><span data-stu-id="4428c-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4428c-197">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="4428c-197">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="4428c-198">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4428c-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4428c-199">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="4428c-199">disableAccountManager</span></span>|<span data-ttu-id="4428c-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="4428c-200">Boolean</span></span>|<span data-ttu-id="4428c-201">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="4428c-201">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="4428c-202">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="4428c-202">setEduPolicies</span></span>|[<span data-ttu-id="4428c-203">включить</span><span class="sxs-lookup"><span data-stu-id="4428c-203">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4428c-204">Указывает, следует ли включить/отключить или не настроить общие политики среды образования для ПК по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4428c-204">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="4428c-205">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="4428c-205">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="4428c-206">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4428c-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4428c-207">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="4428c-207">disableEduPolicies</span></span>|<span data-ttu-id="4428c-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="4428c-208">Boolean</span></span>|<span data-ttu-id="4428c-209">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="4428c-209">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="4428c-210">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="4428c-210">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="4428c-211">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="4428c-211">setPowerPolicies</span></span>|[<span data-ttu-id="4428c-212">включить</span><span class="sxs-lookup"><span data-stu-id="4428c-212">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4428c-213">Указывает, следует ли включить или отключить общие политики питания ПК по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4428c-213">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="4428c-214">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4428c-214">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4428c-215">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="4428c-215">disablePowerPolicies</span></span>|<span data-ttu-id="4428c-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="4428c-216">Boolean</span></span>|<span data-ttu-id="4428c-217">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="4428c-217">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="4428c-218">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="4428c-218">signInOnResume</span></span>|[<span data-ttu-id="4428c-219">включить</span><span class="sxs-lookup"><span data-stu-id="4428c-219">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4428c-220">Указывает требование для входов в любое время, когда устройство просыпается из режима сна.</span><span class="sxs-lookup"><span data-stu-id="4428c-220">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="4428c-221">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4428c-221">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="4428c-222">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="4428c-222">disableSignInOnResume</span></span>|<span data-ttu-id="4428c-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="4428c-223">Boolean</span></span>|<span data-ttu-id="4428c-224">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="4428c-224">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="4428c-225">enabled</span><span class="sxs-lookup"><span data-stu-id="4428c-225">enabled</span></span>|<span data-ttu-id="4428c-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="4428c-226">Boolean</span></span>|<span data-ttu-id="4428c-227">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="4428c-227">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="4428c-228">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="4428c-228">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="4428c-229">Int32</span><span class="sxs-lookup"><span data-stu-id="4428c-229">Int32</span></span>|<span data-ttu-id="4428c-230">Определяет длительность (в секундах) пребывания устройства в режиме бездействия перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="4428c-230">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="4428c-231">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="4428c-231">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="4428c-232">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="4428c-232">kioskAppDisplayName</span></span>|<span data-ttu-id="4428c-233">String</span><span class="sxs-lookup"><span data-stu-id="4428c-233">String</span></span>|<span data-ttu-id="4428c-234">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, определяемого с помощью свойства SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="4428c-234">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="4428c-235">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="4428c-235">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="4428c-236">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="4428c-236">kioskAppUserModelId</span></span>|<span data-ttu-id="4428c-237">String</span><span class="sxs-lookup"><span data-stu-id="4428c-237">String</span></span>|<span data-ttu-id="4428c-238">Определяет идентификатор пользовательской модели для приложения, используемого с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="4428c-238">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="4428c-239">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="4428c-239">maintenanceStartTime</span></span>|<span data-ttu-id="4428c-240">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="4428c-240">TimeOfDay</span></span>|<span data-ttu-id="4428c-241">Указывает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="4428c-241">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="4428c-242">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="4428c-242">fastFirstSignIn</span></span>|[<span data-ttu-id="4428c-243">включить</span><span class="sxs-lookup"><span data-stu-id="4428c-243">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="4428c-244">Указывает, следует ли автоматически подключать новые учетные записи Azure AD без администрирования к заранее настроенным локальным учетным записям кандидата.</span><span class="sxs-lookup"><span data-stu-id="4428c-244">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="4428c-245">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="4428c-245">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="4428c-246">Отклик</span><span class="sxs-lookup"><span data-stu-id="4428c-246">Response</span></span>
<span data-ttu-id="4428c-247">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4428c-247">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4428c-248">Пример</span><span class="sxs-lookup"><span data-stu-id="4428c-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="4428c-249">Запрос</span><span class="sxs-lookup"><span data-stu-id="4428c-249">Request</span></span>
<span data-ttu-id="4428c-250">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4428c-250">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4428c-251">Отклик</span><span class="sxs-lookup"><span data-stu-id="4428c-251">Response</span></span>
<span data-ttu-id="4428c-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4428c-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




