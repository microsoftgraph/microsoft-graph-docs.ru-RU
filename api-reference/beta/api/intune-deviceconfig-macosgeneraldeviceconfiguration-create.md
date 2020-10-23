---
title: Create macOSGeneralDeviceConfiguration
description: Создание объекта macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee139961988844061258f23f611a2c300464ff55
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724833"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="42851-103">Create macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="42851-103">Create macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="42851-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42851-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42851-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42851-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42851-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42851-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42851-107">Создание объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42851-107">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42851-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="42851-108">Prerequisites</span></span>
<span data-ttu-id="42851-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42851-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42851-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42851-111">Permission type</span></span>|<span data-ttu-id="42851-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="42851-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42851-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42851-113">Delegated (work or school account)</span></span>|<span data-ttu-id="42851-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42851-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="42851-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42851-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42851-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42851-116">Not supported.</span></span>|
|<span data-ttu-id="42851-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42851-117">Application</span></span>|<span data-ttu-id="42851-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42851-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="42851-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42851-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="42851-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="42851-120">Request headers</span></span>
|<span data-ttu-id="42851-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42851-121">Header</span></span>|<span data-ttu-id="42851-122">Значение</span><span class="sxs-lookup"><span data-stu-id="42851-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42851-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42851-123">Authorization</span></span>|<span data-ttu-id="42851-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42851-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42851-125">Accept</span><span class="sxs-lookup"><span data-stu-id="42851-125">Accept</span></span>|<span data-ttu-id="42851-126">application/json</span><span class="sxs-lookup"><span data-stu-id="42851-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42851-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="42851-127">Request body</span></span>
<span data-ttu-id="42851-128">В тексте запроса добавьте представление объекта macOSGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42851-128">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="42851-129">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="42851-129">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="42851-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="42851-130">Property</span></span>|<span data-ttu-id="42851-131">Тип</span><span class="sxs-lookup"><span data-stu-id="42851-131">Type</span></span>|<span data-ttu-id="42851-132">Описание</span><span class="sxs-lookup"><span data-stu-id="42851-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42851-133">id</span><span class="sxs-lookup"><span data-stu-id="42851-133">id</span></span>|<span data-ttu-id="42851-134">Строка</span><span class="sxs-lookup"><span data-stu-id="42851-134">String</span></span>|<span data-ttu-id="42851-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="42851-135">Key of the entity.</span></span> <span data-ttu-id="42851-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42851-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42851-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42851-137">lastModifiedDateTime</span></span>|<span data-ttu-id="42851-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42851-138">DateTimeOffset</span></span>|<span data-ttu-id="42851-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="42851-139">DateTime the object was last modified.</span></span> <span data-ttu-id="42851-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42851-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42851-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="42851-141">roleScopeTagIds</span></span>|<span data-ttu-id="42851-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="42851-142">String collection</span></span>|<span data-ttu-id="42851-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="42851-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="42851-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42851-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42851-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="42851-145">supportsScopeTags</span></span>|<span data-ttu-id="42851-146">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-146">Boolean</span></span>|<span data-ttu-id="42851-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="42851-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="42851-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="42851-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="42851-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="42851-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="42851-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="42851-150">This property is read-only.</span></span> <span data-ttu-id="42851-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42851-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42851-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="42851-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="42851-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="42851-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="42851-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="42851-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="42851-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42851-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42851-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="42851-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="42851-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="42851-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="42851-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="42851-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="42851-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42851-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42851-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="42851-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="42851-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="42851-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="42851-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="42851-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="42851-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42851-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42851-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="42851-164">createdDateTime</span></span>|<span data-ttu-id="42851-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42851-165">DateTimeOffset</span></span>|<span data-ttu-id="42851-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="42851-166">DateTime the object was created.</span></span> <span data-ttu-id="42851-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42851-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42851-168">description</span><span class="sxs-lookup"><span data-stu-id="42851-168">description</span></span>|<span data-ttu-id="42851-169">Строка</span><span class="sxs-lookup"><span data-stu-id="42851-169">String</span></span>|<span data-ttu-id="42851-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42851-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="42851-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42851-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42851-172">displayName</span><span class="sxs-lookup"><span data-stu-id="42851-172">displayName</span></span>|<span data-ttu-id="42851-173">Строка</span><span class="sxs-lookup"><span data-stu-id="42851-173">String</span></span>|<span data-ttu-id="42851-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42851-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="42851-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="42851-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42851-176">version</span><span class="sxs-lookup"><span data-stu-id="42851-176">version</span></span>|<span data-ttu-id="42851-177">Int32</span><span class="sxs-lookup"><span data-stu-id="42851-177">Int32</span></span>|<span data-ttu-id="42851-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="42851-178">Version of the device configuration.</span></span> <span data-ttu-id="42851-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="42851-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="42851-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="42851-180">compliantAppsList</span></span>|<span data-ttu-id="42851-181">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="42851-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="42851-182">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="42851-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="42851-183">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="42851-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="42851-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="42851-184">compliantAppListType</span></span>|[<span data-ttu-id="42851-185">апплисттипе</span><span class="sxs-lookup"><span data-stu-id="42851-185">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="42851-186">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="42851-186">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="42851-187">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="42851-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="42851-188">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="42851-188">emailInDomainSuffixes</span></span>|<span data-ttu-id="42851-189">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="42851-189">String collection</span></span>|<span data-ttu-id="42851-190">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="42851-190">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="42851-191">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="42851-191">passwordBlockSimple</span></span>|<span data-ttu-id="42851-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-192">Boolean</span></span>|<span data-ttu-id="42851-193">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="42851-193">Block simple passwords.</span></span>|
|<span data-ttu-id="42851-194">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="42851-194">passwordExpirationDays</span></span>|<span data-ttu-id="42851-195">Int32</span><span class="sxs-lookup"><span data-stu-id="42851-195">Int32</span></span>|<span data-ttu-id="42851-196">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="42851-196">Number of days before the password expires.</span></span>|
|<span data-ttu-id="42851-197">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="42851-197">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="42851-198">Int32</span><span class="sxs-lookup"><span data-stu-id="42851-198">Int32</span></span>|<span data-ttu-id="42851-199">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="42851-199">Number of character sets a password must contain.</span></span> <span data-ttu-id="42851-200">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="42851-200">Valid values 0 to 4</span></span>|
|<span data-ttu-id="42851-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="42851-201">passwordMinimumLength</span></span>|<span data-ttu-id="42851-202">Int32</span><span class="sxs-lookup"><span data-stu-id="42851-202">Int32</span></span>|<span data-ttu-id="42851-203">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="42851-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="42851-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="42851-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="42851-205">Int32</span><span class="sxs-lookup"><span data-stu-id="42851-205">Int32</span></span>|<span data-ttu-id="42851-206">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="42851-206">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="42851-207">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="42851-207">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="42851-208">Int32</span><span class="sxs-lookup"><span data-stu-id="42851-208">Int32</span></span>|<span data-ttu-id="42851-209">Период бездействия (в минутах), по истечении которого будет гаснуть экран.</span><span class="sxs-lookup"><span data-stu-id="42851-209">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="42851-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="42851-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="42851-211">Int32</span><span class="sxs-lookup"><span data-stu-id="42851-211">Int32</span></span>|<span data-ttu-id="42851-212">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="42851-212">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="42851-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="42851-213">passwordRequiredType</span></span>|[<span data-ttu-id="42851-214">рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="42851-214">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="42851-215">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="42851-215">Type of password that is required.</span></span> <span data-ttu-id="42851-216">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="42851-216">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="42851-217">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="42851-217">passwordRequired</span></span>|<span data-ttu-id="42851-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-218">Boolean</span></span>|<span data-ttu-id="42851-219">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="42851-219">Whether or not to require a password.</span></span>|
|<span data-ttu-id="42851-220">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="42851-220">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="42851-221">Int32</span><span class="sxs-lookup"><span data-stu-id="42851-221">Int32</span></span>|<span data-ttu-id="42851-222">Количество допустимых неудачных попыток ввести секретный код на экран блокировки устройства.</span><span class="sxs-lookup"><span data-stu-id="42851-222">The number of allowed failed attempts to enter the passcode at the device's lock screen.</span></span> <span data-ttu-id="42851-223">Допустимые значения — от 2 до 11</span><span class="sxs-lookup"><span data-stu-id="42851-223">Valid values 2 to 11</span></span>|
|<span data-ttu-id="42851-224">пассвордминутесунтилфаиледлогинресет</span><span class="sxs-lookup"><span data-stu-id="42851-224">passwordMinutesUntilFailedLoginReset</span></span>|<span data-ttu-id="42851-225">Int32</span><span class="sxs-lookup"><span data-stu-id="42851-225">Int32</span></span>|<span data-ttu-id="42851-226">Количество минут до сброса имени входа после того, как будет достигнуто максимальное количество неудачных попыток входа.</span><span class="sxs-lookup"><span data-stu-id="42851-226">The number of minutes before the login is reset after the maximum number of unsuccessful login attempts is reached.</span></span>|
|<span data-ttu-id="42851-227">кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="42851-227">keychainBlockCloudSync</span></span>|<span data-ttu-id="42851-228">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-228">Boolean</span></span>|<span data-ttu-id="42851-229">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="42851-229">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="42851-230">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="42851-230">airPrintBlocked</span></span>|<span data-ttu-id="42851-231">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-231">Boolean</span></span>|<span data-ttu-id="42851-232">Указывает, заблокировано ли Аирпринт (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="42851-232">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="42851-233">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="42851-233">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="42851-234">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-234">Boolean</span></span>|<span data-ttu-id="42851-235">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (macOS 10,13 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="42851-235">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="42851-236">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="42851-236">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="42851-237">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-237">Boolean</span></span>|<span data-ttu-id="42851-238">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="42851-238">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="42851-239">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (macOS 10,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="42851-239">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="42851-240">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="42851-240">safariBlockAutofill</span></span>|<span data-ttu-id="42851-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-241">Boolean</span></span>|<span data-ttu-id="42851-242">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="42851-242">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="42851-243">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="42851-243">cameraBlocked</span></span>|<span data-ttu-id="42851-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-244">Boolean</span></span>|<span data-ttu-id="42851-245">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="42851-245">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="42851-246">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="42851-246">iTunesBlockMusicService</span></span>|<span data-ttu-id="42851-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-247">Boolean</span></span>|<span data-ttu-id="42851-248">Указывает, следует ли заблокировать музыкальную службу и вернуть приложение "Музыка" в классический режим.</span><span class="sxs-lookup"><span data-stu-id="42851-248">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="42851-249">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="42851-249">spotlightBlockInternetResults</span></span>|<span data-ttu-id="42851-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-250">Boolean</span></span>|<span data-ttu-id="42851-251">Указывает, следует ли запретить получение результатов из поиска в Интернете.</span><span class="sxs-lookup"><span data-stu-id="42851-251">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="42851-252">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="42851-252">keyboardBlockDictation</span></span>|<span data-ttu-id="42851-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-253">Boolean</span></span>|<span data-ttu-id="42851-254">Указывает, следует ли запретить пользователю использовать диктовку.</span><span class="sxs-lookup"><span data-stu-id="42851-254">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="42851-255">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="42851-255">definitionLookupBlocked</span></span>|<span data-ttu-id="42851-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-256">Boolean</span></span>|<span data-ttu-id="42851-257">Указывает, следует ли заблокировать Поиск определений.</span><span class="sxs-lookup"><span data-stu-id="42851-257">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="42851-258">апплеватчблоккаутаунлокк</span><span class="sxs-lookup"><span data-stu-id="42851-258">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="42851-259">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-259">Boolean</span></span>|<span data-ttu-id="42851-260">Указывает, следует ли запретить пользователям разблокирование своего Mac-адреса с контрольной записью Apple.</span><span class="sxs-lookup"><span data-stu-id="42851-260">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="42851-261">итунесблоккфилешаринг</span><span class="sxs-lookup"><span data-stu-id="42851-261">iTunesBlockFileSharing</span></span>|<span data-ttu-id="42851-262">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-262">Boolean</span></span>|<span data-ttu-id="42851-263">Указывает, следует ли запретить передачу файлов с помощью iTunes.</span><span class="sxs-lookup"><span data-stu-id="42851-263">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="42851-264">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="42851-264">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="42851-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-265">Boolean</span></span>|<span data-ttu-id="42851-266">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="42851-266">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="42851-267">иклаудблоккмаил</span><span class="sxs-lookup"><span data-stu-id="42851-267">iCloudBlockMail</span></span>|<span data-ttu-id="42851-268">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-268">Boolean</span></span>|<span data-ttu-id="42851-269">Указывает, следует ли запретить синхронизацию почты для iCloud.</span><span class="sxs-lookup"><span data-stu-id="42851-269">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="42851-270">иклаудблоккаддрессбук</span><span class="sxs-lookup"><span data-stu-id="42851-270">iCloudBlockAddressBook</span></span>|<span data-ttu-id="42851-271">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-271">Boolean</span></span>|<span data-ttu-id="42851-272">Указывает, следует ли запретить синхронизацию контактов с iCloud.</span><span class="sxs-lookup"><span data-stu-id="42851-272">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="42851-273">иклаудблокккалендар</span><span class="sxs-lookup"><span data-stu-id="42851-273">iCloudBlockCalendar</span></span>|<span data-ttu-id="42851-274">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-274">Boolean</span></span>|<span data-ttu-id="42851-275">Указывает, следует ли запретить синхронизацию календарей в iCloud.</span><span class="sxs-lookup"><span data-stu-id="42851-275">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="42851-276">иклаудблоккреминдерс</span><span class="sxs-lookup"><span data-stu-id="42851-276">iCloudBlockReminders</span></span>|<span data-ttu-id="42851-277">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-277">Boolean</span></span>|<span data-ttu-id="42851-278">Указывает, следует ли запретить синхронизацию напоминаний для iCloud.</span><span class="sxs-lookup"><span data-stu-id="42851-278">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="42851-279">иклаудблоккбукмаркс</span><span class="sxs-lookup"><span data-stu-id="42851-279">iCloudBlockBookmarks</span></span>|<span data-ttu-id="42851-280">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-280">Boolean</span></span>|<span data-ttu-id="42851-281">Указывает, следует ли блокировать синхронизацию закладок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="42851-281">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="42851-282">иклаудблоккнотес</span><span class="sxs-lookup"><span data-stu-id="42851-282">iCloudBlockNotes</span></span>|<span data-ttu-id="42851-283">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-283">Boolean</span></span>|<span data-ttu-id="42851-284">Указывает, следует ли запретить синхронизацию заметок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="42851-284">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="42851-285">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="42851-285">airDropBlocked</span></span>|<span data-ttu-id="42851-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-286">Boolean</span></span>|<span data-ttu-id="42851-287">Указывает, следует ли запретить AirDrop.</span><span class="sxs-lookup"><span data-stu-id="42851-287">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="42851-288">пассвордблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="42851-288">passwordBlockModification</span></span>|<span data-ttu-id="42851-289">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-289">Boolean</span></span>|<span data-ttu-id="42851-290">Указывает, следует ли запретить изменение секретного кода.</span><span class="sxs-lookup"><span data-stu-id="42851-290">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="42851-291">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="42851-291">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="42851-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-292">Boolean</span></span>|<span data-ttu-id="42851-293">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="42851-293">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="42851-294">пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="42851-294">passwordBlockAutoFill</span></span>|<span data-ttu-id="42851-295">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-295">Boolean</span></span>|<span data-ttu-id="42851-296">Указывает, следует ли заблокировать функцию автозаполнения паролей.</span><span class="sxs-lookup"><span data-stu-id="42851-296">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="42851-297">пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="42851-297">passwordBlockProximityRequests</span></span>|<span data-ttu-id="42851-298">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-298">Boolean</span></span>|<span data-ttu-id="42851-299">Указывает, следует ли запретить запрашивать пароли с ближайших устройств.</span><span class="sxs-lookup"><span data-stu-id="42851-299">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="42851-300">пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="42851-300">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="42851-301">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-301">Boolean</span></span>|<span data-ttu-id="42851-302">Указывает, следует ли заблокировать общий доступ к паролям с помощью функции паролей AirDrop.</span><span class="sxs-lookup"><span data-stu-id="42851-302">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="42851-303">софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="42851-303">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="42851-304">Int32</span><span class="sxs-lookup"><span data-stu-id="42851-304">Int32</span></span>|<span data-ttu-id="42851-305">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="42851-305">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="42851-306">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="42851-306">Valid values 0 to 90</span></span>|
|<span data-ttu-id="42851-307">софтвареупдатесфорцеделайед</span><span class="sxs-lookup"><span data-stu-id="42851-307">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="42851-308">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-308">Boolean</span></span>|<span data-ttu-id="42851-309">Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="42851-309">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="42851-310">упдатеделайполици</span><span class="sxs-lookup"><span data-stu-id="42851-310">updateDelayPolicy</span></span>|[<span data-ttu-id="42851-311">macOSSoftwareUpdateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="42851-311">macOSSoftwareUpdateDelayPolicy</span></span>](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|<span data-ttu-id="42851-312">Определяет, следует ли откладывать обновления для ОС и/или приложений для macOS.</span><span class="sxs-lookup"><span data-stu-id="42851-312">Determines whether to delay OS and/or app updates for macOS.</span></span> <span data-ttu-id="42851-313">Возможные значения: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span><span class="sxs-lookup"><span data-stu-id="42851-313">Possible values are: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span></span>|
|<span data-ttu-id="42851-314">контенткачингблоккед</span><span class="sxs-lookup"><span data-stu-id="42851-314">contentCachingBlocked</span></span>|<span data-ttu-id="42851-315">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-315">Boolean</span></span>|<span data-ttu-id="42851-316">Указывает, следует ли запретить кэширование контента.</span><span class="sxs-lookup"><span data-stu-id="42851-316">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="42851-317">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="42851-317">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="42851-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-318">Boolean</span></span>|<span data-ttu-id="42851-319">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="42851-319">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="42851-320">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="42851-320">screenCaptureBlocked</span></span>|<span data-ttu-id="42851-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-321">Boolean</span></span>|<span data-ttu-id="42851-322">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="42851-322">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="42851-323">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="42851-323">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="42851-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-324">Boolean</span></span>|<span data-ttu-id="42851-325">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "аудитория".</span><span class="sxs-lookup"><span data-stu-id="42851-325">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="42851-326">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="42851-326">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="42851-327">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="42851-327">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="42851-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-328">Boolean</span></span>|<span data-ttu-id="42851-329">Указывает, следует ли автоматически предоставлять разрешение преподавателю управляемого курса в приложении аудитории для просмотра экрана учащегося без выдачи запросов.</span><span class="sxs-lookup"><span data-stu-id="42851-329">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="42851-330">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="42851-330">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="42851-331">классрумфорцеаутоматикаллижоинклассес</span><span class="sxs-lookup"><span data-stu-id="42851-331">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="42851-332">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-332">Boolean</span></span>|<span data-ttu-id="42851-333">Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося.</span><span class="sxs-lookup"><span data-stu-id="42851-333">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="42851-334">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="42851-334">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="42851-335">классрумфорцерекуестпермиссионтолеавеклассес</span><span class="sxs-lookup"><span data-stu-id="42851-335">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="42851-336">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-336">Boolean</span></span>|<span data-ttu-id="42851-337">Указывает, должен ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса.</span><span class="sxs-lookup"><span data-stu-id="42851-337">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="42851-338">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="42851-338">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="42851-339">классрумфорцеунпромптедаппанддевицелокк</span><span class="sxs-lookup"><span data-stu-id="42851-339">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="42851-340">Логический</span><span class="sxs-lookup"><span data-stu-id="42851-340">Boolean</span></span>|<span data-ttu-id="42851-341">Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся.</span><span class="sxs-lookup"><span data-stu-id="42851-341">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="42851-342">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="42851-342">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="42851-343">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="42851-343">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="42851-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="42851-344">Boolean</span></span>|<span data-ttu-id="42851-345">Указывает, следует ли запретить пользователю продолжать работу, начатую на устройстве MacOS, на другом устройстве iOS или MacOS (MacOS 10,15 или более поздней версии).</span><span class="sxs-lookup"><span data-stu-id="42851-345">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|
|<span data-ttu-id="42851-346">привациакцессконтролс</span><span class="sxs-lookup"><span data-stu-id="42851-346">privacyAccessControls</span></span>|<span data-ttu-id="42851-347">Коллекция [макоспривациакцессконтролитем](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="42851-347">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="42851-348">Список элементов управления политикой настройки конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="42851-348">List of privacy preference policy controls.</span></span> <span data-ttu-id="42851-349">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="42851-349">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="42851-350">Ответ</span><span class="sxs-lookup"><span data-stu-id="42851-350">Response</span></span>
<span data-ttu-id="42851-351">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="42851-351">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42851-352">Пример</span><span class="sxs-lookup"><span data-stu-id="42851-352">Example</span></span>

### <a name="request"></a><span data-ttu-id="42851-353">Запрос</span><span class="sxs-lookup"><span data-stu-id="42851-353">Request</span></span>
<span data-ttu-id="42851-354">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42851-354">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4680

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

### <a name="response"></a><span data-ttu-id="42851-355">Отклик</span><span class="sxs-lookup"><span data-stu-id="42851-355">Response</span></span>
<span data-ttu-id="42851-p127">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="42851-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4852

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





