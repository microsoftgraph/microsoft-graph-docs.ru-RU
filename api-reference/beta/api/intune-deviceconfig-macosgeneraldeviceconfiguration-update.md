---
title: Update macOSGeneralDeviceConfiguration
description: Обновление свойств объекта macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b3a14472d035dc050f78aa3bf1feec4876cc90db
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271200"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="fb76a-103">Update macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb76a-103">Update macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="fb76a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb76a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb76a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb76a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb76a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb76a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb76a-107">Обновление свойств объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb76a-107">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb76a-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fb76a-108">Prerequisites</span></span>
<span data-ttu-id="fb76a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb76a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb76a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb76a-111">Permission type</span></span>|<span data-ttu-id="fb76a-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb76a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb76a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb76a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb76a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb76a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fb76a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb76a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb76a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb76a-116">Not supported.</span></span>|
|<span data-ttu-id="fb76a-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="fb76a-117">Application</span></span>|<span data-ttu-id="fb76a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb76a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb76a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb76a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fb76a-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fb76a-120">Request headers</span></span>
|<span data-ttu-id="fb76a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb76a-121">Header</span></span>|<span data-ttu-id="fb76a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb76a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb76a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fb76a-123">Authorization</span></span>|<span data-ttu-id="fb76a-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb76a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb76a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb76a-125">Accept</span></span>|<span data-ttu-id="fb76a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb76a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb76a-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb76a-127">Request body</span></span>
<span data-ttu-id="fb76a-128">В теле запроса добавьте представление объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb76a-128">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="fb76a-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb76a-129">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="fb76a-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb76a-130">Property</span></span>|<span data-ttu-id="fb76a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fb76a-131">Type</span></span>|<span data-ttu-id="fb76a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fb76a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb76a-133">id</span><span class="sxs-lookup"><span data-stu-id="fb76a-133">id</span></span>|<span data-ttu-id="fb76a-134">String</span><span class="sxs-lookup"><span data-stu-id="fb76a-134">String</span></span>|<span data-ttu-id="fb76a-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fb76a-135">Key of the entity.</span></span> <span data-ttu-id="fb76a-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb76a-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb76a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb76a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="fb76a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb76a-138">DateTimeOffset</span></span>|<span data-ttu-id="fb76a-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fb76a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="fb76a-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb76a-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb76a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fb76a-141">roleScopeTagIds</span></span>|<span data-ttu-id="fb76a-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fb76a-142">String collection</span></span>|<span data-ttu-id="fb76a-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fb76a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fb76a-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb76a-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb76a-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="fb76a-145">supportsScopeTags</span></span>|<span data-ttu-id="fb76a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-146">Boolean</span></span>|<span data-ttu-id="fb76a-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="fb76a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fb76a-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="fb76a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fb76a-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fb76a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fb76a-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb76a-150">This property is read-only.</span></span> <span data-ttu-id="fb76a-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb76a-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb76a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fb76a-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fb76a-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fb76a-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fb76a-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fb76a-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fb76a-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb76a-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb76a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fb76a-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fb76a-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fb76a-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fb76a-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fb76a-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fb76a-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb76a-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb76a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fb76a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fb76a-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fb76a-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fb76a-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fb76a-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fb76a-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb76a-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb76a-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb76a-164">createdDateTime</span></span>|<span data-ttu-id="fb76a-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb76a-165">DateTimeOffset</span></span>|<span data-ttu-id="fb76a-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fb76a-166">DateTime the object was created.</span></span> <span data-ttu-id="fb76a-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb76a-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb76a-168">description</span><span class="sxs-lookup"><span data-stu-id="fb76a-168">description</span></span>|<span data-ttu-id="fb76a-169">String</span><span class="sxs-lookup"><span data-stu-id="fb76a-169">String</span></span>|<span data-ttu-id="fb76a-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb76a-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fb76a-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb76a-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb76a-172">displayName</span><span class="sxs-lookup"><span data-stu-id="fb76a-172">displayName</span></span>|<span data-ttu-id="fb76a-173">String</span><span class="sxs-lookup"><span data-stu-id="fb76a-173">String</span></span>|<span data-ttu-id="fb76a-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb76a-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fb76a-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb76a-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb76a-176">version</span><span class="sxs-lookup"><span data-stu-id="fb76a-176">version</span></span>|<span data-ttu-id="fb76a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="fb76a-177">Int32</span></span>|<span data-ttu-id="fb76a-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb76a-178">Version of the device configuration.</span></span> <span data-ttu-id="fb76a-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb76a-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fb76a-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="fb76a-180">compliantAppsList</span></span>|<span data-ttu-id="fb76a-181">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="fb76a-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="fb76a-182">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="fb76a-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="fb76a-183">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="fb76a-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="fb76a-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="fb76a-184">compliantAppListType</span></span>|[<span data-ttu-id="fb76a-185">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="fb76a-185">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="fb76a-186">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="fb76a-186">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="fb76a-187">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="fb76a-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="fb76a-188">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="fb76a-188">emailInDomainSuffixes</span></span>|<span data-ttu-id="fb76a-189">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fb76a-189">String collection</span></span>|<span data-ttu-id="fb76a-190">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="fb76a-190">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="fb76a-191">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="fb76a-191">passwordBlockSimple</span></span>|<span data-ttu-id="fb76a-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-192">Boolean</span></span>|<span data-ttu-id="fb76a-193">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="fb76a-193">Block simple passwords.</span></span>|
|<span data-ttu-id="fb76a-194">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fb76a-194">passwordExpirationDays</span></span>|<span data-ttu-id="fb76a-195">Int32</span><span class="sxs-lookup"><span data-stu-id="fb76a-195">Int32</span></span>|<span data-ttu-id="fb76a-196">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="fb76a-196">Number of days before the password expires.</span></span>|
|<span data-ttu-id="fb76a-197">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="fb76a-197">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="fb76a-198">Int32</span><span class="sxs-lookup"><span data-stu-id="fb76a-198">Int32</span></span>|<span data-ttu-id="fb76a-199">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="fb76a-199">Number of character sets a password must contain.</span></span> <span data-ttu-id="fb76a-200">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="fb76a-200">Valid values 0 to 4</span></span>|
|<span data-ttu-id="fb76a-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fb76a-201">passwordMinimumLength</span></span>|<span data-ttu-id="fb76a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="fb76a-202">Int32</span></span>|<span data-ttu-id="fb76a-203">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="fb76a-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="fb76a-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="fb76a-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="fb76a-205">Int32</span><span class="sxs-lookup"><span data-stu-id="fb76a-205">Int32</span></span>|<span data-ttu-id="fb76a-206">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="fb76a-206">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="fb76a-207">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="fb76a-207">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="fb76a-208">Int32</span><span class="sxs-lookup"><span data-stu-id="fb76a-208">Int32</span></span>|<span data-ttu-id="fb76a-209">Период бездействия (в минутах), по истечении которого будет гаснуть экран.</span><span class="sxs-lookup"><span data-stu-id="fb76a-209">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="fb76a-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="fb76a-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="fb76a-211">Int32</span><span class="sxs-lookup"><span data-stu-id="fb76a-211">Int32</span></span>|<span data-ttu-id="fb76a-212">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="fb76a-212">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="fb76a-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="fb76a-213">passwordRequiredType</span></span>|[<span data-ttu-id="fb76a-214">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="fb76a-214">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="fb76a-215">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="fb76a-215">Type of password that is required.</span></span> <span data-ttu-id="fb76a-216">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="fb76a-216">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="fb76a-217">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="fb76a-217">passwordRequired</span></span>|<span data-ttu-id="fb76a-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-218">Boolean</span></span>|<span data-ttu-id="fb76a-219">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="fb76a-219">Whether or not to require a password.</span></span>|
|<span data-ttu-id="fb76a-220">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="fb76a-220">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="fb76a-221">Int32</span><span class="sxs-lookup"><span data-stu-id="fb76a-221">Int32</span></span>|<span data-ttu-id="fb76a-222">Количество допустимых неудачных попыток ввести секретный код на экран блокировки устройства.</span><span class="sxs-lookup"><span data-stu-id="fb76a-222">The number of allowed failed attempts to enter the passcode at the device's lock screen.</span></span> <span data-ttu-id="fb76a-223">Допустимые значения — от 2 до 11</span><span class="sxs-lookup"><span data-stu-id="fb76a-223">Valid values 2 to 11</span></span>|
|<span data-ttu-id="fb76a-224">пассвордминутесунтилфаиледлогинресет</span><span class="sxs-lookup"><span data-stu-id="fb76a-224">passwordMinutesUntilFailedLoginReset</span></span>|<span data-ttu-id="fb76a-225">Int32</span><span class="sxs-lookup"><span data-stu-id="fb76a-225">Int32</span></span>|<span data-ttu-id="fb76a-226">Количество минут до сброса имени входа после того, как будет достигнуто максимальное количество неудачных попыток входа.</span><span class="sxs-lookup"><span data-stu-id="fb76a-226">The number of minutes before the login is reset after the maximum number of unsuccessful login attempts is reached.</span></span>|
|<span data-ttu-id="fb76a-227">кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="fb76a-227">keychainBlockCloudSync</span></span>|<span data-ttu-id="fb76a-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-228">Boolean</span></span>|<span data-ttu-id="fb76a-229">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="fb76a-229">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="fb76a-230">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="fb76a-230">airPrintBlocked</span></span>|<span data-ttu-id="fb76a-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-231">Boolean</span></span>|<span data-ttu-id="fb76a-232">Указывает, заблокировано ли Аирпринт (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="fb76a-232">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="fb76a-233">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="fb76a-233">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="fb76a-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-234">Boolean</span></span>|<span data-ttu-id="fb76a-235">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (macOS 10,13 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="fb76a-235">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="fb76a-236">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="fb76a-236">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="fb76a-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-237">Boolean</span></span>|<span data-ttu-id="fb76a-238">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="fb76a-238">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="fb76a-239">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (macOS 10,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="fb76a-239">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="fb76a-240">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="fb76a-240">safariBlockAutofill</span></span>|<span data-ttu-id="fb76a-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-241">Boolean</span></span>|<span data-ttu-id="fb76a-242">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="fb76a-242">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="fb76a-243">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="fb76a-243">cameraBlocked</span></span>|<span data-ttu-id="fb76a-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-244">Boolean</span></span>|<span data-ttu-id="fb76a-245">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="fb76a-245">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="fb76a-246">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="fb76a-246">iTunesBlockMusicService</span></span>|<span data-ttu-id="fb76a-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-247">Boolean</span></span>|<span data-ttu-id="fb76a-248">Указывает, следует ли заблокировать музыкальную службу и вернуть приложение "Музыка" в классический режим.</span><span class="sxs-lookup"><span data-stu-id="fb76a-248">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="fb76a-249">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="fb76a-249">spotlightBlockInternetResults</span></span>|<span data-ttu-id="fb76a-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-250">Boolean</span></span>|<span data-ttu-id="fb76a-251">Указывает, следует ли запретить получение результатов из поиска в Интернете.</span><span class="sxs-lookup"><span data-stu-id="fb76a-251">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="fb76a-252">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="fb76a-252">keyboardBlockDictation</span></span>|<span data-ttu-id="fb76a-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-253">Boolean</span></span>|<span data-ttu-id="fb76a-254">Указывает, следует ли запретить пользователю использовать диктовку.</span><span class="sxs-lookup"><span data-stu-id="fb76a-254">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="fb76a-255">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="fb76a-255">definitionLookupBlocked</span></span>|<span data-ttu-id="fb76a-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-256">Boolean</span></span>|<span data-ttu-id="fb76a-257">Указывает, следует ли заблокировать Поиск определений.</span><span class="sxs-lookup"><span data-stu-id="fb76a-257">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="fb76a-258">апплеватчблоккаутаунлокк</span><span class="sxs-lookup"><span data-stu-id="fb76a-258">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="fb76a-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-259">Boolean</span></span>|<span data-ttu-id="fb76a-260">Указывает, следует ли запретить пользователям разблокирование своего Mac-адреса с контрольной записью Apple.</span><span class="sxs-lookup"><span data-stu-id="fb76a-260">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="fb76a-261">итунесблоккфилешаринг</span><span class="sxs-lookup"><span data-stu-id="fb76a-261">iTunesBlockFileSharing</span></span>|<span data-ttu-id="fb76a-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-262">Boolean</span></span>|<span data-ttu-id="fb76a-263">Указывает, следует ли запретить передачу файлов с помощью iTunes.</span><span class="sxs-lookup"><span data-stu-id="fb76a-263">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="fb76a-264">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="fb76a-264">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="fb76a-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-265">Boolean</span></span>|<span data-ttu-id="fb76a-266">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="fb76a-266">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="fb76a-267">иклаудблоккмаил</span><span class="sxs-lookup"><span data-stu-id="fb76a-267">iCloudBlockMail</span></span>|<span data-ttu-id="fb76a-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-268">Boolean</span></span>|<span data-ttu-id="fb76a-269">Указывает, следует ли запретить синхронизацию почты для iCloud.</span><span class="sxs-lookup"><span data-stu-id="fb76a-269">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="fb76a-270">иклаудблоккаддрессбук</span><span class="sxs-lookup"><span data-stu-id="fb76a-270">iCloudBlockAddressBook</span></span>|<span data-ttu-id="fb76a-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-271">Boolean</span></span>|<span data-ttu-id="fb76a-272">Указывает, следует ли запретить синхронизацию контактов с iCloud.</span><span class="sxs-lookup"><span data-stu-id="fb76a-272">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="fb76a-273">иклаудблокккалендар</span><span class="sxs-lookup"><span data-stu-id="fb76a-273">iCloudBlockCalendar</span></span>|<span data-ttu-id="fb76a-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-274">Boolean</span></span>|<span data-ttu-id="fb76a-275">Указывает, следует ли запретить синхронизацию календарей в iCloud.</span><span class="sxs-lookup"><span data-stu-id="fb76a-275">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="fb76a-276">иклаудблоккреминдерс</span><span class="sxs-lookup"><span data-stu-id="fb76a-276">iCloudBlockReminders</span></span>|<span data-ttu-id="fb76a-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-277">Boolean</span></span>|<span data-ttu-id="fb76a-278">Указывает, следует ли запретить синхронизацию напоминаний для iCloud.</span><span class="sxs-lookup"><span data-stu-id="fb76a-278">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="fb76a-279">иклаудблоккбукмаркс</span><span class="sxs-lookup"><span data-stu-id="fb76a-279">iCloudBlockBookmarks</span></span>|<span data-ttu-id="fb76a-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-280">Boolean</span></span>|<span data-ttu-id="fb76a-281">Указывает, следует ли блокировать синхронизацию закладок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="fb76a-281">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="fb76a-282">иклаудблоккнотес</span><span class="sxs-lookup"><span data-stu-id="fb76a-282">iCloudBlockNotes</span></span>|<span data-ttu-id="fb76a-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-283">Boolean</span></span>|<span data-ttu-id="fb76a-284">Указывает, следует ли запретить синхронизацию заметок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="fb76a-284">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="fb76a-285">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="fb76a-285">airDropBlocked</span></span>|<span data-ttu-id="fb76a-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-286">Boolean</span></span>|<span data-ttu-id="fb76a-287">Указывает, следует ли запретить AirDrop.</span><span class="sxs-lookup"><span data-stu-id="fb76a-287">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="fb76a-288">пассвордблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="fb76a-288">passwordBlockModification</span></span>|<span data-ttu-id="fb76a-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-289">Boolean</span></span>|<span data-ttu-id="fb76a-290">Указывает, следует ли запретить изменение секретного кода.</span><span class="sxs-lookup"><span data-stu-id="fb76a-290">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="fb76a-291">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="fb76a-291">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="fb76a-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-292">Boolean</span></span>|<span data-ttu-id="fb76a-293">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="fb76a-293">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="fb76a-294">пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="fb76a-294">passwordBlockAutoFill</span></span>|<span data-ttu-id="fb76a-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-295">Boolean</span></span>|<span data-ttu-id="fb76a-296">Указывает, следует ли заблокировать функцию автозаполнения паролей.</span><span class="sxs-lookup"><span data-stu-id="fb76a-296">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="fb76a-297">пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="fb76a-297">passwordBlockProximityRequests</span></span>|<span data-ttu-id="fb76a-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-298">Boolean</span></span>|<span data-ttu-id="fb76a-299">Указывает, следует ли запретить запрашивать пароли с ближайших устройств.</span><span class="sxs-lookup"><span data-stu-id="fb76a-299">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="fb76a-300">пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="fb76a-300">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="fb76a-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-301">Boolean</span></span>|<span data-ttu-id="fb76a-302">Указывает, следует ли заблокировать общий доступ к паролям с помощью функции паролей AirDrop.</span><span class="sxs-lookup"><span data-stu-id="fb76a-302">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="fb76a-303">софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="fb76a-303">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="fb76a-304">Int32</span><span class="sxs-lookup"><span data-stu-id="fb76a-304">Int32</span></span>|<span data-ttu-id="fb76a-305">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="fb76a-305">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="fb76a-306">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="fb76a-306">Valid values 0 to 90</span></span>|
|<span data-ttu-id="fb76a-307">упдатеделайполици</span><span class="sxs-lookup"><span data-stu-id="fb76a-307">updateDelayPolicy</span></span>|[<span data-ttu-id="fb76a-308">macOSSoftwareUpdateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="fb76a-308">macOSSoftwareUpdateDelayPolicy</span></span>](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|<span data-ttu-id="fb76a-309">Определяет, следует ли откладывать обновления для ОС и/или приложений для macOS.</span><span class="sxs-lookup"><span data-stu-id="fb76a-309">Determines whether to delay OS and/or app updates for macOS.</span></span> <span data-ttu-id="fb76a-310">Возможные значения: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span><span class="sxs-lookup"><span data-stu-id="fb76a-310">Possible values are: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span></span>|
|<span data-ttu-id="fb76a-311">контенткачингблоккед</span><span class="sxs-lookup"><span data-stu-id="fb76a-311">contentCachingBlocked</span></span>|<span data-ttu-id="fb76a-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-312">Boolean</span></span>|<span data-ttu-id="fb76a-313">Указывает, следует ли запретить кэширование контента.</span><span class="sxs-lookup"><span data-stu-id="fb76a-313">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="fb76a-314">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="fb76a-314">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="fb76a-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-315">Boolean</span></span>|<span data-ttu-id="fb76a-316">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="fb76a-316">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="fb76a-317">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="fb76a-317">screenCaptureBlocked</span></span>|<span data-ttu-id="fb76a-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-318">Boolean</span></span>|<span data-ttu-id="fb76a-319">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="fb76a-319">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="fb76a-320">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="fb76a-320">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="fb76a-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-321">Boolean</span></span>|<span data-ttu-id="fb76a-322">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "аудитория".</span><span class="sxs-lookup"><span data-stu-id="fb76a-322">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="fb76a-323">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="fb76a-323">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="fb76a-324">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="fb76a-324">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="fb76a-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-325">Boolean</span></span>|<span data-ttu-id="fb76a-326">Указывает, следует ли автоматически предоставлять разрешение преподавателю управляемого курса в приложении аудитории для просмотра экрана учащегося без выдачи запросов.</span><span class="sxs-lookup"><span data-stu-id="fb76a-326">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="fb76a-327">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="fb76a-327">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="fb76a-328">классрумфорцеаутоматикаллижоинклассес</span><span class="sxs-lookup"><span data-stu-id="fb76a-328">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="fb76a-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-329">Boolean</span></span>|<span data-ttu-id="fb76a-330">Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося.</span><span class="sxs-lookup"><span data-stu-id="fb76a-330">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="fb76a-331">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="fb76a-331">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="fb76a-332">классрумфорцерекуестпермиссионтолеавеклассес</span><span class="sxs-lookup"><span data-stu-id="fb76a-332">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="fb76a-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-333">Boolean</span></span>|<span data-ttu-id="fb76a-334">Указывает, должен ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса.</span><span class="sxs-lookup"><span data-stu-id="fb76a-334">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="fb76a-335">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="fb76a-335">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="fb76a-336">классрумфорцеунпромптедаппанддевицелокк</span><span class="sxs-lookup"><span data-stu-id="fb76a-336">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="fb76a-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-337">Boolean</span></span>|<span data-ttu-id="fb76a-338">Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся.</span><span class="sxs-lookup"><span data-stu-id="fb76a-338">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="fb76a-339">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="fb76a-339">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="fb76a-340">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="fb76a-340">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="fb76a-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb76a-341">Boolean</span></span>|<span data-ttu-id="fb76a-342">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве MacOS, на другом устройстве iOS или MacOS (MacOS 10,15 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="fb76a-342">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|
|<span data-ttu-id="fb76a-343">привациакцессконтролс</span><span class="sxs-lookup"><span data-stu-id="fb76a-343">privacyAccessControls</span></span>|<span data-ttu-id="fb76a-344">Коллекция [макоспривациакцессконтролитем](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="fb76a-344">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="fb76a-345">Список элементов управления политикой настройки конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="fb76a-345">List of privacy preference policy controls.</span></span> <span data-ttu-id="fb76a-346">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="fb76a-346">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="fb76a-347">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb76a-347">Response</span></span>
<span data-ttu-id="fb76a-348">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fb76a-348">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb76a-349">Пример</span><span class="sxs-lookup"><span data-stu-id="fb76a-349">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb76a-350">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb76a-350">Request</span></span>
<span data-ttu-id="fb76a-351">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb76a-351">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4640

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
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
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

### <a name="response"></a><span data-ttu-id="fb76a-352">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb76a-352">Response</span></span>
<span data-ttu-id="fb76a-p127">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb76a-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4812

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
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
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




