---
title: Создание windowsIdentityProtectionConfiguration
description: Создайте новый объект WindowsIdentityProtectionConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 674e4fccb6777c527b1051fddc0926253966a8cd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150957"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="e2fb9-103">Создание windowsIdentityProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2fb9-103">Create windowsIdentityProtectionConfiguration</span></span>

<span data-ttu-id="e2fb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2fb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2fb9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2fb9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2fb9-107">Создайте [новый объект WindowsIdentityProtectionConfiguration.](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e2fb9-107">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2fb9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e2fb9-108">Prerequisites</span></span>
<span data-ttu-id="e2fb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2fb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2fb9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2fb9-111">Permission type</span></span>|<span data-ttu-id="e2fb9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2fb9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2fb9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2fb9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2fb9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2fb9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2fb9-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2fb9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2fb9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-116">Not supported.</span></span>|
|<span data-ttu-id="e2fb9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e2fb9-117">Application</span></span>|<span data-ttu-id="e2fb9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2fb9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2fb9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2fb9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e2fb9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e2fb9-120">Request headers</span></span>
|<span data-ttu-id="e2fb9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2fb9-121">Header</span></span>|<span data-ttu-id="e2fb9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e2fb9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2fb9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2fb9-123">Authorization</span></span>|<span data-ttu-id="e2fb9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2fb9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e2fb9-125">Accept</span></span>|<span data-ttu-id="e2fb9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2fb9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2fb9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2fb9-127">Request body</span></span>
<span data-ttu-id="e2fb9-128">В теле запроса поставляем представление JSON для объекта WindowsIdentityProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-128">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="e2fb9-129">В следующей таблице показаны свойства, необходимые при создании windowsIdentityProtectionConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-129">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="e2fb9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2fb9-130">Property</span></span>|<span data-ttu-id="e2fb9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e2fb9-131">Type</span></span>|<span data-ttu-id="e2fb9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e2fb9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2fb9-133">id</span><span class="sxs-lookup"><span data-stu-id="e2fb9-133">id</span></span>|<span data-ttu-id="e2fb9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e2fb9-134">String</span></span>|<span data-ttu-id="e2fb9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-135">Key of the entity.</span></span> <span data-ttu-id="e2fb9-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2fb9-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2fb9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2fb9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e2fb9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2fb9-138">DateTimeOffset</span></span>|<span data-ttu-id="e2fb9-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e2fb9-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2fb9-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2fb9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e2fb9-141">roleScopeTagIds</span></span>|<span data-ttu-id="e2fb9-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e2fb9-142">String collection</span></span>|<span data-ttu-id="e2fb9-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e2fb9-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2fb9-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2fb9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e2fb9-145">supportsScopeTags</span></span>|<span data-ttu-id="e2fb9-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2fb9-146">Boolean</span></span>|<span data-ttu-id="e2fb9-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e2fb9-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e2fb9-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e2fb9-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-150">This property is read-only.</span></span> <span data-ttu-id="e2fb9-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2fb9-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2fb9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e2fb9-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e2fb9-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e2fb9-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e2fb9-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e2fb9-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2fb9-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2fb9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e2fb9-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e2fb9-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e2fb9-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e2fb9-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e2fb9-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2fb9-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2fb9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e2fb9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e2fb9-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e2fb9-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e2fb9-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e2fb9-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2fb9-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2fb9-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2fb9-164">createdDateTime</span></span>|<span data-ttu-id="e2fb9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2fb9-165">DateTimeOffset</span></span>|<span data-ttu-id="e2fb9-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-166">DateTime the object was created.</span></span> <span data-ttu-id="e2fb9-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2fb9-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2fb9-168">description</span><span class="sxs-lookup"><span data-stu-id="e2fb9-168">description</span></span>|<span data-ttu-id="e2fb9-169">Строка</span><span class="sxs-lookup"><span data-stu-id="e2fb9-169">String</span></span>|<span data-ttu-id="e2fb9-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e2fb9-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2fb9-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2fb9-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e2fb9-172">displayName</span></span>|<span data-ttu-id="e2fb9-173">Строка</span><span class="sxs-lookup"><span data-stu-id="e2fb9-173">String</span></span>|<span data-ttu-id="e2fb9-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e2fb9-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2fb9-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2fb9-176">version</span><span class="sxs-lookup"><span data-stu-id="e2fb9-176">version</span></span>|<span data-ttu-id="e2fb9-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e2fb9-177">Int32</span></span>|<span data-ttu-id="e2fb9-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-178">Version of the device configuration.</span></span> <span data-ttu-id="e2fb9-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2fb9-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2fb9-180">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="e2fb9-180">useSecurityKeyForSignin</span></span>|<span data-ttu-id="e2fb9-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2fb9-181">Boolean</span></span>|<span data-ttu-id="e2fb9-182">Значение Boolean, используемая для того, чтобы включить ключ безопасности Windows Hello в качестве учетных данных с логотипом.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-182">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="e2fb9-183">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="e2fb9-183">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="e2fb9-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2fb9-184">Boolean</span></span>|<span data-ttu-id="e2fb9-185">Значение Boolean, используемого для расширения функции распознавания лиц для проверки подлинности лиц в Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-185">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="e2fb9-186">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e2fb9-186">pinMinimumLength</span></span>|<span data-ttu-id="e2fb9-187">Int32</span><span class="sxs-lookup"><span data-stu-id="e2fb9-187">Int32</span></span>|<span data-ttu-id="e2fb9-188">Значение Integer, которое задает минимальное количество символов, необходимых для ПИН-кода Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-188">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="e2fb9-189">Допустимые значения : от 4 до 127 включительно и меньше или меньше значения, установленного для максимального ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-189">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="e2fb9-190">Допустимые значения от 4 до 127</span><span class="sxs-lookup"><span data-stu-id="e2fb9-190">Valid values 4 to 127</span></span>|
|<span data-ttu-id="e2fb9-191">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="e2fb9-191">pinMaximumLength</span></span>|<span data-ttu-id="e2fb9-192">Int32</span><span class="sxs-lookup"><span data-stu-id="e2fb9-192">Int32</span></span>|<span data-ttu-id="e2fb9-193">Значение Integer, которое задает максимальное количество символов, разрешенных для пин-кода работы.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-193">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="e2fb9-194">Допустимые значения от 4 до 127 включительно и больше или равны значению, за набором для минимального ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-194">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="e2fb9-195">Допустимые значения от 4 до 127</span><span class="sxs-lookup"><span data-stu-id="e2fb9-195">Valid values 4 to 127</span></span>|
|<span data-ttu-id="e2fb9-196">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="e2fb9-196">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="e2fb9-197">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="e2fb9-197">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="e2fb9-198">Это значение настраивает использование символов верхнего шкафа в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-198">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="e2fb9-199">Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-199">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="e2fb9-200">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="e2fb9-200">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="e2fb9-201">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="e2fb9-201">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="e2fb9-202">Это значение настраивает использование символов нижнего регистра в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-202">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="e2fb9-203">Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-203">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="e2fb9-204">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="e2fb9-204">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="e2fb9-205">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="e2fb9-205">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="e2fb9-206">Управление возможностью использования специальных символов в ПИН-коде Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-206">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="e2fb9-207">Возможные значения: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-207">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="e2fb9-208">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="e2fb9-208">pinExpirationInDays</span></span>|<span data-ttu-id="e2fb9-209">Int32</span><span class="sxs-lookup"><span data-stu-id="e2fb9-209">Int32</span></span>|<span data-ttu-id="e2fb9-210">Значение integer указывает период (в днях), который ПИН-код можно использовать до того, как система потребует от пользователя его изменить.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-210">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="e2fb9-211">Допустимые значения : от 0 до 730 включительно.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-211">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="e2fb9-212">Допустимые значения: от 0 до 730.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-212">Valid values 0 to 730</span></span>|
|<span data-ttu-id="e2fb9-213">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="e2fb9-213">pinPreviousBlockCount</span></span>|<span data-ttu-id="e2fb9-214">Int32</span><span class="sxs-lookup"><span data-stu-id="e2fb9-214">Int32</span></span>|<span data-ttu-id="e2fb9-215">Контролирует возможность предотвращения использования пользователями прошлых ПИН-данных.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-215">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="e2fb9-216">Это должно быть установлено между 0 и 50 включительно, и текущий ПИН-код пользователя включен в это число.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-216">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="e2fb9-217">Если установлено 0, предыдущие ПИН-данные не сохраняются.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-217">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="e2fb9-218">История ПИН-кода не сохраняется с помощью сброса ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-218">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="e2fb9-219">Допустимые значения: от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-219">Valid values 0 to 50</span></span>|
|<span data-ttu-id="e2fb9-220">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="e2fb9-220">pinRecoveryEnabled</span></span>|<span data-ttu-id="e2fb9-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2fb9-221">Boolean</span></span>|<span data-ttu-id="e2fb9-222">Значение Boolean, которое позволяет пользователю изменять ПИН-код с помощью службы восстановления ПИН-кода Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-222">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="e2fb9-223">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="e2fb9-223">securityDeviceRequired</span></span>|<span data-ttu-id="e2fb9-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2fb9-224">Boolean</span></span>|<span data-ttu-id="e2fb9-225">Управление, необходимо ли требовать доверенный модуль платформы (TPM) для обеспечения Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-225">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="e2fb9-226">TPM предоставляет дополнительные преимущества безопасности в том, что данные, хранимые на нем, не могут использоваться на других устройствах.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-226">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="e2fb9-227">Если установлено false, все устройства могут устанавливать Windows Hello для бизнеса, даже если не существует понятного TPM.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-227">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="e2fb9-228">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="e2fb9-228">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="e2fb9-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2fb9-229">Boolean</span></span>|<span data-ttu-id="e2fb9-230">Управление использованием биометрических жестов, таких как лицо и отпечатки пальцев, в качестве альтернативы ПИН-коду Windows Hello для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-230">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="e2fb9-231">Если установлено false, биометрические жесты не допускаются.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-231">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="e2fb9-232">Пользователи по-прежнему должны настраивать ПИН-код в качестве резервного копирования в случае сбоев.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-232">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="e2fb9-233">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="e2fb9-233">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="e2fb9-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2fb9-234">Boolean</span></span>|<span data-ttu-id="e2fb9-235">Значение Boolean, которое позволяет Windows Hello для бизнеса использовать сертификаты для проверки подлинности локального ресурса.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-235">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="e2fb9-236">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="e2fb9-236">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="e2fb9-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2fb9-237">Boolean</span></span>|<span data-ttu-id="e2fb9-238">Значение Boolean, которое блокирует Windows Hello для бизнеса как метод для подписания в Windows.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-238">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="e2fb9-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2fb9-239">Response</span></span>
<span data-ttu-id="e2fb9-240">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект WindowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-240">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2fb9-241">Пример</span><span class="sxs-lookup"><span data-stu-id="e2fb9-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2fb9-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2fb9-242">Request</span></span>
<span data-ttu-id="e2fb9-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-243">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e2fb9-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2fb9-244">Response</span></span>
<span data-ttu-id="e2fb9-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2fb9-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




