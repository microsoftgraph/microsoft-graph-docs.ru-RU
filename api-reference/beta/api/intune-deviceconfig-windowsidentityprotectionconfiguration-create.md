---
title: Создание Виндовсидентитипротектионконфигуратион
description: Создание нового объекта Виндовсидентитипротектионконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 661af9649e9e3bee677c2d16002305c7bc281524
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35962430"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="d381b-103">Создание Виндовсидентитипротектионконфигуратион</span><span class="sxs-lookup"><span data-stu-id="d381b-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="d381b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d381b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d381b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d381b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d381b-106">Создание нового объекта [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d381b-106">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d381b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d381b-107">Prerequisites</span></span>
<span data-ttu-id="d381b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d381b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d381b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d381b-110">Permission type</span></span>|<span data-ttu-id="d381b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d381b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d381b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d381b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d381b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d381b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d381b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d381b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d381b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d381b-115">Not supported.</span></span>|
|<span data-ttu-id="d381b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d381b-116">Application</span></span>|<span data-ttu-id="d381b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d381b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d381b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d381b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d381b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d381b-119">Request headers</span></span>
|<span data-ttu-id="d381b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d381b-120">Header</span></span>|<span data-ttu-id="d381b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d381b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d381b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d381b-122">Authorization</span></span>|<span data-ttu-id="d381b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d381b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d381b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d381b-124">Accept</span></span>|<span data-ttu-id="d381b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d381b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d381b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d381b-126">Request body</span></span>
<span data-ttu-id="d381b-127">В тексте запроса добавьте представление объекта Виндовсидентитипротектионконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d381b-127">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="d381b-128">В следующей таблице приведены свойства, необходимые при создании Виндовсидентитипротектионконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="d381b-128">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="d381b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d381b-129">Property</span></span>|<span data-ttu-id="d381b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d381b-130">Type</span></span>|<span data-ttu-id="d381b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d381b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d381b-132">id</span><span class="sxs-lookup"><span data-stu-id="d381b-132">id</span></span>|<span data-ttu-id="d381b-133">String</span><span class="sxs-lookup"><span data-stu-id="d381b-133">String</span></span>|<span data-ttu-id="d381b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d381b-134">Key of the entity.</span></span> <span data-ttu-id="d381b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d381b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d381b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d381b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d381b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d381b-137">DateTimeOffset</span></span>|<span data-ttu-id="d381b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d381b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d381b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d381b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d381b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d381b-140">roleScopeTagIds</span></span>|<span data-ttu-id="d381b-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d381b-141">String collection</span></span>|<span data-ttu-id="d381b-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d381b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d381b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d381b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d381b-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d381b-144">supportsScopeTags</span></span>|<span data-ttu-id="d381b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d381b-145">Boolean</span></span>|<span data-ttu-id="d381b-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d381b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d381b-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d381b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d381b-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d381b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d381b-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d381b-149">This property is read-only.</span></span> <span data-ttu-id="d381b-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d381b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d381b-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d381b-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d381b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d381b-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d381b-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d381b-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d381b-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d381b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d381b-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d381b-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d381b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d381b-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d381b-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d381b-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d381b-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d381b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d381b-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d381b-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d381b-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d381b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d381b-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d381b-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d381b-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d381b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d381b-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d381b-163">createdDateTime</span></span>|<span data-ttu-id="d381b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d381b-164">DateTimeOffset</span></span>|<span data-ttu-id="d381b-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d381b-165">DateTime the object was created.</span></span> <span data-ttu-id="d381b-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d381b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d381b-167">description</span><span class="sxs-lookup"><span data-stu-id="d381b-167">description</span></span>|<span data-ttu-id="d381b-168">String</span><span class="sxs-lookup"><span data-stu-id="d381b-168">String</span></span>|<span data-ttu-id="d381b-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d381b-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d381b-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d381b-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d381b-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d381b-171">displayName</span></span>|<span data-ttu-id="d381b-172">Строка</span><span class="sxs-lookup"><span data-stu-id="d381b-172">String</span></span>|<span data-ttu-id="d381b-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d381b-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d381b-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d381b-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d381b-175">version</span><span class="sxs-lookup"><span data-stu-id="d381b-175">version</span></span>|<span data-ttu-id="d381b-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d381b-176">Int32</span></span>|<span data-ttu-id="d381b-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d381b-177">Version of the device configuration.</span></span> <span data-ttu-id="d381b-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d381b-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d381b-179">Усесекуритикэйфорсигнин</span><span class="sxs-lookup"><span data-stu-id="d381b-179">useSecurityKeyForSignin</span></span>|<span data-ttu-id="d381b-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="d381b-180">Boolean</span></span>|<span data-ttu-id="d381b-181">Логическое значение, используемое для включения ключа безопасности Windows Hello в качестве учетных данных для входа.</span><span class="sxs-lookup"><span data-stu-id="d381b-181">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="d381b-182">ЕнханцедантиспуфингфорфаЦиалфеатуресенаблед</span><span class="sxs-lookup"><span data-stu-id="d381b-182">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="d381b-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="d381b-183">Boolean</span></span>|<span data-ttu-id="d381b-184">Логическое значение, используемое для включения расширенного средства защиты от спуфинга для распознавания функции лица при проверке подлинности Windows Hello для лиц.</span><span class="sxs-lookup"><span data-stu-id="d381b-184">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="d381b-185">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d381b-185">pinMinimumLength</span></span>|<span data-ttu-id="d381b-186">Int32</span><span class="sxs-lookup"><span data-stu-id="d381b-186">Int32</span></span>|<span data-ttu-id="d381b-187">Целочисленное значение, задающее минимальное число символов, необходимое для ПИН-кода Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d381b-187">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d381b-188">Допустимые значения: от 4 до 127 включительно и меньше или равны набору значений для максимального ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="d381b-188">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="d381b-189">Допустимые значения — от 4 до 127</span><span class="sxs-lookup"><span data-stu-id="d381b-189">Valid values 4 to 127</span></span>|
|<span data-ttu-id="d381b-190">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="d381b-190">pinMaximumLength</span></span>|<span data-ttu-id="d381b-191">Int32</span><span class="sxs-lookup"><span data-stu-id="d381b-191">Int32</span></span>|<span data-ttu-id="d381b-192">Целое значение, задающее максимальное количество символов для рабочего ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="d381b-192">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="d381b-193">Допустимые значения: от 4 до 127 включительно и больше или равны значению, заданному для минимального ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="d381b-193">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="d381b-194">Допустимые значения — от 4 до 127</span><span class="sxs-lookup"><span data-stu-id="d381b-194">Valid values 4 to 127</span></span>|
|<span data-ttu-id="d381b-195">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d381b-195">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="d381b-196">Конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="d381b-196">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d381b-197">Это значение позволяет настроить использование символов верхнего регистра в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d381b-197">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d381b-198">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d381b-198">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d381b-199">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d381b-199">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="d381b-200">Конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="d381b-200">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d381b-201">Это значение позволяет настроить использование символов нижнего регистра в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d381b-201">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d381b-202">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d381b-202">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d381b-203">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="d381b-203">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="d381b-204">Конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="d381b-204">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d381b-205">Управляет возможностью использования специальных символов в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d381b-205">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="d381b-206">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d381b-206">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d381b-207">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="d381b-207">pinExpirationInDays</span></span>|<span data-ttu-id="d381b-208">Int32</span><span class="sxs-lookup"><span data-stu-id="d381b-208">Int32</span></span>|<span data-ttu-id="d381b-209">Integer value указывает период времени (в днях), в течение которого можно использовать ПИН-код, прежде чем система потребует от пользователя изменить его.</span><span class="sxs-lookup"><span data-stu-id="d381b-209">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="d381b-210">Допустимые значения: от 0 до 730 включительно.</span><span class="sxs-lookup"><span data-stu-id="d381b-210">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="d381b-211">Допустимые значения: от 0 до 730.</span><span class="sxs-lookup"><span data-stu-id="d381b-211">Valid values 0 to 730</span></span>|
|<span data-ttu-id="d381b-212">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="d381b-212">pinPreviousBlockCount</span></span>|<span data-ttu-id="d381b-213">Int32</span><span class="sxs-lookup"><span data-stu-id="d381b-213">Int32</span></span>|<span data-ttu-id="d381b-214">Управляет возможностью запретить пользователям использовать прошлые контакты.</span><span class="sxs-lookup"><span data-stu-id="d381b-214">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="d381b-215">Он должен иметь значение от 0 до 50 включительно, а текущий ПИН-код пользователя включен в этот счетчик.</span><span class="sxs-lookup"><span data-stu-id="d381b-215">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="d381b-216">Если задано значение 0, предыдущие ПИН-коды не сохраняются.</span><span class="sxs-lookup"><span data-stu-id="d381b-216">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="d381b-217">История ПИН-кодов не сохраняется при сбросе ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="d381b-217">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="d381b-218">Допустимые значения: от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="d381b-218">Valid values 0 to 50</span></span>|
|<span data-ttu-id="d381b-219">Пинрековеренаблед</span><span class="sxs-lookup"><span data-stu-id="d381b-219">pinRecoveryEnabled</span></span>|<span data-ttu-id="d381b-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="d381b-220">Boolean</span></span>|<span data-ttu-id="d381b-221">Логическое значение, которое позволяет пользователю изменить свой ПИН-код с помощью службы восстановления ПИН-кода Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d381b-221">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="d381b-222">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="d381b-222">securityDeviceRequired</span></span>|<span data-ttu-id="d381b-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="d381b-223">Boolean</span></span>|<span data-ttu-id="d381b-224">Определяет, требуется ли доверенный ПЛАТФОРМЕНный модуль для подготовки Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d381b-224">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="d381b-225">TPM предоставляет дополнительные преимущества безопасности, которые хранятся на нем, не могут использоваться на других устройствах.</span><span class="sxs-lookup"><span data-stu-id="d381b-225">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="d381b-226">Если задано значение false, все устройства могут подготавливать Windows Hello для бизнеса, даже если нет пригодного к использованию доверенного платформенного модуля.</span><span class="sxs-lookup"><span data-stu-id="d381b-226">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="d381b-227">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="d381b-227">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="d381b-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="d381b-228">Boolean</span></span>|<span data-ttu-id="d381b-229">Управляет использованием биометрических жестов, таких как лицо и отпечаток, в качестве альтернативы ПИН-коду Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="d381b-229">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="d381b-230">Если задано значение false, биометрические жесты не разрешены.</span><span class="sxs-lookup"><span data-stu-id="d381b-230">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="d381b-231">Пользователи по-прежнему должны настроить ПИН-код в качестве резервной копии в случае сбоев.</span><span class="sxs-lookup"><span data-stu-id="d381b-231">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="d381b-232">Усецертификатесфоронпремисесаусенаблед</span><span class="sxs-lookup"><span data-stu-id="d381b-232">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="d381b-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="d381b-233">Boolean</span></span>|<span data-ttu-id="d381b-234">Логическое значение, которое позволяет Windows Hello для бизнеса использовать сертификаты для проверки подлинности локальных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d381b-234">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="d381b-235">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="d381b-235">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="d381b-236">Логический</span><span class="sxs-lookup"><span data-stu-id="d381b-236">Boolean</span></span>|<span data-ttu-id="d381b-237">Логическое значение, блокирующее Windows Hello для бизнеса в качестве способа входа в Windows.</span><span class="sxs-lookup"><span data-stu-id="d381b-237">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="d381b-238">Отклик</span><span class="sxs-lookup"><span data-stu-id="d381b-238">Response</span></span>
<span data-ttu-id="d381b-239">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсидентитипротектионконфигуратион](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d381b-239">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d381b-240">Пример</span><span class="sxs-lookup"><span data-stu-id="d381b-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="d381b-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="d381b-241">Request</span></span>
<span data-ttu-id="d381b-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d381b-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d381b-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="d381b-243">Response</span></span>
<span data-ttu-id="d381b-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d381b-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





