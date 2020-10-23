---
title: Создание androidForWorkGeneralDeviceConfiguration
description: Создание нового объекта androidForWorkGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 63f7b1a25d2d0768ef1578016f8207aaa52bff41
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703442"
---
# <a name="create-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="c3bc7-103">Создание androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c3bc7-103">Create androidForWorkGeneralDeviceConfiguration</span></span>

<span data-ttu-id="c3bc7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3bc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3bc7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3bc7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3bc7-107">Создание нового объекта [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c3bc7-107">Create a new [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3bc7-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c3bc7-108">Prerequisites</span></span>
<span data-ttu-id="c3bc7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3bc7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3bc7-111">Permission type</span></span>|<span data-ttu-id="c3bc7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3bc7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3bc7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3bc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3bc7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3bc7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3bc7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3bc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3bc7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-116">Not supported.</span></span>|
|<span data-ttu-id="c3bc7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3bc7-117">Application</span></span>|<span data-ttu-id="c3bc7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3bc7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3bc7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3bc7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c3bc7-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c3bc7-120">Request headers</span></span>
|<span data-ttu-id="c3bc7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3bc7-121">Header</span></span>|<span data-ttu-id="c3bc7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3bc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3bc7-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3bc7-123">Authorization</span></span>|<span data-ttu-id="c3bc7-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3bc7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3bc7-125">Accept</span></span>|<span data-ttu-id="c3bc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3bc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3bc7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3bc7-127">Request body</span></span>
<span data-ttu-id="c3bc7-128">В тексте запроса добавьте представление объекта androidForWorkGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-128">In the request body, supply a JSON representation for the androidForWorkGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="c3bc7-129">В следующей таблице приведены свойства, необходимые при создании androidForWorkGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-129">The following table shows the properties that are required when you create the androidForWorkGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="c3bc7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3bc7-130">Property</span></span>|<span data-ttu-id="c3bc7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c3bc7-131">Type</span></span>|<span data-ttu-id="c3bc7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c3bc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3bc7-133">id</span><span class="sxs-lookup"><span data-stu-id="c3bc7-133">id</span></span>|<span data-ttu-id="c3bc7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c3bc7-134">String</span></span>|<span data-ttu-id="c3bc7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-135">Key of the entity.</span></span> <span data-ttu-id="c3bc7-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bc7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3bc7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c3bc7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3bc7-138">DateTimeOffset</span></span>|<span data-ttu-id="c3bc7-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c3bc7-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bc7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c3bc7-141">roleScopeTagIds</span></span>|<span data-ttu-id="c3bc7-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c3bc7-142">String collection</span></span>|<span data-ttu-id="c3bc7-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c3bc7-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bc7-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c3bc7-145">supportsScopeTags</span></span>|<span data-ttu-id="c3bc7-146">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-146">Boolean</span></span>|<span data-ttu-id="c3bc7-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c3bc7-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c3bc7-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c3bc7-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-150">This property is read-only.</span></span> <span data-ttu-id="c3bc7-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bc7-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c3bc7-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c3bc7-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c3bc7-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c3bc7-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c3bc7-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bc7-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c3bc7-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c3bc7-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c3bc7-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c3bc7-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c3bc7-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bc7-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c3bc7-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c3bc7-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="c3bc7-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c3bc7-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c3bc7-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bc7-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3bc7-164">createdDateTime</span></span>|<span data-ttu-id="c3bc7-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3bc7-165">DateTimeOffset</span></span>|<span data-ttu-id="c3bc7-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-166">DateTime the object was created.</span></span> <span data-ttu-id="c3bc7-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bc7-168">description</span><span class="sxs-lookup"><span data-stu-id="c3bc7-168">description</span></span>|<span data-ttu-id="c3bc7-169">Строка</span><span class="sxs-lookup"><span data-stu-id="c3bc7-169">String</span></span>|<span data-ttu-id="c3bc7-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c3bc7-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bc7-172">displayName</span><span class="sxs-lookup"><span data-stu-id="c3bc7-172">displayName</span></span>|<span data-ttu-id="c3bc7-173">Строка</span><span class="sxs-lookup"><span data-stu-id="c3bc7-173">String</span></span>|<span data-ttu-id="c3bc7-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c3bc7-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bc7-176">version</span><span class="sxs-lookup"><span data-stu-id="c3bc7-176">version</span></span>|<span data-ttu-id="c3bc7-177">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-177">Int32</span></span>|<span data-ttu-id="c3bc7-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-178">Version of the device configuration.</span></span> <span data-ttu-id="c3bc7-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c3bc7-180">пассвордблоккфацеунлокк</span><span class="sxs-lookup"><span data-stu-id="c3bc7-180">passwordBlockFaceUnlock</span></span>|<span data-ttu-id="c3bc7-181">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-181">Boolean</span></span>|<span data-ttu-id="c3bc7-182">Указывает, следует ли заблокировать разблокировку лица.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-182">Indicates whether or not to block face unlock.</span></span>|
|<span data-ttu-id="c3bc7-183">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c3bc7-183">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c3bc7-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3bc7-184">Boolean</span></span>|<span data-ttu-id="c3bc7-185">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-185">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="c3bc7-186">пассвордблоккирисунлокк</span><span class="sxs-lookup"><span data-stu-id="c3bc7-186">passwordBlockIrisUnlock</span></span>|<span data-ttu-id="c3bc7-187">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-187">Boolean</span></span>|<span data-ttu-id="c3bc7-188">Указывает, следует ли заблокировать разблокировку IRI.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-188">Indicates whether or not to block iris unlock.</span></span>|
|<span data-ttu-id="c3bc7-189">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="c3bc7-189">passwordBlockTrustAgents</span></span>|<span data-ttu-id="c3bc7-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3bc7-190">Boolean</span></span>|<span data-ttu-id="c3bc7-191">Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-191">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="c3bc7-192">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c3bc7-192">passwordExpirationDays</span></span>|<span data-ttu-id="c3bc7-193">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-193">Int32</span></span>|<span data-ttu-id="c3bc7-194">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-194">Number of days before the password expires.</span></span> <span data-ttu-id="c3bc7-195">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-195">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c3bc7-196">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c3bc7-196">passwordMinimumLength</span></span>|<span data-ttu-id="c3bc7-197">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-197">Int32</span></span>|<span data-ttu-id="c3bc7-198">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-198">Minimum length of passwords.</span></span> <span data-ttu-id="c3bc7-199">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-199">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c3bc7-200">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c3bc7-200">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c3bc7-201">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-201">Int32</span></span>|<span data-ttu-id="c3bc7-202">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-202">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c3bc7-203">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c3bc7-203">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c3bc7-204">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-204">Int32</span></span>|<span data-ttu-id="c3bc7-205">Количество предыдущих паролей, которые следует заблокировать.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-205">Number of previous passwords to block.</span></span> <span data-ttu-id="c3bc7-206">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-206">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c3bc7-207">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c3bc7-207">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c3bc7-208">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-208">Int32</span></span>|<span data-ttu-id="c3bc7-209">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-209">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="c3bc7-210">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-210">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c3bc7-211">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c3bc7-211">passwordRequiredType</span></span>|[<span data-ttu-id="c3bc7-212">андроидфорворкрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c3bc7-212">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="c3bc7-213">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-213">Type of password that is required.</span></span> <span data-ttu-id="c3bc7-214">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-214">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="c3bc7-215">воркпрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="c3bc7-215">workProfileDataSharingType</span></span>|[<span data-ttu-id="c3bc7-216">андроидфорворккросспрофиледаташарингтипе</span><span class="sxs-lookup"><span data-stu-id="c3bc7-216">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="c3bc7-217">Тип разрешенного общего доступа к данным.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-217">Type of data sharing that is allowed.</span></span> <span data-ttu-id="c3bc7-218">Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-218">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="c3bc7-219">воркпрофилеблоккнотификатионсвхиледевицелоккед</span><span class="sxs-lookup"><span data-stu-id="c3bc7-219">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="c3bc7-220">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-220">Boolean</span></span>|<span data-ttu-id="c3bc7-221">Указывает, следует ли блокировать уведомления, когда устройство заблокировано.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-221">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="c3bc7-222">воркпрофилеблоккаддингаккаунтс</span><span class="sxs-lookup"><span data-stu-id="c3bc7-222">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="c3bc7-223">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-223">Boolean</span></span>|<span data-ttu-id="c3bc7-224">Запретить пользователям добавлять и удалять учетные записи в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-224">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="c3bc7-225">воркпрофилеблуетусенаблеконтактшаринг</span><span class="sxs-lookup"><span data-stu-id="c3bc7-225">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="c3bc7-226">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-226">Boolean</span></span>|<span data-ttu-id="c3bc7-227">Разрешить устройствам Bluetooth получать доступ к корпоративным контактам.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-227">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="c3bc7-228">воркпрофилеблоккскринкаптуре</span><span class="sxs-lookup"><span data-stu-id="c3bc7-228">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="c3bc7-229">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-229">Boolean</span></span>|<span data-ttu-id="c3bc7-230">Блокировать снимок экрана в рабочем профиле.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-230">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="c3bc7-231">воркпрофилеблокккросспрофилекаллерид</span><span class="sxs-lookup"><span data-stu-id="c3bc7-231">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="c3bc7-232">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-232">Boolean</span></span>|<span data-ttu-id="c3bc7-233">Блокировать отображение идентификатора исполнителя рабочего профиля в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-233">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="c3bc7-234">Свойства workprofileblockcamera</span><span class="sxs-lookup"><span data-stu-id="c3bc7-234">workProfileBlockCamera</span></span>|<span data-ttu-id="c3bc7-235">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-235">Boolean</span></span>|<span data-ttu-id="c3bc7-236">Блокировать камеру рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-236">Block work profile camera.</span></span>|
|<span data-ttu-id="c3bc7-237">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="c3bc7-237">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="c3bc7-238">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-238">Boolean</span></span>|<span data-ttu-id="c3bc7-239">Блокировать доступность контактов для рабочих профилей в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-239">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="c3bc7-240">воркпрофилеблокккросспрофилекопипасте</span><span class="sxs-lookup"><span data-stu-id="c3bc7-240">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="c3bc7-241">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-241">Boolean</span></span>|<span data-ttu-id="c3bc7-242">Логическое значение, которое указывает, включено ли для параметра возможность копирования и вставки в нескольких профилях.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-242">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="c3bc7-243">воркпрофиледефаултапппермиссионполици</span><span class="sxs-lookup"><span data-stu-id="c3bc7-243">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="c3bc7-244">андроидфорворкдефаултапппермиссионполицитипе</span><span class="sxs-lookup"><span data-stu-id="c3bc7-244">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="c3bc7-245">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-245">Type of password that is required.</span></span> <span data-ttu-id="c3bc7-246">Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-246">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="c3bc7-247">воркпрофилепассвордблоккфацеунлокк</span><span class="sxs-lookup"><span data-stu-id="c3bc7-247">workProfilePasswordBlockFaceUnlock</span></span>|<span data-ttu-id="c3bc7-248">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-248">Boolean</span></span>|<span data-ttu-id="c3bc7-249">Указывает, следует ли заблокировать разблокировку лица для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-249">Indicates whether or not to block face unlock for work profile.</span></span>|
|<span data-ttu-id="c3bc7-250">Свойства workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="c3bc7-250">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c3bc7-251">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-251">Boolean</span></span>|<span data-ttu-id="c3bc7-252">Указывает, следует ли заблокировать разблокировку отпечатков пальцев для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-252">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="c3bc7-253">воркпрофилепассвордблоккирисунлокк</span><span class="sxs-lookup"><span data-stu-id="c3bc7-253">workProfilePasswordBlockIrisUnlock</span></span>|<span data-ttu-id="c3bc7-254">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-254">Boolean</span></span>|<span data-ttu-id="c3bc7-255">Указывает, следует ли заблокировать разблокировку IRI для рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-255">Indicates whether or not to block iris unlock for work profile.</span></span>|
|<span data-ttu-id="c3bc7-256">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="c3bc7-256">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="c3bc7-257">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-257">Boolean</span></span>|<span data-ttu-id="c3bc7-258">Указывает, следует ли заблокировать для рабочего профиля интеллектуальную блокировку и другие агенты доверия.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-258">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="c3bc7-259">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c3bc7-259">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="c3bc7-260">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-260">Int32</span></span>|<span data-ttu-id="c3bc7-261">Количество дней до истечения срока действия пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-261">Number of days before the work profile password expires.</span></span> <span data-ttu-id="c3bc7-262">Допустимые значения: от 1 до 365.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-262">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c3bc7-263">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c3bc7-263">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="c3bc7-264">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-264">Int32</span></span>|<span data-ttu-id="c3bc7-265">Минимальная длина пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-265">Minimum length of work profile password.</span></span> <span data-ttu-id="c3bc7-266">Допустимые значения: от 4 до 16.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-266">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c3bc7-267">воркпрофилепассвордминнумерикчарактерс</span><span class="sxs-lookup"><span data-stu-id="c3bc7-267">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="c3bc7-268">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-268">Int32</span></span>|<span data-ttu-id="c3bc7-269">Минимальное количество числовых символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-269">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="c3bc7-270">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="c3bc7-270">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c3bc7-271">воркпрофилепассвордминнонлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="c3bc7-271">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="c3bc7-272">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-272">Int32</span></span>|<span data-ttu-id="c3bc7-273">Минимальное количество небуквенных символов, необходимых в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-273">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="c3bc7-274">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="c3bc7-274">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c3bc7-275">воркпрофилепассвордминлеттерчарактерс</span><span class="sxs-lookup"><span data-stu-id="c3bc7-275">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="c3bc7-276">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-276">Int32</span></span>|<span data-ttu-id="c3bc7-277">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-277">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="c3bc7-278">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="c3bc7-278">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c3bc7-279">воркпрофилепассвордминловеркасечарактерс</span><span class="sxs-lookup"><span data-stu-id="c3bc7-279">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="c3bc7-280">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-280">Int32</span></span>|<span data-ttu-id="c3bc7-281">Минимальное количество символов нижнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-281">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="c3bc7-282">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="c3bc7-282">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c3bc7-283">воркпрофилепассвордминупперкасечарактерс</span><span class="sxs-lookup"><span data-stu-id="c3bc7-283">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="c3bc7-284">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-284">Int32</span></span>|<span data-ttu-id="c3bc7-285">Минимальное количество символов верхнего регистра в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-285">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="c3bc7-286">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="c3bc7-286">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c3bc7-287">воркпрофилепассвордминсимболчарактерс</span><span class="sxs-lookup"><span data-stu-id="c3bc7-287">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="c3bc7-288">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-288">Int32</span></span>|<span data-ttu-id="c3bc7-289">Минимальное количество символов в пароле рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-289">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="c3bc7-290">Допустимые значения — от 1 до 10</span><span class="sxs-lookup"><span data-stu-id="c3bc7-290">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c3bc7-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c3bc7-291">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c3bc7-292">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-292">Int32</span></span>|<span data-ttu-id="c3bc7-293">Время с момента последнего действия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="c3bc7-293">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c3bc7-294">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c3bc7-294">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c3bc7-295">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-295">Int32</span></span>|<span data-ttu-id="c3bc7-296">Число паролей предыдущих рабочих профилей, которые необходимо заблокировать.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-296">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="c3bc7-297">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-297">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c3bc7-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c3bc7-298">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c3bc7-299">Int32</span><span class="sxs-lookup"><span data-stu-id="c3bc7-299">Int32</span></span>|<span data-ttu-id="c3bc7-300">Количество неудачных попыток входа, разрешенных до удаления профиля работы и удаления всех корпоративных данных.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-300">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="c3bc7-301">Допустимые значения — от 1 до 16.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-301">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c3bc7-302">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c3bc7-302">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="c3bc7-303">андроидфорворкрекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c3bc7-303">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="c3bc7-304">Тип требуемого пароля рабочего профиля.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-304">Type of work profile password that is required.</span></span> <span data-ttu-id="c3bc7-305">Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-305">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="c3bc7-306">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="c3bc7-306">workProfileRequirePassword</span></span>|<span data-ttu-id="c3bc7-307">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-307">Boolean</span></span>|<span data-ttu-id="c3bc7-308">Пароль обязателен или не для рабочего профиля</span><span class="sxs-lookup"><span data-stu-id="c3bc7-308">Password is required or not for work profile</span></span>|
|<span data-ttu-id="c3bc7-309">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c3bc7-309">securityRequireVerifyApps</span></span>|<span data-ttu-id="c3bc7-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3bc7-310">Boolean</span></span>|<span data-ttu-id="c3bc7-311">Указывает, что требуется включить функцию проверки приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-311">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="c3bc7-312">Свойства vpnalwaysonpackageidentifier</span><span class="sxs-lookup"><span data-stu-id="c3bc7-312">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="c3bc7-313">Строка</span><span class="sxs-lookup"><span data-stu-id="c3bc7-313">String</span></span>|<span data-ttu-id="c3bc7-314">Включение режима блокировки для постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-314">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="c3bc7-315">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="c3bc7-315">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="c3bc7-316">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-316">Boolean</span></span>|<span data-ttu-id="c3bc7-317">Включение режима блокировки для постоянного подключения VPN.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-317">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="c3bc7-318">воркпрофилеалловвиджетс</span><span class="sxs-lookup"><span data-stu-id="c3bc7-318">workProfileAllowWidgets</span></span>|<span data-ttu-id="c3bc7-319">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-319">Boolean</span></span>|<span data-ttu-id="c3bc7-320">Разрешить графические элементы из приложений профилей рабочих приложений.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-320">Allow widgets from work profile apps.</span></span>|
|<span data-ttu-id="c3bc7-321">воркпрофилеблоккперсоналаппинсталлсфромункновнсаурцес</span><span class="sxs-lookup"><span data-stu-id="c3bc7-321">workProfileBlockPersonalAppInstallsFromUnknownSources</span></span>|<span data-ttu-id="c3bc7-322">Логический</span><span class="sxs-lookup"><span data-stu-id="c3bc7-322">Boolean</span></span>|<span data-ttu-id="c3bc7-323">Запретить установку приложений из неизвестных источников в личном профиле.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-323">Prevent app installations from unknown sources in the personal profile.</span></span>|



## <a name="response"></a><span data-ttu-id="c3bc7-324">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3bc7-324">Response</span></span>
<span data-ttu-id="c3bc7-325">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-325">If successful, this method returns a `201 Created` response code and a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3bc7-326">Пример</span><span class="sxs-lookup"><span data-stu-id="c3bc7-326">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3bc7-327">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3bc7-327">Request</span></span>
<span data-ttu-id="c3bc7-328">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-328">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3079

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="c3bc7-329">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3bc7-329">Response</span></span>
<span data-ttu-id="c3bc7-p131">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3bc7-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3251

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "id": "a931a366-a366-a931-66a3-31a966a331a9",
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





