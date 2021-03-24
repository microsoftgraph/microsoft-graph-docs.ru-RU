---
title: Create macOSGeneralDeviceConfiguration
description: Создание объекта macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 343798542aab40e769b18cf8e4a33993d40af3f2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137261"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="f50cc-103">Create macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f50cc-103">Create macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="f50cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f50cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f50cc-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f50cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f50cc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f50cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f50cc-107">Создание объекта [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f50cc-107">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f50cc-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f50cc-108">Prerequisites</span></span>
<span data-ttu-id="f50cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f50cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f50cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f50cc-111">Permission type</span></span>|<span data-ttu-id="f50cc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f50cc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f50cc-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f50cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f50cc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f50cc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f50cc-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f50cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f50cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f50cc-116">Not supported.</span></span>|
|<span data-ttu-id="f50cc-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f50cc-117">Application</span></span>|<span data-ttu-id="f50cc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f50cc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f50cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f50cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f50cc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f50cc-120">Request headers</span></span>
|<span data-ttu-id="f50cc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f50cc-121">Header</span></span>|<span data-ttu-id="f50cc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f50cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f50cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f50cc-123">Authorization</span></span>|<span data-ttu-id="f50cc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f50cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f50cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f50cc-125">Accept</span></span>|<span data-ttu-id="f50cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f50cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f50cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f50cc-127">Request body</span></span>
<span data-ttu-id="f50cc-128">В тексте запроса добавьте представление объекта macOSGeneralDeviceConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f50cc-128">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="f50cc-129">В приведенной ниже таблице показаны, которые необходимо указывать при создании объекта macOSGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f50cc-129">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="f50cc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f50cc-130">Property</span></span>|<span data-ttu-id="f50cc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f50cc-131">Type</span></span>|<span data-ttu-id="f50cc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f50cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f50cc-133">id</span><span class="sxs-lookup"><span data-stu-id="f50cc-133">id</span></span>|<span data-ttu-id="f50cc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f50cc-134">String</span></span>|<span data-ttu-id="f50cc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f50cc-135">Key of the entity.</span></span> <span data-ttu-id="f50cc-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f50cc-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f50cc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f50cc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f50cc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f50cc-138">DateTimeOffset</span></span>|<span data-ttu-id="f50cc-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f50cc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f50cc-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f50cc-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f50cc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f50cc-141">roleScopeTagIds</span></span>|<span data-ttu-id="f50cc-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f50cc-142">String collection</span></span>|<span data-ttu-id="f50cc-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="f50cc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f50cc-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f50cc-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f50cc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f50cc-145">supportsScopeTags</span></span>|<span data-ttu-id="f50cc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-146">Boolean</span></span>|<span data-ttu-id="f50cc-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="f50cc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f50cc-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="f50cc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f50cc-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f50cc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f50cc-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f50cc-150">This property is read-only.</span></span> <span data-ttu-id="f50cc-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f50cc-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f50cc-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f50cc-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f50cc-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f50cc-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f50cc-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f50cc-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f50cc-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f50cc-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f50cc-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f50cc-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f50cc-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f50cc-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f50cc-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f50cc-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f50cc-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f50cc-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f50cc-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f50cc-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f50cc-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f50cc-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f50cc-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="f50cc-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f50cc-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f50cc-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f50cc-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f50cc-164">createdDateTime</span></span>|<span data-ttu-id="f50cc-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f50cc-165">DateTimeOffset</span></span>|<span data-ttu-id="f50cc-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f50cc-166">DateTime the object was created.</span></span> <span data-ttu-id="f50cc-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f50cc-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f50cc-168">description</span><span class="sxs-lookup"><span data-stu-id="f50cc-168">description</span></span>|<span data-ttu-id="f50cc-169">Строка</span><span class="sxs-lookup"><span data-stu-id="f50cc-169">String</span></span>|<span data-ttu-id="f50cc-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f50cc-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f50cc-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f50cc-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f50cc-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f50cc-172">displayName</span></span>|<span data-ttu-id="f50cc-173">Строка</span><span class="sxs-lookup"><span data-stu-id="f50cc-173">String</span></span>|<span data-ttu-id="f50cc-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f50cc-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f50cc-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f50cc-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f50cc-176">version</span><span class="sxs-lookup"><span data-stu-id="f50cc-176">version</span></span>|<span data-ttu-id="f50cc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f50cc-177">Int32</span></span>|<span data-ttu-id="f50cc-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f50cc-178">Version of the device configuration.</span></span> <span data-ttu-id="f50cc-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f50cc-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f50cc-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="f50cc-180">compliantAppsList</span></span>|<span data-ttu-id="f50cc-181">Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="f50cc-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f50cc-182">Список приложений, соответствующих требованиям (список разрешений или блокировок, определяется свойством CompliantAppListType).</span><span class="sxs-lookup"><span data-stu-id="f50cc-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="f50cc-183">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f50cc-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f50cc-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="f50cc-184">compliantAppListType</span></span>|[<span data-ttu-id="f50cc-185">appListType</span><span class="sxs-lookup"><span data-stu-id="f50cc-185">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="f50cc-186">Список, включенный в CompliantAppsList.</span><span class="sxs-lookup"><span data-stu-id="f50cc-186">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="f50cc-187">Возможные значения: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span><span class="sxs-lookup"><span data-stu-id="f50cc-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="f50cc-188">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="f50cc-188">emailInDomainSuffixes</span></span>|<span data-ttu-id="f50cc-189">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f50cc-189">String collection</span></span>|<span data-ttu-id="f50cc-190">Электронный адрес без суффикса, соответствующего одной из этих строк, будет считаться не добавленным в домен.</span><span class="sxs-lookup"><span data-stu-id="f50cc-190">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="f50cc-191">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f50cc-191">passwordBlockSimple</span></span>|<span data-ttu-id="f50cc-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-192">Boolean</span></span>|<span data-ttu-id="f50cc-193">Блокировка простых паролей.</span><span class="sxs-lookup"><span data-stu-id="f50cc-193">Block simple passwords.</span></span>|
|<span data-ttu-id="f50cc-194">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f50cc-194">passwordExpirationDays</span></span>|<span data-ttu-id="f50cc-195">Int32</span><span class="sxs-lookup"><span data-stu-id="f50cc-195">Int32</span></span>|<span data-ttu-id="f50cc-196">Количество дней до окончания срока действия пароля.</span><span class="sxs-lookup"><span data-stu-id="f50cc-196">Number of days before the password expires.</span></span>|
|<span data-ttu-id="f50cc-197">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f50cc-197">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="f50cc-198">Int32</span><span class="sxs-lookup"><span data-stu-id="f50cc-198">Int32</span></span>|<span data-ttu-id="f50cc-199">Количество наборов символов, которые должен содержать пароль.</span><span class="sxs-lookup"><span data-stu-id="f50cc-199">Number of character sets a password must contain.</span></span> <span data-ttu-id="f50cc-200">Допустимые значения: от 0 до 4.</span><span class="sxs-lookup"><span data-stu-id="f50cc-200">Valid values 0 to 4</span></span>|
|<span data-ttu-id="f50cc-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f50cc-201">passwordMinimumLength</span></span>|<span data-ttu-id="f50cc-202">Int32</span><span class="sxs-lookup"><span data-stu-id="f50cc-202">Int32</span></span>|<span data-ttu-id="f50cc-203">Минимальная длина паролей.</span><span class="sxs-lookup"><span data-stu-id="f50cc-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="f50cc-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f50cc-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f50cc-205">Int32</span><span class="sxs-lookup"><span data-stu-id="f50cc-205">Int32</span></span>|<span data-ttu-id="f50cc-206">Период бездействия (в минутах), по истечении которого будет запрашиваться пароль.</span><span class="sxs-lookup"><span data-stu-id="f50cc-206">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="f50cc-207">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f50cc-207">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f50cc-208">Int32</span><span class="sxs-lookup"><span data-stu-id="f50cc-208">Int32</span></span>|<span data-ttu-id="f50cc-209">Период бездействия (в минутах), по истечении которого будет гаснуть экран.</span><span class="sxs-lookup"><span data-stu-id="f50cc-209">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="f50cc-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f50cc-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f50cc-211">Int32</span><span class="sxs-lookup"><span data-stu-id="f50cc-211">Int32</span></span>|<span data-ttu-id="f50cc-212">Количество предыдущих паролей, которые требуется блокировать.</span><span class="sxs-lookup"><span data-stu-id="f50cc-212">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="f50cc-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f50cc-213">passwordRequiredType</span></span>|[<span data-ttu-id="f50cc-214">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f50cc-214">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f50cc-215">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="f50cc-215">Type of password that is required.</span></span> <span data-ttu-id="f50cc-216">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="f50cc-216">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f50cc-217">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="f50cc-217">passwordRequired</span></span>|<span data-ttu-id="f50cc-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-218">Boolean</span></span>|<span data-ttu-id="f50cc-219">Определяет, нужно ли запрашивать ввод пароля.</span><span class="sxs-lookup"><span data-stu-id="f50cc-219">Whether or not to require a password.</span></span>|
|<span data-ttu-id="f50cc-220">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="f50cc-220">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="f50cc-221">Int32</span><span class="sxs-lookup"><span data-stu-id="f50cc-221">Int32</span></span>|<span data-ttu-id="f50cc-222">Количество разрешенных неудачных попыток ввести пароль на экране блокировки устройства.</span><span class="sxs-lookup"><span data-stu-id="f50cc-222">The number of allowed failed attempts to enter the passcode at the device's lock screen.</span></span> <span data-ttu-id="f50cc-223">Допустимые значения от 2 до 11</span><span class="sxs-lookup"><span data-stu-id="f50cc-223">Valid values 2 to 11</span></span>|
|<span data-ttu-id="f50cc-224">passwordMinutesUntilFailedLoginReset</span><span class="sxs-lookup"><span data-stu-id="f50cc-224">passwordMinutesUntilFailedLoginReset</span></span>|<span data-ttu-id="f50cc-225">Int32</span><span class="sxs-lookup"><span data-stu-id="f50cc-225">Int32</span></span>|<span data-ttu-id="f50cc-226">Количество минут до сброса входа после максимального количества неудачных попыток входа.</span><span class="sxs-lookup"><span data-stu-id="f50cc-226">The number of minutes before the login is reset after the maximum number of unsuccessful login attempts is reached.</span></span>|
|<span data-ttu-id="f50cc-227">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="f50cc-227">keychainBlockCloudSync</span></span>|<span data-ttu-id="f50cc-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-228">Boolean</span></span>|<span data-ttu-id="f50cc-229">Указывает, заблокирована ли синхронизация ключей iCloud (macOS 10.12 и более поздней).</span><span class="sxs-lookup"><span data-stu-id="f50cc-229">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="f50cc-230">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="f50cc-230">airPrintBlocked</span></span>|<span data-ttu-id="f50cc-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-231">Boolean</span></span>|<span data-ttu-id="f50cc-232">Указывает, заблокирована или нет AirPrint (macOS 10.12 и более поздней).</span><span class="sxs-lookup"><span data-stu-id="f50cc-232">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="f50cc-233">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="f50cc-233">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="f50cc-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-234">Boolean</span></span>|<span data-ttu-id="f50cc-235">Указывает, требуются ли доверенные сертификаты для связи печати TLS (macOS 10.13 и более поздней).</span><span class="sxs-lookup"><span data-stu-id="f50cc-235">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="f50cc-236">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="f50cc-236">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="f50cc-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-237">Boolean</span></span>|<span data-ttu-id="f50cc-238">Указывает, заблокировано ли обнаружение принтеров AirPrint для iBeacon.</span><span class="sxs-lookup"><span data-stu-id="f50cc-238">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="f50cc-239">Это предотвращает фишинговые маяки Bluetooth AirPrint для сетевого трафика (macOS 10.3 и более поздней).</span><span class="sxs-lookup"><span data-stu-id="f50cc-239">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="f50cc-240">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="f50cc-240">safariBlockAutofill</span></span>|<span data-ttu-id="f50cc-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-241">Boolean</span></span>|<span data-ttu-id="f50cc-242">Указывает, следует ли запретить использовать автозаполнение в Safari.</span><span class="sxs-lookup"><span data-stu-id="f50cc-242">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="f50cc-243">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="f50cc-243">cameraBlocked</span></span>|<span data-ttu-id="f50cc-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-244">Boolean</span></span>|<span data-ttu-id="f50cc-245">Указывает, следует ли запретить доступ к камере устройства.</span><span class="sxs-lookup"><span data-stu-id="f50cc-245">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="f50cc-246">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="f50cc-246">iTunesBlockMusicService</span></span>|<span data-ttu-id="f50cc-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-247">Boolean</span></span>|<span data-ttu-id="f50cc-248">Указывает, следует ли блокировать службу "Музыка" и перенаторять приложение Music в классический режим.</span><span class="sxs-lookup"><span data-stu-id="f50cc-248">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="f50cc-249">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="f50cc-249">spotlightBlockInternetResults</span></span>|<span data-ttu-id="f50cc-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-250">Boolean</span></span>|<span data-ttu-id="f50cc-251">Указывает, следует ли блокировать Spotlight для возврата результатов поиска в Интернете.</span><span class="sxs-lookup"><span data-stu-id="f50cc-251">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="f50cc-252">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="f50cc-252">keyboardBlockDictation</span></span>|<span data-ttu-id="f50cc-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-253">Boolean</span></span>|<span data-ttu-id="f50cc-254">Указывает, следует ли блокировать пользователю использование ввода диктанта.</span><span class="sxs-lookup"><span data-stu-id="f50cc-254">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="f50cc-255">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="f50cc-255">definitionLookupBlocked</span></span>|<span data-ttu-id="f50cc-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-256">Boolean</span></span>|<span data-ttu-id="f50cc-257">Указывает, следует ли блокировать просмотр определения.</span><span class="sxs-lookup"><span data-stu-id="f50cc-257">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="f50cc-258">AppleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="f50cc-258">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="f50cc-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-259">Boolean</span></span>|<span data-ttu-id="f50cc-260">Указывает, следует ли блокировать пользователям разблокировку mac с помощью Apple Watch.</span><span class="sxs-lookup"><span data-stu-id="f50cc-260">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="f50cc-261">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="f50cc-261">iTunesBlockFileSharing</span></span>|<span data-ttu-id="f50cc-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-262">Boolean</span></span>|<span data-ttu-id="f50cc-263">Указывает, следует ли блокировать перенос файлов с помощью iTunes.</span><span class="sxs-lookup"><span data-stu-id="f50cc-263">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="f50cc-264">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="f50cc-264">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="f50cc-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-265">Boolean</span></span>|<span data-ttu-id="f50cc-266">Указывает, следует ли заблокировать синхронизацию документов iCloud.</span><span class="sxs-lookup"><span data-stu-id="f50cc-266">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="f50cc-267">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="f50cc-267">iCloudBlockMail</span></span>|<span data-ttu-id="f50cc-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-268">Boolean</span></span>|<span data-ttu-id="f50cc-269">Указывает, следует ли блокировать iCloud при синхронизации почты.</span><span class="sxs-lookup"><span data-stu-id="f50cc-269">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="f50cc-270">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="f50cc-270">iCloudBlockAddressBook</span></span>|<span data-ttu-id="f50cc-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-271">Boolean</span></span>|<span data-ttu-id="f50cc-272">Указывает, следует ли блокировать iCloud при синхронизации контактов.</span><span class="sxs-lookup"><span data-stu-id="f50cc-272">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="f50cc-273">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="f50cc-273">iCloudBlockCalendar</span></span>|<span data-ttu-id="f50cc-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-274">Boolean</span></span>|<span data-ttu-id="f50cc-275">Указывает, следует ли блокировать iCloud от синхронизации календарей.</span><span class="sxs-lookup"><span data-stu-id="f50cc-275">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="f50cc-276">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="f50cc-276">iCloudBlockReminders</span></span>|<span data-ttu-id="f50cc-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-277">Boolean</span></span>|<span data-ttu-id="f50cc-278">Указывает, следует ли блокировать iCloud при синхронизации напоминаний.</span><span class="sxs-lookup"><span data-stu-id="f50cc-278">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="f50cc-279">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="f50cc-279">iCloudBlockBookmarks</span></span>|<span data-ttu-id="f50cc-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-280">Boolean</span></span>|<span data-ttu-id="f50cc-281">Указывает, следует ли блокировать iCloud при синхронизации закладок.</span><span class="sxs-lookup"><span data-stu-id="f50cc-281">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="f50cc-282">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="f50cc-282">iCloudBlockNotes</span></span>|<span data-ttu-id="f50cc-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-283">Boolean</span></span>|<span data-ttu-id="f50cc-284">Указывает, следует ли блокировать iCloud при синхронизации заметок.</span><span class="sxs-lookup"><span data-stu-id="f50cc-284">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="f50cc-285">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="f50cc-285">airDropBlocked</span></span>|<span data-ttu-id="f50cc-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-286">Boolean</span></span>|<span data-ttu-id="f50cc-287">Указывает, разрешить или не разрешить AirDrop.</span><span class="sxs-lookup"><span data-stu-id="f50cc-287">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="f50cc-288">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="f50cc-288">passwordBlockModification</span></span>|<span data-ttu-id="f50cc-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-289">Boolean</span></span>|<span data-ttu-id="f50cc-290">Указывает, следует ли разрешить изменение пароля.</span><span class="sxs-lookup"><span data-stu-id="f50cc-290">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="f50cc-291">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="f50cc-291">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="f50cc-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-292">Boolean</span></span>|<span data-ttu-id="f50cc-293">Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.</span><span class="sxs-lookup"><span data-stu-id="f50cc-293">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="f50cc-294">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="f50cc-294">passwordBlockAutoFill</span></span>|<span data-ttu-id="f50cc-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-295">Boolean</span></span>|<span data-ttu-id="f50cc-296">Указывает, следует ли блокировать функцию AutoFill Passwords.</span><span class="sxs-lookup"><span data-stu-id="f50cc-296">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="f50cc-297">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="f50cc-297">passwordBlockProximityRequests</span></span>|<span data-ttu-id="f50cc-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-298">Boolean</span></span>|<span data-ttu-id="f50cc-299">Указывает, следует ли блокировать запрашивающие пароли с близлежащих устройств.</span><span class="sxs-lookup"><span data-stu-id="f50cc-299">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="f50cc-300">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="f50cc-300">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="f50cc-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-301">Boolean</span></span>|<span data-ttu-id="f50cc-302">Указывает, следует ли блокировать совместное использование паролей с помощью функции паролей AirDrop.</span><span class="sxs-lookup"><span data-stu-id="f50cc-302">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="f50cc-303">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="f50cc-303">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="f50cc-304">Int32</span><span class="sxs-lookup"><span data-stu-id="f50cc-304">Int32</span></span>|<span data-ttu-id="f50cc-305">Задает время, за которое будет отламывно обновление программного обеспечения для контролируемого устройства.</span><span class="sxs-lookup"><span data-stu-id="f50cc-305">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="f50cc-306">Допустимые значения: от 0 до 90.</span><span class="sxs-lookup"><span data-stu-id="f50cc-306">Valid values 0 to 90</span></span>|
|<span data-ttu-id="f50cc-307">updateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="f50cc-307">updateDelayPolicy</span></span>|[<span data-ttu-id="f50cc-308">macOSSoftwareUpdateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="f50cc-308">macOSSoftwareUpdateDelayPolicy</span></span>](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|<span data-ttu-id="f50cc-309">Определяет, откладывать ли обновления ОС и/или приложений для macOS.</span><span class="sxs-lookup"><span data-stu-id="f50cc-309">Determines whether to delay OS and/or app updates for macOS.</span></span> <span data-ttu-id="f50cc-310">Возможные значения: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span><span class="sxs-lookup"><span data-stu-id="f50cc-310">Possible values are: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span></span>|
|<span data-ttu-id="f50cc-311">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="f50cc-311">contentCachingBlocked</span></span>|<span data-ttu-id="f50cc-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-312">Boolean</span></span>|<span data-ttu-id="f50cc-313">Указывает, следует ли разрешить кэшинг контента.</span><span class="sxs-lookup"><span data-stu-id="f50cc-313">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="f50cc-314">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="f50cc-314">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="f50cc-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-315">Boolean</span></span>|<span data-ttu-id="f50cc-316">Указывает, следует ли заблокировать медиатеку iCloud.</span><span class="sxs-lookup"><span data-stu-id="f50cc-316">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="f50cc-317">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="f50cc-317">screenCaptureBlocked</span></span>|<span data-ttu-id="f50cc-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-318">Boolean</span></span>|<span data-ttu-id="f50cc-319">Указывает, следует ли запретить пользователю делать снимки экрана.</span><span class="sxs-lookup"><span data-stu-id="f50cc-319">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="f50cc-320">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="f50cc-320">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="f50cc-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-321">Boolean</span></span>|<span data-ttu-id="f50cc-322">Указывает, следует ли разрешить удаленное наблюдение экрана в приложении Classroom.</span><span class="sxs-lookup"><span data-stu-id="f50cc-322">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="f50cc-323">Требуется регистрация MDM через менеджера школы Apple или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="f50cc-323">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="f50cc-324">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="f50cc-324">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="f50cc-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-325">Boolean</span></span>|<span data-ttu-id="f50cc-326">Указывает, следует ли автоматически давать преподавателю управляемого курса в приложении Classroom разрешение на просмотр экрана учащегося без запроса.</span><span class="sxs-lookup"><span data-stu-id="f50cc-326">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="f50cc-327">Требуется регистрация MDM через менеджера школы Apple или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="f50cc-327">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="f50cc-328">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="f50cc-328">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="f50cc-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-329">Boolean</span></span>|<span data-ttu-id="f50cc-330">Указывает, следует ли автоматически давать разрешения на запросы преподавателя без запроса учащегося.</span><span class="sxs-lookup"><span data-stu-id="f50cc-330">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="f50cc-331">Требуется регистрация MDM через менеджера школы Apple или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="f50cc-331">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="f50cc-332">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="f50cc-332">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="f50cc-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-333">Boolean</span></span>|<span data-ttu-id="f50cc-334">Указывает, потребуется ли учащемуся, зарегистрированным на неугодном курсе через Класс, запрашивать разрешения у преподавателя при попытке покинуть курс.</span><span class="sxs-lookup"><span data-stu-id="f50cc-334">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="f50cc-335">Требуется регистрация MDM через менеджера школы Apple или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="f50cc-335">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="f50cc-336">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="f50cc-336">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="f50cc-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-337">Boolean</span></span>|<span data-ttu-id="f50cc-338">Указывает, следует ли разрешить преподавателю заблокировать приложения или устройство без запроса учащегося.</span><span class="sxs-lookup"><span data-stu-id="f50cc-338">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="f50cc-339">Требуется регистрация MDM через менеджера школы Apple или Apple Business Manager.</span><span class="sxs-lookup"><span data-stu-id="f50cc-339">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="f50cc-340">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="f50cc-340">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="f50cc-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="f50cc-341">Boolean</span></span>|<span data-ttu-id="f50cc-342">Указывает, следует ли блокировать пользователю продолжение работы, которую они начали на устройстве MacOS на другом устройстве iOS или MacOS (MacOS 10.15 или более поздней).</span><span class="sxs-lookup"><span data-stu-id="f50cc-342">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|
|<span data-ttu-id="f50cc-343">privacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="f50cc-343">privacyAccessControls</span></span>|<span data-ttu-id="f50cc-344">[коллекция macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="f50cc-344">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="f50cc-345">Список элементов управления политиками конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f50cc-345">List of privacy preference policy controls.</span></span> <span data-ttu-id="f50cc-346">Эта коллекция может содержать не более 10 000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f50cc-346">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f50cc-347">Ответ</span><span class="sxs-lookup"><span data-stu-id="f50cc-347">Response</span></span>
<span data-ttu-id="f50cc-348">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f50cc-348">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f50cc-349">Пример</span><span class="sxs-lookup"><span data-stu-id="f50cc-349">Example</span></span>

### <a name="request"></a><span data-ttu-id="f50cc-350">Запрос</span><span class="sxs-lookup"><span data-stu-id="f50cc-350">Request</span></span>
<span data-ttu-id="f50cc-351">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f50cc-351">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="f50cc-352">Отклик</span><span class="sxs-lookup"><span data-stu-id="f50cc-352">Response</span></span>
<span data-ttu-id="f50cc-p127">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f50cc-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




