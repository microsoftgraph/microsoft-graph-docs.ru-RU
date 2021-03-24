---
title: Создание androidWorkProfileGeneralDeviceConfiguration
description: Создайте новый объект AndroidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 544823c73a25c940266997546e66c3a47f450c02
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148143"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="3f0d7-103">Создание androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3f0d7-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="3f0d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f0d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f0d7-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f0d7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f0d7-107">Создайте новый [объект AndroidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3f0d7-107">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f0d7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3f0d7-108">Prerequisites</span></span>
<span data-ttu-id="3f0d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f0d7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f0d7-111">Permission type</span></span>|<span data-ttu-id="3f0d7-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f0d7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f0d7-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f0d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f0d7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f0d7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f0d7-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f0d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f0d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-116">Not supported.</span></span>|
|<span data-ttu-id="3f0d7-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3f0d7-117">Application</span></span>|<span data-ttu-id="3f0d7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f0d7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f0d7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f0d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3f0d7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3f0d7-120">Request headers</span></span>
|<span data-ttu-id="3f0d7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f0d7-121">Header</span></span>|<span data-ttu-id="3f0d7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3f0d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f0d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f0d7-123">Authorization</span></span>|<span data-ttu-id="3f0d7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f0d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f0d7-125">Accept</span></span>|<span data-ttu-id="3f0d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f0d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f0d7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f0d7-127">Request body</span></span>
<span data-ttu-id="3f0d7-128">В теле запроса предоставляем представление JSON для объекта AndroidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-128">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="3f0d7-129">В следующей таблице показаны свойства, необходимые при создании androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-129">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="3f0d7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f0d7-130">Property</span></span>|<span data-ttu-id="3f0d7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3f0d7-131">Type</span></span>|<span data-ttu-id="3f0d7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3f0d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f0d7-133">id</span><span class="sxs-lookup"><span data-stu-id="3f0d7-133">id</span></span>|<span data-ttu-id="3f0d7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3f0d7-134">String</span></span>|<span data-ttu-id="3f0d7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-135">Key of the entity.</span></span> <span data-ttu-id="3f0d7-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f0d7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f0d7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3f0d7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f0d7-138">DateTimeOffset</span></span>|<span data-ttu-id="3f0d7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3f0d7-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f0d7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3f0d7-141">roleScopeTagIds</span></span>|<span data-ttu-id="3f0d7-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3f0d7-142">String collection</span></span>|<span data-ttu-id="3f0d7-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3f0d7-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f0d7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3f0d7-145">supportsScopeTags</span></span>|<span data-ttu-id="3f0d7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-146">Boolean</span></span>|<span data-ttu-id="3f0d7-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3f0d7-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3f0d7-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3f0d7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-150">This property is read-only.</span></span> <span data-ttu-id="3f0d7-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f0d7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3f0d7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="3f0d7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="3f0d7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="3f0d7-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="3f0d7-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f0d7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3f0d7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="3f0d7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="3f0d7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="3f0d7-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="3f0d7-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f0d7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3f0d7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="3f0d7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="3f0d7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="3f0d7-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="3f0d7-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f0d7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f0d7-164">createdDateTime</span></span>|<span data-ttu-id="3f0d7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f0d7-165">DateTimeOffset</span></span>|<span data-ttu-id="3f0d7-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-166">DateTime the object was created.</span></span> <span data-ttu-id="3f0d7-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f0d7-168">description</span><span class="sxs-lookup"><span data-stu-id="3f0d7-168">description</span></span>|<span data-ttu-id="3f0d7-169">Строка</span><span class="sxs-lookup"><span data-stu-id="3f0d7-169">String</span></span>|<span data-ttu-id="3f0d7-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3f0d7-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f0d7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="3f0d7-172">displayName</span></span>|<span data-ttu-id="3f0d7-173">Строка</span><span class="sxs-lookup"><span data-stu-id="3f0d7-173">String</span></span>|<span data-ttu-id="3f0d7-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3f0d7-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f0d7-176">version</span><span class="sxs-lookup"><span data-stu-id="3f0d7-176">version</span></span>|<span data-ttu-id="3f0d7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-177">Int32</span></span>|<span data-ttu-id="3f0d7-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-178">Version of the device configuration.</span></span> <span data-ttu-id="3f0d7-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3f0d7-180">passwordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="3f0d7-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="3f0d7-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-181">Boolean</span></span>|<span data-ttu-id="3f0d7-182">Указывает, следует ли блокировать разблокирование лица.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="3f0d7-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="3f0d7-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="3f0d7-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-184">Boolean</span></span>|<span data-ttu-id="3f0d7-185">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="3f0d7-186">passwordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="3f0d7-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="3f0d7-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-187">Boolean</span></span>|<span data-ttu-id="3f0d7-188">Указывает, следует ли блокировать разблокировку радужной оболочки радужной оболочки.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="3f0d7-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="3f0d7-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="3f0d7-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-190">Boolean</span></span>|<span data-ttu-id="3f0d7-191">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="3f0d7-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3f0d7-192">passwordExpirationDays</span></span>|<span data-ttu-id="3f0d7-193">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-193">Int32</span></span>|<span data-ttu-id="3f0d7-194">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-194">Number of days before the password expires.</span></span> <span data-ttu-id="3f0d7-195">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="3f0d7-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3f0d7-196">passwordMinimumLength</span></span>|<span data-ttu-id="3f0d7-197">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-197">Int32</span></span>|<span data-ttu-id="3f0d7-198">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-198">Minimum length of passwords.</span></span> <span data-ttu-id="3f0d7-199">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3f0d7-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="3f0d7-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="3f0d7-201">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-201">Int32</span></span>|<span data-ttu-id="3f0d7-202">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="3f0d7-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3f0d7-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3f0d7-204">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-204">Int32</span></span>|<span data-ttu-id="3f0d7-205">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-205">Number of previous passwords to block.</span></span> <span data-ttu-id="3f0d7-206">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="3f0d7-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="3f0d7-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="3f0d7-208">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-208">Int32</span></span>|<span data-ttu-id="3f0d7-209">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="3f0d7-210">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="3f0d7-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f0d7-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3f0d7-211">passwordRequiredType</span></span>|[<span data-ttu-id="3f0d7-212">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3f0d7-212">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="3f0d7-213">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-213">Type of password that is required.</span></span> <span data-ttu-id="3f0d7-214">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="3f0d7-215">workProfileAllowAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="3f0d7-215">workProfileAllowAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="3f0d7-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-216">Boolean</span></span>|<span data-ttu-id="3f0d7-217">Указывает, следует ли разрешить установку приложений из неизвестных источников.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-217">Indicates whether to allow installation of apps from unknown sources.</span></span>|
|<span data-ttu-id="3f0d7-218">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="3f0d7-218">workProfileDataSharingType</span></span>|[<span data-ttu-id="3f0d7-219">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="3f0d7-219">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="3f0d7-220">Тип разрешенного обмена данными.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-220">Type of data sharing that is allowed.</span></span> <span data-ttu-id="3f0d7-221">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-221">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="3f0d7-222">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="3f0d7-222">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="3f0d7-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-223">Boolean</span></span>|<span data-ttu-id="3f0d7-224">Указывает, следует ли блокировать уведомления во время блокировки устройства.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-224">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="3f0d7-225">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="3f0d7-225">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="3f0d7-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-226">Boolean</span></span>|<span data-ttu-id="3f0d7-227">Блокировать добавление и удаление учетных записей в профиле работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-227">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="3f0d7-228">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="3f0d7-228">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="3f0d7-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-229">Boolean</span></span>|<span data-ttu-id="3f0d7-230">Разрешить устройствам Bluetooth доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-230">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="3f0d7-231">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="3f0d7-231">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="3f0d7-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-232">Boolean</span></span>|<span data-ttu-id="3f0d7-233">Блокировка захвата экрана в профиле работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-233">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="3f0d7-234">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="3f0d7-234">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="3f0d7-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-235">Boolean</span></span>|<span data-ttu-id="3f0d7-236">Блокировка ИД вызываемой личности вызываемой на экране работы в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-236">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="3f0d7-237">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="3f0d7-237">workProfileBlockCamera</span></span>|<span data-ttu-id="3f0d7-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-238">Boolean</span></span>|<span data-ttu-id="3f0d7-239">Блокировка камеры профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-239">Block work profile camera.</span></span>|
|<span data-ttu-id="3f0d7-240">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="3f0d7-240">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="3f0d7-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-241">Boolean</span></span>|<span data-ttu-id="3f0d7-242">Блокировка доступности контактов профилей работы в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-242">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="3f0d7-243">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="3f0d7-243">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="3f0d7-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-244">Boolean</span></span>|<span data-ttu-id="3f0d7-245">Boolean, который указывает, включен ли параметр, который не позволяет копировать/вклеить перекрестный профиль.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-245">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="3f0d7-246">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="3f0d7-246">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="3f0d7-247">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="3f0d7-247">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="3f0d7-248">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-248">Type of password that is required.</span></span> <span data-ttu-id="3f0d7-249">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-249">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="3f0d7-250">workProfilePasswordBlockFaceUnlock</span><span class="sxs-lookup"><span data-stu-id="3f0d7-250">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="3f0d7-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-251">Boolean</span></span>|<span data-ttu-id="3f0d7-252">Указывает, следует ли блокировать разблокировку лица для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-252">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="3f0d7-253">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="3f0d7-253">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="3f0d7-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-254">Boolean</span></span>|<span data-ttu-id="3f0d7-255">Указывает, следует ли блокировать разблокировку отпечатков пальцев для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-255">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="3f0d7-256">workProfilePasswordBlockIrisUnlock</span><span class="sxs-lookup"><span data-stu-id="3f0d7-256">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="3f0d7-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-257">Boolean</span></span>|<span data-ttu-id="3f0d7-258">Указывает, следует ли блокировать разблокировку радужной оболочки радужной оболочки для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-258">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="3f0d7-259">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="3f0d7-259">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="3f0d7-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-260">Boolean</span></span>|<span data-ttu-id="3f0d7-261">Указывает, следует ли блокировать Smart Lock и другие агенты доверия для профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-261">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="3f0d7-262">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3f0d7-262">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="3f0d7-263">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-263">Int32</span></span>|<span data-ttu-id="3f0d7-264">Количество дней до истечения срока действия пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-264">Number of days before the work profile password expires.</span></span> <span data-ttu-id="3f0d7-265">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-265">Valid values 1 to 365</span></span>|
|<span data-ttu-id="3f0d7-266">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3f0d7-266">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="3f0d7-267">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-267">Int32</span></span>|<span data-ttu-id="3f0d7-268">Минимальная длина пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-268">Minimum length of work profile password.</span></span> <span data-ttu-id="3f0d7-269">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-269">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3f0d7-270">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="3f0d7-270">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="3f0d7-271">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-271">Int32</span></span>|<span data-ttu-id="3f0d7-272">Минимум # числимые символы, необходимые в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-272">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="3f0d7-273">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="3f0d7-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="3f0d7-274">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="3f0d7-274">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="3f0d7-275">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-275">Int32</span></span>|<span data-ttu-id="3f0d7-276">Минимальное количество символов без букв, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-276">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="3f0d7-277">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="3f0d7-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="3f0d7-278">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="3f0d7-278">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="3f0d7-279">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-279">Int32</span></span>|<span data-ttu-id="3f0d7-280">Минимальный # буквы символов, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-280">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="3f0d7-281">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="3f0d7-281">Valid values 1 to 10</span></span>|
|<span data-ttu-id="3f0d7-282">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="3f0d7-282">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="3f0d7-283">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-283">Int32</span></span>|<span data-ttu-id="3f0d7-284">Минимальное количество символов нижнего уровня, необходимых для пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-284">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="3f0d7-285">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="3f0d7-285">Valid values 1 to 10</span></span>|
|<span data-ttu-id="3f0d7-286">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="3f0d7-286">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="3f0d7-287">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-287">Int32</span></span>|<span data-ttu-id="3f0d7-288">Минимальный # символов верхнего уровня, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-288">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="3f0d7-289">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="3f0d7-289">Valid values 1 to 10</span></span>|
|<span data-ttu-id="3f0d7-290">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="3f0d7-290">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="3f0d7-291">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-291">Int32</span></span>|<span data-ttu-id="3f0d7-292">Минимальный # символов, необходимых в пароле профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-292">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="3f0d7-293">Допустимые значения от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="3f0d7-293">Valid values 1 to 10</span></span>|
|<span data-ttu-id="3f0d7-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="3f0d7-294">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="3f0d7-295">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-295">Int32</span></span>|<span data-ttu-id="3f0d7-296">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="3f0d7-296">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="3f0d7-297">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3f0d7-297">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3f0d7-298">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-298">Int32</span></span>|<span data-ttu-id="3f0d7-299">Количество предыдущих паролей профилей работы для блокировки.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-299">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="3f0d7-300">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-300">Valid values 0 to 24</span></span>|
|<span data-ttu-id="3f0d7-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="3f0d7-301">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="3f0d7-302">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d7-302">Int32</span></span>|<span data-ttu-id="3f0d7-303">Количество входов в сбои, разрешенные до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-303">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="3f0d7-304">Допустимые значения от 1 до 16</span><span class="sxs-lookup"><span data-stu-id="3f0d7-304">Valid values 1 to 16</span></span>|
|<span data-ttu-id="3f0d7-305">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3f0d7-305">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="3f0d7-306">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3f0d7-306">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="3f0d7-307">Тип необходимого пароля профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-307">Type of work profile password that is required.</span></span> <span data-ttu-id="3f0d7-308">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-308">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="3f0d7-309">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="3f0d7-309">workProfileRequirePassword</span></span>|<span data-ttu-id="3f0d7-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-310">Boolean</span></span>|<span data-ttu-id="3f0d7-311">Пароль требуется или не требуется для профиля работы</span><span class="sxs-lookup"><span data-stu-id="3f0d7-311">Password is required or not for work profile</span></span>|
|<span data-ttu-id="3f0d7-312">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="3f0d7-312">securityRequireVerifyApps</span></span>|<span data-ttu-id="3f0d7-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-313">Boolean</span></span>|<span data-ttu-id="3f0d7-314">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-314">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="3f0d7-315">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="3f0d7-315">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="3f0d7-316">Строка</span><span class="sxs-lookup"><span data-stu-id="3f0d7-316">String</span></span>|<span data-ttu-id="3f0d7-317">Включить режим блокировки для всегда на VPN.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="3f0d7-318">VPNEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="3f0d7-318">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="3f0d7-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-319">Boolean</span></span>|<span data-ttu-id="3f0d7-320">Включить режим блокировки для всегда на VPN.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-320">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="3f0d7-321">workProfileAllowWidgets</span><span class="sxs-lookup"><span data-stu-id="3f0d7-321">workProfileAllowWidgets</span></span>|<span data-ttu-id="3f0d7-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-322">Boolean</span></span>|<span data-ttu-id="3f0d7-323">Разрешить виджеты из приложений профиля работы.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-323">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="3f0d7-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="3f0d7-324">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="3f0d7-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f0d7-325">Boolean</span></span>|<span data-ttu-id="3f0d7-326">Предотвращение установок приложений из неизвестных источников в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-326">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="3f0d7-327">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f0d7-327">Response</span></span>
<span data-ttu-id="3f0d7-328">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект AndroidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-328">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f0d7-329">Пример</span><span class="sxs-lookup"><span data-stu-id="3f0d7-329">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f0d7-330">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f0d7-330">Request</span></span>
<span data-ttu-id="3f0d7-331">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-331">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3f0d7-332">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f0d7-332">Response</span></span>
<span data-ttu-id="3f0d7-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f0d7-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




