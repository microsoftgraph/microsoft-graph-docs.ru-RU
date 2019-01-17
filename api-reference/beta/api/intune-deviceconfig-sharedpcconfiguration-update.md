---
title: Обновление объекта sharedPCConfiguration
description: Обновляет свойства объекта sharedPCConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 98d44ed39fbb975d2a3e71789ccf20a514c4d3db
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949082"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="418ad-103">Обновление объекта sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="418ad-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="418ad-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="418ad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="418ad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="418ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="418ad-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="418ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="418ad-107">Обновляет свойства объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="418ad-107">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="418ad-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="418ad-108">Prerequisites</span></span>
<span data-ttu-id="418ad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="418ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="418ad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="418ad-111">Permission type</span></span>|<span data-ttu-id="418ad-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="418ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="418ad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="418ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="418ad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="418ad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="418ad-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="418ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="418ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="418ad-116">Not supported.</span></span>|
|<span data-ttu-id="418ad-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="418ad-117">Application</span></span>|<span data-ttu-id="418ad-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="418ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="418ad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="418ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="418ad-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="418ad-120">Request headers</span></span>
|<span data-ttu-id="418ad-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="418ad-121">Header</span></span>|<span data-ttu-id="418ad-122">Значение</span><span class="sxs-lookup"><span data-stu-id="418ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="418ad-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="418ad-123">Authorization</span></span>|<span data-ttu-id="418ad-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="418ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="418ad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="418ad-125">Accept</span></span>|<span data-ttu-id="418ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="418ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="418ad-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="418ad-127">Request body</span></span>
<span data-ttu-id="418ad-128">В теле запроса добавьте представление объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="418ad-128">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="418ad-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="418ad-129">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="418ad-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="418ad-130">Property</span></span>|<span data-ttu-id="418ad-131">Тип</span><span class="sxs-lookup"><span data-stu-id="418ad-131">Type</span></span>|<span data-ttu-id="418ad-132">Описание</span><span class="sxs-lookup"><span data-stu-id="418ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="418ad-133">id</span><span class="sxs-lookup"><span data-stu-id="418ad-133">id</span></span>|<span data-ttu-id="418ad-134">Строка</span><span class="sxs-lookup"><span data-stu-id="418ad-134">String</span></span>|<span data-ttu-id="418ad-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="418ad-135">Key of the entity.</span></span> <span data-ttu-id="418ad-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="418ad-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418ad-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="418ad-137">lastModifiedDateTime</span></span>|<span data-ttu-id="418ad-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="418ad-138">DateTimeOffset</span></span>|<span data-ttu-id="418ad-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="418ad-139">DateTime the object was last modified.</span></span> <span data-ttu-id="418ad-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="418ad-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418ad-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="418ad-141">roleScopeTagIds</span></span>|<span data-ttu-id="418ad-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="418ad-142">String collection</span></span>|<span data-ttu-id="418ad-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="418ad-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="418ad-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="418ad-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418ad-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="418ad-145">supportsScopeTags</span></span>|<span data-ttu-id="418ad-146">Логический</span><span class="sxs-lookup"><span data-stu-id="418ad-146">Boolean</span></span>|<span data-ttu-id="418ad-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="418ad-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="418ad-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="418ad-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="418ad-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="418ad-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="418ad-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="418ad-150">This property is read-only.</span></span> <span data-ttu-id="418ad-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="418ad-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418ad-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="418ad-152">createdDateTime</span></span>|<span data-ttu-id="418ad-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="418ad-153">DateTimeOffset</span></span>|<span data-ttu-id="418ad-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="418ad-154">DateTime the object was created.</span></span> <span data-ttu-id="418ad-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="418ad-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418ad-156">описание</span><span class="sxs-lookup"><span data-stu-id="418ad-156">description</span></span>|<span data-ttu-id="418ad-157">Строка</span><span class="sxs-lookup"><span data-stu-id="418ad-157">String</span></span>|<span data-ttu-id="418ad-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="418ad-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="418ad-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="418ad-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418ad-160">displayName</span><span class="sxs-lookup"><span data-stu-id="418ad-160">displayName</span></span>|<span data-ttu-id="418ad-161">Строка</span><span class="sxs-lookup"><span data-stu-id="418ad-161">String</span></span>|<span data-ttu-id="418ad-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="418ad-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="418ad-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="418ad-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418ad-164">version</span><span class="sxs-lookup"><span data-stu-id="418ad-164">version</span></span>|<span data-ttu-id="418ad-165">Int32</span><span class="sxs-lookup"><span data-stu-id="418ad-165">Int32</span></span>|<span data-ttu-id="418ad-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="418ad-166">Version of the device configuration.</span></span> <span data-ttu-id="418ad-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="418ad-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="418ad-168">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="418ad-168">accountManagerPolicy</span></span>|[<span data-ttu-id="418ad-169">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="418ad-169">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="418ad-170">Задает способ управления учетными записями на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="418ad-170">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="418ad-171">Применяется, только если для параметра disableAccountManager задано значение false.</span><span class="sxs-lookup"><span data-stu-id="418ad-171">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="418ad-172">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="418ad-172">allowedAccounts</span></span>|[<span data-ttu-id="418ad-173">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="418ad-173">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="418ad-174">Указывает тип учетных записей, которые можно использовать на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="418ad-174">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="418ad-175">Возможные значения: `guest`, `domain`.</span><span class="sxs-lookup"><span data-stu-id="418ad-175">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="418ad-176">localStorage</span><span class="sxs-lookup"><span data-stu-id="418ad-176">localStorage</span></span>|[<span data-ttu-id="418ad-177">Включение</span><span class="sxs-lookup"><span data-stu-id="418ad-177">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="418ad-178">Указывает, можно ли разместить локальное хранилище на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="418ad-178">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="418ad-179">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="418ad-179">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="418ad-180">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="418ad-180">allowLocalStorage</span></span>|<span data-ttu-id="418ad-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="418ad-181">Boolean</span></span>|<span data-ttu-id="418ad-182">Указывает, можно ли разместить локальное хранилище на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="418ad-182">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="418ad-183">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="418ad-183">setAccountManager</span></span>|[<span data-ttu-id="418ad-184">Включение</span><span class="sxs-lookup"><span data-stu-id="418ad-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="418ad-185">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="418ad-185">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="418ad-186">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="418ad-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="418ad-187">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="418ad-187">disableAccountManager</span></span>|<span data-ttu-id="418ad-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="418ad-188">Boolean</span></span>|<span data-ttu-id="418ad-189">Отключает диспетчер учетных записей в режиме совместного использования компьютера.</span><span class="sxs-lookup"><span data-stu-id="418ad-189">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="418ad-190">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="418ad-190">setEduPolicies</span></span>|[<span data-ttu-id="418ad-191">Включение</span><span class="sxs-lookup"><span data-stu-id="418ad-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="418ad-192">Указывает ли политики по умолчанию общих ПК education среды должен быть включен или отключен или не настроен.</span><span class="sxs-lookup"><span data-stu-id="418ad-192">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="418ad-193">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="418ad-193">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="418ad-194">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="418ad-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="418ad-195">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="418ad-195">disableEduPolicies</span></span>|<span data-ttu-id="418ad-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="418ad-196">Boolean</span></span>|<span data-ttu-id="418ad-197">Указывает, следует ли отключить стандартные политики среды совместного использования компьютера для образования.</span><span class="sxs-lookup"><span data-stu-id="418ad-197">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="418ad-198">Для Windows 10 RS2 и более поздних версий эта политика будет применяться без установки значения True для параметра Enabled.</span><span class="sxs-lookup"><span data-stu-id="418ad-198">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="418ad-199">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="418ad-199">setPowerPolicies</span></span>|[<span data-ttu-id="418ad-200">Включение</span><span class="sxs-lookup"><span data-stu-id="418ad-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="418ad-201">Указывает, будет ли политики по умолчанию общих PC power должен быть отключен.</span><span class="sxs-lookup"><span data-stu-id="418ad-201">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="418ad-202">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="418ad-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="418ad-203">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="418ad-203">disablePowerPolicies</span></span>|<span data-ttu-id="418ad-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="418ad-204">Boolean</span></span>|<span data-ttu-id="418ad-205">Указывает, следует ли отключить стандартные политики электропитания для общего компьютера.</span><span class="sxs-lookup"><span data-stu-id="418ad-205">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="418ad-206">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="418ad-206">signInOnResume</span></span>|[<span data-ttu-id="418ad-207">Включение</span><span class="sxs-lookup"><span data-stu-id="418ad-207">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="418ad-208">Определяет требования для входа в каждый раз, когда устройство выходит из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="418ad-208">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="418ad-209">Возможные значения: `notConfigured`, `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="418ad-209">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="418ad-210">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="418ad-210">disableSignInOnResume</span></span>|<span data-ttu-id="418ad-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="418ad-211">Boolean</span></span>|<span data-ttu-id="418ad-212">Отключает обязательный вход в систему при выходе устройства из спящего режима.</span><span class="sxs-lookup"><span data-stu-id="418ad-212">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="418ad-213">enabled</span><span class="sxs-lookup"><span data-stu-id="418ad-213">enabled</span></span>|<span data-ttu-id="418ad-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="418ad-214">Boolean</span></span>|<span data-ttu-id="418ad-215">Включает режим общего компьютера и применяет политики совместного использования ПК.</span><span class="sxs-lookup"><span data-stu-id="418ad-215">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="418ad-216">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="418ad-216">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="418ad-217">Int32</span><span class="sxs-lookup"><span data-stu-id="418ad-217">Int32</span></span>|<span data-ttu-id="418ad-218">Определяет длительность (в секундах) простоя устройства перед переходом в спящий режим.</span><span class="sxs-lookup"><span data-stu-id="418ad-218">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="418ad-219">Если задать значение 0, переход в спящий режим отключается.</span><span class="sxs-lookup"><span data-stu-id="418ad-219">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="418ad-220">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="418ad-220">kioskAppDisplayName</span></span>|<span data-ttu-id="418ad-221">String</span><span class="sxs-lookup"><span data-stu-id="418ad-221">String</span></span>|<span data-ttu-id="418ad-222">Задает текст для учетной записи, который отображается на экране входа в систему и используется для запуска приложения, указанного в свойстве SetKioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="418ad-222">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="418ad-223">Применяется, только если задано свойство KioskAppUserModelId.</span><span class="sxs-lookup"><span data-stu-id="418ad-223">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="418ad-224">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="418ad-224">kioskAppUserModelId</span></span>|<span data-ttu-id="418ad-225">String</span><span class="sxs-lookup"><span data-stu-id="418ad-225">String</span></span>|<span data-ttu-id="418ad-226">Задает ИД пользовательской модели для приложения, используемый с ограниченным доступом.</span><span class="sxs-lookup"><span data-stu-id="418ad-226">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="418ad-227">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="418ad-227">maintenanceStartTime</span></span>|<span data-ttu-id="418ad-228">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="418ad-228">TimeOfDay</span></span>|<span data-ttu-id="418ad-229">Задает ежедневное время начала обслуживания.</span><span class="sxs-lookup"><span data-stu-id="418ad-229">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="418ad-230">Отклик</span><span class="sxs-lookup"><span data-stu-id="418ad-230">Response</span></span>
<span data-ttu-id="418ad-231">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="418ad-231">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="418ad-232">Пример</span><span class="sxs-lookup"><span data-stu-id="418ad-232">Example</span></span>
### <a name="request"></a><span data-ttu-id="418ad-233">Запрос</span><span class="sxs-lookup"><span data-stu-id="418ad-233">Request</span></span>
<span data-ttu-id="418ad-234">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="418ad-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1119

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "allowedAccounts": "domain",
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

### <a name="response"></a><span data-ttu-id="418ad-235">Ответ</span><span class="sxs-lookup"><span data-stu-id="418ad-235">Response</span></span>
<span data-ttu-id="418ad-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="418ad-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1287

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
  "allowedAccounts": "domain",
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





