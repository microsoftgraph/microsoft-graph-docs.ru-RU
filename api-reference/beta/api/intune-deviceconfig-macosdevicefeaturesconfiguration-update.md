---
title: Обновление объекта macOSDeviceFeaturesConfiguration
description: Обновление свойств объекта macOSDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cd01d28fafbde46131195c3ca5e9a9e250ca8ca2
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41635827"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="425d2-103">Обновление объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="425d2-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="425d2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="425d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="425d2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="425d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="425d2-106">Обновление свойств объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="425d2-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="425d2-107">Prerequisites</span></span>
<span data-ttu-id="425d2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="425d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="425d2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="425d2-110">Permission type</span></span>|<span data-ttu-id="425d2-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="425d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="425d2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="425d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="425d2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="425d2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="425d2-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="425d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="425d2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="425d2-115">Not supported.</span></span>|
|<span data-ttu-id="425d2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="425d2-116">Application</span></span>|<span data-ttu-id="425d2-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="425d2-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="425d2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="425d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="425d2-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="425d2-119">Request headers</span></span>
|<span data-ttu-id="425d2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="425d2-120">Header</span></span>|<span data-ttu-id="425d2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="425d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="425d2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="425d2-122">Authorization</span></span>|<span data-ttu-id="425d2-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="425d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="425d2-124">Accept</span><span class="sxs-lookup"><span data-stu-id="425d2-124">Accept</span></span>|<span data-ttu-id="425d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="425d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="425d2-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="425d2-126">Request body</span></span>
<span data-ttu-id="425d2-127">В теле запроса добавьте представление объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="425d2-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="425d2-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="425d2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="425d2-129">Property</span></span>|<span data-ttu-id="425d2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="425d2-130">Type</span></span>|<span data-ttu-id="425d2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="425d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="425d2-132">id</span><span class="sxs-lookup"><span data-stu-id="425d2-132">id</span></span>|<span data-ttu-id="425d2-133">String</span><span class="sxs-lookup"><span data-stu-id="425d2-133">String</span></span>|<span data-ttu-id="425d2-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="425d2-134">Key of the entity.</span></span> <span data-ttu-id="425d2-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="425d2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="425d2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="425d2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="425d2-137">DateTimeOffset</span></span>|<span data-ttu-id="425d2-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="425d2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="425d2-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="425d2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="425d2-140">roleScopeTagIds</span></span>|<span data-ttu-id="425d2-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="425d2-141">String collection</span></span>|<span data-ttu-id="425d2-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="425d2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="425d2-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="425d2-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="425d2-144">supportsScopeTags</span></span>|<span data-ttu-id="425d2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-145">Boolean</span></span>|<span data-ttu-id="425d2-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="425d2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="425d2-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="425d2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="425d2-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="425d2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="425d2-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="425d2-149">This property is read-only.</span></span> <span data-ttu-id="425d2-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="425d2-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="425d2-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="425d2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="425d2-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="425d2-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="425d2-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="425d2-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="425d2-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="425d2-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="425d2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="425d2-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="425d2-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="425d2-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="425d2-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="425d2-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="425d2-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="425d2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="425d2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="425d2-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="425d2-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="425d2-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="425d2-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="425d2-163">createdDateTime</span></span>|<span data-ttu-id="425d2-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="425d2-164">DateTimeOffset</span></span>|<span data-ttu-id="425d2-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="425d2-165">DateTime the object was created.</span></span> <span data-ttu-id="425d2-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="425d2-167">description</span><span class="sxs-lookup"><span data-stu-id="425d2-167">description</span></span>|<span data-ttu-id="425d2-168">String</span><span class="sxs-lookup"><span data-stu-id="425d2-168">String</span></span>|<span data-ttu-id="425d2-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="425d2-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="425d2-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="425d2-171">displayName</span><span class="sxs-lookup"><span data-stu-id="425d2-171">displayName</span></span>|<span data-ttu-id="425d2-172">Строка</span><span class="sxs-lookup"><span data-stu-id="425d2-172">String</span></span>|<span data-ttu-id="425d2-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="425d2-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="425d2-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="425d2-175">version</span><span class="sxs-lookup"><span data-stu-id="425d2-175">version</span></span>|<span data-ttu-id="425d2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="425d2-176">Int32</span></span>|<span data-ttu-id="425d2-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="425d2-177">Version of the device configuration.</span></span> <span data-ttu-id="425d2-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="425d2-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="425d2-179">аирпринтдестинатионс</span><span class="sxs-lookup"><span data-stu-id="425d2-179">airPrintDestinations</span></span>|<span data-ttu-id="425d2-180">Коллекция [аирпринтдестинатион](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="425d2-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="425d2-181">Массив принтеров Аирпринт, которые должны отображаться всегда.</span><span class="sxs-lookup"><span data-stu-id="425d2-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="425d2-182">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="425d2-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="425d2-183">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="425d2-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="425d2-184">аутолаунчитемс</span><span class="sxs-lookup"><span data-stu-id="425d2-184">autoLaunchItems</span></span>|<span data-ttu-id="425d2-185">Коллекция [макослаунчитем](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="425d2-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="425d2-186">Список приложений, файлов, папок и других элементов, которые запускаются при входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="425d2-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="425d2-187">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="425d2-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="425d2-188">админшовхостинфо</span><span class="sxs-lookup"><span data-stu-id="425d2-188">adminShowHostInfo</span></span>|<span data-ttu-id="425d2-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-189">Boolean</span></span>|<span data-ttu-id="425d2-190">Показывать ли сведения об узле администратора в окне входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="425d2-191">логинвиндовтекст</span><span class="sxs-lookup"><span data-stu-id="425d2-191">loginWindowText</span></span>|<span data-ttu-id="425d2-192">Строка</span><span class="sxs-lookup"><span data-stu-id="425d2-192">String</span></span>|<span data-ttu-id="425d2-193">Настраиваемый текст, отображаемый в окне входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="425d2-194">аусоризедусерслиссидден</span><span class="sxs-lookup"><span data-stu-id="425d2-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="425d2-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-195">Boolean</span></span>|<span data-ttu-id="425d2-196">Указывает, следует ли отображать диалоговое окно имя и пароль или список пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="425d2-197">аусоризедусерслиссиделокалусерс</span><span class="sxs-lookup"><span data-stu-id="425d2-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="425d2-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-198">Boolean</span></span>|<span data-ttu-id="425d2-199">Отображение только сетевых и системных пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="425d2-200">аусоризедусерслиссидемобилеаккаунтс</span><span class="sxs-lookup"><span data-stu-id="425d2-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="425d2-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-201">Boolean</span></span>|<span data-ttu-id="425d2-202">Следует ли скрыть пользователей для мобильных устройств в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="425d2-203">аусоризедусерслистинклуденетворкусерс</span><span class="sxs-lookup"><span data-stu-id="425d2-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="425d2-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-204">Boolean</span></span>|<span data-ttu-id="425d2-205">Показывать ли пользователей сети в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="425d2-206">аусоризедусерслиссидеадминусерс</span><span class="sxs-lookup"><span data-stu-id="425d2-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="425d2-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-207">Boolean</span></span>|<span data-ttu-id="425d2-208">Указывает, следует ли скрыть пользователей Admin в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="425d2-209">аусоризедусерслистшовосерманажедусерс</span><span class="sxs-lookup"><span data-stu-id="425d2-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="425d2-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-210">Boolean</span></span>|<span data-ttu-id="425d2-211">Указывает, следует ли показывать других пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="425d2-212">шутдовндисаблед</span><span class="sxs-lookup"><span data-stu-id="425d2-212">shutDownDisabled</span></span>|<span data-ttu-id="425d2-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-213">Boolean</span></span>|<span data-ttu-id="425d2-214">Указывает, следует ли скрыть элемент кнопка "завершение работы" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="425d2-215">рестартдисаблед</span><span class="sxs-lookup"><span data-stu-id="425d2-215">restartDisabled</span></span>|<span data-ttu-id="425d2-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-216">Boolean</span></span>|<span data-ttu-id="425d2-217">Указывает, следует ли скрыть элемент "Кнопка перезапуска" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="425d2-218">слипдисаблед</span><span class="sxs-lookup"><span data-stu-id="425d2-218">sleepDisabled</span></span>|<span data-ttu-id="425d2-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-219">Boolean</span></span>|<span data-ttu-id="425d2-220">Указывает, следует ли скрыть пункт меню "сон" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="425d2-221">консолеакцессдисаблед</span><span class="sxs-lookup"><span data-stu-id="425d2-221">consoleAccessDisabled</span></span>|<span data-ttu-id="425d2-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-222">Boolean</span></span>|<span data-ttu-id="425d2-223">Будет ли другой пользователь игнорировать использование консоли ">"> специального имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="425d2-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="425d2-224">шутдовндисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="425d2-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="425d2-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-225">Boolean</span></span>|<span data-ttu-id="425d2-226">Будет ли отключен элемент меню "завершение работы" в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="425d2-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="425d2-227">рестартдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="425d2-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="425d2-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-228">Boolean</span></span>|<span data-ttu-id="425d2-229">Будет ли отключен элемент меню перезапуска в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="425d2-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="425d2-230">повероффдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="425d2-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="425d2-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-231">Boolean</span></span>|<span data-ttu-id="425d2-232">Будет ли отключен элемент меню Power of Power в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="425d2-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="425d2-233">логаутдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="425d2-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="425d2-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-234">Boolean</span></span>|<span data-ttu-id="425d2-235">Будет ли отключен элемент меню журнала в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="425d2-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="425d2-236">скринлоккдисаблеиммедиате</span><span class="sxs-lookup"><span data-stu-id="425d2-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="425d2-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="425d2-237">Boolean</span></span>|<span data-ttu-id="425d2-238">Следует ли отключить функции немедленной блокировки экрана.</span><span class="sxs-lookup"><span data-stu-id="425d2-238">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="425d2-239">ассоЦиатеддомаинс</span><span class="sxs-lookup"><span data-stu-id="425d2-239">associatedDomains</span></span>|<span data-ttu-id="425d2-240">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="425d2-240">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="425d2-241">Получает или задает список, который сопоставляет приложения с их связанными доменами.</span><span class="sxs-lookup"><span data-stu-id="425d2-241">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="425d2-242">Ключ должен соответствовать ИДЕНТИФИКАТОРу приложения, а значение должно быть строкой в виде "Service: domain", где Domain — это полное доменное имя узла (например,:ексампле.. com).</span><span class="sxs-lookup"><span data-stu-id="425d2-242">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="425d2-243">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="425d2-243">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="425d2-244">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="425d2-244">singleSignOnExtension</span></span>|[<span data-ttu-id="425d2-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="425d2-245">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="425d2-246">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-246">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="425d2-247">Устарело: вместо этого используйте Макоссинглесигнонекстенсион.</span><span class="sxs-lookup"><span data-stu-id="425d2-247">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="425d2-248">макоссинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="425d2-248">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="425d2-249">макоссинглесигнонекстенсион</span><span class="sxs-lookup"><span data-stu-id="425d2-249">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="425d2-250">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="425d2-250">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="425d2-251">Отклик</span><span class="sxs-lookup"><span data-stu-id="425d2-251">Response</span></span>
<span data-ttu-id="425d2-252">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="425d2-252">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="425d2-253">Пример</span><span class="sxs-lookup"><span data-stu-id="425d2-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="425d2-254">Запрос</span><span class="sxs-lookup"><span data-stu-id="425d2-254">Request</span></span>
<span data-ttu-id="425d2-255">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="425d2-255">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2468

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "Path value",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "Login Window Text value",
  "authorizedUsersListHidden": true,
  "authorizedUsersListHideLocalUsers": true,
  "authorizedUsersListHideMobileAccounts": true,
  "authorizedUsersListIncludeNetworkUsers": true,
  "authorizedUsersListHideAdminUsers": true,
  "authorizedUsersListShowOtherManagedUsers": true,
  "shutDownDisabled": true,
  "restartDisabled": true,
  "sleepDisabled": true,
  "consoleAccessDisabled": true,
  "shutDownDisabledWhileLoggedIn": true,
  "restartDisabledWhileLoggedIn": true,
  "powerOffDisabledWhileLoggedIn": true,
  "logOutDisabledWhileLoggedIn": true,
  "screenLockDisableImmediate": true,
  "associatedDomains": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.singleSignOnExtension"
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSSingleSignOnExtension"
  }
}
```

### <a name="response"></a><span data-ttu-id="425d2-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="425d2-256">Response</span></span>
<span data-ttu-id="425d2-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="425d2-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2640

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "Path value",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "Login Window Text value",
  "authorizedUsersListHidden": true,
  "authorizedUsersListHideLocalUsers": true,
  "authorizedUsersListHideMobileAccounts": true,
  "authorizedUsersListIncludeNetworkUsers": true,
  "authorizedUsersListHideAdminUsers": true,
  "authorizedUsersListShowOtherManagedUsers": true,
  "shutDownDisabled": true,
  "restartDisabled": true,
  "sleepDisabled": true,
  "consoleAccessDisabled": true,
  "shutDownDisabledWhileLoggedIn": true,
  "restartDisabledWhileLoggedIn": true,
  "powerOffDisabledWhileLoggedIn": true,
  "logOutDisabledWhileLoggedIn": true,
  "screenLockDisableImmediate": true,
  "associatedDomains": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "singleSignOnExtension": {
    "@odata.type": "microsoft.graph.singleSignOnExtension"
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSSingleSignOnExtension"
  }
}
```





