---
title: Update macOSGeneralDeviceConfiguration
description: Обновление свойств объекта macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5b03c29028998970e75d4e79a8fe67508a9acd9e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048045"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="b473b-103">Update macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b473b-103">Update macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="b473b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b473b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b473b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b473b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b473b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b473b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b473b-107">Обновление свойств объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b473b-107">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b473b-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b473b-108">Prerequisites</span></span>
<span data-ttu-id="b473b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b473b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b473b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b473b-111">Permission type</span></span>|<span data-ttu-id="b473b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b473b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b473b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b473b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b473b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b473b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b473b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b473b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b473b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b473b-116">Not supported.</span></span>|
|<span data-ttu-id="b473b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b473b-117">Application</span></span>|<span data-ttu-id="b473b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b473b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b473b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b473b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b473b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b473b-120">Request headers</span></span>
|<span data-ttu-id="b473b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b473b-121">Header</span></span>|<span data-ttu-id="b473b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b473b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b473b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b473b-123">Authorization</span></span>|<span data-ttu-id="b473b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b473b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b473b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b473b-125">Accept</span></span>|<span data-ttu-id="b473b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b473b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b473b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b473b-127">Request body</span></span>
<span data-ttu-id="b473b-128">В теле запроса добавьте представление объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b473b-128">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="b473b-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b473b-129">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="b473b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b473b-130">Property</span></span>|<span data-ttu-id="b473b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b473b-131">Type</span></span>|<span data-ttu-id="b473b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b473b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b473b-133">id</span><span class="sxs-lookup"><span data-stu-id="b473b-133">id</span></span>|<span data-ttu-id="b473b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b473b-134">String</span></span>|<span data-ttu-id="b473b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b473b-135">Key of the entity.</span></span> <span data-ttu-id="b473b-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b473b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b473b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b473b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b473b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b473b-138">DateTimeOffset</span></span>|<span data-ttu-id="b473b-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b473b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b473b-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b473b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b473b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b473b-141">roleScopeTagIds</span></span>|<span data-ttu-id="b473b-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b473b-142">String collection</span></span>|<span data-ttu-id="b473b-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b473b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b473b-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b473b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b473b-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="b473b-145">supportsScopeTags</span></span>|<span data-ttu-id="b473b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-146">Boolean</span></span>|<span data-ttu-id="b473b-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="b473b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b473b-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="b473b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b473b-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="b473b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b473b-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b473b-150">This property is read-only.</span></span> <span data-ttu-id="b473b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b473b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b473b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b473b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b473b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b473b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b473b-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b473b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b473b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b473b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b473b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b473b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b473b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b473b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b473b-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b473b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b473b-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b473b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b473b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b473b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b473b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b473b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b473b-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="b473b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b473b-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b473b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b473b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b473b-164">createdDateTime</span></span>|<span data-ttu-id="b473b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b473b-165">DateTimeOffset</span></span>|<span data-ttu-id="b473b-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b473b-166">DateTime the object was created.</span></span> <span data-ttu-id="b473b-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b473b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b473b-168">description</span><span class="sxs-lookup"><span data-stu-id="b473b-168">description</span></span>|<span data-ttu-id="b473b-169">String</span><span class="sxs-lookup"><span data-stu-id="b473b-169">String</span></span>|<span data-ttu-id="b473b-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b473b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b473b-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b473b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b473b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b473b-172">displayName</span></span>|<span data-ttu-id="b473b-173">Строка</span><span class="sxs-lookup"><span data-stu-id="b473b-173">String</span></span>|<span data-ttu-id="b473b-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b473b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b473b-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b473b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b473b-176">version</span><span class="sxs-lookup"><span data-stu-id="b473b-176">version</span></span>|<span data-ttu-id="b473b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b473b-177">Int32</span></span>|<span data-ttu-id="b473b-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b473b-178">Version of the device configuration.</span></span> <span data-ttu-id="b473b-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b473b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b473b-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="b473b-180">compliantAppsList</span></span>|<span data-ttu-id="b473b-181">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="b473b-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b473b-182">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="b473b-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="b473b-183">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="b473b-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b473b-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="b473b-184">compliantAppListType</span></span>|[<span data-ttu-id="b473b-185">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="b473b-185">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="b473b-186">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="b473b-186">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="b473b-187">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="b473b-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b473b-188">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="b473b-188">emailInDomainSuffixes</span></span>|<span data-ttu-id="b473b-189">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b473b-189">String collection</span></span>|<span data-ttu-id="b473b-190">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="b473b-190">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="b473b-191">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b473b-191">passwordBlockSimple</span></span>|<span data-ttu-id="b473b-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-192">Boolean</span></span>|<span data-ttu-id="b473b-193">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="b473b-193">Block simple passwords.</span></span>|
|<span data-ttu-id="b473b-194">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b473b-194">passwordExpirationDays</span></span>|<span data-ttu-id="b473b-195">Int32</span><span class="sxs-lookup"><span data-stu-id="b473b-195">Int32</span></span>|<span data-ttu-id="b473b-196">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="b473b-196">Number of days before the password expires.</span></span>|
|<span data-ttu-id="b473b-197">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b473b-197">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b473b-198">Int32</span><span class="sxs-lookup"><span data-stu-id="b473b-198">Int32</span></span>|<span data-ttu-id="b473b-199">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="b473b-199">Number of character sets a password must contain.</span></span> <span data-ttu-id="b473b-200">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="b473b-200">Valid values 0 to 4</span></span>|
|<span data-ttu-id="b473b-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b473b-201">passwordMinimumLength</span></span>|<span data-ttu-id="b473b-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b473b-202">Int32</span></span>|<span data-ttu-id="b473b-203">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="b473b-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="b473b-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b473b-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b473b-205">Int32</span><span class="sxs-lookup"><span data-stu-id="b473b-205">Int32</span></span>|<span data-ttu-id="b473b-206">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="b473b-206">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="b473b-207">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b473b-207">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b473b-208">Int32</span><span class="sxs-lookup"><span data-stu-id="b473b-208">Int32</span></span>|<span data-ttu-id="b473b-209">Период бездействия (в минутах), по истечении которого будет гаснуть экран.</span><span class="sxs-lookup"><span data-stu-id="b473b-209">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="b473b-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b473b-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b473b-211">Int32</span><span class="sxs-lookup"><span data-stu-id="b473b-211">Int32</span></span>|<span data-ttu-id="b473b-212">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="b473b-212">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="b473b-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b473b-213">passwordRequiredType</span></span>|[<span data-ttu-id="b473b-214">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="b473b-214">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b473b-215">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="b473b-215">Type of password that is required.</span></span> <span data-ttu-id="b473b-216">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="b473b-216">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b473b-217">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b473b-217">passwordRequired</span></span>|<span data-ttu-id="b473b-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-218">Boolean</span></span>|<span data-ttu-id="b473b-219">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="b473b-219">Whether or not to require a password.</span></span>|
|<span data-ttu-id="b473b-220">кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="b473b-220">keychainBlockCloudSync</span></span>|<span data-ttu-id="b473b-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-221">Boolean</span></span>|<span data-ttu-id="b473b-222">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="b473b-222">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="b473b-223">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="b473b-223">airPrintBlocked</span></span>|<span data-ttu-id="b473b-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-224">Boolean</span></span>|<span data-ttu-id="b473b-225">Указывает, заблокировано ли Аирпринт (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="b473b-225">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="b473b-226">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="b473b-226">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="b473b-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-227">Boolean</span></span>|<span data-ttu-id="b473b-228">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (macOS 10,13 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="b473b-228">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="b473b-229">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="b473b-229">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="b473b-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-230">Boolean</span></span>|<span data-ttu-id="b473b-231">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="b473b-231">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="b473b-232">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (macOS 10,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="b473b-232">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="b473b-233">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b473b-233">safariBlockAutofill</span></span>|<span data-ttu-id="b473b-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-234">Boolean</span></span>|<span data-ttu-id="b473b-235">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="b473b-235">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="b473b-236">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b473b-236">cameraBlocked</span></span>|<span data-ttu-id="b473b-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-237">Boolean</span></span>|<span data-ttu-id="b473b-238">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="b473b-238">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="b473b-239">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="b473b-239">iTunesBlockMusicService</span></span>|<span data-ttu-id="b473b-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-240">Boolean</span></span>|<span data-ttu-id="b473b-241">Указывает, следует ли заблокировать музыкальную службу и вернуть приложение "Музыка" в классический режим.</span><span class="sxs-lookup"><span data-stu-id="b473b-241">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="b473b-242">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="b473b-242">spotlightBlockInternetResults</span></span>|<span data-ttu-id="b473b-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-243">Boolean</span></span>|<span data-ttu-id="b473b-244">Указывает, следует ли запретить получение результатов из поиска в Интернете.</span><span class="sxs-lookup"><span data-stu-id="b473b-244">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="b473b-245">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="b473b-245">keyboardBlockDictation</span></span>|<span data-ttu-id="b473b-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-246">Boolean</span></span>|<span data-ttu-id="b473b-247">Указывает, следует ли запретить пользователю использовать диктовку.</span><span class="sxs-lookup"><span data-stu-id="b473b-247">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="b473b-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="b473b-248">definitionLookupBlocked</span></span>|<span data-ttu-id="b473b-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-249">Boolean</span></span>|<span data-ttu-id="b473b-250">Указывает, следует ли заблокировать Поиск определений.</span><span class="sxs-lookup"><span data-stu-id="b473b-250">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="b473b-251">апплеватчблоккаутаунлокк</span><span class="sxs-lookup"><span data-stu-id="b473b-251">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="b473b-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-252">Boolean</span></span>|<span data-ttu-id="b473b-253">Указывает, следует ли запретить пользователям разблокирование своего Mac-адреса с контрольной записью Apple.</span><span class="sxs-lookup"><span data-stu-id="b473b-253">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="b473b-254">итунесблоккфилешаринг</span><span class="sxs-lookup"><span data-stu-id="b473b-254">iTunesBlockFileSharing</span></span>|<span data-ttu-id="b473b-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-255">Boolean</span></span>|<span data-ttu-id="b473b-256">Указывает, следует ли запретить передачу файлов с помощью iTunes.</span><span class="sxs-lookup"><span data-stu-id="b473b-256">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="b473b-257">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="b473b-257">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="b473b-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-258">Boolean</span></span>|<span data-ttu-id="b473b-259">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="b473b-259">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="b473b-260">иклаудблоккмаил</span><span class="sxs-lookup"><span data-stu-id="b473b-260">iCloudBlockMail</span></span>|<span data-ttu-id="b473b-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-261">Boolean</span></span>|<span data-ttu-id="b473b-262">Указывает, следует ли запретить синхронизацию почты для iCloud.</span><span class="sxs-lookup"><span data-stu-id="b473b-262">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="b473b-263">иклаудблоккаддрессбук</span><span class="sxs-lookup"><span data-stu-id="b473b-263">iCloudBlockAddressBook</span></span>|<span data-ttu-id="b473b-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-264">Boolean</span></span>|<span data-ttu-id="b473b-265">Указывает, следует ли запретить синхронизацию контактов с iCloud.</span><span class="sxs-lookup"><span data-stu-id="b473b-265">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="b473b-266">иклаудблокккалендар</span><span class="sxs-lookup"><span data-stu-id="b473b-266">iCloudBlockCalendar</span></span>|<span data-ttu-id="b473b-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-267">Boolean</span></span>|<span data-ttu-id="b473b-268">Указывает, следует ли запретить синхронизацию календарей в iCloud.</span><span class="sxs-lookup"><span data-stu-id="b473b-268">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="b473b-269">иклаудблоккреминдерс</span><span class="sxs-lookup"><span data-stu-id="b473b-269">iCloudBlockReminders</span></span>|<span data-ttu-id="b473b-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-270">Boolean</span></span>|<span data-ttu-id="b473b-271">Указывает, следует ли запретить синхронизацию напоминаний для iCloud.</span><span class="sxs-lookup"><span data-stu-id="b473b-271">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="b473b-272">иклаудблоккбукмаркс</span><span class="sxs-lookup"><span data-stu-id="b473b-272">iCloudBlockBookmarks</span></span>|<span data-ttu-id="b473b-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-273">Boolean</span></span>|<span data-ttu-id="b473b-274">Указывает, следует ли блокировать синхронизацию закладок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="b473b-274">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="b473b-275">иклаудблоккнотес</span><span class="sxs-lookup"><span data-stu-id="b473b-275">iCloudBlockNotes</span></span>|<span data-ttu-id="b473b-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-276">Boolean</span></span>|<span data-ttu-id="b473b-277">Указывает, следует ли запретить синхронизацию заметок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="b473b-277">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="b473b-278">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="b473b-278">airDropBlocked</span></span>|<span data-ttu-id="b473b-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-279">Boolean</span></span>|<span data-ttu-id="b473b-280">Указывает, следует ли запретить AirDrop.</span><span class="sxs-lookup"><span data-stu-id="b473b-280">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="b473b-281">пассвордблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="b473b-281">passwordBlockModification</span></span>|<span data-ttu-id="b473b-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-282">Boolean</span></span>|<span data-ttu-id="b473b-283">Указывает, следует ли запретить изменение секретного кода.</span><span class="sxs-lookup"><span data-stu-id="b473b-283">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="b473b-284">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="b473b-284">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="b473b-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-285">Boolean</span></span>|<span data-ttu-id="b473b-286">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="b473b-286">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="b473b-287">пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="b473b-287">passwordBlockAutoFill</span></span>|<span data-ttu-id="b473b-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-288">Boolean</span></span>|<span data-ttu-id="b473b-289">Указывает, следует ли заблокировать функцию автозаполнения паролей.</span><span class="sxs-lookup"><span data-stu-id="b473b-289">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="b473b-290">пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="b473b-290">passwordBlockProximityRequests</span></span>|<span data-ttu-id="b473b-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-291">Boolean</span></span>|<span data-ttu-id="b473b-292">Указывает, следует ли запретить запрашивать пароли с ближайших устройств.</span><span class="sxs-lookup"><span data-stu-id="b473b-292">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="b473b-293">пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="b473b-293">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="b473b-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-294">Boolean</span></span>|<span data-ttu-id="b473b-295">Указывает, следует ли заблокировать общий доступ к паролям с помощью функции паролей AirDrop.</span><span class="sxs-lookup"><span data-stu-id="b473b-295">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="b473b-296">софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="b473b-296">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="b473b-297">Int32</span><span class="sxs-lookup"><span data-stu-id="b473b-297">Int32</span></span>|<span data-ttu-id="b473b-298">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="b473b-298">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="b473b-299">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="b473b-299">Valid values 0 to 90</span></span>|
|<span data-ttu-id="b473b-300">софтвареупдатесфорцеделайед</span><span class="sxs-lookup"><span data-stu-id="b473b-300">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="b473b-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-301">Boolean</span></span>|<span data-ttu-id="b473b-302">Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="b473b-302">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b473b-303">упдатеделайполици</span><span class="sxs-lookup"><span data-stu-id="b473b-303">updateDelayPolicy</span></span>|[<span data-ttu-id="b473b-304">макоссофтвареупдатеделайполици</span><span class="sxs-lookup"><span data-stu-id="b473b-304">macOSSoftwareUpdateDelayPolicy</span></span>](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|<span data-ttu-id="b473b-305">Определяет, следует ли откладывать обновления для ОС и/или приложений для macOS.</span><span class="sxs-lookup"><span data-stu-id="b473b-305">Determines whether to delay OS and/or app updates for macOS.</span></span> <span data-ttu-id="b473b-306">Возможные значения: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span><span class="sxs-lookup"><span data-stu-id="b473b-306">Possible values are: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span></span>|
|<span data-ttu-id="b473b-307">контенткачингблоккед</span><span class="sxs-lookup"><span data-stu-id="b473b-307">contentCachingBlocked</span></span>|<span data-ttu-id="b473b-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-308">Boolean</span></span>|<span data-ttu-id="b473b-309">Указывает, следует ли запретить кэширование контента.</span><span class="sxs-lookup"><span data-stu-id="b473b-309">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="b473b-310">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="b473b-310">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="b473b-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-311">Boolean</span></span>|<span data-ttu-id="b473b-312">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="b473b-312">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="b473b-313">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b473b-313">screenCaptureBlocked</span></span>|<span data-ttu-id="b473b-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-314">Boolean</span></span>|<span data-ttu-id="b473b-315">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="b473b-315">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="b473b-316">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b473b-316">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="b473b-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-317">Boolean</span></span>|<span data-ttu-id="b473b-318">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "аудитория".</span><span class="sxs-lookup"><span data-stu-id="b473b-318">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="b473b-319">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="b473b-319">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="b473b-320">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b473b-320">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="b473b-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-321">Boolean</span></span>|<span data-ttu-id="b473b-322">Указывает, следует ли автоматически предоставлять разрешение преподавателю управляемого курса в приложении аудитории для просмотра экрана учащегося без выдачи запросов.</span><span class="sxs-lookup"><span data-stu-id="b473b-322">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="b473b-323">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="b473b-323">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="b473b-324">классрумфорцеаутоматикаллижоинклассес</span><span class="sxs-lookup"><span data-stu-id="b473b-324">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="b473b-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-325">Boolean</span></span>|<span data-ttu-id="b473b-326">Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося.</span><span class="sxs-lookup"><span data-stu-id="b473b-326">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="b473b-327">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="b473b-327">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="b473b-328">классрумфорцерекуестпермиссионтолеавеклассес</span><span class="sxs-lookup"><span data-stu-id="b473b-328">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="b473b-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-329">Boolean</span></span>|<span data-ttu-id="b473b-330">Указывает, должен ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса.</span><span class="sxs-lookup"><span data-stu-id="b473b-330">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="b473b-331">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="b473b-331">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="b473b-332">классрумфорцеунпромптедаппанддевицелокк</span><span class="sxs-lookup"><span data-stu-id="b473b-332">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="b473b-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-333">Boolean</span></span>|<span data-ttu-id="b473b-334">Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся.</span><span class="sxs-lookup"><span data-stu-id="b473b-334">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="b473b-335">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="b473b-335">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="b473b-336">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="b473b-336">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="b473b-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="b473b-337">Boolean</span></span>|<span data-ttu-id="b473b-338">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве MacOS, на другом устройстве iOS или MacOS (MacOS 10,15 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="b473b-338">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|
|<span data-ttu-id="b473b-339">привациакцессконтролс</span><span class="sxs-lookup"><span data-stu-id="b473b-339">privacyAccessControls</span></span>|<span data-ttu-id="b473b-340">Коллекция [макоспривациакцессконтролитем](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="b473b-340">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="b473b-341">Список элементов управления политикой настройки конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b473b-341">List of privacy preference policy controls.</span></span> <span data-ttu-id="b473b-342">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="b473b-342">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b473b-343">Ответ</span><span class="sxs-lookup"><span data-stu-id="b473b-343">Response</span></span>
<span data-ttu-id="b473b-344">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b473b-344">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b473b-345">Пример</span><span class="sxs-lookup"><span data-stu-id="b473b-345">Example</span></span>

### <a name="request"></a><span data-ttu-id="b473b-346">Запрос</span><span class="sxs-lookup"><span data-stu-id="b473b-346">Request</span></span>
<span data-ttu-id="b473b-347">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b473b-347">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4596

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
  "updateDelayPolicy": "delayOSUpdateVisibility",
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true,
  "privacyAccessControls": [
    {
      "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
          "allowed": true
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="b473b-348">Отклик</span><span class="sxs-lookup"><span data-stu-id="b473b-348">Response</span></span>
<span data-ttu-id="b473b-p126">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b473b-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4768

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
  "updateDelayPolicy": "delayOSUpdateVisibility",
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true,
  "privacyAccessControls": [
    {
      "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
          "allowed": true
        }
      ]
    }
  ]
}
```






