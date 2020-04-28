---
title: Обновление объекта macOSDeviceFeaturesConfiguration
description: Обновление свойств объекта macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a615bef0cd18ce7ef28ba71adcbe8935736846b5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43438101"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="a3cee-103">Обновление объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="a3cee-103">Update macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="a3cee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3cee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3cee-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3cee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3cee-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3cee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3cee-107">Обновление свойств объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-107">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3cee-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a3cee-108">Prerequisites</span></span>
<span data-ttu-id="a3cee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3cee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3cee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3cee-111">Permission type</span></span>|<span data-ttu-id="a3cee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3cee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3cee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3cee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3cee-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3cee-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3cee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3cee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3cee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3cee-116">Not supported.</span></span>|
|<span data-ttu-id="a3cee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3cee-117">Application</span></span>|<span data-ttu-id="a3cee-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3cee-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3cee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3cee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a3cee-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a3cee-120">Request headers</span></span>
|<span data-ttu-id="a3cee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3cee-121">Header</span></span>|<span data-ttu-id="a3cee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a3cee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3cee-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a3cee-123">Authorization</span></span>|<span data-ttu-id="a3cee-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a3cee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3cee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a3cee-125">Accept</span></span>|<span data-ttu-id="a3cee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3cee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3cee-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a3cee-127">Request body</span></span>
<span data-ttu-id="a3cee-128">В теле запроса добавьте представление объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3cee-128">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="a3cee-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-129">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="a3cee-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3cee-130">Property</span></span>|<span data-ttu-id="a3cee-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a3cee-131">Type</span></span>|<span data-ttu-id="a3cee-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a3cee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3cee-133">id</span><span class="sxs-lookup"><span data-stu-id="a3cee-133">id</span></span>|<span data-ttu-id="a3cee-134">String</span><span class="sxs-lookup"><span data-stu-id="a3cee-134">String</span></span>|<span data-ttu-id="a3cee-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a3cee-135">Key of the entity.</span></span> <span data-ttu-id="a3cee-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3cee-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3cee-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a3cee-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3cee-138">DateTimeOffset</span></span>|<span data-ttu-id="a3cee-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a3cee-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a3cee-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3cee-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a3cee-141">roleScopeTagIds</span></span>|<span data-ttu-id="a3cee-142">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a3cee-142">String collection</span></span>|<span data-ttu-id="a3cee-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a3cee-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a3cee-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3cee-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a3cee-145">supportsScopeTags</span></span>|<span data-ttu-id="a3cee-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-146">Boolean</span></span>|<span data-ttu-id="a3cee-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a3cee-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a3cee-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a3cee-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a3cee-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a3cee-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a3cee-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3cee-150">This property is read-only.</span></span> <span data-ttu-id="a3cee-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3cee-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a3cee-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a3cee-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a3cee-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a3cee-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a3cee-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a3cee-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3cee-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a3cee-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a3cee-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a3cee-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a3cee-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a3cee-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a3cee-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3cee-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a3cee-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a3cee-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a3cee-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a3cee-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a3cee-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a3cee-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3cee-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3cee-164">createdDateTime</span></span>|<span data-ttu-id="a3cee-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3cee-165">DateTimeOffset</span></span>|<span data-ttu-id="a3cee-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a3cee-166">DateTime the object was created.</span></span> <span data-ttu-id="a3cee-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3cee-168">description</span><span class="sxs-lookup"><span data-stu-id="a3cee-168">description</span></span>|<span data-ttu-id="a3cee-169">String</span><span class="sxs-lookup"><span data-stu-id="a3cee-169">String</span></span>|<span data-ttu-id="a3cee-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3cee-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a3cee-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3cee-172">displayName</span><span class="sxs-lookup"><span data-stu-id="a3cee-172">displayName</span></span>|<span data-ttu-id="a3cee-173">Строка</span><span class="sxs-lookup"><span data-stu-id="a3cee-173">String</span></span>|<span data-ttu-id="a3cee-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3cee-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a3cee-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3cee-176">version</span><span class="sxs-lookup"><span data-stu-id="a3cee-176">version</span></span>|<span data-ttu-id="a3cee-177">Int32</span><span class="sxs-lookup"><span data-stu-id="a3cee-177">Int32</span></span>|<span data-ttu-id="a3cee-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a3cee-178">Version of the device configuration.</span></span> <span data-ttu-id="a3cee-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a3cee-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3cee-180">аирпринтдестинатионс</span><span class="sxs-lookup"><span data-stu-id="a3cee-180">airPrintDestinations</span></span>|<span data-ttu-id="a3cee-181">Коллекция [аирпринтдестинатион](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="a3cee-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="a3cee-182">Массив принтеров Аирпринт, которые должны отображаться всегда.</span><span class="sxs-lookup"><span data-stu-id="a3cee-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="a3cee-183">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a3cee-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a3cee-184">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="a3cee-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="a3cee-185">аутолаунчитемс</span><span class="sxs-lookup"><span data-stu-id="a3cee-185">autoLaunchItems</span></span>|<span data-ttu-id="a3cee-186">Коллекция [макослаунчитем](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="a3cee-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="a3cee-187">Список приложений, файлов, папок и других элементов, которые запускаются при входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3cee-187">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="a3cee-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a3cee-188">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a3cee-189">админшовхостинфо</span><span class="sxs-lookup"><span data-stu-id="a3cee-189">adminShowHostInfo</span></span>|<span data-ttu-id="a3cee-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-190">Boolean</span></span>|<span data-ttu-id="a3cee-191">Показывать ли сведения об узле администратора в окне входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-191">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="a3cee-192">логинвиндовтекст</span><span class="sxs-lookup"><span data-stu-id="a3cee-192">loginWindowText</span></span>|<span data-ttu-id="a3cee-193">String</span><span class="sxs-lookup"><span data-stu-id="a3cee-193">String</span></span>|<span data-ttu-id="a3cee-194">Настраиваемый текст, отображаемый в окне входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-194">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="a3cee-195">аусоризедусерслиссидден</span><span class="sxs-lookup"><span data-stu-id="a3cee-195">authorizedUsersListHidden</span></span>|<span data-ttu-id="a3cee-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-196">Boolean</span></span>|<span data-ttu-id="a3cee-197">Указывает, следует ли отображать диалоговое окно имя и пароль или список пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-197">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="a3cee-198">аусоризедусерслиссиделокалусерс</span><span class="sxs-lookup"><span data-stu-id="a3cee-198">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="a3cee-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-199">Boolean</span></span>|<span data-ttu-id="a3cee-200">Отображение только сетевых и системных пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-200">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="a3cee-201">аусоризедусерслиссидемобилеаккаунтс</span><span class="sxs-lookup"><span data-stu-id="a3cee-201">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="a3cee-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-202">Boolean</span></span>|<span data-ttu-id="a3cee-203">Следует ли скрыть пользователей для мобильных устройств в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-203">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="a3cee-204">аусоризедусерслистинклуденетворкусерс</span><span class="sxs-lookup"><span data-stu-id="a3cee-204">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="a3cee-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-205">Boolean</span></span>|<span data-ttu-id="a3cee-206">Показывать ли пользователей сети в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-206">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="a3cee-207">аусоризедусерслиссидеадминусерс</span><span class="sxs-lookup"><span data-stu-id="a3cee-207">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="a3cee-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-208">Boolean</span></span>|<span data-ttu-id="a3cee-209">Указывает, следует ли скрыть пользователей Admin в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-209">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="a3cee-210">аусоризедусерслистшовосерманажедусерс</span><span class="sxs-lookup"><span data-stu-id="a3cee-210">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="a3cee-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-211">Boolean</span></span>|<span data-ttu-id="a3cee-212">Указывает, следует ли показывать других пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-212">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="a3cee-213">шутдовндисаблед</span><span class="sxs-lookup"><span data-stu-id="a3cee-213">shutDownDisabled</span></span>|<span data-ttu-id="a3cee-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-214">Boolean</span></span>|<span data-ttu-id="a3cee-215">Указывает, следует ли скрыть элемент кнопка "завершение работы" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-215">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="a3cee-216">рестартдисаблед</span><span class="sxs-lookup"><span data-stu-id="a3cee-216">restartDisabled</span></span>|<span data-ttu-id="a3cee-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-217">Boolean</span></span>|<span data-ttu-id="a3cee-218">Указывает, следует ли скрыть элемент "Кнопка перезапуска" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-218">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="a3cee-219">слипдисаблед</span><span class="sxs-lookup"><span data-stu-id="a3cee-219">sleepDisabled</span></span>|<span data-ttu-id="a3cee-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-220">Boolean</span></span>|<span data-ttu-id="a3cee-221">Указывает, следует ли скрыть пункт меню "сон" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-221">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="a3cee-222">консолеакцессдисаблед</span><span class="sxs-lookup"><span data-stu-id="a3cee-222">consoleAccessDisabled</span></span>|<span data-ttu-id="a3cee-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-223">Boolean</span></span>|<span data-ttu-id="a3cee-224">Будет ли другой пользователь игнорировать использование консоли ">"> специального имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="a3cee-224">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="a3cee-225">шутдовндисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="a3cee-225">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="a3cee-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-226">Boolean</span></span>|<span data-ttu-id="a3cee-227">Будет ли отключен элемент меню "завершение работы" в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="a3cee-227">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="a3cee-228">рестартдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="a3cee-228">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="a3cee-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-229">Boolean</span></span>|<span data-ttu-id="a3cee-230">Будет ли отключен элемент меню перезапуска в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="a3cee-230">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="a3cee-231">повероффдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="a3cee-231">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="a3cee-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-232">Boolean</span></span>|<span data-ttu-id="a3cee-233">Будет ли отключен элемент меню Power of Power в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="a3cee-233">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="a3cee-234">логаутдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="a3cee-234">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="a3cee-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-235">Boolean</span></span>|<span data-ttu-id="a3cee-236">Будет ли отключен элемент меню журнала в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="a3cee-236">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="a3cee-237">скринлоккдисаблеиммедиате</span><span class="sxs-lookup"><span data-stu-id="a3cee-237">screenLockDisableImmediate</span></span>|<span data-ttu-id="a3cee-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3cee-238">Boolean</span></span>|<span data-ttu-id="a3cee-239">Следует ли отключить функции немедленной блокировки экрана.</span><span class="sxs-lookup"><span data-stu-id="a3cee-239">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="a3cee-240">ассоЦиатеддомаинс</span><span class="sxs-lookup"><span data-stu-id="a3cee-240">associatedDomains</span></span>|<span data-ttu-id="a3cee-241">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a3cee-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a3cee-242">Получает или задает список, который сопоставляет приложения с их связанными доменами.</span><span class="sxs-lookup"><span data-stu-id="a3cee-242">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="a3cee-243">Ключ должен соответствовать ИДЕНТИФИКАТОРу приложения, а значение должно быть строкой в виде "Service: domain", где Domain — это полное доменное имя узла (например,:ексампле.. com).</span><span class="sxs-lookup"><span data-stu-id="a3cee-243">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="a3cee-244">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="a3cee-244">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a3cee-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="a3cee-245">singleSignOnExtension</span></span>|[<span data-ttu-id="a3cee-246">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="a3cee-246">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="a3cee-247">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-247">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="a3cee-248">Устарело: вместо этого используйте Макоссинглесигнонекстенсион.</span><span class="sxs-lookup"><span data-stu-id="a3cee-248">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="a3cee-249">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="a3cee-249">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="a3cee-250">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="a3cee-250">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="a3cee-251">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="a3cee-251">Gets or sets a single sign-on extension profile.</span></span>|



## <a name="response"></a><span data-ttu-id="a3cee-252">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3cee-252">Response</span></span>
<span data-ttu-id="a3cee-253">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a3cee-253">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3cee-254">Пример</span><span class="sxs-lookup"><span data-stu-id="a3cee-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3cee-255">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3cee-255">Request</span></span>
<span data-ttu-id="a3cee-256">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3cee-256">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a3cee-257">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3cee-257">Response</span></span>
<span data-ttu-id="a3cee-p117">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a3cee-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



