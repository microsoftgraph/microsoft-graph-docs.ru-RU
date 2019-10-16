---
title: Create macOSGeneralDeviceConfiguration
description: Создание объекта macOSGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 183013fb06d1fef856ab4f2d5c717d627bab0ddd
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533590"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="fa332-103">Create macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="fa332-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="fa332-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa332-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa332-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa332-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa332-106">Создание объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa332-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa332-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fa332-107">Prerequisites</span></span>
<span data-ttu-id="fa332-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa332-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa332-110">Permission type</span></span>|<span data-ttu-id="fa332-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa332-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa332-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa332-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa332-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa332-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa332-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa332-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa332-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa332-115">Not supported.</span></span>|
|<span data-ttu-id="fa332-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="fa332-116">Application</span></span>|<span data-ttu-id="fa332-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa332-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa332-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa332-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa332-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa332-119">Request headers</span></span>
|<span data-ttu-id="fa332-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa332-120">Header</span></span>|<span data-ttu-id="fa332-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fa332-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa332-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa332-122">Authorization</span></span>|<span data-ttu-id="fa332-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa332-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa332-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fa332-124">Accept</span></span>|<span data-ttu-id="fa332-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa332-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa332-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa332-126">Request body</span></span>
<span data-ttu-id="fa332-127">В тексте запроса добавьте представление объекта macOSGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa332-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="fa332-128">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fa332-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="fa332-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa332-129">Property</span></span>|<span data-ttu-id="fa332-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fa332-130">Type</span></span>|<span data-ttu-id="fa332-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fa332-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa332-132">id</span><span class="sxs-lookup"><span data-stu-id="fa332-132">id</span></span>|<span data-ttu-id="fa332-133">String</span><span class="sxs-lookup"><span data-stu-id="fa332-133">String</span></span>|<span data-ttu-id="fa332-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fa332-134">Key of the entity.</span></span> <span data-ttu-id="fa332-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa332-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa332-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa332-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fa332-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa332-137">DateTimeOffset</span></span>|<span data-ttu-id="fa332-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fa332-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fa332-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa332-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa332-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fa332-140">roleScopeTagIds</span></span>|<span data-ttu-id="fa332-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa332-141">String collection</span></span>|<span data-ttu-id="fa332-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="fa332-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fa332-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa332-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa332-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="fa332-144">supportsScopeTags</span></span>|<span data-ttu-id="fa332-145">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-145">Boolean</span></span>|<span data-ttu-id="fa332-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="fa332-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fa332-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="fa332-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fa332-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="fa332-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fa332-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fa332-149">This property is read-only.</span></span> <span data-ttu-id="fa332-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa332-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa332-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fa332-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fa332-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fa332-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fa332-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fa332-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fa332-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa332-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa332-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fa332-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fa332-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fa332-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fa332-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fa332-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fa332-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa332-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa332-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fa332-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fa332-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="fa332-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fa332-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="fa332-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fa332-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa332-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa332-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa332-163">createdDateTime</span></span>|<span data-ttu-id="fa332-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa332-164">DateTimeOffset</span></span>|<span data-ttu-id="fa332-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fa332-165">DateTime the object was created.</span></span> <span data-ttu-id="fa332-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa332-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa332-167">description</span><span class="sxs-lookup"><span data-stu-id="fa332-167">description</span></span>|<span data-ttu-id="fa332-168">String</span><span class="sxs-lookup"><span data-stu-id="fa332-168">String</span></span>|<span data-ttu-id="fa332-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fa332-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fa332-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa332-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa332-171">displayName</span><span class="sxs-lookup"><span data-stu-id="fa332-171">displayName</span></span>|<span data-ttu-id="fa332-172">Строка</span><span class="sxs-lookup"><span data-stu-id="fa332-172">String</span></span>|<span data-ttu-id="fa332-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fa332-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fa332-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fa332-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa332-175">version</span><span class="sxs-lookup"><span data-stu-id="fa332-175">version</span></span>|<span data-ttu-id="fa332-176">Int32</span><span class="sxs-lookup"><span data-stu-id="fa332-176">Int32</span></span>|<span data-ttu-id="fa332-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fa332-177">Version of the device configuration.</span></span> <span data-ttu-id="fa332-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fa332-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fa332-179">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="fa332-179">compliantAppsList</span></span>|<span data-ttu-id="fa332-180">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="fa332-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="fa332-181">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="fa332-181">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="fa332-182">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="fa332-182">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="fa332-183">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="fa332-183">compliantAppListType</span></span>|[<span data-ttu-id="fa332-184">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="fa332-184">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="fa332-185">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="fa332-185">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="fa332-186">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="fa332-186">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="fa332-187">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="fa332-187">emailInDomainSuffixes</span></span>|<span data-ttu-id="fa332-188">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fa332-188">String collection</span></span>|<span data-ttu-id="fa332-189">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="fa332-189">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="fa332-190">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="fa332-190">passwordBlockSimple</span></span>|<span data-ttu-id="fa332-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa332-191">Boolean</span></span>|<span data-ttu-id="fa332-192">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="fa332-192">Block simple passwords.</span></span>|
|<span data-ttu-id="fa332-193">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="fa332-193">passwordExpirationDays</span></span>|<span data-ttu-id="fa332-194">Int32</span><span class="sxs-lookup"><span data-stu-id="fa332-194">Int32</span></span>|<span data-ttu-id="fa332-195">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="fa332-195">Number of days before the password expires.</span></span>|
|<span data-ttu-id="fa332-196">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="fa332-196">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="fa332-197">Int32</span><span class="sxs-lookup"><span data-stu-id="fa332-197">Int32</span></span>|<span data-ttu-id="fa332-198">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="fa332-198">Number of character sets a password must contain.</span></span> <span data-ttu-id="fa332-199">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="fa332-199">Valid values 0 to 4</span></span>|
|<span data-ttu-id="fa332-200">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="fa332-200">passwordMinimumLength</span></span>|<span data-ttu-id="fa332-201">Int32</span><span class="sxs-lookup"><span data-stu-id="fa332-201">Int32</span></span>|<span data-ttu-id="fa332-202">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="fa332-202">Minimum length of passwords.</span></span>|
|<span data-ttu-id="fa332-203">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="fa332-203">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="fa332-204">Int32</span><span class="sxs-lookup"><span data-stu-id="fa332-204">Int32</span></span>|<span data-ttu-id="fa332-205">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="fa332-205">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="fa332-206">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="fa332-206">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="fa332-207">Int32</span><span class="sxs-lookup"><span data-stu-id="fa332-207">Int32</span></span>|<span data-ttu-id="fa332-208">Период бездействия (в минутах), по истечении которого будет гаснуть экран.</span><span class="sxs-lookup"><span data-stu-id="fa332-208">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="fa332-209">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="fa332-209">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="fa332-210">Int32</span><span class="sxs-lookup"><span data-stu-id="fa332-210">Int32</span></span>|<span data-ttu-id="fa332-211">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="fa332-211">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="fa332-212">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="fa332-212">passwordRequiredType</span></span>|[<span data-ttu-id="fa332-213">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="fa332-213">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="fa332-214">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="fa332-214">Type of password that is required.</span></span> <span data-ttu-id="fa332-215">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="fa332-215">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="fa332-216">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="fa332-216">passwordRequired</span></span>|<span data-ttu-id="fa332-217">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-217">Boolean</span></span>|<span data-ttu-id="fa332-218">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="fa332-218">Whether or not to require a password.</span></span>|
|<span data-ttu-id="fa332-219">кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="fa332-219">keychainBlockCloudSync</span></span>|<span data-ttu-id="fa332-220">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-220">Boolean</span></span>|<span data-ttu-id="fa332-221">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="fa332-221">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="fa332-222">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="fa332-222">airPrintBlocked</span></span>|<span data-ttu-id="fa332-223">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-223">Boolean</span></span>|<span data-ttu-id="fa332-224">Указывает, заблокировано ли Аирпринт (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="fa332-224">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="fa332-225">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="fa332-225">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="fa332-226">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-226">Boolean</span></span>|<span data-ttu-id="fa332-227">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (macOS 10,13 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="fa332-227">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="fa332-228">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="fa332-228">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="fa332-229">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-229">Boolean</span></span>|<span data-ttu-id="fa332-230">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="fa332-230">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="fa332-231">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (macOS 10,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="fa332-231">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="fa332-232">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="fa332-232">safariBlockAutofill</span></span>|<span data-ttu-id="fa332-233">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-233">Boolean</span></span>|<span data-ttu-id="fa332-234">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="fa332-234">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="fa332-235">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="fa332-235">cameraBlocked</span></span>|<span data-ttu-id="fa332-236">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-236">Boolean</span></span>|<span data-ttu-id="fa332-237">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="fa332-237">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="fa332-238">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="fa332-238">iTunesBlockMusicService</span></span>|<span data-ttu-id="fa332-239">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-239">Boolean</span></span>|<span data-ttu-id="fa332-240">Указывает, следует ли заблокировать музыкальную службу и вернуть приложение "Музыка" в классический режим.</span><span class="sxs-lookup"><span data-stu-id="fa332-240">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="fa332-241">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="fa332-241">spotlightBlockInternetResults</span></span>|<span data-ttu-id="fa332-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa332-242">Boolean</span></span>|<span data-ttu-id="fa332-243">Указывает, следует ли запретить получение результатов из поиска в Интернете.</span><span class="sxs-lookup"><span data-stu-id="fa332-243">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="fa332-244">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="fa332-244">keyboardBlockDictation</span></span>|<span data-ttu-id="fa332-245">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-245">Boolean</span></span>|<span data-ttu-id="fa332-246">Указывает, следует ли запретить пользователю использовать диктовку.</span><span class="sxs-lookup"><span data-stu-id="fa332-246">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="fa332-247">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="fa332-247">definitionLookupBlocked</span></span>|<span data-ttu-id="fa332-248">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-248">Boolean</span></span>|<span data-ttu-id="fa332-249">Указывает, следует ли заблокировать Поиск определений.</span><span class="sxs-lookup"><span data-stu-id="fa332-249">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="fa332-250">апплеватчблоккаутаунлокк</span><span class="sxs-lookup"><span data-stu-id="fa332-250">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="fa332-251">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-251">Boolean</span></span>|<span data-ttu-id="fa332-252">Указывает, следует ли запретить пользователям разблокирование своего Mac-адреса с контрольной записью Apple.</span><span class="sxs-lookup"><span data-stu-id="fa332-252">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="fa332-253">итунесблоккфилешаринг</span><span class="sxs-lookup"><span data-stu-id="fa332-253">iTunesBlockFileSharing</span></span>|<span data-ttu-id="fa332-254">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-254">Boolean</span></span>|<span data-ttu-id="fa332-255">Указывает, следует ли запретить передачу файлов с помощью iTunes.</span><span class="sxs-lookup"><span data-stu-id="fa332-255">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="fa332-256">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="fa332-256">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="fa332-257">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-257">Boolean</span></span>|<span data-ttu-id="fa332-258">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="fa332-258">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="fa332-259">иклаудблоккмаил</span><span class="sxs-lookup"><span data-stu-id="fa332-259">iCloudBlockMail</span></span>|<span data-ttu-id="fa332-260">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-260">Boolean</span></span>|<span data-ttu-id="fa332-261">Указывает, следует ли запретить синхронизацию почты для iCloud.</span><span class="sxs-lookup"><span data-stu-id="fa332-261">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="fa332-262">иклаудблоккаддрессбук</span><span class="sxs-lookup"><span data-stu-id="fa332-262">iCloudBlockAddressBook</span></span>|<span data-ttu-id="fa332-263">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-263">Boolean</span></span>|<span data-ttu-id="fa332-264">Указывает, следует ли запретить синхронизацию контактов с iCloud.</span><span class="sxs-lookup"><span data-stu-id="fa332-264">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="fa332-265">иклаудблокккалендар</span><span class="sxs-lookup"><span data-stu-id="fa332-265">iCloudBlockCalendar</span></span>|<span data-ttu-id="fa332-266">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-266">Boolean</span></span>|<span data-ttu-id="fa332-267">Указывает, следует ли запретить синхронизацию календарей в iCloud.</span><span class="sxs-lookup"><span data-stu-id="fa332-267">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="fa332-268">иклаудблоккреминдерс</span><span class="sxs-lookup"><span data-stu-id="fa332-268">iCloudBlockReminders</span></span>|<span data-ttu-id="fa332-269">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-269">Boolean</span></span>|<span data-ttu-id="fa332-270">Указывает, следует ли запретить синхронизацию напоминаний для iCloud.</span><span class="sxs-lookup"><span data-stu-id="fa332-270">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="fa332-271">иклаудблоккбукмаркс</span><span class="sxs-lookup"><span data-stu-id="fa332-271">iCloudBlockBookmarks</span></span>|<span data-ttu-id="fa332-272">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-272">Boolean</span></span>|<span data-ttu-id="fa332-273">Указывает, следует ли блокировать синхронизацию закладок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="fa332-273">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="fa332-274">иклаудблоккнотес</span><span class="sxs-lookup"><span data-stu-id="fa332-274">iCloudBlockNotes</span></span>|<span data-ttu-id="fa332-275">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-275">Boolean</span></span>|<span data-ttu-id="fa332-276">Указывает, следует ли запретить синхронизацию заметок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="fa332-276">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="fa332-277">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="fa332-277">airDropBlocked</span></span>|<span data-ttu-id="fa332-278">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-278">Boolean</span></span>|<span data-ttu-id="fa332-279">Указывает, следует ли запретить AirDrop.</span><span class="sxs-lookup"><span data-stu-id="fa332-279">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="fa332-280">пассвордблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="fa332-280">passwordBlockModification</span></span>|<span data-ttu-id="fa332-281">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-281">Boolean</span></span>|<span data-ttu-id="fa332-282">Указывает, следует ли запретить изменение секретного кода.</span><span class="sxs-lookup"><span data-stu-id="fa332-282">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="fa332-283">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="fa332-283">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="fa332-284">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-284">Boolean</span></span>|<span data-ttu-id="fa332-285">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="fa332-285">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="fa332-286">пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="fa332-286">passwordBlockAutoFill</span></span>|<span data-ttu-id="fa332-287">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-287">Boolean</span></span>|<span data-ttu-id="fa332-288">Указывает, следует ли заблокировать функцию автозаполнения паролей.</span><span class="sxs-lookup"><span data-stu-id="fa332-288">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="fa332-289">пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="fa332-289">passwordBlockProximityRequests</span></span>|<span data-ttu-id="fa332-290">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-290">Boolean</span></span>|<span data-ttu-id="fa332-291">Указывает, следует ли запретить запрашивать пароли с ближайших устройств.</span><span class="sxs-lookup"><span data-stu-id="fa332-291">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="fa332-292">пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="fa332-292">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="fa332-293">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-293">Boolean</span></span>|<span data-ttu-id="fa332-294">Указывает, следует ли заблокировать общий доступ к паролям с помощью функции паролей AirDrop.</span><span class="sxs-lookup"><span data-stu-id="fa332-294">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="fa332-295">софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="fa332-295">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="fa332-296">Int32</span><span class="sxs-lookup"><span data-stu-id="fa332-296">Int32</span></span>|<span data-ttu-id="fa332-297">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="fa332-297">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="fa332-298">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="fa332-298">Valid values 0 to 90</span></span>|
|<span data-ttu-id="fa332-299">софтвареупдатесфорцеделайед</span><span class="sxs-lookup"><span data-stu-id="fa332-299">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="fa332-300">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-300">Boolean</span></span>|<span data-ttu-id="fa332-301">Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="fa332-301">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="fa332-302">контенткачингблоккед</span><span class="sxs-lookup"><span data-stu-id="fa332-302">contentCachingBlocked</span></span>|<span data-ttu-id="fa332-303">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-303">Boolean</span></span>|<span data-ttu-id="fa332-304">Указывает, следует ли запретить кэширование контента.</span><span class="sxs-lookup"><span data-stu-id="fa332-304">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="fa332-305">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="fa332-305">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="fa332-306">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-306">Boolean</span></span>|<span data-ttu-id="fa332-307">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="fa332-307">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="fa332-308">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="fa332-308">screenCaptureBlocked</span></span>|<span data-ttu-id="fa332-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa332-309">Boolean</span></span>|<span data-ttu-id="fa332-310">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="fa332-310">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="fa332-311">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="fa332-311">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="fa332-312">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-312">Boolean</span></span>|<span data-ttu-id="fa332-313">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "аудитория".</span><span class="sxs-lookup"><span data-stu-id="fa332-313">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="fa332-314">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="fa332-314">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="fa332-315">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="fa332-315">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="fa332-316">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-316">Boolean</span></span>|<span data-ttu-id="fa332-317">Указывает, следует ли автоматически предоставлять разрешение преподавателю управляемого курса в приложении аудитории для просмотра экрана учащегося без выдачи запросов.</span><span class="sxs-lookup"><span data-stu-id="fa332-317">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="fa332-318">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="fa332-318">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="fa332-319">классрумфорцеаутоматикаллижоинклассес</span><span class="sxs-lookup"><span data-stu-id="fa332-319">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="fa332-320">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-320">Boolean</span></span>|<span data-ttu-id="fa332-321">Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося.</span><span class="sxs-lookup"><span data-stu-id="fa332-321">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="fa332-322">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="fa332-322">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="fa332-323">классрумфорцерекуестпермиссионтолеавеклассес</span><span class="sxs-lookup"><span data-stu-id="fa332-323">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="fa332-324">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-324">Boolean</span></span>|<span data-ttu-id="fa332-325">Указывает, должен ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса.</span><span class="sxs-lookup"><span data-stu-id="fa332-325">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="fa332-326">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="fa332-326">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="fa332-327">классрумфорцеунпромптедаппанддевицелокк</span><span class="sxs-lookup"><span data-stu-id="fa332-327">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="fa332-328">Логический</span><span class="sxs-lookup"><span data-stu-id="fa332-328">Boolean</span></span>|<span data-ttu-id="fa332-329">Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся.</span><span class="sxs-lookup"><span data-stu-id="fa332-329">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="fa332-330">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="fa332-330">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="fa332-331">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="fa332-331">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="fa332-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa332-332">Boolean</span></span>|<span data-ttu-id="fa332-333">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве MacOS, на другом устройстве iOS или MacOS (MacOS 10,15 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="fa332-333">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="fa332-334">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa332-334">Response</span></span>
<span data-ttu-id="fa332-335">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fa332-335">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa332-336">Пример</span><span class="sxs-lookup"><span data-stu-id="fa332-336">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa332-337">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa332-337">Request</span></span>
<span data-ttu-id="fa332-338">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa332-338">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="fa332-339">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa332-339">Response</span></span>
<span data-ttu-id="fa332-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa332-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






