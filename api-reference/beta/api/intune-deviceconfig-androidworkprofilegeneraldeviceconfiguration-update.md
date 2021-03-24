---
title: Обновление androidWorkProfileGeneralDeviceConfiguration
description: Обновление свойств объекта AndroidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e1a0c563e83051968d970c9b5bdda69f178b9f68
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148115"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="2b16d-103">Обновление androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b16d-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="2b16d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b16d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b16d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b16d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b16d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2b16d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b16d-107">Обновление свойств объекта [AndroidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b16d-107">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b16d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2b16d-108">Prerequisites</span></span>
<span data-ttu-id="2b16d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b16d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b16d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b16d-111">Permission type</span></span>|<span data-ttu-id="2b16d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b16d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b16d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b16d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b16d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b16d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b16d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b16d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b16d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b16d-116">Not supported.</span></span>|
|<span data-ttu-id="2b16d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="2b16d-117">Application</span></span>|<span data-ttu-id="2b16d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b16d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b16d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b16d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2b16d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2b16d-120">Request headers</span></span>
|<span data-ttu-id="2b16d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b16d-121">Header</span></span>|<span data-ttu-id="2b16d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2b16d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b16d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b16d-123">Authorization</span></span>|<span data-ttu-id="2b16d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b16d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b16d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b16d-125">Accept</span></span>|<span data-ttu-id="2b16d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b16d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b16d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b16d-127">Request body</span></span>
<span data-ttu-id="2b16d-128">В теле запроса предоставляем представление JSON для [объекта AndroidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b16d-128">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="2b16d-129">В следующей таблице показаны свойства, необходимые при создании [androidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b16d-129">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="2b16d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2b16d-130">Property</span></span>|<span data-ttu-id="2b16d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2b16d-131">Type</span></span>|<span data-ttu-id="2b16d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2b16d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b16d-133">id</span><span class="sxs-lookup"><span data-stu-id="2b16d-133">id</span></span>|<span data-ttu-id="2b16d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2b16d-134">String</span></span>|<span data-ttu-id="2b16d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2b16d-135">Key of the entity.</span></span> <span data-ttu-id="2b16d-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b16d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b16d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b16d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2b16d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b16d-138">DateTimeOffset</span></span>|<span data-ttu-id="2b16d-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2b16d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2b16d-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b16d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b16d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b16d-141">roleScopeTagIds</span></span>|<span data-ttu-id="2b16d-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2b16d-142">String collection</span></span>|<span data-ttu-id="2b16d-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="2b16d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2b16d-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b16d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b16d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2b16d-145">supportsScopeTags</span></span>|<span data-ttu-id="2b16d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-146">Boolean</span></span>|<span data-ttu-id="2b16d-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="2b16d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2b16d-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="2b16d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2b16d-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="2b16d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2b16d-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2b16d-150">This property is read-only.</span></span> <span data-ttu-id="2b16d-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b16d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b16d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2b16d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="2b16d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="2b16d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="2b16d-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2b16d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="2b16d-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b16d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b16d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2b16d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="2b16d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="2b16d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="2b16d-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2b16d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="2b16d-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b16d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b16d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2b16d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="2b16d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="2b16d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="2b16d-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="2b16d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="2b16d-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b16d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b16d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b16d-164">createdDateTime</span></span>|<span data-ttu-id="2b16d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b16d-165">DateTimeOffset</span></span>|<span data-ttu-id="2b16d-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2b16d-166">DateTime the object was created.</span></span> <span data-ttu-id="2b16d-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b16d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b16d-168">description</span><span class="sxs-lookup"><span data-stu-id="2b16d-168">description</span></span>|<span data-ttu-id="2b16d-169">Строка</span><span class="sxs-lookup"><span data-stu-id="2b16d-169">String</span></span>|<span data-ttu-id="2b16d-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b16d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2b16d-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b16d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b16d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="2b16d-172">displayName</span></span>|<span data-ttu-id="2b16d-173">Строка</span><span class="sxs-lookup"><span data-stu-id="2b16d-173">String</span></span>|<span data-ttu-id="2b16d-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b16d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2b16d-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b16d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b16d-176">version</span><span class="sxs-lookup"><span data-stu-id="2b16d-176">version</span></span>|<span data-ttu-id="2b16d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-177">Int32</span></span>|<span data-ttu-id="2b16d-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2b16d-178">Version of the device configuration.</span></span> <span data-ttu-id="2b16d-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2b16d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b16d-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="2b16d-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="2b16d-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-181">Boolean</span></span>|<span data-ttu-id="2b16d-182">Указывает, следует ли блокировать разблокирование лица.</span><span class="sxs-lookup"><span data-stu-id="2b16d-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="2b16d-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="2b16d-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="2b16d-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-184">Boolean</span></span>|<span data-ttu-id="2b16d-185">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="2b16d-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="2b16d-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="2b16d-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="2b16d-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-187">Boolean</span></span>|<span data-ttu-id="2b16d-188">Указывает, следует ли блокировать разблокировку радужной оболочки радужной оболочки.</span><span class="sxs-lookup"><span data-stu-id="2b16d-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="2b16d-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="2b16d-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="2b16d-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-190">Boolean</span></span>|<span data-ttu-id="2b16d-191">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="2b16d-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="2b16d-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2b16d-192">passwordExpirationDays</span></span>|<span data-ttu-id="2b16d-193">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-193">Int32</span></span>|<span data-ttu-id="2b16d-194">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="2b16d-194">Number of days before the password expires.</span></span> <span data-ttu-id="2b16d-195">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="2b16d-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2b16d-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2b16d-196">passwordMinimumLength</span></span>|<span data-ttu-id="2b16d-197">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-197">Int32</span></span>|<span data-ttu-id="2b16d-198">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="2b16d-198">Minimum length of passwords.</span></span> <span data-ttu-id="2b16d-199">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="2b16d-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2b16d-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2b16d-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2b16d-201">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-201">Int32</span></span>|<span data-ttu-id="2b16d-202">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="2b16d-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2b16d-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2b16d-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2b16d-204">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-204">Int32</span></span>|<span data-ttu-id="2b16d-205">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="2b16d-205">Number of previous passwords to block.</span></span> <span data-ttu-id="2b16d-206">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="2b16d-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2b16d-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2b16d-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2b16d-208">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-208">Int32</span></span>|<span data-ttu-id="2b16d-209">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="2b16d-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="2b16d-210">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="2b16d-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2b16d-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2b16d-211">passwordRequiredType</span></span>|[<span data-ttu-id="2b16d-212">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2b16d-212">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="2b16d-213">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="2b16d-213">Type of password that is required.</span></span> <span data-ttu-id="2b16d-214">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="2b16d-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="2b16d-215">workProfileAllowAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="2b16d-215">workProfileAllowAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="2b16d-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-216">Boolean</span></span>|<span data-ttu-id="2b16d-217">Указывает, следует ли разрешить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="2b16d-217">Indicates whether to allow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="2b16d-218">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="2b16d-218">workProfileDataSharingType</span></span>|[<span data-ttu-id="2b16d-219">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="2b16d-219">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="2b16d-220">Тип разрешенного обмена данными.</span><span class="sxs-lookup"><span data-stu-id="2b16d-220">Type of data sharing that is allowed.</span></span> <span data-ttu-id="2b16d-221">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="2b16d-221">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="2b16d-222">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="2b16d-222">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="2b16d-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-223">Boolean</span></span>|<span data-ttu-id="2b16d-224">Указывает, следует ли блокировать уведомления во время блокировки устройства.</span><span class="sxs-lookup"><span data-stu-id="2b16d-224">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="2b16d-225">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="2b16d-225">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="2b16d-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-226">Boolean</span></span>|<span data-ttu-id="2b16d-227">Блокировать добавление и удаление учетных записей в профиле работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-227">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="2b16d-228">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="2b16d-228">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="2b16d-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-229">Boolean</span></span>|<span data-ttu-id="2b16d-230">Разрешить устройствам Bluetooth доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="2b16d-230">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="2b16d-231">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="2b16d-231">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="2b16d-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-232">Boolean</span></span>|<span data-ttu-id="2b16d-233">Блокировка захвата экрана в профиле работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-233">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="2b16d-234">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="2b16d-234">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="2b16d-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-235">Boolean</span></span>|<span data-ttu-id="2b16d-236">Блокировка ИД вызываемой личности вызываемой на экране работы в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="2b16d-236">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="2b16d-237">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="2b16d-237">workProfileBlockCamera</span></span>|<span data-ttu-id="2b16d-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-238">Boolean</span></span>|<span data-ttu-id="2b16d-239">Блокировка камеры профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-239">Block work profile camera.</span></span>|
|<span data-ttu-id="2b16d-240">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="2b16d-240">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="2b16d-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-241">Boolean</span></span>|<span data-ttu-id="2b16d-242">Блокировка доступности контактов профилей работы в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="2b16d-242">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="2b16d-243">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="2b16d-243">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="2b16d-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-244">Boolean</span></span>|<span data-ttu-id="2b16d-245">Boolean, который указывает, включен ли параметр, который не позволяет копировать/вклеить перекрестный профиль.</span><span class="sxs-lookup"><span data-stu-id="2b16d-245">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="2b16d-246">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="2b16d-246">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="2b16d-247">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="2b16d-247">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="2b16d-248">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="2b16d-248">Type of password that is required.</span></span> <span data-ttu-id="2b16d-249">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="2b16d-249">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="2b16d-250">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="2b16d-250">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="2b16d-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-251">Boolean</span></span>|<span data-ttu-id="2b16d-252">Указывает, следует ли блокировать разблокировку лица для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-252">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="2b16d-253">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="2b16d-253">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="2b16d-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-254">Boolean</span></span>|<span data-ttu-id="2b16d-255">Указывает, следует ли блокировать разблокировку отпечатков пальцев для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-255">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="2b16d-256">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="2b16d-256">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="2b16d-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-257">Boolean</span></span>|<span data-ttu-id="2b16d-258">Указывает, следует ли блокировать разблокировку радужной оболочки радужной оболочки для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-258">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="2b16d-259">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="2b16d-259">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="2b16d-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-260">Boolean</span></span>|<span data-ttu-id="2b16d-261">Указывает, следует ли блокировать Smart Lock и другие агенты доверия для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-261">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="2b16d-262">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2b16d-262">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="2b16d-263">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-263">Int32</span></span>|<span data-ttu-id="2b16d-264">Количество дней до истечения срока действия пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-264">Number of days before the work profile password expires.</span></span> <span data-ttu-id="2b16d-265">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="2b16d-265">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2b16d-266">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2b16d-266">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="2b16d-267">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-267">Int32</span></span>|<span data-ttu-id="2b16d-268">Минимальная длина пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-268">Minimum length of work profile password.</span></span> <span data-ttu-id="2b16d-269">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="2b16d-269">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2b16d-270">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="2b16d-270">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="2b16d-271">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-271">Int32</span></span>|<span data-ttu-id="2b16d-272">Минимум # числимые символы, необходимые в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-272">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="2b16d-273">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="2b16d-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2b16d-274">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="2b16d-274">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="2b16d-275">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-275">Int32</span></span>|<span data-ttu-id="2b16d-276">Минимальное количество символов без букв, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-276">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="2b16d-277">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="2b16d-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2b16d-278">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="2b16d-278">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="2b16d-279">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-279">Int32</span></span>|<span data-ttu-id="2b16d-280">Минимальный # буквы символов, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-280">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="2b16d-281">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="2b16d-281">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2b16d-282">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="2b16d-282">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="2b16d-283">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-283">Int32</span></span>|<span data-ttu-id="2b16d-284">Минимальное количество символов нижнего уровня, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-284">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="2b16d-285">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="2b16d-285">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2b16d-286">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="2b16d-286">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="2b16d-287">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-287">Int32</span></span>|<span data-ttu-id="2b16d-288">Минимальный # символов верхнего уровня, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-288">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="2b16d-289">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="2b16d-289">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2b16d-290">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="2b16d-290">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="2b16d-291">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-291">Int32</span></span>|<span data-ttu-id="2b16d-292">Минимальный # символов, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-292">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="2b16d-293">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="2b16d-293">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2b16d-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2b16d-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2b16d-295">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-295">Int32</span></span>|<span data-ttu-id="2b16d-296">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="2b16d-296">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2b16d-297">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2b16d-297">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2b16d-298">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-298">Int32</span></span>|<span data-ttu-id="2b16d-299">Количество предыдущих паролей профилей работы для блокировки.</span><span class="sxs-lookup"><span data-stu-id="2b16d-299">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="2b16d-300">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="2b16d-300">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2b16d-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2b16d-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2b16d-302">Int32</span><span class="sxs-lookup"><span data-stu-id="2b16d-302">Int32</span></span>|<span data-ttu-id="2b16d-303">Количество входов в сбои, разрешенные до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="2b16d-303">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="2b16d-304">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="2b16d-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2b16d-305">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2b16d-305">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="2b16d-306">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2b16d-306">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="2b16d-307">Тип необходимого пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-307">Type of work profile password that is required.</span></span> <span data-ttu-id="2b16d-308">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="2b16d-308">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="2b16d-309">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="2b16d-309">workProfileRequirePassword</span></span>|<span data-ttu-id="2b16d-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-310">Boolean</span></span>|<span data-ttu-id="2b16d-311">Пароль требуется или не требуется для профиля работы</span><span class="sxs-lookup"><span data-stu-id="2b16d-311">Password is required or not for work profile</span></span>|
|<span data-ttu-id="2b16d-312">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="2b16d-312">securityRequireVerifyApps</span></span>|<span data-ttu-id="2b16d-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-313">Boolean</span></span>|<span data-ttu-id="2b16d-314">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="2b16d-314">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="2b16d-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="2b16d-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="2b16d-316">Строка</span><span class="sxs-lookup"><span data-stu-id="2b16d-316">String</span></span>|<span data-ttu-id="2b16d-317">Включить режим блокировки для всегда на VPN.</span><span class="sxs-lookup"><span data-stu-id="2b16d-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="2b16d-318">VPNEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="2b16d-318">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="2b16d-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-319">Boolean</span></span>|<span data-ttu-id="2b16d-320">Включить режим блокировки для всегда на VPN.</span><span class="sxs-lookup"><span data-stu-id="2b16d-320">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="2b16d-321">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="2b16d-321">workProfileAllowWidgets</span></span>|<span data-ttu-id="2b16d-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-322">Boolean</span></span>|<span data-ttu-id="2b16d-323">Разрешить виджеты из приложений профиля работы.</span><span class="sxs-lookup"><span data-stu-id="2b16d-323">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="2b16d-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="2b16d-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="2b16d-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b16d-325">Boolean</span></span>|<span data-ttu-id="2b16d-326">Предотвращение установок приложений из неизвестных источников в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="2b16d-326">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="2b16d-327">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b16d-327">Response</span></span>
<span data-ttu-id="2b16d-328">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2b16d-328">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b16d-329">Пример</span><span class="sxs-lookup"><span data-stu-id="2b16d-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b16d-330">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b16d-330">Request</span></span>
<span data-ttu-id="2b16d-331">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b16d-331">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2b16d-332">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b16d-332">Response</span></span>
<span data-ttu-id="2b16d-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2b16d-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




