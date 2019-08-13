---
title: Обновление объекта macOSDeviceFeaturesConfiguration
description: Обновление свойств объекта macOSDeviceFeaturesConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ba695812f73e321d6bc3b8ad0a03396a7cb7550d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338814"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="6449e-103">Обновление объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="6449e-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="6449e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6449e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6449e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6449e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6449e-106">Обновление свойств объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6449e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6449e-107">Prerequisites</span></span>
<span data-ttu-id="6449e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6449e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6449e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6449e-110">Permission type</span></span>|<span data-ttu-id="6449e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6449e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6449e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6449e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6449e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6449e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6449e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6449e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6449e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6449e-115">Not supported.</span></span>|
|<span data-ttu-id="6449e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6449e-116">Application</span></span>|<span data-ttu-id="6449e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6449e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6449e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6449e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6449e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6449e-119">Request headers</span></span>
|<span data-ttu-id="6449e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6449e-120">Header</span></span>|<span data-ttu-id="6449e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6449e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6449e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6449e-122">Authorization</span></span>|<span data-ttu-id="6449e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6449e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6449e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="6449e-124">Accept</span></span>|<span data-ttu-id="6449e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6449e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6449e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6449e-126">Request body</span></span>
<span data-ttu-id="6449e-127">В теле запроса добавьте представление объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6449e-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="6449e-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="6449e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="6449e-129">Property</span></span>|<span data-ttu-id="6449e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6449e-130">Type</span></span>|<span data-ttu-id="6449e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6449e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6449e-132">id</span><span class="sxs-lookup"><span data-stu-id="6449e-132">id</span></span>|<span data-ttu-id="6449e-133">String</span><span class="sxs-lookup"><span data-stu-id="6449e-133">String</span></span>|<span data-ttu-id="6449e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6449e-134">Key of the entity.</span></span> <span data-ttu-id="6449e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6449e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6449e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6449e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6449e-137">DateTimeOffset</span></span>|<span data-ttu-id="6449e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6449e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6449e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6449e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6449e-140">roleScopeTagIds</span></span>|<span data-ttu-id="6449e-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6449e-141">String collection</span></span>|<span data-ttu-id="6449e-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="6449e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6449e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6449e-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="6449e-144">supportsScopeTags</span></span>|<span data-ttu-id="6449e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-145">Boolean</span></span>|<span data-ttu-id="6449e-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="6449e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6449e-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="6449e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6449e-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="6449e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6449e-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6449e-149">This property is read-only.</span></span> <span data-ttu-id="6449e-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6449e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6449e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="6449e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="6449e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="6449e-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6449e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="6449e-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6449e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6449e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="6449e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="6449e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="6449e-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6449e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="6449e-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6449e-159">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="6449e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="6449e-160">девицеманажементаппликабилитируледевицемоде</span><span class="sxs-lookup"><span data-stu-id="6449e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="6449e-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="6449e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="6449e-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6449e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6449e-163">createdDateTime</span></span>|<span data-ttu-id="6449e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6449e-164">DateTimeOffset</span></span>|<span data-ttu-id="6449e-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6449e-165">DateTime the object was created.</span></span> <span data-ttu-id="6449e-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6449e-167">description</span><span class="sxs-lookup"><span data-stu-id="6449e-167">description</span></span>|<span data-ttu-id="6449e-168">String</span><span class="sxs-lookup"><span data-stu-id="6449e-168">String</span></span>|<span data-ttu-id="6449e-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6449e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6449e-170">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6449e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="6449e-171">displayName</span></span>|<span data-ttu-id="6449e-172">Строка</span><span class="sxs-lookup"><span data-stu-id="6449e-172">String</span></span>|<span data-ttu-id="6449e-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6449e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6449e-174">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6449e-175">version</span><span class="sxs-lookup"><span data-stu-id="6449e-175">version</span></span>|<span data-ttu-id="6449e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="6449e-176">Int32</span></span>|<span data-ttu-id="6449e-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6449e-177">Version of the device configuration.</span></span> <span data-ttu-id="6449e-178">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6449e-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6449e-179">аирпринтдестинатионс</span><span class="sxs-lookup"><span data-stu-id="6449e-179">airPrintDestinations</span></span>|<span data-ttu-id="6449e-180">Коллекция [аирпринтдестинатион](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="6449e-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="6449e-181">Массив принтеров Аирпринт, которые должны отображаться всегда.</span><span class="sxs-lookup"><span data-stu-id="6449e-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="6449e-182">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6449e-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="6449e-183">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="6449e-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="6449e-184">аутолаунчитемс</span><span class="sxs-lookup"><span data-stu-id="6449e-184">autoLaunchItems</span></span>|<span data-ttu-id="6449e-185">Коллекция [макослаунчитем](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="6449e-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="6449e-186">Список приложений, файлов, папок и других элементов, которые запускаются при входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="6449e-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="6449e-187">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6449e-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6449e-188">админшовхостинфо</span><span class="sxs-lookup"><span data-stu-id="6449e-188">adminShowHostInfo</span></span>|<span data-ttu-id="6449e-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-189">Boolean</span></span>|<span data-ttu-id="6449e-190">Показывать ли сведения об узле администратора в окне входа.</span><span class="sxs-lookup"><span data-stu-id="6449e-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="6449e-191">логинвиндовтекст</span><span class="sxs-lookup"><span data-stu-id="6449e-191">loginWindowText</span></span>|<span data-ttu-id="6449e-192">String</span><span class="sxs-lookup"><span data-stu-id="6449e-192">String</span></span>|<span data-ttu-id="6449e-193">Настраиваемый текст, отображаемый в окне входа.</span><span class="sxs-lookup"><span data-stu-id="6449e-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="6449e-194">аусоризедусерслиссидден</span><span class="sxs-lookup"><span data-stu-id="6449e-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="6449e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-195">Boolean</span></span>|<span data-ttu-id="6449e-196">Указывает, следует ли отображать диалоговое окно имя и пароль или список пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="6449e-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="6449e-197">аусоризедусерслиссиделокалусерс</span><span class="sxs-lookup"><span data-stu-id="6449e-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="6449e-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-198">Boolean</span></span>|<span data-ttu-id="6449e-199">Отображение только сетевых и системных пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="6449e-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6449e-200">аусоризедусерслиссидемобилеаккаунтс</span><span class="sxs-lookup"><span data-stu-id="6449e-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="6449e-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-201">Boolean</span></span>|<span data-ttu-id="6449e-202">Следует ли скрыть пользователей для мобильных устройств в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="6449e-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6449e-203">аусоризедусерслистинклуденетворкусерс</span><span class="sxs-lookup"><span data-stu-id="6449e-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="6449e-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-204">Boolean</span></span>|<span data-ttu-id="6449e-205">Показывать ли пользователей сети в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="6449e-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6449e-206">аусоризедусерслиссидеадминусерс</span><span class="sxs-lookup"><span data-stu-id="6449e-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="6449e-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-207">Boolean</span></span>|<span data-ttu-id="6449e-208">Указывает, следует ли скрыть пользователей Admin в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="6449e-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6449e-209">аусоризедусерслистшовосерманажедусерс</span><span class="sxs-lookup"><span data-stu-id="6449e-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="6449e-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-210">Boolean</span></span>|<span data-ttu-id="6449e-211">Указывает, следует ли показывать других пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="6449e-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="6449e-212">шутдовндисаблед</span><span class="sxs-lookup"><span data-stu-id="6449e-212">shutDownDisabled</span></span>|<span data-ttu-id="6449e-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-213">Boolean</span></span>|<span data-ttu-id="6449e-214">Указывает, следует ли скрыть элемент кнопка "завершение работы" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="6449e-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="6449e-215">рестартдисаблед</span><span class="sxs-lookup"><span data-stu-id="6449e-215">restartDisabled</span></span>|<span data-ttu-id="6449e-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-216">Boolean</span></span>|<span data-ttu-id="6449e-217">Указывает, следует ли скрыть элемент "Кнопка перезапуска" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="6449e-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="6449e-218">слипдисаблед</span><span class="sxs-lookup"><span data-stu-id="6449e-218">sleepDisabled</span></span>|<span data-ttu-id="6449e-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-219">Boolean</span></span>|<span data-ttu-id="6449e-220">Указывает, следует ли скрыть пункт меню "сон" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="6449e-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="6449e-221">консолеакцессдисаблед</span><span class="sxs-lookup"><span data-stu-id="6449e-221">consoleAccessDisabled</span></span>|<span data-ttu-id="6449e-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-222">Boolean</span></span>|<span data-ttu-id="6449e-223">Будет ли другой пользователь игнорировать использование консоли ">"> специального имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="6449e-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="6449e-224">шутдовндисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="6449e-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="6449e-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-225">Boolean</span></span>|<span data-ttu-id="6449e-226">Будет ли отключен элемент меню "завершение работы" в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="6449e-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="6449e-227">рестартдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="6449e-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="6449e-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-228">Boolean</span></span>|<span data-ttu-id="6449e-229">Будет ли отключен элемент меню перезапуска в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="6449e-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="6449e-230">повероффдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="6449e-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="6449e-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-231">Boolean</span></span>|<span data-ttu-id="6449e-232">Будет ли отключен элемент меню Power of Power в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="6449e-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="6449e-233">логаутдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="6449e-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="6449e-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-234">Boolean</span></span>|<span data-ttu-id="6449e-235">Будет ли отключен элемент меню журнала в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="6449e-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="6449e-236">скринлоккдисаблеиммедиате</span><span class="sxs-lookup"><span data-stu-id="6449e-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="6449e-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="6449e-237">Boolean</span></span>|<span data-ttu-id="6449e-238">Следует ли отключить функции немедленной блокировки экрана.</span><span class="sxs-lookup"><span data-stu-id="6449e-238">Whether to disable the immediate screen lock functions.</span></span>|



## <a name="response"></a><span data-ttu-id="6449e-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="6449e-239">Response</span></span>
<span data-ttu-id="6449e-240">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6449e-240">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6449e-241">Пример</span><span class="sxs-lookup"><span data-stu-id="6449e-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="6449e-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="6449e-242">Request</span></span>
<span data-ttu-id="6449e-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6449e-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2107

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
  "screenLockDisableImmediate": true
}
```

### <a name="response"></a><span data-ttu-id="6449e-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="6449e-244">Response</span></span>
<span data-ttu-id="6449e-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6449e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2279

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
  "screenLockDisableImmediate": true
}
```






