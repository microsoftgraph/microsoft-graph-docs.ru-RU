---
title: Обновление Виндовсидентитипротектионконфигуратион
description: Обновление свойств объекта Виндовсидентитипротектионконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4660f6aafe03fdc11c0dbf04b0eb90d657f7f5b4
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37532843"
---
# <a name="update-windowsidentityprotectionconfiguration"></a><span data-ttu-id="4104f-103">Обновление Виндовсидентитипротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="4104f-103">Update windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="4104f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4104f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4104f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4104f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4104f-106">Обновление свойств объекта [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4104f-106">Update the properties of a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4104f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4104f-107">Prerequisites</span></span>
<span data-ttu-id="4104f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4104f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4104f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4104f-110">Permission type</span></span>|<span data-ttu-id="4104f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4104f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4104f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4104f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4104f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4104f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4104f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4104f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4104f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4104f-115">Not supported.</span></span>|
|<span data-ttu-id="4104f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4104f-116">Application</span></span>|<span data-ttu-id="4104f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4104f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4104f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4104f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4104f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4104f-119">Request headers</span></span>
|<span data-ttu-id="4104f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4104f-120">Header</span></span>|<span data-ttu-id="4104f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4104f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4104f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4104f-122">Authorization</span></span>|<span data-ttu-id="4104f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4104f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4104f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4104f-124">Accept</span></span>|<span data-ttu-id="4104f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4104f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4104f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4104f-126">Request body</span></span>
<span data-ttu-id="4104f-127">В тексте запроса добавьте представление объекта [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4104f-127">In the request body, supply a JSON representation for the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="4104f-128">В следующей таблице приведены свойства, необходимые при создании [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4104f-128">The following table shows the properties that are required when you create the [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md).</span></span>

|<span data-ttu-id="4104f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4104f-129">Property</span></span>|<span data-ttu-id="4104f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4104f-130">Type</span></span>|<span data-ttu-id="4104f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4104f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4104f-132">id</span><span class="sxs-lookup"><span data-stu-id="4104f-132">id</span></span>|<span data-ttu-id="4104f-133">String</span><span class="sxs-lookup"><span data-stu-id="4104f-133">String</span></span>|<span data-ttu-id="4104f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4104f-134">Key of the entity.</span></span> <span data-ttu-id="4104f-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4104f-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4104f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4104f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4104f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4104f-137">DateTimeOffset</span></span>|<span data-ttu-id="4104f-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4104f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4104f-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4104f-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4104f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4104f-140">roleScopeTagIds</span></span>|<span data-ttu-id="4104f-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4104f-141">String collection</span></span>|<span data-ttu-id="4104f-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="4104f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4104f-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4104f-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4104f-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="4104f-144">supportsScopeTags</span></span>|<span data-ttu-id="4104f-145">Логический</span><span class="sxs-lookup"><span data-stu-id="4104f-145">Boolean</span></span>|<span data-ttu-id="4104f-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="4104f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4104f-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="4104f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4104f-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="4104f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4104f-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4104f-149">This property is read-only.</span></span> <span data-ttu-id="4104f-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4104f-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4104f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4104f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4104f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4104f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4104f-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4104f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4104f-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4104f-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4104f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4104f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4104f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4104f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4104f-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4104f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4104f-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4104f-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4104f-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4104f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4104f-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4104f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4104f-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4104f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4104f-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4104f-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4104f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4104f-163">createdDateTime</span></span>|<span data-ttu-id="4104f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4104f-164">DateTimeOffset</span></span>|<span data-ttu-id="4104f-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4104f-165">DateTime the object was created.</span></span> <span data-ttu-id="4104f-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4104f-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4104f-167">description</span><span class="sxs-lookup"><span data-stu-id="4104f-167">description</span></span>|<span data-ttu-id="4104f-168">String</span><span class="sxs-lookup"><span data-stu-id="4104f-168">String</span></span>|<span data-ttu-id="4104f-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4104f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4104f-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4104f-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4104f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4104f-171">displayName</span></span>|<span data-ttu-id="4104f-172">Строка</span><span class="sxs-lookup"><span data-stu-id="4104f-172">String</span></span>|<span data-ttu-id="4104f-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4104f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4104f-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4104f-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4104f-175">version</span><span class="sxs-lookup"><span data-stu-id="4104f-175">version</span></span>|<span data-ttu-id="4104f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4104f-176">Int32</span></span>|<span data-ttu-id="4104f-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4104f-177">Version of the device configuration.</span></span> <span data-ttu-id="4104f-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4104f-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4104f-179">усесекуритикэйфорсигнин</span><span class="sxs-lookup"><span data-stu-id="4104f-179">useSecurityKeyForSignin</span></span>|<span data-ttu-id="4104f-180">Логический</span><span class="sxs-lookup"><span data-stu-id="4104f-180">Boolean</span></span>|<span data-ttu-id="4104f-181">Логическое значение, используемое для включения ключа безопасности Windows Hello в качестве учетных данных для входа.</span><span class="sxs-lookup"><span data-stu-id="4104f-181">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="4104f-182">енханцедантиспуфингфорфаЦиалфеатуресенаблед</span><span class="sxs-lookup"><span data-stu-id="4104f-182">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="4104f-183">Логический</span><span class="sxs-lookup"><span data-stu-id="4104f-183">Boolean</span></span>|<span data-ttu-id="4104f-184">Логическое значение, используемое для включения расширенного средства защиты от спуфинга для распознавания функции лица при проверке подлинности Windows Hello для лиц.</span><span class="sxs-lookup"><span data-stu-id="4104f-184">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="4104f-185">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4104f-185">pinMinimumLength</span></span>|<span data-ttu-id="4104f-186">Int32</span><span class="sxs-lookup"><span data-stu-id="4104f-186">Int32</span></span>|<span data-ttu-id="4104f-187">Целочисленное значение, задающее минимальное число символов, необходимое для ПИН-кода Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4104f-187">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="4104f-188">Допустимые значения: от 4 до 127 включительно и меньше или равны набору значений для максимального ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="4104f-188">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="4104f-189">Допустимые значения — от 4 до 127</span><span class="sxs-lookup"><span data-stu-id="4104f-189">Valid values 4 to 127</span></span>|
|<span data-ttu-id="4104f-190">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="4104f-190">pinMaximumLength</span></span>|<span data-ttu-id="4104f-191">Int32</span><span class="sxs-lookup"><span data-stu-id="4104f-191">Int32</span></span>|<span data-ttu-id="4104f-192">Целое значение, задающее максимальное количество символов для рабочего ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="4104f-192">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="4104f-193">Допустимые значения: от 4 до 127 включительно и больше или равны значению, заданному для минимального ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="4104f-193">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="4104f-194">Допустимые значения — от 4 до 127</span><span class="sxs-lookup"><span data-stu-id="4104f-194">Valid values 4 to 127</span></span>|
|<span data-ttu-id="4104f-195">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="4104f-195">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="4104f-196">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="4104f-196">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="4104f-197">Это значение позволяет настроить использование символов верхнего регистра в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4104f-197">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="4104f-198">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="4104f-198">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="4104f-199">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="4104f-199">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="4104f-200">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="4104f-200">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="4104f-201">Это значение позволяет настроить использование символов нижнего регистра в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4104f-201">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="4104f-202">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="4104f-202">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="4104f-203">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="4104f-203">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="4104f-204">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="4104f-204">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="4104f-205">Управляет возможностью использования специальных символов в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4104f-205">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="4104f-206">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="4104f-206">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="4104f-207">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="4104f-207">pinExpirationInDays</span></span>|<span data-ttu-id="4104f-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4104f-208">Int32</span></span>|<span data-ttu-id="4104f-209">Integer value указывает период времени (в днях), в течение которого можно использовать ПИН-код, прежде чем система потребует от пользователя изменить его.</span><span class="sxs-lookup"><span data-stu-id="4104f-209">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="4104f-210">Допустимые значения: от 0 до 730 включительно.</span><span class="sxs-lookup"><span data-stu-id="4104f-210">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="4104f-211">Допустимые значения: от 0 до 730.</span><span class="sxs-lookup"><span data-stu-id="4104f-211">Valid values 0 to 730</span></span>|
|<span data-ttu-id="4104f-212">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="4104f-212">pinPreviousBlockCount</span></span>|<span data-ttu-id="4104f-213">Int32</span><span class="sxs-lookup"><span data-stu-id="4104f-213">Int32</span></span>|<span data-ttu-id="4104f-214">Управляет возможностью запретить пользователям использовать прошлые контакты.</span><span class="sxs-lookup"><span data-stu-id="4104f-214">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="4104f-215">Он должен иметь значение от 0 до 50 включительно, а текущий ПИН-код пользователя включен в этот счетчик.</span><span class="sxs-lookup"><span data-stu-id="4104f-215">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="4104f-216">Если задано значение 0, предыдущие ПИН-коды не сохраняются.</span><span class="sxs-lookup"><span data-stu-id="4104f-216">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="4104f-217">История ПИН-кодов не сохраняется при сбросе ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="4104f-217">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="4104f-218">Допустимые значения: от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="4104f-218">Valid values 0 to 50</span></span>|
|<span data-ttu-id="4104f-219">пинрековеренаблед</span><span class="sxs-lookup"><span data-stu-id="4104f-219">pinRecoveryEnabled</span></span>|<span data-ttu-id="4104f-220">Логический</span><span class="sxs-lookup"><span data-stu-id="4104f-220">Boolean</span></span>|<span data-ttu-id="4104f-221">Логическое значение, которое позволяет пользователю изменить свой ПИН-код с помощью службы восстановления ПИН-кода Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4104f-221">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="4104f-222">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="4104f-222">securityDeviceRequired</span></span>|<span data-ttu-id="4104f-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="4104f-223">Boolean</span></span>|<span data-ttu-id="4104f-224">Определяет, требуется ли доверенный ПЛАТФОРМЕНный модуль для подготовки Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4104f-224">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="4104f-225">TPM предоставляет дополнительные преимущества безопасности, которые хранятся на нем, не могут использоваться на других устройствах.</span><span class="sxs-lookup"><span data-stu-id="4104f-225">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="4104f-226">Если задано значение false, все устройства могут подготавливать Windows Hello для бизнеса, даже если нет пригодного к использованию доверенного платформенного модуля.</span><span class="sxs-lookup"><span data-stu-id="4104f-226">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="4104f-227">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="4104f-227">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="4104f-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="4104f-228">Boolean</span></span>|<span data-ttu-id="4104f-229">Управляет использованием биометрических жестов, таких как лицо и отпечаток, в качестве альтернативы ПИН-коду Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4104f-229">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="4104f-230">Если задано значение false, биометрические жесты не разрешены.</span><span class="sxs-lookup"><span data-stu-id="4104f-230">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="4104f-231">Пользователи по-прежнему должны настроить ПИН-код в качестве резервной копии в случае сбоев.</span><span class="sxs-lookup"><span data-stu-id="4104f-231">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="4104f-232">усецертификатесфоронпремисесаусенаблед</span><span class="sxs-lookup"><span data-stu-id="4104f-232">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="4104f-233">Логический</span><span class="sxs-lookup"><span data-stu-id="4104f-233">Boolean</span></span>|<span data-ttu-id="4104f-234">Логическое значение, которое позволяет Windows Hello для бизнеса использовать сертификаты для проверки подлинности локальных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4104f-234">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="4104f-235">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="4104f-235">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="4104f-236">Логический</span><span class="sxs-lookup"><span data-stu-id="4104f-236">Boolean</span></span>|<span data-ttu-id="4104f-237">Логическое значение, блокирующее Windows Hello для бизнеса в качестве способа входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="4104f-237">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="4104f-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="4104f-238">Response</span></span>
<span data-ttu-id="4104f-239">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4104f-239">If successful, this method returns a `200 OK` response code and an updated [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4104f-240">Пример</span><span class="sxs-lookup"><span data-stu-id="4104f-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="4104f-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="4104f-241">Request</span></span>
<span data-ttu-id="4104f-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4104f-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4104f-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="4104f-243">Response</span></span>
<span data-ttu-id="4104f-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4104f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






