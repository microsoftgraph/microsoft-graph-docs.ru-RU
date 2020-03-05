---
title: Обновление Виндовсидентитипротектионконфигуратион
description: Обновление свойств объекта Виндовсидентитипротектионконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 18b9ceb8b410baf9ea006bf76c8a86188ff96498
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42475805"
---
# <a name="update-windowsidentityprotectionconfiguration"></a><span data-ttu-id="f165f-103">Обновление Виндовсидентитипротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="f165f-103">Update windowsIdentityProtectionConfiguration</span></span>

<span data-ttu-id="f165f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f165f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f165f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f165f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f165f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f165f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f165f-107">Обновление свойств объекта [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f165f-107">Update the properties of a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f165f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f165f-108">Prerequisites</span></span>
<span data-ttu-id="f165f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f165f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f165f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f165f-111">Permission type</span></span>|<span data-ttu-id="f165f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f165f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f165f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f165f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f165f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f165f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f165f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f165f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f165f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f165f-116">Not supported.</span></span>|
|<span data-ttu-id="f165f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f165f-117">Application</span></span>|<span data-ttu-id="f165f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f165f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f165f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f165f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f165f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f165f-120">Request headers</span></span>
|<span data-ttu-id="f165f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f165f-121">Header</span></span>|<span data-ttu-id="f165f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f165f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f165f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f165f-123">Authorization</span></span>|<span data-ttu-id="f165f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f165f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f165f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f165f-125">Accept</span></span>|<span data-ttu-id="f165f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f165f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f165f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f165f-127">Request body</span></span>
<span data-ttu-id="f165f-128">В тексте запроса добавьте представление объекта [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f165f-128">In the request body, supply a JSON representation for the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="f165f-129">В следующей таблице приведены свойства, необходимые при создании [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f165f-129">The following table shows the properties that are required when you create the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span></span>

|<span data-ttu-id="f165f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f165f-130">Property</span></span>|<span data-ttu-id="f165f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f165f-131">Type</span></span>|<span data-ttu-id="f165f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f165f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f165f-133">id</span><span class="sxs-lookup"><span data-stu-id="f165f-133">id</span></span>|<span data-ttu-id="f165f-134">String</span><span class="sxs-lookup"><span data-stu-id="f165f-134">String</span></span>|<span data-ttu-id="f165f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f165f-135">Key of the entity.</span></span> <span data-ttu-id="f165f-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f165f-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f165f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f165f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f165f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f165f-138">DateTimeOffset</span></span>|<span data-ttu-id="f165f-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f165f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f165f-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f165f-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f165f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f165f-141">roleScopeTagIds</span></span>|<span data-ttu-id="f165f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f165f-142">String collection</span></span>|<span data-ttu-id="f165f-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f165f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f165f-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f165f-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f165f-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="f165f-145">supportsScopeTags</span></span>|<span data-ttu-id="f165f-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f165f-146">Boolean</span></span>|<span data-ttu-id="f165f-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f165f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f165f-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="f165f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f165f-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f165f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f165f-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f165f-150">This property is read-only.</span></span> <span data-ttu-id="f165f-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f165f-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f165f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f165f-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f165f-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f165f-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f165f-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f165f-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f165f-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f165f-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f165f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f165f-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f165f-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f165f-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f165f-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f165f-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f165f-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f165f-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f165f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f165f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f165f-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f165f-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f165f-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f165f-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f165f-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f165f-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f165f-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f165f-164">createdDateTime</span></span>|<span data-ttu-id="f165f-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f165f-165">DateTimeOffset</span></span>|<span data-ttu-id="f165f-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f165f-166">DateTime the object was created.</span></span> <span data-ttu-id="f165f-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f165f-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f165f-168">description</span><span class="sxs-lookup"><span data-stu-id="f165f-168">description</span></span>|<span data-ttu-id="f165f-169">String</span><span class="sxs-lookup"><span data-stu-id="f165f-169">String</span></span>|<span data-ttu-id="f165f-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f165f-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f165f-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f165f-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f165f-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f165f-172">displayName</span></span>|<span data-ttu-id="f165f-173">Строка</span><span class="sxs-lookup"><span data-stu-id="f165f-173">String</span></span>|<span data-ttu-id="f165f-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f165f-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f165f-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f165f-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f165f-176">version</span><span class="sxs-lookup"><span data-stu-id="f165f-176">version</span></span>|<span data-ttu-id="f165f-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f165f-177">Int32</span></span>|<span data-ttu-id="f165f-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f165f-178">Version of the device configuration.</span></span> <span data-ttu-id="f165f-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f165f-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f165f-180">усесекуритикэйфорсигнин</span><span class="sxs-lookup"><span data-stu-id="f165f-180">useSecurityKeyForSignin</span></span>|<span data-ttu-id="f165f-181">Логический</span><span class="sxs-lookup"><span data-stu-id="f165f-181">Boolean</span></span>|<span data-ttu-id="f165f-182">Логическое значение, используемое для включения ключа безопасности Windows Hello в качестве учетных данных для входа.</span><span class="sxs-lookup"><span data-stu-id="f165f-182">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="f165f-183">енханцедантиспуфингфорфаЦиалфеатуресенаблед</span><span class="sxs-lookup"><span data-stu-id="f165f-183">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="f165f-184">Логический</span><span class="sxs-lookup"><span data-stu-id="f165f-184">Boolean</span></span>|<span data-ttu-id="f165f-185">Логическое значение, используемое для включения расширенного средства защиты от спуфинга для распознавания функции лица при проверке подлинности Windows Hello для лиц.</span><span class="sxs-lookup"><span data-stu-id="f165f-185">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="f165f-186">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f165f-186">pinMinimumLength</span></span>|<span data-ttu-id="f165f-187">Int32</span><span class="sxs-lookup"><span data-stu-id="f165f-187">Int32</span></span>|<span data-ttu-id="f165f-188">Целочисленное значение, задающее минимальное число символов, необходимое для ПИН-кода Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f165f-188">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="f165f-189">Допустимые значения: от 4 до 127 включительно и меньше или равны набору значений для максимального ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="f165f-189">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="f165f-190">Допустимые значения — от 4 до 127</span><span class="sxs-lookup"><span data-stu-id="f165f-190">Valid values 4 to 127</span></span>|
|<span data-ttu-id="f165f-191">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="f165f-191">pinMaximumLength</span></span>|<span data-ttu-id="f165f-192">Int32</span><span class="sxs-lookup"><span data-stu-id="f165f-192">Int32</span></span>|<span data-ttu-id="f165f-193">Целое значение, задающее максимальное количество символов для рабочего ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="f165f-193">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="f165f-194">Допустимые значения: от 4 до 127 включительно и больше или равны значению, заданному для минимального ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="f165f-194">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="f165f-195">Допустимые значения — от 4 до 127</span><span class="sxs-lookup"><span data-stu-id="f165f-195">Valid values 4 to 127</span></span>|
|<span data-ttu-id="f165f-196">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="f165f-196">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="f165f-197">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="f165f-197">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="f165f-198">Это значение позволяет настроить использование символов верхнего регистра в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f165f-198">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="f165f-199">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="f165f-199">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="f165f-200">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="f165f-200">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="f165f-201">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="f165f-201">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="f165f-202">Это значение позволяет настроить использование символов нижнего регистра в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f165f-202">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="f165f-203">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="f165f-203">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="f165f-204">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="f165f-204">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="f165f-205">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="f165f-205">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="f165f-206">Управляет возможностью использования специальных символов в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f165f-206">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="f165f-207">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="f165f-207">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="f165f-208">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="f165f-208">pinExpirationInDays</span></span>|<span data-ttu-id="f165f-209">Int32</span><span class="sxs-lookup"><span data-stu-id="f165f-209">Int32</span></span>|<span data-ttu-id="f165f-210">Integer value указывает период времени (в днях), в течение которого можно использовать ПИН-код, прежде чем система потребует от пользователя изменить его.</span><span class="sxs-lookup"><span data-stu-id="f165f-210">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="f165f-211">Допустимые значения: от 0 до 730 включительно.</span><span class="sxs-lookup"><span data-stu-id="f165f-211">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="f165f-212">Допустимые значения: от 0 до 730.</span><span class="sxs-lookup"><span data-stu-id="f165f-212">Valid values 0 to 730</span></span>|
|<span data-ttu-id="f165f-213">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="f165f-213">pinPreviousBlockCount</span></span>|<span data-ttu-id="f165f-214">Int32</span><span class="sxs-lookup"><span data-stu-id="f165f-214">Int32</span></span>|<span data-ttu-id="f165f-215">Управляет возможностью запретить пользователям использовать прошлые контакты.</span><span class="sxs-lookup"><span data-stu-id="f165f-215">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="f165f-216">Он должен иметь значение от 0 до 50 включительно, а текущий ПИН-код пользователя включен в этот счетчик.</span><span class="sxs-lookup"><span data-stu-id="f165f-216">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="f165f-217">Если задано значение 0, предыдущие ПИН-коды не сохраняются.</span><span class="sxs-lookup"><span data-stu-id="f165f-217">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="f165f-218">История ПИН-кодов не сохраняется при сбросе ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="f165f-218">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="f165f-219">Допустимые значения: от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="f165f-219">Valid values 0 to 50</span></span>|
|<span data-ttu-id="f165f-220">пинрековеренаблед</span><span class="sxs-lookup"><span data-stu-id="f165f-220">pinRecoveryEnabled</span></span>|<span data-ttu-id="f165f-221">Логический</span><span class="sxs-lookup"><span data-stu-id="f165f-221">Boolean</span></span>|<span data-ttu-id="f165f-222">Логическое значение, которое позволяет пользователю изменить свой ПИН-код с помощью службы восстановления ПИН-кода Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f165f-222">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="f165f-223">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="f165f-223">securityDeviceRequired</span></span>|<span data-ttu-id="f165f-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="f165f-224">Boolean</span></span>|<span data-ttu-id="f165f-225">Определяет, требуется ли доверенный ПЛАТФОРМЕНный модуль для подготовки Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f165f-225">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="f165f-226">TPM предоставляет дополнительные преимущества безопасности, которые хранятся на нем, не могут использоваться на других устройствах.</span><span class="sxs-lookup"><span data-stu-id="f165f-226">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="f165f-227">Если задано значение false, все устройства могут подготавливать Windows Hello для бизнеса, даже если нет пригодного к использованию доверенного платформенного модуля.</span><span class="sxs-lookup"><span data-stu-id="f165f-227">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="f165f-228">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="f165f-228">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="f165f-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="f165f-229">Boolean</span></span>|<span data-ttu-id="f165f-230">Управляет использованием биометрических жестов, таких как лицо и отпечаток, в качестве альтернативы ПИН-коду Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f165f-230">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="f165f-231">Если задано значение false, биометрические жесты не разрешены.</span><span class="sxs-lookup"><span data-stu-id="f165f-231">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="f165f-232">Пользователи по-прежнему должны настроить ПИН-код в качестве резервной копии в случае сбоев.</span><span class="sxs-lookup"><span data-stu-id="f165f-232">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="f165f-233">усецертификатесфоронпремисесаусенаблед</span><span class="sxs-lookup"><span data-stu-id="f165f-233">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="f165f-234">Логический</span><span class="sxs-lookup"><span data-stu-id="f165f-234">Boolean</span></span>|<span data-ttu-id="f165f-235">Логическое значение, которое позволяет Windows Hello для бизнеса использовать сертификаты для проверки подлинности локальных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f165f-235">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="f165f-236">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="f165f-236">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="f165f-237">Логический</span><span class="sxs-lookup"><span data-stu-id="f165f-237">Boolean</span></span>|<span data-ttu-id="f165f-238">Логическое значение, блокирующее Windows Hello для бизнеса в качестве способа входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="f165f-238">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="f165f-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="f165f-239">Response</span></span>
<span data-ttu-id="f165f-240">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f165f-240">If successful, this method returns a `200 OK` response code and an updated [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f165f-241">Пример</span><span class="sxs-lookup"><span data-stu-id="f165f-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="f165f-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="f165f-242">Request</span></span>
<span data-ttu-id="f165f-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f165f-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1583

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
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
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="f165f-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="f165f-244">Response</span></span>
<span data-ttu-id="f165f-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f165f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1755

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
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
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```





