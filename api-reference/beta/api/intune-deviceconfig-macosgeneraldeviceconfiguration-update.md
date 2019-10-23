---
title: Update macOSGeneralDeviceConfiguration
description: Обновление свойств объекта macOSGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e37e0375a6ff3214484ac96de0c5baa352f2f08d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533583"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="cb25c-103">Update macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="cb25c-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="cb25c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb25c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb25c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb25c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb25c-106">Обновление свойств объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb25c-106">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb25c-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cb25c-107">Prerequisites</span></span>
<span data-ttu-id="cb25c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb25c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb25c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb25c-110">Permission type</span></span>|<span data-ttu-id="cb25c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb25c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb25c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb25c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb25c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb25c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cb25c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb25c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb25c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb25c-115">Not supported.</span></span>|
|<span data-ttu-id="cb25c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb25c-116">Application</span></span>|<span data-ttu-id="cb25c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb25c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb25c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb25c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cb25c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cb25c-119">Request headers</span></span>
|<span data-ttu-id="cb25c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb25c-120">Header</span></span>|<span data-ttu-id="cb25c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cb25c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb25c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb25c-122">Authorization</span></span>|<span data-ttu-id="cb25c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb25c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb25c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cb25c-124">Accept</span></span>|<span data-ttu-id="cb25c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cb25c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb25c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb25c-126">Request body</span></span>
<span data-ttu-id="cb25c-127">В теле запроса добавьте представление объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb25c-127">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="cb25c-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb25c-128">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="cb25c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb25c-129">Property</span></span>|<span data-ttu-id="cb25c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cb25c-130">Type</span></span>|<span data-ttu-id="cb25c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cb25c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb25c-132">id</span><span class="sxs-lookup"><span data-stu-id="cb25c-132">id</span></span>|<span data-ttu-id="cb25c-133">String</span><span class="sxs-lookup"><span data-stu-id="cb25c-133">String</span></span>|<span data-ttu-id="cb25c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cb25c-134">Key of the entity.</span></span> <span data-ttu-id="cb25c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb25c-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb25c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb25c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cb25c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb25c-137">DateTimeOffset</span></span>|<span data-ttu-id="cb25c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cb25c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="cb25c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb25c-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb25c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cb25c-140">roleScopeTagIds</span></span>|<span data-ttu-id="cb25c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cb25c-141">String collection</span></span>|<span data-ttu-id="cb25c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="cb25c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cb25c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb25c-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb25c-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="cb25c-144">supportsScopeTags</span></span>|<span data-ttu-id="cb25c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-145">Boolean</span></span>|<span data-ttu-id="cb25c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="cb25c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cb25c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="cb25c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cb25c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="cb25c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cb25c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb25c-149">This property is read-only.</span></span> <span data-ttu-id="cb25c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb25c-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb25c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cb25c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="cb25c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="cb25c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="cb25c-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cb25c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="cb25c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb25c-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb25c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cb25c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="cb25c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="cb25c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="cb25c-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cb25c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="cb25c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb25c-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb25c-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cb25c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="cb25c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="cb25c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="cb25c-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="cb25c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="cb25c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb25c-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb25c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb25c-163">createdDateTime</span></span>|<span data-ttu-id="cb25c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb25c-164">DateTimeOffset</span></span>|<span data-ttu-id="cb25c-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cb25c-165">DateTime the object was created.</span></span> <span data-ttu-id="cb25c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb25c-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb25c-167">description</span><span class="sxs-lookup"><span data-stu-id="cb25c-167">description</span></span>|<span data-ttu-id="cb25c-168">String</span><span class="sxs-lookup"><span data-stu-id="cb25c-168">String</span></span>|<span data-ttu-id="cb25c-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cb25c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cb25c-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb25c-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb25c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="cb25c-171">displayName</span></span>|<span data-ttu-id="cb25c-172">Строка</span><span class="sxs-lookup"><span data-stu-id="cb25c-172">String</span></span>|<span data-ttu-id="cb25c-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cb25c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cb25c-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cb25c-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb25c-175">version</span><span class="sxs-lookup"><span data-stu-id="cb25c-175">version</span></span>|<span data-ttu-id="cb25c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="cb25c-176">Int32</span></span>|<span data-ttu-id="cb25c-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cb25c-177">Version of the device configuration.</span></span> <span data-ttu-id="cb25c-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cb25c-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cb25c-179">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="cb25c-179">compliantAppsList</span></span>|<span data-ttu-id="cb25c-180">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="cb25c-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="cb25c-181">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="cb25c-181">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="cb25c-182">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="cb25c-182">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="cb25c-183">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="cb25c-183">compliantAppListType</span></span>|[<span data-ttu-id="cb25c-184">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="cb25c-184">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="cb25c-185">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="cb25c-185">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="cb25c-186">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="cb25c-186">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="cb25c-187">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="cb25c-187">emailInDomainSuffixes</span></span>|<span data-ttu-id="cb25c-188">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cb25c-188">String collection</span></span>|<span data-ttu-id="cb25c-189">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="cb25c-189">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="cb25c-190">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="cb25c-190">passwordBlockSimple</span></span>|<span data-ttu-id="cb25c-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-191">Boolean</span></span>|<span data-ttu-id="cb25c-192">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="cb25c-192">Block simple passwords.</span></span>|
|<span data-ttu-id="cb25c-193">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cb25c-193">passwordExpirationDays</span></span>|<span data-ttu-id="cb25c-194">Int32</span><span class="sxs-lookup"><span data-stu-id="cb25c-194">Int32</span></span>|<span data-ttu-id="cb25c-195">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="cb25c-195">Number of days before the password expires.</span></span>|
|<span data-ttu-id="cb25c-196">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="cb25c-196">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="cb25c-197">Int32</span><span class="sxs-lookup"><span data-stu-id="cb25c-197">Int32</span></span>|<span data-ttu-id="cb25c-198">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="cb25c-198">Number of character sets a password must contain.</span></span> <span data-ttu-id="cb25c-199">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="cb25c-199">Valid values 0 to 4</span></span>|
|<span data-ttu-id="cb25c-200">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cb25c-200">passwordMinimumLength</span></span>|<span data-ttu-id="cb25c-201">Int32</span><span class="sxs-lookup"><span data-stu-id="cb25c-201">Int32</span></span>|<span data-ttu-id="cb25c-202">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="cb25c-202">Minimum length of passwords.</span></span>|
|<span data-ttu-id="cb25c-203">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="cb25c-203">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="cb25c-204">Int32</span><span class="sxs-lookup"><span data-stu-id="cb25c-204">Int32</span></span>|<span data-ttu-id="cb25c-205">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="cb25c-205">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="cb25c-206">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="cb25c-206">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="cb25c-207">Int32</span><span class="sxs-lookup"><span data-stu-id="cb25c-207">Int32</span></span>|<span data-ttu-id="cb25c-208">Период бездействия (в минутах), по истечении которого будет гаснуть экран.</span><span class="sxs-lookup"><span data-stu-id="cb25c-208">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="cb25c-209">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="cb25c-209">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="cb25c-210">Int32</span><span class="sxs-lookup"><span data-stu-id="cb25c-210">Int32</span></span>|<span data-ttu-id="cb25c-211">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="cb25c-211">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="cb25c-212">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cb25c-212">passwordRequiredType</span></span>|[<span data-ttu-id="cb25c-213">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="cb25c-213">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="cb25c-214">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="cb25c-214">Type of password that is required.</span></span> <span data-ttu-id="cb25c-215">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="cb25c-215">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="cb25c-216">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="cb25c-216">passwordRequired</span></span>|<span data-ttu-id="cb25c-217">Логический</span><span class="sxs-lookup"><span data-stu-id="cb25c-217">Boolean</span></span>|<span data-ttu-id="cb25c-218">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="cb25c-218">Whether or not to require a password.</span></span>|
|<span data-ttu-id="cb25c-219">кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="cb25c-219">keychainBlockCloudSync</span></span>|<span data-ttu-id="cb25c-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-220">Boolean</span></span>|<span data-ttu-id="cb25c-221">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="cb25c-221">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="cb25c-222">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="cb25c-222">airPrintBlocked</span></span>|<span data-ttu-id="cb25c-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-223">Boolean</span></span>|<span data-ttu-id="cb25c-224">Указывает, заблокировано ли Аирпринт (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="cb25c-224">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="cb25c-225">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="cb25c-225">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="cb25c-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-226">Boolean</span></span>|<span data-ttu-id="cb25c-227">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (macOS 10,13 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="cb25c-227">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="cb25c-228">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="cb25c-228">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="cb25c-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-229">Boolean</span></span>|<span data-ttu-id="cb25c-230">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="cb25c-230">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="cb25c-231">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (macOS 10,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="cb25c-231">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="cb25c-232">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="cb25c-232">safariBlockAutofill</span></span>|<span data-ttu-id="cb25c-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-233">Boolean</span></span>|<span data-ttu-id="cb25c-234">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="cb25c-234">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="cb25c-235">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="cb25c-235">cameraBlocked</span></span>|<span data-ttu-id="cb25c-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-236">Boolean</span></span>|<span data-ttu-id="cb25c-237">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="cb25c-237">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="cb25c-238">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="cb25c-238">iTunesBlockMusicService</span></span>|<span data-ttu-id="cb25c-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-239">Boolean</span></span>|<span data-ttu-id="cb25c-240">Указывает, следует ли заблокировать музыкальную службу и вернуть приложение "Музыка" в классический режим.</span><span class="sxs-lookup"><span data-stu-id="cb25c-240">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="cb25c-241">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="cb25c-241">spotlightBlockInternetResults</span></span>|<span data-ttu-id="cb25c-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-242">Boolean</span></span>|<span data-ttu-id="cb25c-243">Указывает, следует ли запретить получение результатов из поиска в Интернете.</span><span class="sxs-lookup"><span data-stu-id="cb25c-243">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="cb25c-244">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="cb25c-244">keyboardBlockDictation</span></span>|<span data-ttu-id="cb25c-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-245">Boolean</span></span>|<span data-ttu-id="cb25c-246">Указывает, следует ли запретить пользователю использовать диктовку.</span><span class="sxs-lookup"><span data-stu-id="cb25c-246">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="cb25c-247">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="cb25c-247">definitionLookupBlocked</span></span>|<span data-ttu-id="cb25c-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-248">Boolean</span></span>|<span data-ttu-id="cb25c-249">Указывает, следует ли заблокировать Поиск определений.</span><span class="sxs-lookup"><span data-stu-id="cb25c-249">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="cb25c-250">апплеватчблоккаутаунлокк</span><span class="sxs-lookup"><span data-stu-id="cb25c-250">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="cb25c-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-251">Boolean</span></span>|<span data-ttu-id="cb25c-252">Указывает, следует ли запретить пользователям разблокирование своего Mac-адреса с контрольной записью Apple.</span><span class="sxs-lookup"><span data-stu-id="cb25c-252">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="cb25c-253">итунесблоккфилешаринг</span><span class="sxs-lookup"><span data-stu-id="cb25c-253">iTunesBlockFileSharing</span></span>|<span data-ttu-id="cb25c-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-254">Boolean</span></span>|<span data-ttu-id="cb25c-255">Указывает, следует ли запретить передачу файлов с помощью iTunes.</span><span class="sxs-lookup"><span data-stu-id="cb25c-255">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="cb25c-256">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="cb25c-256">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="cb25c-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-257">Boolean</span></span>|<span data-ttu-id="cb25c-258">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="cb25c-258">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="cb25c-259">иклаудблоккмаил</span><span class="sxs-lookup"><span data-stu-id="cb25c-259">iCloudBlockMail</span></span>|<span data-ttu-id="cb25c-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-260">Boolean</span></span>|<span data-ttu-id="cb25c-261">Указывает, следует ли запретить синхронизацию почты для iCloud.</span><span class="sxs-lookup"><span data-stu-id="cb25c-261">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="cb25c-262">иклаудблоккаддрессбук</span><span class="sxs-lookup"><span data-stu-id="cb25c-262">iCloudBlockAddressBook</span></span>|<span data-ttu-id="cb25c-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-263">Boolean</span></span>|<span data-ttu-id="cb25c-264">Указывает, следует ли запретить синхронизацию контактов с iCloud.</span><span class="sxs-lookup"><span data-stu-id="cb25c-264">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="cb25c-265">иклаудблокккалендар</span><span class="sxs-lookup"><span data-stu-id="cb25c-265">iCloudBlockCalendar</span></span>|<span data-ttu-id="cb25c-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-266">Boolean</span></span>|<span data-ttu-id="cb25c-267">Указывает, следует ли запретить синхронизацию календарей в iCloud.</span><span class="sxs-lookup"><span data-stu-id="cb25c-267">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="cb25c-268">иклаудблоккреминдерс</span><span class="sxs-lookup"><span data-stu-id="cb25c-268">iCloudBlockReminders</span></span>|<span data-ttu-id="cb25c-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-269">Boolean</span></span>|<span data-ttu-id="cb25c-270">Указывает, следует ли запретить синхронизацию напоминаний для iCloud.</span><span class="sxs-lookup"><span data-stu-id="cb25c-270">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="cb25c-271">иклаудблоккбукмаркс</span><span class="sxs-lookup"><span data-stu-id="cb25c-271">iCloudBlockBookmarks</span></span>|<span data-ttu-id="cb25c-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-272">Boolean</span></span>|<span data-ttu-id="cb25c-273">Указывает, следует ли блокировать синхронизацию закладок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="cb25c-273">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="cb25c-274">иклаудблоккнотес</span><span class="sxs-lookup"><span data-stu-id="cb25c-274">iCloudBlockNotes</span></span>|<span data-ttu-id="cb25c-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-275">Boolean</span></span>|<span data-ttu-id="cb25c-276">Указывает, следует ли запретить синхронизацию заметок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="cb25c-276">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="cb25c-277">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="cb25c-277">airDropBlocked</span></span>|<span data-ttu-id="cb25c-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-278">Boolean</span></span>|<span data-ttu-id="cb25c-279">Указывает, следует ли запретить AirDrop.</span><span class="sxs-lookup"><span data-stu-id="cb25c-279">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="cb25c-280">пассвордблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="cb25c-280">passwordBlockModification</span></span>|<span data-ttu-id="cb25c-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-281">Boolean</span></span>|<span data-ttu-id="cb25c-282">Указывает, следует ли запретить изменение секретного кода.</span><span class="sxs-lookup"><span data-stu-id="cb25c-282">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="cb25c-283">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="cb25c-283">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="cb25c-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-284">Boolean</span></span>|<span data-ttu-id="cb25c-285">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="cb25c-285">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="cb25c-286">пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="cb25c-286">passwordBlockAutoFill</span></span>|<span data-ttu-id="cb25c-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-287">Boolean</span></span>|<span data-ttu-id="cb25c-288">Указывает, следует ли заблокировать функцию автозаполнения паролей.</span><span class="sxs-lookup"><span data-stu-id="cb25c-288">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="cb25c-289">пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="cb25c-289">passwordBlockProximityRequests</span></span>|<span data-ttu-id="cb25c-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-290">Boolean</span></span>|<span data-ttu-id="cb25c-291">Указывает, следует ли запретить запрашивать пароли с ближайших устройств.</span><span class="sxs-lookup"><span data-stu-id="cb25c-291">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="cb25c-292">пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="cb25c-292">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="cb25c-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-293">Boolean</span></span>|<span data-ttu-id="cb25c-294">Указывает, следует ли заблокировать общий доступ к паролям с помощью функции паролей AirDrop.</span><span class="sxs-lookup"><span data-stu-id="cb25c-294">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="cb25c-295">софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="cb25c-295">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="cb25c-296">Int32</span><span class="sxs-lookup"><span data-stu-id="cb25c-296">Int32</span></span>|<span data-ttu-id="cb25c-297">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="cb25c-297">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="cb25c-298">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="cb25c-298">Valid values 0 to 90</span></span>|
|<span data-ttu-id="cb25c-299">софтвареупдатесфорцеделайед</span><span class="sxs-lookup"><span data-stu-id="cb25c-299">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="cb25c-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-300">Boolean</span></span>|<span data-ttu-id="cb25c-301">Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="cb25c-301">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="cb25c-302">контенткачингблоккед</span><span class="sxs-lookup"><span data-stu-id="cb25c-302">contentCachingBlocked</span></span>|<span data-ttu-id="cb25c-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-303">Boolean</span></span>|<span data-ttu-id="cb25c-304">Указывает, следует ли запретить кэширование контента.</span><span class="sxs-lookup"><span data-stu-id="cb25c-304">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="cb25c-305">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="cb25c-305">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="cb25c-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-306">Boolean</span></span>|<span data-ttu-id="cb25c-307">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="cb25c-307">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="cb25c-308">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="cb25c-308">screenCaptureBlocked</span></span>|<span data-ttu-id="cb25c-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-309">Boolean</span></span>|<span data-ttu-id="cb25c-310">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="cb25c-310">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="cb25c-311">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="cb25c-311">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="cb25c-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-312">Boolean</span></span>|<span data-ttu-id="cb25c-313">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "аудитория".</span><span class="sxs-lookup"><span data-stu-id="cb25c-313">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="cb25c-314">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="cb25c-314">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="cb25c-315">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="cb25c-315">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="cb25c-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-316">Boolean</span></span>|<span data-ttu-id="cb25c-317">Указывает, следует ли автоматически предоставлять разрешение преподавателю управляемого курса в приложении аудитории для просмотра экрана учащегося без выдачи запросов.</span><span class="sxs-lookup"><span data-stu-id="cb25c-317">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="cb25c-318">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="cb25c-318">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="cb25c-319">классрумфорцеаутоматикаллижоинклассес</span><span class="sxs-lookup"><span data-stu-id="cb25c-319">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="cb25c-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-320">Boolean</span></span>|<span data-ttu-id="cb25c-321">Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося.</span><span class="sxs-lookup"><span data-stu-id="cb25c-321">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="cb25c-322">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="cb25c-322">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="cb25c-323">классрумфорцерекуестпермиссионтолеавеклассес</span><span class="sxs-lookup"><span data-stu-id="cb25c-323">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="cb25c-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-324">Boolean</span></span>|<span data-ttu-id="cb25c-325">Указывает, должен ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса.</span><span class="sxs-lookup"><span data-stu-id="cb25c-325">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="cb25c-326">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="cb25c-326">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="cb25c-327">классрумфорцеунпромптедаппанддевицелокк</span><span class="sxs-lookup"><span data-stu-id="cb25c-327">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="cb25c-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-328">Boolean</span></span>|<span data-ttu-id="cb25c-329">Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся.</span><span class="sxs-lookup"><span data-stu-id="cb25c-329">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="cb25c-330">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="cb25c-330">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="cb25c-331">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="cb25c-331">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="cb25c-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb25c-332">Boolean</span></span>|<span data-ttu-id="cb25c-333">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве MacOS, на другом устройстве iOS или MacOS (MacOS 10,15 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="cb25c-333">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="cb25c-334">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb25c-334">Response</span></span>
<span data-ttu-id="cb25c-335">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cb25c-335">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb25c-336">Пример</span><span class="sxs-lookup"><span data-stu-id="cb25c-336">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb25c-337">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb25c-337">Request</span></span>
<span data-ttu-id="cb25c-338">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb25c-338">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3146

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true
}
```

### <a name="response"></a><span data-ttu-id="cb25c-339">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb25c-339">Response</span></span>
<span data-ttu-id="cb25c-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb25c-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3318

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true
}
```






