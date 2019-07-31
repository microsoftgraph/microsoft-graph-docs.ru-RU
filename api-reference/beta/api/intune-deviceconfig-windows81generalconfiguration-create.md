---
title: Создание windows81GeneralConfiguration
description: Создание объекта windows81GeneralConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: be8f9d72a6ce7b2e3a43c5f8cffe697c58866e07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975027"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="d8fdf-103">Создание windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8fdf-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="d8fdf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8fdf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8fdf-106">Создание объекта [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-106">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8fdf-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d8fdf-107">Prerequisites</span></span>
<span data-ttu-id="d8fdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8fdf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8fdf-110">Permission type</span></span>|<span data-ttu-id="d8fdf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8fdf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8fdf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8fdf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8fdf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8fdf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8fdf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8fdf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8fdf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-115">Not supported.</span></span>|
|<span data-ttu-id="d8fdf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8fdf-116">Application</span></span>|<span data-ttu-id="d8fdf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8fdf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8fdf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d8fdf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8fdf-119">Request headers</span></span>
|<span data-ttu-id="d8fdf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8fdf-120">Header</span></span>|<span data-ttu-id="d8fdf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d8fdf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8fdf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8fdf-122">Authorization</span></span>|<span data-ttu-id="d8fdf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8fdf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d8fdf-124">Accept</span></span>|<span data-ttu-id="d8fdf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8fdf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8fdf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8fdf-126">Request body</span></span>
<span data-ttu-id="d8fdf-127">В теле запроса добавьте представление объекта windows81GeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-127">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="d8fdf-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта windows81GeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-128">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="d8fdf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8fdf-129">Property</span></span>|<span data-ttu-id="d8fdf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d8fdf-130">Type</span></span>|<span data-ttu-id="d8fdf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d8fdf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8fdf-132">id</span><span class="sxs-lookup"><span data-stu-id="d8fdf-132">id</span></span>|<span data-ttu-id="d8fdf-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d8fdf-133">String</span></span>|<span data-ttu-id="d8fdf-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-134">Key of the entity.</span></span> <span data-ttu-id="d8fdf-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fdf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8fdf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d8fdf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8fdf-137">DateTimeOffset</span></span>|<span data-ttu-id="d8fdf-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d8fdf-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fdf-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8fdf-140">roleScopeTagIds</span></span>|<span data-ttu-id="d8fdf-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d8fdf-141">String collection</span></span>|<span data-ttu-id="d8fdf-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d8fdf-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fdf-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="d8fdf-144">supportsScopeTags</span></span>|<span data-ttu-id="d8fdf-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-145">Boolean</span></span>|<span data-ttu-id="d8fdf-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d8fdf-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d8fdf-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d8fdf-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-149">This property is read-only.</span></span> <span data-ttu-id="d8fdf-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fdf-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d8fdf-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d8fdf-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d8fdf-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d8fdf-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d8fdf-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fdf-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d8fdf-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d8fdf-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d8fdf-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d8fdf-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d8fdf-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fdf-159">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d8fdf-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d8fdf-160">Девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="d8fdf-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d8fdf-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d8fdf-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fdf-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8fdf-163">createdDateTime</span></span>|<span data-ttu-id="d8fdf-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8fdf-164">DateTimeOffset</span></span>|<span data-ttu-id="d8fdf-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-165">DateTime the object was created.</span></span> <span data-ttu-id="d8fdf-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fdf-167">description</span><span class="sxs-lookup"><span data-stu-id="d8fdf-167">description</span></span>|<span data-ttu-id="d8fdf-168">String</span><span class="sxs-lookup"><span data-stu-id="d8fdf-168">String</span></span>|<span data-ttu-id="d8fdf-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d8fdf-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fdf-171">displayName</span><span class="sxs-lookup"><span data-stu-id="d8fdf-171">displayName</span></span>|<span data-ttu-id="d8fdf-172">Строка</span><span class="sxs-lookup"><span data-stu-id="d8fdf-172">String</span></span>|<span data-ttu-id="d8fdf-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d8fdf-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fdf-175">version</span><span class="sxs-lookup"><span data-stu-id="d8fdf-175">version</span></span>|<span data-ttu-id="d8fdf-176">Int32</span><span class="sxs-lookup"><span data-stu-id="d8fdf-176">Int32</span></span>|<span data-ttu-id="d8fdf-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-177">Version of the device configuration.</span></span> <span data-ttu-id="d8fdf-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d8fdf-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8fdf-179">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="d8fdf-179">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="d8fdf-180">Логический</span><span class="sxs-lookup"><span data-stu-id="d8fdf-180">Boolean</span></span>|<span data-ttu-id="d8fdf-181">Указывает, следует ли запретить пользователю добавлять учетные записи электронной почты на устройства, не связанные с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-181">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="d8fdf-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="d8fdf-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="d8fdf-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-183">Boolean</span></span>|<span data-ttu-id="d8fdf-184">Указывает, применяется ли эта политика только к Windows 8.1.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="d8fdf-185">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-185">This property is read-only.</span></span>|
|<span data-ttu-id="d8fdf-186">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="d8fdf-186">browserBlockAutofill</span></span>|<span data-ttu-id="d8fdf-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-187">Boolean</span></span>|<span data-ttu-id="d8fdf-188">Указывает, следует ли заблокировать автозаполнение.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-188">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="d8fdf-189">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="d8fdf-189">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="d8fdf-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-190">Boolean</span></span>|<span data-ttu-id="d8fdf-191">Указывает, следует ли заблокировать автоматическое обнаружение сайтов интрасети.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-191">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="d8fdf-192">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="d8fdf-192">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="d8fdf-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-193">Boolean</span></span>|<span data-ttu-id="d8fdf-194">Указывает, следует ли заблокировать доступ к корпоративному режиму.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-194">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="d8fdf-195">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="d8fdf-195">browserBlockJavaScript</span></span>|<span data-ttu-id="d8fdf-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-196">Boolean</span></span>|<span data-ttu-id="d8fdf-197">Указывает, следует ли запретить использование JavaScript.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-197">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="d8fdf-198">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="d8fdf-198">browserBlockPlugins</span></span>|<span data-ttu-id="d8fdf-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-199">Boolean</span></span>|<span data-ttu-id="d8fdf-200">Указывает, следует ли заблокировать подключаемые модули.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-200">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="d8fdf-201">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="d8fdf-201">browserBlockPopups</span></span>|<span data-ttu-id="d8fdf-202">Логический</span><span class="sxs-lookup"><span data-stu-id="d8fdf-202">Boolean</span></span>|<span data-ttu-id="d8fdf-203">Указывает, следует ли блокировать всплывающие окна.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-203">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="d8fdf-204">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="d8fdf-204">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="d8fdf-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-205">Boolean</span></span>|<span data-ttu-id="d8fdf-206">Указывает, следует ли запретить пользователю отправлять заголовок DNT.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-206">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="d8fdf-207">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="d8fdf-207">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="d8fdf-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-208">Boolean</span></span>|<span data-ttu-id="d8fdf-209">Указывает, следует ли блокировать переход на сайты интрасети при вводе одного слова.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-209">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="d8fdf-210">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="d8fdf-210">browserRequireSmartScreen</span></span>|<span data-ttu-id="d8fdf-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-211">Boolean</span></span>|<span data-ttu-id="d8fdf-212">Указывает, обязательно ли использовать фильтр Smart Screen.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-212">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="d8fdf-213">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="d8fdf-213">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="d8fdf-214">String</span><span class="sxs-lookup"><span data-stu-id="d8fdf-214">String</span></span>|<span data-ttu-id="d8fdf-215">Расположение списка сайтов, запускаемых в корпоративном режиме.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-215">The enterprise mode site list location.</span></span> <span data-ttu-id="d8fdf-216">Это может быть локальный файл, локальная сеть или HTTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-216">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="d8fdf-217">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="d8fdf-217">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="d8fdf-218">Интернетситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="d8fdf-218">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="d8fdf-219">Уровень интернет-безопасности.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-219">The internet security level.</span></span> <span data-ttu-id="d8fdf-220">Возможные значения: `userDefined`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-220">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="d8fdf-221">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="d8fdf-221">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="d8fdf-222">Ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="d8fdf-222">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="d8fdf-223">Уровень безопасности интрасети.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-223">The Intranet security level.</span></span> <span data-ttu-id="d8fdf-224">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-224">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="d8fdf-225">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="d8fdf-225">browserLoggingReportLocation</span></span>|<span data-ttu-id="d8fdf-226">String</span><span class="sxs-lookup"><span data-stu-id="d8fdf-226">String</span></span>|<span data-ttu-id="d8fdf-227">Расположение хранения отчетов.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-227">The logging report location.</span></span>|
|<span data-ttu-id="d8fdf-228">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="d8fdf-228">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="d8fdf-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-229">Boolean</span></span>|<span data-ttu-id="d8fdf-230">Указывает, обязателен ли высокий уровень безопасности для опасных сайтов.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-230">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="d8fdf-231">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="d8fdf-231">browserRequireFirewall</span></span>|<span data-ttu-id="d8fdf-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-232">Boolean</span></span>|<span data-ttu-id="d8fdf-233">Указывает, обязательно ли использовать брандмауэр.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-233">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="d8fdf-234">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="d8fdf-234">browserRequireFraudWarning</span></span>|<span data-ttu-id="d8fdf-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-235">Boolean</span></span>|<span data-ttu-id="d8fdf-236">Указывает, обязательно ли предупреждение о мошенничестве.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-236">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="d8fdf-237">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="d8fdf-237">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="d8fdf-238">Ситесекуритилевел</span><span class="sxs-lookup"><span data-stu-id="d8fdf-238">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="d8fdf-239">Уровень безопасности надежных сайтов.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-239">The trusted sites security level.</span></span> <span data-ttu-id="d8fdf-240">Возможные значения: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-240">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="d8fdf-241">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="d8fdf-241">cellularBlockDataRoaming</span></span>|<span data-ttu-id="d8fdf-242">Логический</span><span class="sxs-lookup"><span data-stu-id="d8fdf-242">Boolean</span></span>|<span data-ttu-id="d8fdf-243">Указывает, следует ли блокировать передачу данных в роуминге.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-243">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="d8fdf-244">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="d8fdf-244">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="d8fdf-245">Логический</span><span class="sxs-lookup"><span data-stu-id="d8fdf-245">Boolean</span></span>|<span data-ttu-id="d8fdf-246">Указывает, следует ли заблокировать отправку диагностических данных.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-246">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="d8fdf-247">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="d8fdf-247">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="d8fdf-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-248">Boolean</span></span>|<span data-ttu-id="d8fdf-249">Указывает, следует ли запретить использование графического пароля и ПИН-кода.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-249">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="d8fdf-250">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d8fdf-250">passwordExpirationDays</span></span>|<span data-ttu-id="d8fdf-251">Int32</span><span class="sxs-lookup"><span data-stu-id="d8fdf-251">Int32</span></span>|<span data-ttu-id="d8fdf-252">Срок действия пароля (в днях).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-252">Password expiration in days.</span></span>|
|<span data-ttu-id="d8fdf-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d8fdf-253">passwordMinimumLength</span></span>|<span data-ttu-id="d8fdf-254">Int32</span><span class="sxs-lookup"><span data-stu-id="d8fdf-254">Int32</span></span>|<span data-ttu-id="d8fdf-255">Минимальная длина пароля.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-255">The minimum password length.</span></span>|
|<span data-ttu-id="d8fdf-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d8fdf-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d8fdf-257">Int32</span><span class="sxs-lookup"><span data-stu-id="d8fdf-257">Int32</span></span>|<span data-ttu-id="d8fdf-258">Время бездействия до отключения экрана (в минутах).</span><span class="sxs-lookup"><span data-stu-id="d8fdf-258">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="d8fdf-259">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d8fdf-259">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="d8fdf-260">Int32</span><span class="sxs-lookup"><span data-stu-id="d8fdf-260">Int32</span></span>|<span data-ttu-id="d8fdf-261">Количество наборов символов, которые требуются для пароля.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-261">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="d8fdf-262">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d8fdf-262">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d8fdf-263">Int32</span><span class="sxs-lookup"><span data-stu-id="d8fdf-263">Int32</span></span>|<span data-ttu-id="d8fdf-264">Количество предыдущих паролей, повторное использование которых следует запретить.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-264">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="d8fdf-265">Допустимые значения: от 0 до 24.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-265">Valid values 0 to 24</span></span>|
|<span data-ttu-id="d8fdf-266">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d8fdf-266">passwordRequiredType</span></span>|[<span data-ttu-id="d8fdf-267">Рекуиредпассвордтипе</span><span class="sxs-lookup"><span data-stu-id="d8fdf-267">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d8fdf-268">Требуемый тип пароля.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-268">The required password type.</span></span> <span data-ttu-id="d8fdf-269">Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-269">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d8fdf-270">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="d8fdf-270">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="d8fdf-271">Int32</span><span class="sxs-lookup"><span data-stu-id="d8fdf-271">Int32</span></span>|<span data-ttu-id="d8fdf-272">Количество неудачных попыток входа до восстановления заводских настроек.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-272">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="d8fdf-273">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="d8fdf-273">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="d8fdf-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-274">Boolean</span></span>|<span data-ttu-id="d8fdf-275">Указывает, обязательно ли шифрование данных на мобильном устройстве.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-275">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="d8fdf-276">Минимумаутоинсталлклассификатион</span><span class="sxs-lookup"><span data-stu-id="d8fdf-276">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="d8fdf-277">Упдатеклассификатион</span><span class="sxs-lookup"><span data-stu-id="d8fdf-277">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="d8fdf-278">Минимальная Классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-278">The minimum update classification to install automatically.</span></span> <span data-ttu-id="d8fdf-279">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-279">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="d8fdf-280">Упдатесминимумаутоинсталлклассификатион</span><span class="sxs-lookup"><span data-stu-id="d8fdf-280">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="d8fdf-281">Упдатеклассификатион</span><span class="sxs-lookup"><span data-stu-id="d8fdf-281">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="d8fdf-282">Минимальная Классификация обновлений, устанавливаемая автоматически.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-282">The minimum update classification to install automatically.</span></span> <span data-ttu-id="d8fdf-283">Возможные значения: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-283">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="d8fdf-284">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="d8fdf-284">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="d8fdf-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8fdf-285">Boolean</span></span>|<span data-ttu-id="d8fdf-286">Указывает, обязательно ли автоматическое обновление.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-286">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="d8fdf-287">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="d8fdf-287">userAccountControlSettings</span></span>|[<span data-ttu-id="d8fdf-288">Виндовсусераккаунтконтролсеттингс</span><span class="sxs-lookup"><span data-stu-id="d8fdf-288">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="d8fdf-289">Настройки контроля учетных записей.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-289">The user account control settings.</span></span> <span data-ttu-id="d8fdf-290">Возможные значения: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-290">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="d8fdf-291">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="d8fdf-291">workFoldersUrl</span></span>|<span data-ttu-id="d8fdf-292">String</span><span class="sxs-lookup"><span data-stu-id="d8fdf-292">String</span></span>|<span data-ttu-id="d8fdf-293">URL-адрес рабочей папки.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-293">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="d8fdf-294">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8fdf-294">Response</span></span>
<span data-ttu-id="d8fdf-295">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-295">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8fdf-296">Пример</span><span class="sxs-lookup"><span data-stu-id="d8fdf-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8fdf-297">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8fdf-297">Request</span></span>
<span data-ttu-id="d8fdf-298">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-298">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2697

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
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
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="d8fdf-299">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8fdf-299">Response</span></span>
<span data-ttu-id="d8fdf-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8fdf-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2869

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
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
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```





