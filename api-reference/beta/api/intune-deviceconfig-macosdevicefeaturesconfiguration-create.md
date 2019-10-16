---
title: Создание объекта macOSDeviceFeaturesConfiguration
description: Создание объекта macOSDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1645fedd18e3f0baf8f791ea8b9850dfb2db6078
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533660"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="8ff93-103">Создание объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="8ff93-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="8ff93-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ff93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ff93-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ff93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ff93-106">Создание объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff93-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ff93-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8ff93-107">Prerequisites</span></span>
<span data-ttu-id="8ff93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ff93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ff93-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ff93-110">Permission type</span></span>|<span data-ttu-id="8ff93-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ff93-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ff93-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ff93-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ff93-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff93-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ff93-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ff93-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ff93-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ff93-115">Not supported.</span></span>|
|<span data-ttu-id="8ff93-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8ff93-116">Application</span></span>|<span data-ttu-id="8ff93-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff93-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ff93-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ff93-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8ff93-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ff93-119">Request headers</span></span>
|<span data-ttu-id="8ff93-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8ff93-120">Header</span></span>|<span data-ttu-id="8ff93-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8ff93-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ff93-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ff93-122">Authorization</span></span>|<span data-ttu-id="8ff93-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ff93-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ff93-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8ff93-124">Accept</span></span>|<span data-ttu-id="8ff93-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8ff93-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ff93-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ff93-126">Request body</span></span>
<span data-ttu-id="8ff93-127">В теле запроса добавьте представление объекта macOSDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ff93-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="8ff93-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="8ff93-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="8ff93-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ff93-129">Property</span></span>|<span data-ttu-id="8ff93-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8ff93-130">Type</span></span>|<span data-ttu-id="8ff93-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8ff93-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ff93-132">id</span><span class="sxs-lookup"><span data-stu-id="8ff93-132">id</span></span>|<span data-ttu-id="8ff93-133">String</span><span class="sxs-lookup"><span data-stu-id="8ff93-133">String</span></span>|<span data-ttu-id="8ff93-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8ff93-134">Key of the entity.</span></span> <span data-ttu-id="8ff93-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff93-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff93-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ff93-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8ff93-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ff93-137">DateTimeOffset</span></span>|<span data-ttu-id="8ff93-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8ff93-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8ff93-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff93-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff93-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8ff93-140">roleScopeTagIds</span></span>|<span data-ttu-id="8ff93-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8ff93-141">String collection</span></span>|<span data-ttu-id="8ff93-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8ff93-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8ff93-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff93-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff93-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8ff93-144">supportsScopeTags</span></span>|<span data-ttu-id="8ff93-145">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-145">Boolean</span></span>|<span data-ttu-id="8ff93-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8ff93-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8ff93-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8ff93-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8ff93-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8ff93-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8ff93-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8ff93-149">This property is read-only.</span></span> <span data-ttu-id="8ff93-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff93-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff93-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8ff93-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="8ff93-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="8ff93-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="8ff93-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8ff93-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="8ff93-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff93-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff93-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8ff93-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="8ff93-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="8ff93-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="8ff93-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8ff93-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="8ff93-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff93-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff93-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8ff93-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="8ff93-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8ff93-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="8ff93-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="8ff93-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="8ff93-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff93-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff93-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8ff93-163">createdDateTime</span></span>|<span data-ttu-id="8ff93-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ff93-164">DateTimeOffset</span></span>|<span data-ttu-id="8ff93-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8ff93-165">DateTime the object was created.</span></span> <span data-ttu-id="8ff93-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff93-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff93-167">description</span><span class="sxs-lookup"><span data-stu-id="8ff93-167">description</span></span>|<span data-ttu-id="8ff93-168">String</span><span class="sxs-lookup"><span data-stu-id="8ff93-168">String</span></span>|<span data-ttu-id="8ff93-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ff93-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8ff93-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff93-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff93-171">displayName</span><span class="sxs-lookup"><span data-stu-id="8ff93-171">displayName</span></span>|<span data-ttu-id="8ff93-172">Строка</span><span class="sxs-lookup"><span data-stu-id="8ff93-172">String</span></span>|<span data-ttu-id="8ff93-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ff93-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8ff93-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff93-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff93-175">version</span><span class="sxs-lookup"><span data-stu-id="8ff93-175">version</span></span>|<span data-ttu-id="8ff93-176">Int32</span><span class="sxs-lookup"><span data-stu-id="8ff93-176">Int32</span></span>|<span data-ttu-id="8ff93-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8ff93-177">Version of the device configuration.</span></span> <span data-ttu-id="8ff93-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8ff93-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8ff93-179">аирпринтдестинатионс</span><span class="sxs-lookup"><span data-stu-id="8ff93-179">airPrintDestinations</span></span>|<span data-ttu-id="8ff93-180">Коллекция [аирпринтдестинатион](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="8ff93-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="8ff93-181">Массив принтеров Аирпринт, которые должны отображаться всегда.</span><span class="sxs-lookup"><span data-stu-id="8ff93-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="8ff93-182">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8ff93-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8ff93-183">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="8ff93-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="8ff93-184">аутолаунчитемс</span><span class="sxs-lookup"><span data-stu-id="8ff93-184">autoLaunchItems</span></span>|<span data-ttu-id="8ff93-185">Коллекция [макослаунчитем](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="8ff93-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="8ff93-186">Список приложений, файлов, папок и других элементов, которые запускаются при входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ff93-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="8ff93-187">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8ff93-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8ff93-188">админшовхостинфо</span><span class="sxs-lookup"><span data-stu-id="8ff93-188">adminShowHostInfo</span></span>|<span data-ttu-id="8ff93-189">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-189">Boolean</span></span>|<span data-ttu-id="8ff93-190">Показывать ли сведения об узле администратора в окне входа.</span><span class="sxs-lookup"><span data-stu-id="8ff93-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="8ff93-191">логинвиндовтекст</span><span class="sxs-lookup"><span data-stu-id="8ff93-191">loginWindowText</span></span>|<span data-ttu-id="8ff93-192">String</span><span class="sxs-lookup"><span data-stu-id="8ff93-192">String</span></span>|<span data-ttu-id="8ff93-193">Настраиваемый текст, отображаемый в окне входа.</span><span class="sxs-lookup"><span data-stu-id="8ff93-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="8ff93-194">аусоризедусерслиссидден</span><span class="sxs-lookup"><span data-stu-id="8ff93-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="8ff93-195">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-195">Boolean</span></span>|<span data-ttu-id="8ff93-196">Указывает, следует ли отображать диалоговое окно имя и пароль или список пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="8ff93-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="8ff93-197">аусоризедусерслиссиделокалусерс</span><span class="sxs-lookup"><span data-stu-id="8ff93-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="8ff93-198">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-198">Boolean</span></span>|<span data-ttu-id="8ff93-199">Отображение только сетевых и системных пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="8ff93-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="8ff93-200">аусоризедусерслиссидемобилеаккаунтс</span><span class="sxs-lookup"><span data-stu-id="8ff93-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="8ff93-201">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-201">Boolean</span></span>|<span data-ttu-id="8ff93-202">Следует ли скрыть пользователей для мобильных устройств в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="8ff93-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="8ff93-203">аусоризедусерслистинклуденетворкусерс</span><span class="sxs-lookup"><span data-stu-id="8ff93-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="8ff93-204">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-204">Boolean</span></span>|<span data-ttu-id="8ff93-205">Показывать ли пользователей сети в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="8ff93-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="8ff93-206">аусоризедусерслиссидеадминусерс</span><span class="sxs-lookup"><span data-stu-id="8ff93-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="8ff93-207">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-207">Boolean</span></span>|<span data-ttu-id="8ff93-208">Указывает, следует ли скрыть пользователей Admin в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="8ff93-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="8ff93-209">аусоризедусерслистшовосерманажедусерс</span><span class="sxs-lookup"><span data-stu-id="8ff93-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="8ff93-210">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-210">Boolean</span></span>|<span data-ttu-id="8ff93-211">Указывает, следует ли показывать других пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="8ff93-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="8ff93-212">шутдовндисаблед</span><span class="sxs-lookup"><span data-stu-id="8ff93-212">shutDownDisabled</span></span>|<span data-ttu-id="8ff93-213">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-213">Boolean</span></span>|<span data-ttu-id="8ff93-214">Указывает, следует ли скрыть элемент кнопка "завершение работы" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="8ff93-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="8ff93-215">рестартдисаблед</span><span class="sxs-lookup"><span data-stu-id="8ff93-215">restartDisabled</span></span>|<span data-ttu-id="8ff93-216">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-216">Boolean</span></span>|<span data-ttu-id="8ff93-217">Указывает, следует ли скрыть элемент "Кнопка перезапуска" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="8ff93-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="8ff93-218">слипдисаблед</span><span class="sxs-lookup"><span data-stu-id="8ff93-218">sleepDisabled</span></span>|<span data-ttu-id="8ff93-219">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-219">Boolean</span></span>|<span data-ttu-id="8ff93-220">Указывает, следует ли скрыть пункт меню "сон" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="8ff93-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="8ff93-221">консолеакцессдисаблед</span><span class="sxs-lookup"><span data-stu-id="8ff93-221">consoleAccessDisabled</span></span>|<span data-ttu-id="8ff93-222">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-222">Boolean</span></span>|<span data-ttu-id="8ff93-223">Будет ли другой пользователь игнорировать использование консоли ">"> специального имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="8ff93-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="8ff93-224">шутдовндисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="8ff93-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="8ff93-225">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-225">Boolean</span></span>|<span data-ttu-id="8ff93-226">Будет ли отключен элемент меню "завершение работы" в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="8ff93-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="8ff93-227">рестартдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="8ff93-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="8ff93-228">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-228">Boolean</span></span>|<span data-ttu-id="8ff93-229">Будет ли отключен элемент меню перезапуска в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="8ff93-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="8ff93-230">повероффдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="8ff93-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="8ff93-231">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-231">Boolean</span></span>|<span data-ttu-id="8ff93-232">Будет ли отключен элемент меню Power of Power в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="8ff93-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="8ff93-233">логаутдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="8ff93-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="8ff93-234">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-234">Boolean</span></span>|<span data-ttu-id="8ff93-235">Будет ли отключен элемент меню журнала в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="8ff93-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="8ff93-236">скринлоккдисаблеиммедиате</span><span class="sxs-lookup"><span data-stu-id="8ff93-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="8ff93-237">Логический</span><span class="sxs-lookup"><span data-stu-id="8ff93-237">Boolean</span></span>|<span data-ttu-id="8ff93-238">Следует ли отключить функции немедленной блокировки экрана.</span><span class="sxs-lookup"><span data-stu-id="8ff93-238">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="8ff93-239">ассоЦиатеддомаинс</span><span class="sxs-lookup"><span data-stu-id="8ff93-239">associatedDomains</span></span>|<span data-ttu-id="8ff93-240">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8ff93-240">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="8ff93-241">Получает или задает список, который сопоставляет приложения с их связанными доменами.</span><span class="sxs-lookup"><span data-stu-id="8ff93-241">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="8ff93-242">Ключ должен соответствовать ИДЕНТИФИКАТОРу приложения, а значение должно быть строкой в виде "Service: domain", где Domain — это полное доменное имя узла (например,:ексампле.. com).</span><span class="sxs-lookup"><span data-stu-id="8ff93-242">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="8ff93-243">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="8ff93-243">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8ff93-244">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="8ff93-244">singleSignOnExtension</span></span>|[<span data-ttu-id="8ff93-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="8ff93-245">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="8ff93-246">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="8ff93-246">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="8ff93-247">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ff93-247">Response</span></span>
<span data-ttu-id="8ff93-248">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8ff93-248">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ff93-249">Пример</span><span class="sxs-lookup"><span data-stu-id="8ff93-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ff93-250">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ff93-250">Request</span></span>
<span data-ttu-id="8ff93-251">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ff93-251">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2362

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
  }
}
```

### <a name="response"></a><span data-ttu-id="8ff93-252">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ff93-252">Response</span></span>
<span data-ttu-id="8ff93-p116">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8ff93-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2534

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
  }
}
```






