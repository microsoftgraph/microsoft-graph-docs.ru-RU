---
title: Обновление объекта sharedPCConfiguration
description: Обновляет свойства объекта sharedPCConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: da0cbba1de768fffd572728d3d416de83917e582
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396331"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="2b547-103">Обновление объекта sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b547-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="2b547-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2b547-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b547-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b547-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b547-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b547-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b547-107">Обновляет свойства объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b547-107">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b547-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2b547-108">Prerequisites</span></span>
<span data-ttu-id="2b547-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2b547-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2b547-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b547-111">Permission type</span></span>|<span data-ttu-id="2b547-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b547-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b547-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b547-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b547-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b547-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b547-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b547-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b547-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b547-116">Not supported.</span></span>|
|<span data-ttu-id="2b547-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b547-117">Application</span></span>|<span data-ttu-id="2b547-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b547-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b547-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b547-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2b547-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b547-120">Request headers</span></span>
|<span data-ttu-id="2b547-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b547-121">Header</span></span>|<span data-ttu-id="2b547-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b547-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b547-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b547-123">Authorization</span></span>|<span data-ttu-id="2b547-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2b547-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b547-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b547-125">Accept</span></span>|<span data-ttu-id="2b547-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b547-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b547-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b547-127">Request body</span></span>
<span data-ttu-id="2b547-128">В теле запроса добавьте представление объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2b547-128">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="2b547-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b547-129">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="2b547-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b547-130">Property</span></span>|<span data-ttu-id="2b547-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2b547-131">Type</span></span>|<span data-ttu-id="2b547-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2b547-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b547-133">id</span><span class="sxs-lookup"><span data-stu-id="2b547-133">id</span></span>|<span data-ttu-id="2b547-134">String</span><span class="sxs-lookup"><span data-stu-id="2b547-134">String</span></span>|<span data-ttu-id="2b547-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2b547-135">Key of the entity.</span></span> <span data-ttu-id="2b547-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b547-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b547-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b547-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2b547-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b547-138">DateTimeOffset</span></span>|<span data-ttu-id="2b547-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2b547-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2b547-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b547-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b547-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b547-141">roleScopeTagIds</span></span>|<span data-ttu-id="2b547-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2b547-142">String collection</span></span>|<span data-ttu-id="2b547-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2b547-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2b547-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b547-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b547-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2b547-145">supportsScopeTags</span></span>|<span data-ttu-id="2b547-146">Логический</span><span class="sxs-lookup"><span data-stu-id="2b547-146">Boolean</span></span>|<span data-ttu-id="2b547-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="2b547-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2b547-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="2b547-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2b547-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2b547-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2b547-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b547-150">This property is read-only.</span></span> <span data-ttu-id="2b547-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b547-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b547-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b547-152">createdDateTime</span></span>|<span data-ttu-id="2b547-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b547-153">DateTimeOffset</span></span>|<span data-ttu-id="2b547-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2b547-154">DateTime the object was created.</span></span> <span data-ttu-id="2b547-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b547-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b547-156">description</span><span class="sxs-lookup"><span data-stu-id="2b547-156">description</span></span>|<span data-ttu-id="2b547-157">String</span><span class="sxs-lookup"><span data-stu-id="2b547-157">String</span></span>|<span data-ttu-id="2b547-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b547-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2b547-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b547-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b547-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2b547-160">displayName</span></span>|<span data-ttu-id="2b547-161">String</span><span class="sxs-lookup"><span data-stu-id="2b547-161">String</span></span>|<span data-ttu-id="2b547-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b547-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2b547-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b547-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b547-164">version</span><span class="sxs-lookup"><span data-stu-id="2b547-164">version</span></span>|<span data-ttu-id="2b547-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2b547-165">Int32</span></span>|<span data-ttu-id="2b547-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b547-166">Version of the device configuration.</span></span> <span data-ttu-id="2b547-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b547-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b547-168">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="2b547-168">accountManagerPolicy</span></span>|[<span data-ttu-id="2b547-169">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="2b547-169">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="2b547-170">Задает способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="2b547-170">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="2b547-171">Применяется, только если для параметра disableAccountManager задано значение false.</span><span class="sxs-lookup"><span data-stu-id="2b547-171">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="2b547-172">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="2b547-172">allowedAccounts</span></span>|[<span data-ttu-id="2b547-173">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="2b547-173">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="2b547-174">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="2b547-174">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="2b547-175">Возможные значения: `notConfigured`, `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="2b547-175">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="2b547-176">localStorage</span><span class="sxs-lookup"><span data-stu-id="2b547-176">localStorage</span></span>|<span data-ttu-id="2b547-177">[Включение] (.. /Resources/Intune-Shared-enablement</span><span class="sxs-lookup"><span data-stu-id="2b547-177">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="2b547-178">публикацию повторно)</span><span class="sxs-lookup"><span data-stu-id="2b547-178">.md)</span></span>|<span data-ttu-id="2b547-179">Указывает, можно ли разместить локальное хранилище на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="2b547-179">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="2b547-180">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2b547-180">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="2b547-181">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="2b547-181">allowLocalStorage</span></span>|<span data-ttu-id="2b547-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b547-182">Boolean</span></span>|<span data-ttu-id="2b547-183">Указывает, можно ли разместить локальное хранилище на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="2b547-183">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="2b547-184">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="2b547-184">setAccountManager</span></span>|<span data-ttu-id="2b547-185">[Включение] (.. /Resources/Intune-Shared-enablement</span><span class="sxs-lookup"><span data-stu-id="2b547-185">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="2b547-186">публикацию повторно)</span><span class="sxs-lookup"><span data-stu-id="2b547-186">.md)</span></span>|<span data-ttu-id="2b547-187">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="2b547-187">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="2b547-188">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2b547-188">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="2b547-189">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="2b547-189">disableAccountManager</span></span>|<span data-ttu-id="2b547-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b547-190">Boolean</span></span>|<span data-ttu-id="2b547-191">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="2b547-191">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="2b547-192">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="2b547-192">setEduPolicies</span></span>|<span data-ttu-id="2b547-193">[Включение] (.. /Resources/Intune-Shared-enablement</span><span class="sxs-lookup"><span data-stu-id="2b547-193">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="2b547-194">публикацию повторно)</span><span class="sxs-lookup"><span data-stu-id="2b547-194">.md)</span></span>|<span data-ttu-id="2b547-195">Указывает ли политики по умолчанию общих ПК education среды должен быть включен или отключен или не настроен.</span><span class="sxs-lookup"><span data-stu-id="2b547-195">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="2b547-196">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="2b547-196">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="2b547-197">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2b547-197">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="2b547-198">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="2b547-198">disableEduPolicies</span></span>|<span data-ttu-id="2b547-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b547-199">Boolean</span></span>|<span data-ttu-id="2b547-200">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="2b547-200">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="2b547-201">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="2b547-201">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="2b547-202">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="2b547-202">setPowerPolicies</span></span>|<span data-ttu-id="2b547-203">[Включение] (.. /Resources/Intune-Shared-enablement</span><span class="sxs-lookup"><span data-stu-id="2b547-203">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="2b547-204">публикацию повторно)</span><span class="sxs-lookup"><span data-stu-id="2b547-204">.md)</span></span>|<span data-ttu-id="2b547-205">Указывает, будет ли политики по умолчанию общих PC power должен быть отключен.</span><span class="sxs-lookup"><span data-stu-id="2b547-205">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="2b547-206">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2b547-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="2b547-207">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="2b547-207">disablePowerPolicies</span></span>|<span data-ttu-id="2b547-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b547-208">Boolean</span></span>|<span data-ttu-id="2b547-209">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="2b547-209">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="2b547-210">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="2b547-210">signInOnResume</span></span>|<span data-ttu-id="2b547-211">[Включение] (.. /Resources/Intune-Shared-enablement</span><span class="sxs-lookup"><span data-stu-id="2b547-211">[enablement](../resources/intune-shared-enablement</span></span>
<span data-ttu-id="2b547-212">публикацию повторно)</span><span class="sxs-lookup"><span data-stu-id="2b547-212">.md)</span></span>|<span data-ttu-id="2b547-213">Определяет требования для входа в каждый раз, когда устройство выходит из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="2b547-213">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="2b547-214">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="2b547-214">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="2b547-215">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="2b547-215">disableSignInOnResume</span></span>|<span data-ttu-id="2b547-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b547-216">Boolean</span></span>|<span data-ttu-id="2b547-217">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="2b547-217">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="2b547-218">enabled</span><span class="sxs-lookup"><span data-stu-id="2b547-218">enabled</span></span>|<span data-ttu-id="2b547-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b547-219">Boolean</span></span>|<span data-ttu-id="2b547-220">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="2b547-220">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="2b547-221">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="2b547-221">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="2b547-222">Int32</span><span class="sxs-lookup"><span data-stu-id="2b547-222">Int32</span></span>|<span data-ttu-id="2b547-223">Определяет длительность (в секундах) простоя устройства перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="2b547-223">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="2b547-224">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="2b547-224">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="2b547-225">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="2b547-225">kioskAppDisplayName</span></span>|<span data-ttu-id="2b547-226">String</span><span class="sxs-lookup"><span data-stu-id="2b547-226">String</span></span>|<span data-ttu-id="2b547-227">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, указанного в свойстве SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="2b547-227">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="2b547-228">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="2b547-228">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="2b547-229">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="2b547-229">kioskAppUserModelId</span></span>|<span data-ttu-id="2b547-230">String</span><span class="sxs-lookup"><span data-stu-id="2b547-230">String</span></span>|<span data-ttu-id="2b547-231">Задает ИД пользовательской модели для приложения, используемый с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="2b547-231">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="2b547-232">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="2b547-232">maintenanceStartTime</span></span>|<span data-ttu-id="2b547-233">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2b547-233">TimeOfDay</span></span>|<span data-ttu-id="2b547-234">Задает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="2b547-234">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="2b547-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b547-235">Response</span></span>
<span data-ttu-id="2b547-236">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2b547-236">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b547-237">Пример</span><span class="sxs-lookup"><span data-stu-id="2b547-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b547-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b547-238">Request</span></span>
<span data-ttu-id="2b547-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b547-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1114

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="2b547-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b547-240">Response</span></span>
<span data-ttu-id="2b547-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2b547-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1286

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "maintenanceStartTime": "11:59:24.7240000"
}
```




