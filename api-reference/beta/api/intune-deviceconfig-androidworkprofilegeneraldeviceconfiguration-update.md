---
title: Обновление androidWorkProfileGeneralDeviceConfiguration
description: Обновление свойств объекта androidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7b8e9f0bcfcde7ffc4dbc19a469e663b2d8f12b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154686"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="be8bd-103">Обновление androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="be8bd-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="be8bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be8bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="be8bd-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be8bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be8bd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be8bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be8bd-107">Обновление свойств объекта [androidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be8bd-107">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be8bd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be8bd-108">Prerequisites</span></span>
<span data-ttu-id="be8bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be8bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be8bd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be8bd-111">Permission type</span></span>|<span data-ttu-id="be8bd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be8bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be8bd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be8bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="be8bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be8bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="be8bd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be8bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be8bd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be8bd-116">Not supported.</span></span>|
|<span data-ttu-id="be8bd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be8bd-117">Application</span></span>|<span data-ttu-id="be8bd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be8bd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="be8bd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be8bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="be8bd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="be8bd-120">Request headers</span></span>
|<span data-ttu-id="be8bd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be8bd-121">Header</span></span>|<span data-ttu-id="be8bd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="be8bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be8bd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be8bd-123">Authorization</span></span>|<span data-ttu-id="be8bd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be8bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be8bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="be8bd-125">Accept</span></span>|<span data-ttu-id="be8bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="be8bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be8bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be8bd-127">Request body</span></span>
<span data-ttu-id="be8bd-128">В теле запроса предоставляем представление объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="be8bd-128">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="be8bd-129">В следующей таблице показаны свойства, необходимые при создании [объекта androidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="be8bd-129">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="be8bd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="be8bd-130">Property</span></span>|<span data-ttu-id="be8bd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="be8bd-131">Type</span></span>|<span data-ttu-id="be8bd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="be8bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be8bd-133">id</span><span class="sxs-lookup"><span data-stu-id="be8bd-133">id</span></span>|<span data-ttu-id="be8bd-134">String</span><span class="sxs-lookup"><span data-stu-id="be8bd-134">String</span></span>|<span data-ttu-id="be8bd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="be8bd-135">Key of the entity.</span></span> <span data-ttu-id="be8bd-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be8bd-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be8bd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be8bd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="be8bd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be8bd-138">DateTimeOffset</span></span>|<span data-ttu-id="be8bd-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="be8bd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="be8bd-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be8bd-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be8bd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="be8bd-141">roleScopeTagIds</span></span>|<span data-ttu-id="be8bd-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="be8bd-142">String collection</span></span>|<span data-ttu-id="be8bd-143">Список тегов области для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="be8bd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="be8bd-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be8bd-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be8bd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="be8bd-145">supportsScopeTags</span></span>|<span data-ttu-id="be8bd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-146">Boolean</span></span>|<span data-ttu-id="be8bd-147">Указывает, поддерживает ли конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="be8bd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="be8bd-148">Назначение свойству ScopeTags запрещено, если это значение имеет значение false, а сущности не будут видны пользователям с заданной областью действия.</span><span class="sxs-lookup"><span data-stu-id="be8bd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="be8bd-149">Это происходит для устаревших политик, созданных в Silverlight, и их можно устранить, удавшись и повторно создав политику на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="be8bd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="be8bd-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be8bd-150">This property is read-only.</span></span> <span data-ttu-id="be8bd-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be8bd-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be8bd-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="be8bd-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="be8bd-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="be8bd-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="be8bd-154">Применимость выпуска ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="be8bd-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="be8bd-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be8bd-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be8bd-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="be8bd-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="be8bd-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="be8bd-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="be8bd-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="be8bd-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="be8bd-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be8bd-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be8bd-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="be8bd-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="be8bd-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="be8bd-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="be8bd-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="be8bd-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="be8bd-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be8bd-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be8bd-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be8bd-164">createdDateTime</span></span>|<span data-ttu-id="be8bd-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be8bd-165">DateTimeOffset</span></span>|<span data-ttu-id="be8bd-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="be8bd-166">DateTime the object was created.</span></span> <span data-ttu-id="be8bd-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be8bd-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be8bd-168">description</span><span class="sxs-lookup"><span data-stu-id="be8bd-168">description</span></span>|<span data-ttu-id="be8bd-169">String</span><span class="sxs-lookup"><span data-stu-id="be8bd-169">String</span></span>|<span data-ttu-id="be8bd-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="be8bd-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="be8bd-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be8bd-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be8bd-172">displayName</span><span class="sxs-lookup"><span data-stu-id="be8bd-172">displayName</span></span>|<span data-ttu-id="be8bd-173">String</span><span class="sxs-lookup"><span data-stu-id="be8bd-173">String</span></span>|<span data-ttu-id="be8bd-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="be8bd-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="be8bd-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be8bd-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be8bd-176">version</span><span class="sxs-lookup"><span data-stu-id="be8bd-176">version</span></span>|<span data-ttu-id="be8bd-177">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-177">Int32</span></span>|<span data-ttu-id="be8bd-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="be8bd-178">Version of the device configuration.</span></span> <span data-ttu-id="be8bd-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="be8bd-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="be8bd-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="be8bd-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="be8bd-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-181">Boolean</span></span>|<span data-ttu-id="be8bd-182">Указывает, следует ли заблокировать разблокировку лиц.</span><span class="sxs-lookup"><span data-stu-id="be8bd-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="be8bd-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="be8bd-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="be8bd-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-184">Boolean</span></span>|<span data-ttu-id="be8bd-185">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="be8bd-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="be8bd-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="be8bd-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="be8bd-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-187">Boolean</span></span>|<span data-ttu-id="be8bd-188">Указывает, следует ли заблокировать разблокировку радужной оболочки радужной оболочки.</span><span class="sxs-lookup"><span data-stu-id="be8bd-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="be8bd-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="be8bd-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="be8bd-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-190">Boolean</span></span>|<span data-ttu-id="be8bd-191">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="be8bd-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="be8bd-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="be8bd-192">passwordExpirationDays</span></span>|<span data-ttu-id="be8bd-193">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-193">Int32</span></span>|<span data-ttu-id="be8bd-194">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="be8bd-194">Number of days before the password expires.</span></span> <span data-ttu-id="be8bd-195">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="be8bd-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="be8bd-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="be8bd-196">passwordMinimumLength</span></span>|<span data-ttu-id="be8bd-197">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-197">Int32</span></span>|<span data-ttu-id="be8bd-198">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="be8bd-198">Minimum length of passwords.</span></span> <span data-ttu-id="be8bd-199">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="be8bd-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="be8bd-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="be8bd-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="be8bd-201">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-201">Int32</span></span>|<span data-ttu-id="be8bd-202">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="be8bd-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="be8bd-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="be8bd-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="be8bd-204">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-204">Int32</span></span>|<span data-ttu-id="be8bd-205">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="be8bd-205">Number of previous passwords to block.</span></span> <span data-ttu-id="be8bd-206">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="be8bd-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="be8bd-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="be8bd-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="be8bd-208">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-208">Int32</span></span>|<span data-ttu-id="be8bd-209">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="be8bd-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="be8bd-210">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="be8bd-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="be8bd-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="be8bd-211">passwordRequiredType</span></span>|[<span data-ttu-id="be8bd-212">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="be8bd-212">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="be8bd-213">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="be8bd-213">Type of password that is required.</span></span> <span data-ttu-id="be8bd-214">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="be8bd-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="be8bd-215">workProfileAllowAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="be8bd-215">workProfileAllowAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="be8bd-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-216">Boolean</span></span>|<span data-ttu-id="be8bd-217">Указывает, следует ли разрешить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="be8bd-217">Indicates whether to allow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="be8bd-218">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="be8bd-218">workProfileDataSharingType</span></span>|[<span data-ttu-id="be8bd-219">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="be8bd-219">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="be8bd-220">Тип разрешенного общего доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="be8bd-220">Type of data sharing that is allowed.</span></span> <span data-ttu-id="be8bd-221">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="be8bd-221">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="be8bd-222">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="be8bd-222">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="be8bd-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-223">Boolean</span></span>|<span data-ttu-id="be8bd-224">Указывает, следует ли блокировать уведомления во время блокировки устройства.</span><span class="sxs-lookup"><span data-stu-id="be8bd-224">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="be8bd-225">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="be8bd-225">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="be8bd-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-226">Boolean</span></span>|<span data-ttu-id="be8bd-227">Блокировать добавление и удаление учетных записей в профиле работы.</span><span class="sxs-lookup"><span data-stu-id="be8bd-227">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="be8bd-228">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="be8bd-228">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="be8bd-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-229">Boolean</span></span>|<span data-ttu-id="be8bd-230">Разрешить устройствам Bluetooth доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="be8bd-230">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="be8bd-231">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="be8bd-231">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="be8bd-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-232">Boolean</span></span>|<span data-ttu-id="be8bd-233">Блокировка снимка экрана в профиле работы.</span><span class="sxs-lookup"><span data-stu-id="be8bd-233">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="be8bd-234">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="be8bd-234">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="be8bd-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-235">Boolean</span></span>|<span data-ttu-id="be8bd-236">Заблокируют ид вызываемой области для отображения в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="be8bd-236">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="be8bd-237">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="be8bd-237">workProfileBlockCamera</span></span>|<span data-ttu-id="be8bd-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-238">Boolean</span></span>|<span data-ttu-id="be8bd-239">Блокировка камеры профиля работы.</span><span class="sxs-lookup"><span data-stu-id="be8bd-239">Block work profile camera.</span></span>|
|<span data-ttu-id="be8bd-240">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="be8bd-240">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="be8bd-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-241">Boolean</span></span>|<span data-ttu-id="be8bd-242">Блокировка доступности контактов в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="be8bd-242">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="be8bd-243">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="be8bd-243">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="be8bd-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-244">Boolean</span></span>|<span data-ttu-id="be8bd-245">Boolean, который указывает, включен ли параметр для перекрестной копии профиля или в виде вися.</span><span class="sxs-lookup"><span data-stu-id="be8bd-245">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="be8bd-246">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="be8bd-246">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="be8bd-247">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="be8bd-247">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="be8bd-248">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="be8bd-248">Type of password that is required.</span></span> <span data-ttu-id="be8bd-249">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="be8bd-249">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="be8bd-250">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="be8bd-250">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="be8bd-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-251">Boolean</span></span>|<span data-ttu-id="be8bd-252">Указывает, следует ли заблокировать разблокировку лиц для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="be8bd-252">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="be8bd-253">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="be8bd-253">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="be8bd-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-254">Boolean</span></span>|<span data-ttu-id="be8bd-255">Указывает, следует ли заблокировать разблокировку отпечатков пальцев для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="be8bd-255">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="be8bd-256">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="be8bd-256">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="be8bd-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-257">Boolean</span></span>|<span data-ttu-id="be8bd-258">Указывает, следует ли заблокировать разблокировку радужной оболочки радужной оболочки для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="be8bd-258">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="be8bd-259">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="be8bd-259">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="be8bd-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-260">Boolean</span></span>|<span data-ttu-id="be8bd-261">Указывает, следует ли заблокировать smart Lock и другие агенты доверия для работы профиля.</span><span class="sxs-lookup"><span data-stu-id="be8bd-261">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="be8bd-262">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="be8bd-262">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="be8bd-263">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-263">Int32</span></span>|<span data-ttu-id="be8bd-264">Количество дней до истечения срока действия пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="be8bd-264">Number of days before the work profile password expires.</span></span> <span data-ttu-id="be8bd-265">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="be8bd-265">Valid values 1 to 365</span></span>|
|<span data-ttu-id="be8bd-266">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="be8bd-266">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="be8bd-267">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-267">Int32</span></span>|<span data-ttu-id="be8bd-268">Минимальная длина пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="be8bd-268">Minimum length of work profile password.</span></span> <span data-ttu-id="be8bd-269">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="be8bd-269">Valid values 4 to 16</span></span>|
|<span data-ttu-id="be8bd-270">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="be8bd-270">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="be8bd-271">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-271">Int32</span></span>|<span data-ttu-id="be8bd-272">Минимальное число цифр, необходимое для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="be8bd-272">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="be8bd-273">Допустимые значения: от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="be8bd-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="be8bd-274">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="be8bd-274">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="be8bd-275">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-275">Int32</span></span>|<span data-ttu-id="be8bd-276">Минимальное количество символов, не букв, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="be8bd-276">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="be8bd-277">Допустимые значения: от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="be8bd-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="be8bd-278">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="be8bd-278">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="be8bd-279">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-279">Int32</span></span>|<span data-ttu-id="be8bd-280">Минимальное количество букв в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="be8bd-280">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="be8bd-281">Допустимые значения: от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="be8bd-281">Valid values 1 to 10</span></span>|
|<span data-ttu-id="be8bd-282">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="be8bd-282">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="be8bd-283">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-283">Int32</span></span>|<span data-ttu-id="be8bd-284">Минимальное количество символов нижнего уровня, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="be8bd-284">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="be8bd-285">Допустимые значения: от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="be8bd-285">Valid values 1 to 10</span></span>|
|<span data-ttu-id="be8bd-286">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="be8bd-286">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="be8bd-287">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-287">Int32</span></span>|<span data-ttu-id="be8bd-288">Минимальное количество символов верхнего уровня, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="be8bd-288">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="be8bd-289">Допустимые значения: от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="be8bd-289">Valid values 1 to 10</span></span>|
|<span data-ttu-id="be8bd-290">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="be8bd-290">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="be8bd-291">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-291">Int32</span></span>|<span data-ttu-id="be8bd-292">Минимальное количество символов, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="be8bd-292">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="be8bd-293">Допустимые значения: от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="be8bd-293">Valid values 1 to 10</span></span>|
|<span data-ttu-id="be8bd-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="be8bd-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="be8bd-295">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-295">Int32</span></span>|<span data-ttu-id="be8bd-296">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="be8bd-296">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="be8bd-297">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="be8bd-297">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="be8bd-298">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-298">Int32</span></span>|<span data-ttu-id="be8bd-299">Количество предыдущих паролей профилей, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="be8bd-299">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="be8bd-300">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="be8bd-300">Valid values 0 to 24</span></span>|
|<span data-ttu-id="be8bd-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="be8bd-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="be8bd-302">Int32</span><span class="sxs-lookup"><span data-stu-id="be8bd-302">Int32</span></span>|<span data-ttu-id="be8bd-303">Количество неудачных входов, разрешенных до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="be8bd-303">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="be8bd-304">Допустимые значения: от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="be8bd-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="be8bd-305">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="be8bd-305">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="be8bd-306">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="be8bd-306">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="be8bd-307">Тип требуемого пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="be8bd-307">Type of work profile password that is required.</span></span> <span data-ttu-id="be8bd-308">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="be8bd-308">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="be8bd-309">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="be8bd-309">workProfileRequirePassword</span></span>|<span data-ttu-id="be8bd-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-310">Boolean</span></span>|<span data-ttu-id="be8bd-311">Пароль требуется или не требуется для профиля работы</span><span class="sxs-lookup"><span data-stu-id="be8bd-311">Password is required or not for work profile</span></span>|
|<span data-ttu-id="be8bd-312">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="be8bd-312">securityRequireVerifyApps</span></span>|<span data-ttu-id="be8bd-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-313">Boolean</span></span>|<span data-ttu-id="be8bd-314">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="be8bd-314">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="be8bd-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="be8bd-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="be8bd-316">String</span><span class="sxs-lookup"><span data-stu-id="be8bd-316">String</span></span>|<span data-ttu-id="be8bd-317">Включить режим блокировки для постоянно в сети VPN.</span><span class="sxs-lookup"><span data-stu-id="be8bd-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="be8bd-318">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="be8bd-318">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="be8bd-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-319">Boolean</span></span>|<span data-ttu-id="be8bd-320">Включить режим блокировки для постоянно в сети VPN.</span><span class="sxs-lookup"><span data-stu-id="be8bd-320">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="be8bd-321">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="be8bd-321">workProfileAllowWidgets</span></span>|<span data-ttu-id="be8bd-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-322">Boolean</span></span>|<span data-ttu-id="be8bd-323">Разрешить виджеты из приложений рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="be8bd-323">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="be8bd-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="be8bd-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="be8bd-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="be8bd-325">Boolean</span></span>|<span data-ttu-id="be8bd-326">Запретить установку приложений из неизвестных источников в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="be8bd-326">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="be8bd-327">Отклик</span><span class="sxs-lookup"><span data-stu-id="be8bd-327">Response</span></span>
<span data-ttu-id="be8bd-328">В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="be8bd-328">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be8bd-329">Пример</span><span class="sxs-lookup"><span data-stu-id="be8bd-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="be8bd-330">Запрос</span><span class="sxs-lookup"><span data-stu-id="be8bd-330">Request</span></span>
<span data-ttu-id="be8bd-331">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be8bd-331">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3141

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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
  "passwordBlockFaceUnlock": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockIrisUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileAllowAppInstallsFromUnknownSources": true,
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFaceUnlock": true,
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockIrisUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```

### <a name="response"></a><span data-ttu-id="be8bd-332">Отклик</span><span class="sxs-lookup"><span data-stu-id="be8bd-332">Response</span></span>
<span data-ttu-id="be8bd-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be8bd-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3313

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
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
  "passwordBlockFaceUnlock": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockIrisUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileAllowAppInstallsFromUnknownSources": true,
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFaceUnlock": true,
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockIrisUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true,
  "workProfileAllowWidgets": true,
  "workProfileBlockPersonalAppInstallsFromUnknownSources": true
}
```




