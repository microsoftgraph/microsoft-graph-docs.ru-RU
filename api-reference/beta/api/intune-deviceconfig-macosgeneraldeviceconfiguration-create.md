---
title: Create macOSGeneralDeviceConfiguration
description: Создание объекта macOSGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ecfedc2b9ef91930f02a7dd29f68065e5ef55354
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947258"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="c9094-103">Create macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9094-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="c9094-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9094-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9094-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9094-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9094-106">Создание объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9094-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9094-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c9094-107">Prerequisites</span></span>
<span data-ttu-id="c9094-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9094-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9094-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9094-110">Permission type</span></span>|<span data-ttu-id="c9094-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9094-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9094-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9094-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9094-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9094-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9094-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9094-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9094-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9094-115">Not supported.</span></span>|
|<span data-ttu-id="c9094-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9094-116">Application</span></span>|<span data-ttu-id="c9094-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9094-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9094-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9094-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c9094-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9094-119">Request headers</span></span>
|<span data-ttu-id="c9094-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9094-120">Header</span></span>|<span data-ttu-id="c9094-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c9094-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9094-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9094-122">Authorization</span></span>|<span data-ttu-id="c9094-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9094-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9094-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c9094-124">Accept</span></span>|<span data-ttu-id="c9094-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c9094-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9094-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c9094-126">Request body</span></span>
<span data-ttu-id="c9094-127">В тексте запроса добавьте представление объекта macOSGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9094-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="c9094-128">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c9094-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="c9094-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9094-129">Property</span></span>|<span data-ttu-id="c9094-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c9094-130">Type</span></span>|<span data-ttu-id="c9094-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c9094-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9094-132">id</span><span class="sxs-lookup"><span data-stu-id="c9094-132">id</span></span>|<span data-ttu-id="c9094-133">String</span><span class="sxs-lookup"><span data-stu-id="c9094-133">String</span></span>|<span data-ttu-id="c9094-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c9094-134">Key of the entity.</span></span> <span data-ttu-id="c9094-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9094-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9094-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9094-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c9094-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9094-137">DateTimeOffset</span></span>|<span data-ttu-id="c9094-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c9094-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c9094-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9094-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9094-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c9094-140">roleScopeTagIds</span></span>|<span data-ttu-id="c9094-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c9094-141">String collection</span></span>|<span data-ttu-id="c9094-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c9094-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c9094-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9094-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9094-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c9094-144">supportsScopeTags</span></span>|<span data-ttu-id="c9094-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-145">Boolean</span></span>|<span data-ttu-id="c9094-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c9094-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c9094-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c9094-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c9094-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c9094-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c9094-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c9094-149">This property is read-only.</span></span> <span data-ttu-id="c9094-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9094-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9094-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c9094-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="c9094-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="c9094-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="c9094-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c9094-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="c9094-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9094-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9094-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c9094-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="c9094-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="c9094-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="c9094-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c9094-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="c9094-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9094-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9094-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c9094-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="c9094-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="c9094-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="c9094-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="c9094-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="c9094-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9094-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9094-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9094-163">createdDateTime</span></span>|<span data-ttu-id="c9094-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9094-164">DateTimeOffset</span></span>|<span data-ttu-id="c9094-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c9094-165">DateTime the object was created.</span></span> <span data-ttu-id="c9094-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9094-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9094-167">description</span><span class="sxs-lookup"><span data-stu-id="c9094-167">description</span></span>|<span data-ttu-id="c9094-168">String</span><span class="sxs-lookup"><span data-stu-id="c9094-168">String</span></span>|<span data-ttu-id="c9094-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c9094-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9094-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9094-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9094-171">displayName</span><span class="sxs-lookup"><span data-stu-id="c9094-171">displayName</span></span>|<span data-ttu-id="c9094-172">Строка</span><span class="sxs-lookup"><span data-stu-id="c9094-172">String</span></span>|<span data-ttu-id="c9094-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c9094-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9094-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c9094-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9094-175">version</span><span class="sxs-lookup"><span data-stu-id="c9094-175">version</span></span>|<span data-ttu-id="c9094-176">Int32</span><span class="sxs-lookup"><span data-stu-id="c9094-176">Int32</span></span>|<span data-ttu-id="c9094-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c9094-177">Version of the device configuration.</span></span> <span data-ttu-id="c9094-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c9094-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9094-179">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="c9094-179">compliantAppsList</span></span>|<span data-ttu-id="c9094-180">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="c9094-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="c9094-181">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="c9094-181">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="c9094-182">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="c9094-182">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="c9094-183">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="c9094-183">compliantAppListType</span></span>|[<span data-ttu-id="c9094-184">Апплисттипе</span><span class="sxs-lookup"><span data-stu-id="c9094-184">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="c9094-185">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="c9094-185">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="c9094-186">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="c9094-186">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="c9094-187">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="c9094-187">emailInDomainSuffixes</span></span>|<span data-ttu-id="c9094-188">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c9094-188">String collection</span></span>|<span data-ttu-id="c9094-189">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="c9094-189">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="c9094-190">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="c9094-190">passwordBlockSimple</span></span>|<span data-ttu-id="c9094-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-191">Boolean</span></span>|<span data-ttu-id="c9094-192">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="c9094-192">Block simple passwords.</span></span>|
|<span data-ttu-id="c9094-193">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c9094-193">passwordExpirationDays</span></span>|<span data-ttu-id="c9094-194">Int32</span><span class="sxs-lookup"><span data-stu-id="c9094-194">Int32</span></span>|<span data-ttu-id="c9094-195">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="c9094-195">Number of days before the password expires.</span></span>|
|<span data-ttu-id="c9094-196">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c9094-196">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c9094-197">Int32</span><span class="sxs-lookup"><span data-stu-id="c9094-197">Int32</span></span>|<span data-ttu-id="c9094-198">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="c9094-198">Number of character sets a password must contain.</span></span> <span data-ttu-id="c9094-199">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="c9094-199">Valid values 0 to 4</span></span>|
|<span data-ttu-id="c9094-200">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c9094-200">passwordMinimumLength</span></span>|<span data-ttu-id="c9094-201">Int32</span><span class="sxs-lookup"><span data-stu-id="c9094-201">Int32</span></span>|<span data-ttu-id="c9094-202">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="c9094-202">Minimum length of passwords.</span></span>|
|<span data-ttu-id="c9094-203">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="c9094-203">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="c9094-204">Int32</span><span class="sxs-lookup"><span data-stu-id="c9094-204">Int32</span></span>|<span data-ttu-id="c9094-205">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="c9094-205">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="c9094-206">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c9094-206">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c9094-207">Int32</span><span class="sxs-lookup"><span data-stu-id="c9094-207">Int32</span></span>|<span data-ttu-id="c9094-208">Период бездействия (в минутах), по истечении которого будет гаснуть экран.</span><span class="sxs-lookup"><span data-stu-id="c9094-208">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="c9094-209">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c9094-209">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c9094-210">Int32</span><span class="sxs-lookup"><span data-stu-id="c9094-210">Int32</span></span>|<span data-ttu-id="c9094-211">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="c9094-211">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="c9094-212">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c9094-212">passwordRequiredType</span></span>|[<span data-ttu-id="c9094-213">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="c9094-213">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c9094-214">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="c9094-214">Type of password that is required.</span></span> <span data-ttu-id="c9094-215">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="c9094-215">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c9094-216">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="c9094-216">passwordRequired</span></span>|<span data-ttu-id="c9094-217">Логический</span><span class="sxs-lookup"><span data-stu-id="c9094-217">Boolean</span></span>|<span data-ttu-id="c9094-218">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="c9094-218">Whether or not to require a password.</span></span>|
|<span data-ttu-id="c9094-219">Кэйчаинблоккклаудсинк</span><span class="sxs-lookup"><span data-stu-id="c9094-219">keychainBlockCloudSync</span></span>|<span data-ttu-id="c9094-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-220">Boolean</span></span>|<span data-ttu-id="c9094-221">Указывает, заблокирована ли синхронизация ключей iCloud для iCloud (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="c9094-221">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="c9094-222">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="c9094-222">airPrintBlocked</span></span>|<span data-ttu-id="c9094-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-223">Boolean</span></span>|<span data-ttu-id="c9094-224">Указывает, заблокировано ли Аирпринт (macOS 10,12 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="c9094-224">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="c9094-225">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="c9094-225">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="c9094-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-226">Boolean</span></span>|<span data-ttu-id="c9094-227">Указывает, требуются ли доверенные сертификаты для обмена данными при печати TLS (macOS 10,13 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="c9094-227">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="c9094-228">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="c9094-228">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="c9094-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-229">Boolean</span></span>|<span data-ttu-id="c9094-230">Указывает, блокируется ли Ибеакон обнаружение принтеров Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="c9094-230">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="c9094-231">Это предотвращает ложные сигналы Аирпринт Bluetooth от фишинга для сетевого трафика (macOS 10,3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="c9094-231">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="c9094-232">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="c9094-232">safariBlockAutofill</span></span>|<span data-ttu-id="c9094-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-233">Boolean</span></span>|<span data-ttu-id="c9094-234">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="c9094-234">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="c9094-235">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="c9094-235">cameraBlocked</span></span>|<span data-ttu-id="c9094-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-236">Boolean</span></span>|<span data-ttu-id="c9094-237">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="c9094-237">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="c9094-238">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="c9094-238">iTunesBlockMusicService</span></span>|<span data-ttu-id="c9094-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-239">Boolean</span></span>|<span data-ttu-id="c9094-240">Указывает, следует ли заблокировать музыкальную службу и вернуть приложение "Музыка" в классический режим.</span><span class="sxs-lookup"><span data-stu-id="c9094-240">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="c9094-241">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="c9094-241">spotlightBlockInternetResults</span></span>|<span data-ttu-id="c9094-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-242">Boolean</span></span>|<span data-ttu-id="c9094-243">Указывает, следует ли запретить получение результатов из поиска в Интернете.</span><span class="sxs-lookup"><span data-stu-id="c9094-243">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="c9094-244">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="c9094-244">keyboardBlockDictation</span></span>|<span data-ttu-id="c9094-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-245">Boolean</span></span>|<span data-ttu-id="c9094-246">Указывает, следует ли запретить пользователю использовать диктовку.</span><span class="sxs-lookup"><span data-stu-id="c9094-246">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="c9094-247">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="c9094-247">definitionLookupBlocked</span></span>|<span data-ttu-id="c9094-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-248">Boolean</span></span>|<span data-ttu-id="c9094-249">Указывает, следует ли заблокировать Поиск определений.</span><span class="sxs-lookup"><span data-stu-id="c9094-249">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="c9094-250">Апплеватчблоккаутаунлокк</span><span class="sxs-lookup"><span data-stu-id="c9094-250">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="c9094-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-251">Boolean</span></span>|<span data-ttu-id="c9094-252">Указывает, следует ли запретить пользователям разблокирование своего Mac-адреса с контрольной записью Apple.</span><span class="sxs-lookup"><span data-stu-id="c9094-252">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="c9094-253">Итунесблоккфилешаринг</span><span class="sxs-lookup"><span data-stu-id="c9094-253">iTunesBlockFileSharing</span></span>|<span data-ttu-id="c9094-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-254">Boolean</span></span>|<span data-ttu-id="c9094-255">Указывает, следует ли запретить передачу файлов с помощью iTunes.</span><span class="sxs-lookup"><span data-stu-id="c9094-255">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="c9094-256">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="c9094-256">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="c9094-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-257">Boolean</span></span>|<span data-ttu-id="c9094-258">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="c9094-258">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="c9094-259">Иклаудблоккмаил</span><span class="sxs-lookup"><span data-stu-id="c9094-259">iCloudBlockMail</span></span>|<span data-ttu-id="c9094-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-260">Boolean</span></span>|<span data-ttu-id="c9094-261">Указывает, следует ли запретить синхронизацию почты для iCloud.</span><span class="sxs-lookup"><span data-stu-id="c9094-261">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="c9094-262">Иклаудблоккаддрессбук</span><span class="sxs-lookup"><span data-stu-id="c9094-262">iCloudBlockAddressBook</span></span>|<span data-ttu-id="c9094-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-263">Boolean</span></span>|<span data-ttu-id="c9094-264">Указывает, следует ли запретить синхронизацию контактов с iCloud.</span><span class="sxs-lookup"><span data-stu-id="c9094-264">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="c9094-265">Иклаудблокккалендар</span><span class="sxs-lookup"><span data-stu-id="c9094-265">iCloudBlockCalendar</span></span>|<span data-ttu-id="c9094-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-266">Boolean</span></span>|<span data-ttu-id="c9094-267">Указывает, следует ли запретить синхронизацию календарей в iCloud.</span><span class="sxs-lookup"><span data-stu-id="c9094-267">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="c9094-268">Иклаудблоккреминдерс</span><span class="sxs-lookup"><span data-stu-id="c9094-268">iCloudBlockReminders</span></span>|<span data-ttu-id="c9094-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-269">Boolean</span></span>|<span data-ttu-id="c9094-270">Указывает, следует ли запретить синхронизацию напоминаний для iCloud.</span><span class="sxs-lookup"><span data-stu-id="c9094-270">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="c9094-271">Иклаудблоккбукмаркс</span><span class="sxs-lookup"><span data-stu-id="c9094-271">iCloudBlockBookmarks</span></span>|<span data-ttu-id="c9094-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-272">Boolean</span></span>|<span data-ttu-id="c9094-273">Указывает, следует ли блокировать синхронизацию закладок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="c9094-273">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="c9094-274">Иклаудблоккнотес</span><span class="sxs-lookup"><span data-stu-id="c9094-274">iCloudBlockNotes</span></span>|<span data-ttu-id="c9094-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-275">Boolean</span></span>|<span data-ttu-id="c9094-276">Указывает, следует ли запретить синхронизацию заметок в iCloud.</span><span class="sxs-lookup"><span data-stu-id="c9094-276">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="c9094-277">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="c9094-277">airDropBlocked</span></span>|<span data-ttu-id="c9094-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-278">Boolean</span></span>|<span data-ttu-id="c9094-279">Указывает, следует ли запретить AirDrop.</span><span class="sxs-lookup"><span data-stu-id="c9094-279">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="c9094-280">Пассвордблоккмодификатион</span><span class="sxs-lookup"><span data-stu-id="c9094-280">passwordBlockModification</span></span>|<span data-ttu-id="c9094-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-281">Boolean</span></span>|<span data-ttu-id="c9094-282">Указывает, следует ли запретить изменение секретного кода.</span><span class="sxs-lookup"><span data-stu-id="c9094-282">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="c9094-283">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c9094-283">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c9094-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-284">Boolean</span></span>|<span data-ttu-id="c9094-285">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="c9094-285">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="c9094-286">Пассвордблоккаутофилл</span><span class="sxs-lookup"><span data-stu-id="c9094-286">passwordBlockAutoFill</span></span>|<span data-ttu-id="c9094-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-287">Boolean</span></span>|<span data-ttu-id="c9094-288">Указывает, следует ли заблокировать функцию автозаполнения паролей.</span><span class="sxs-lookup"><span data-stu-id="c9094-288">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="c9094-289">Пассвордблоккпроксимитирекуестс</span><span class="sxs-lookup"><span data-stu-id="c9094-289">passwordBlockProximityRequests</span></span>|<span data-ttu-id="c9094-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-290">Boolean</span></span>|<span data-ttu-id="c9094-291">Указывает, следует ли запретить запрашивать пароли с ближайших устройств.</span><span class="sxs-lookup"><span data-stu-id="c9094-291">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="c9094-292">Пассвордблоккаирдропшаринг</span><span class="sxs-lookup"><span data-stu-id="c9094-292">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="c9094-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-293">Boolean</span></span>|<span data-ttu-id="c9094-294">Указывает, следует ли заблокировать общий доступ к паролям с помощью функции паролей AirDrop.</span><span class="sxs-lookup"><span data-stu-id="c9094-294">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="c9094-295">Софтвареупдатесенфорцедделайиндайс</span><span class="sxs-lookup"><span data-stu-id="c9094-295">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="c9094-296">Int32</span><span class="sxs-lookup"><span data-stu-id="c9094-296">Int32</span></span>|<span data-ttu-id="c9094-297">Задает число дней, в течение которых обновление программного обеспечения будет делед для защищенного устройства.</span><span class="sxs-lookup"><span data-stu-id="c9094-297">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="c9094-298">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="c9094-298">Valid values 0 to 90</span></span>|
|<span data-ttu-id="c9094-299">Софтвареупдатесфорцеделайед</span><span class="sxs-lookup"><span data-stu-id="c9094-299">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="c9094-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-300">Boolean</span></span>|<span data-ttu-id="c9094-301">Указывает, следует ли откладывать видимость обновлений программного обеспечения, когда устройство находится в защищенном режиме.</span><span class="sxs-lookup"><span data-stu-id="c9094-301">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="c9094-302">Контенткачингблоккед</span><span class="sxs-lookup"><span data-stu-id="c9094-302">contentCachingBlocked</span></span>|<span data-ttu-id="c9094-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-303">Boolean</span></span>|<span data-ttu-id="c9094-304">Указывает, следует ли запретить кэширование контента.</span><span class="sxs-lookup"><span data-stu-id="c9094-304">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="c9094-305">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="c9094-305">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="c9094-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-306">Boolean</span></span>|<span data-ttu-id="c9094-307">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="c9094-307">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="c9094-308">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="c9094-308">screenCaptureBlocked</span></span>|<span data-ttu-id="c9094-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-309">Boolean</span></span>|<span data-ttu-id="c9094-310">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="c9094-310">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="c9094-311">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="c9094-311">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="c9094-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-312">Boolean</span></span>|<span data-ttu-id="c9094-313">Указывает, следует ли запретить удаленное наблюдение за экраном в приложении "аудитория".</span><span class="sxs-lookup"><span data-stu-id="c9094-313">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="c9094-314">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="c9094-314">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="c9094-315">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="c9094-315">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="c9094-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-316">Boolean</span></span>|<span data-ttu-id="c9094-317">Указывает, следует ли автоматически предоставлять разрешение преподавателю управляемого курса в приложении аудитории для просмотра экрана учащегося без выдачи запросов.</span><span class="sxs-lookup"><span data-stu-id="c9094-317">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="c9094-318">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="c9094-318">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="c9094-319">Классрумфорцеаутоматикаллижоинклассес</span><span class="sxs-lookup"><span data-stu-id="c9094-319">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="c9094-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-320">Boolean</span></span>|<span data-ttu-id="c9094-321">Указывает, следует ли автоматически предоставлять разрешение для запросов преподавателя без запроса учащегося.</span><span class="sxs-lookup"><span data-stu-id="c9094-321">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="c9094-322">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="c9094-322">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="c9094-323">Классрумфорцерекуестпермиссионтолеавеклассес</span><span class="sxs-lookup"><span data-stu-id="c9094-323">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="c9094-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-324">Boolean</span></span>|<span data-ttu-id="c9094-325">Указывает, должен ли студент, зарегистрированный в неуправляемом курсе, запрашивать разрешение у преподавателя при попытке выйти из курса.</span><span class="sxs-lookup"><span data-stu-id="c9094-325">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="c9094-326">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="c9094-326">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="c9094-327">Классрумфорцеунпромптедаппанддевицелокк</span><span class="sxs-lookup"><span data-stu-id="c9094-327">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="c9094-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9094-328">Boolean</span></span>|<span data-ttu-id="c9094-329">Указывает, следует ли запретить преподавателю блокировать приложения или устройство, не запрашивая учащихся.</span><span class="sxs-lookup"><span data-stu-id="c9094-329">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="c9094-330">Требует регистрации MDM с помощью Apple School Manager или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="c9094-330">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|



## <a name="response"></a><span data-ttu-id="c9094-331">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9094-331">Response</span></span>
<span data-ttu-id="c9094-332">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c9094-332">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9094-333">Пример</span><span class="sxs-lookup"><span data-stu-id="c9094-333">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9094-334">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9094-334">Request</span></span>
<span data-ttu-id="c9094-335">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9094-335">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 3102

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
  "classroomForceUnpromptedAppAndDeviceLock": true
}
```

### <a name="response"></a><span data-ttu-id="c9094-336">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9094-336">Response</span></span>
<span data-ttu-id="c9094-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9094-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3274

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
  "classroomForceUnpromptedAppAndDeviceLock": true
}
```





