---
title: Создание объекта macOSDeviceFeaturesConfiguration
description: Создание объекта macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9033d76816d402b190ff9dbffd49d9ef3d4834e5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48017949"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="e2b08-103">Создание объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2b08-103">Create macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="e2b08-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2b08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2b08-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2b08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2b08-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e2b08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2b08-107">Создание объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2b08-107">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2b08-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e2b08-108">Prerequisites</span></span>
<span data-ttu-id="e2b08-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2b08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2b08-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e2b08-111">Permission type</span></span>|<span data-ttu-id="e2b08-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e2b08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2b08-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e2b08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2b08-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2b08-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e2b08-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e2b08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2b08-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2b08-116">Not supported.</span></span>|
|<span data-ttu-id="e2b08-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e2b08-117">Application</span></span>|<span data-ttu-id="e2b08-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2b08-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2b08-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e2b08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e2b08-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e2b08-120">Request headers</span></span>
|<span data-ttu-id="e2b08-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e2b08-121">Header</span></span>|<span data-ttu-id="e2b08-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e2b08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2b08-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2b08-123">Authorization</span></span>|<span data-ttu-id="e2b08-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e2b08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2b08-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e2b08-125">Accept</span></span>|<span data-ttu-id="e2b08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2b08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2b08-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e2b08-127">Request body</span></span>
<span data-ttu-id="e2b08-128">В теле запроса добавьте представление объекта macOSDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2b08-128">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="e2b08-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e2b08-129">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="e2b08-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2b08-130">Property</span></span>|<span data-ttu-id="e2b08-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e2b08-131">Type</span></span>|<span data-ttu-id="e2b08-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e2b08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2b08-133">id</span><span class="sxs-lookup"><span data-stu-id="e2b08-133">id</span></span>|<span data-ttu-id="e2b08-134">String</span><span class="sxs-lookup"><span data-stu-id="e2b08-134">String</span></span>|<span data-ttu-id="e2b08-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e2b08-135">Key of the entity.</span></span> <span data-ttu-id="e2b08-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2b08-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2b08-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2b08-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e2b08-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2b08-138">DateTimeOffset</span></span>|<span data-ttu-id="e2b08-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e2b08-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e2b08-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2b08-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2b08-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e2b08-141">roleScopeTagIds</span></span>|<span data-ttu-id="e2b08-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e2b08-142">String collection</span></span>|<span data-ttu-id="e2b08-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="e2b08-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e2b08-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2b08-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2b08-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="e2b08-145">supportsScopeTags</span></span>|<span data-ttu-id="e2b08-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-146">Boolean</span></span>|<span data-ttu-id="e2b08-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="e2b08-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e2b08-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="e2b08-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e2b08-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="e2b08-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e2b08-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e2b08-150">This property is read-only.</span></span> <span data-ttu-id="e2b08-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2b08-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2b08-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e2b08-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e2b08-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e2b08-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e2b08-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e2b08-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e2b08-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2b08-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2b08-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e2b08-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e2b08-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e2b08-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e2b08-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e2b08-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e2b08-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2b08-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2b08-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e2b08-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e2b08-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e2b08-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e2b08-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e2b08-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e2b08-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2b08-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2b08-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2b08-164">createdDateTime</span></span>|<span data-ttu-id="e2b08-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2b08-165">DateTimeOffset</span></span>|<span data-ttu-id="e2b08-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e2b08-166">DateTime the object was created.</span></span> <span data-ttu-id="e2b08-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2b08-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2b08-168">description</span><span class="sxs-lookup"><span data-stu-id="e2b08-168">description</span></span>|<span data-ttu-id="e2b08-169">String</span><span class="sxs-lookup"><span data-stu-id="e2b08-169">String</span></span>|<span data-ttu-id="e2b08-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2b08-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e2b08-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2b08-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2b08-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e2b08-172">displayName</span></span>|<span data-ttu-id="e2b08-173">String</span><span class="sxs-lookup"><span data-stu-id="e2b08-173">String</span></span>|<span data-ttu-id="e2b08-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2b08-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e2b08-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2b08-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2b08-176">version</span><span class="sxs-lookup"><span data-stu-id="e2b08-176">version</span></span>|<span data-ttu-id="e2b08-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e2b08-177">Int32</span></span>|<span data-ttu-id="e2b08-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e2b08-178">Version of the device configuration.</span></span> <span data-ttu-id="e2b08-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e2b08-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e2b08-180">аирпринтдестинатионс</span><span class="sxs-lookup"><span data-stu-id="e2b08-180">airPrintDestinations</span></span>|<span data-ttu-id="e2b08-181">Коллекция [аирпринтдестинатион](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="e2b08-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="e2b08-182">Массив принтеров Аирпринт, которые должны отображаться всегда.</span><span class="sxs-lookup"><span data-stu-id="e2b08-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="e2b08-183">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e2b08-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="e2b08-184">Наследуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="e2b08-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="e2b08-185">аутолаунчитемс</span><span class="sxs-lookup"><span data-stu-id="e2b08-185">autoLaunchItems</span></span>|<span data-ttu-id="e2b08-186">Коллекция [макослаунчитем](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="e2b08-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="e2b08-187">Список приложений, файлов, папок и других элементов, которые запускаются при входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="e2b08-187">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="e2b08-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e2b08-188">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e2b08-189">админшовхостинфо</span><span class="sxs-lookup"><span data-stu-id="e2b08-189">adminShowHostInfo</span></span>|<span data-ttu-id="e2b08-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-190">Boolean</span></span>|<span data-ttu-id="e2b08-191">Показывать ли сведения об узле администратора в окне входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-191">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="e2b08-192">логинвиндовтекст</span><span class="sxs-lookup"><span data-stu-id="e2b08-192">loginWindowText</span></span>|<span data-ttu-id="e2b08-193">String</span><span class="sxs-lookup"><span data-stu-id="e2b08-193">String</span></span>|<span data-ttu-id="e2b08-194">Настраиваемый текст, отображаемый в окне входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-194">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="e2b08-195">аусоризедусерслиссидден</span><span class="sxs-lookup"><span data-stu-id="e2b08-195">authorizedUsersListHidden</span></span>|<span data-ttu-id="e2b08-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-196">Boolean</span></span>|<span data-ttu-id="e2b08-197">Указывает, следует ли отображать диалоговое окно имя и пароль или список пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-197">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="e2b08-198">аусоризедусерслиссиделокалусерс</span><span class="sxs-lookup"><span data-stu-id="e2b08-198">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="e2b08-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-199">Boolean</span></span>|<span data-ttu-id="e2b08-200">Отображение только сетевых и системных пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-200">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="e2b08-201">аусоризедусерслиссидемобилеаккаунтс</span><span class="sxs-lookup"><span data-stu-id="e2b08-201">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="e2b08-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-202">Boolean</span></span>|<span data-ttu-id="e2b08-203">Следует ли скрыть пользователей для мобильных устройств в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-203">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="e2b08-204">аусоризедусерслистинклуденетворкусерс</span><span class="sxs-lookup"><span data-stu-id="e2b08-204">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="e2b08-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-205">Boolean</span></span>|<span data-ttu-id="e2b08-206">Показывать ли пользователей сети в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-206">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="e2b08-207">аусоризедусерслиссидеадминусерс</span><span class="sxs-lookup"><span data-stu-id="e2b08-207">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="e2b08-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-208">Boolean</span></span>|<span data-ttu-id="e2b08-209">Указывает, следует ли скрыть пользователей Admin в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-209">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="e2b08-210">аусоризедусерслистшовосерманажедусерс</span><span class="sxs-lookup"><span data-stu-id="e2b08-210">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="e2b08-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-211">Boolean</span></span>|<span data-ttu-id="e2b08-212">Указывает, следует ли показывать других пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-212">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="e2b08-213">шутдовндисаблед</span><span class="sxs-lookup"><span data-stu-id="e2b08-213">shutDownDisabled</span></span>|<span data-ttu-id="e2b08-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-214">Boolean</span></span>|<span data-ttu-id="e2b08-215">Указывает, следует ли скрыть элемент кнопка "завершение работы" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-215">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="e2b08-216">рестартдисаблед</span><span class="sxs-lookup"><span data-stu-id="e2b08-216">restartDisabled</span></span>|<span data-ttu-id="e2b08-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-217">Boolean</span></span>|<span data-ttu-id="e2b08-218">Указывает, следует ли скрыть элемент "Кнопка перезапуска" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-218">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="e2b08-219">слипдисаблед</span><span class="sxs-lookup"><span data-stu-id="e2b08-219">sleepDisabled</span></span>|<span data-ttu-id="e2b08-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-220">Boolean</span></span>|<span data-ttu-id="e2b08-221">Указывает, следует ли скрыть пункт меню "сон" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-221">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="e2b08-222">консолеакцессдисаблед</span><span class="sxs-lookup"><span data-stu-id="e2b08-222">consoleAccessDisabled</span></span>|<span data-ttu-id="e2b08-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-223">Boolean</span></span>|<span data-ttu-id="e2b08-224">Будет ли другой пользователь игнорировать использование консоли ">"> специального имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="e2b08-224">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="e2b08-225">шутдовндисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="e2b08-225">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="e2b08-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-226">Boolean</span></span>|<span data-ttu-id="e2b08-227">Будет ли отключен элемент меню "завершение работы" в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="e2b08-227">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="e2b08-228">рестартдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="e2b08-228">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="e2b08-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-229">Boolean</span></span>|<span data-ttu-id="e2b08-230">Будет ли отключен элемент меню перезапуска в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="e2b08-230">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="e2b08-231">повероффдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="e2b08-231">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="e2b08-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-232">Boolean</span></span>|<span data-ttu-id="e2b08-233">Будет ли отключен элемент меню Power of Power в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="e2b08-233">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="e2b08-234">логаутдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="e2b08-234">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="e2b08-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-235">Boolean</span></span>|<span data-ttu-id="e2b08-236">Будет ли отключен элемент меню журнала в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="e2b08-236">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="e2b08-237">скринлоккдисаблеиммедиате</span><span class="sxs-lookup"><span data-stu-id="e2b08-237">screenLockDisableImmediate</span></span>|<span data-ttu-id="e2b08-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-238">Boolean</span></span>|<span data-ttu-id="e2b08-239">Следует ли отключить функции немедленной блокировки экрана.</span><span class="sxs-lookup"><span data-stu-id="e2b08-239">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="e2b08-240">ассоЦиатеддомаинс</span><span class="sxs-lookup"><span data-stu-id="e2b08-240">associatedDomains</span></span>|<span data-ttu-id="e2b08-241">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e2b08-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e2b08-242">Получает или задает список, который сопоставляет приложения с их связанными доменами.</span><span class="sxs-lookup"><span data-stu-id="e2b08-242">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="e2b08-243">Ключ должен соответствовать ИДЕНТИФИКАТОРу приложения, а значение должно быть строкой в виде "Service: domain", где Domain — это полное доменное имя узла (например,:ексампле.. com).</span><span class="sxs-lookup"><span data-stu-id="e2b08-243">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="e2b08-244">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e2b08-244">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e2b08-245">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="e2b08-245">singleSignOnExtension</span></span>|[<span data-ttu-id="e2b08-246">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="e2b08-246">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="e2b08-247">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-247">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="e2b08-248">Устарело: вместо этого используйте Макоссинглесигнонекстенсион.</span><span class="sxs-lookup"><span data-stu-id="e2b08-248">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="e2b08-249">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="e2b08-249">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="e2b08-250">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="e2b08-250">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="e2b08-251">Получает или задает профиль расширения единого входа.</span><span class="sxs-lookup"><span data-stu-id="e2b08-251">Gets or sets a single sign-on extension profile.</span></span>|
|<span data-ttu-id="e2b08-252">контенткачинженаблед</span><span class="sxs-lookup"><span data-stu-id="e2b08-252">contentCachingEnabled</span></span>|<span data-ttu-id="e2b08-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-253">Boolean</span></span>|<span data-ttu-id="e2b08-254">Включает кэширование контента и предотвращает его отключение пользователем.</span><span class="sxs-lookup"><span data-stu-id="e2b08-254">Enables content caching and prevents it from being disabled by the user.</span></span>|
|<span data-ttu-id="e2b08-255">контенткачингтипе</span><span class="sxs-lookup"><span data-stu-id="e2b08-255">contentCachingType</span></span>|[<span data-ttu-id="e2b08-256">macOSContentCachingType</span><span class="sxs-lookup"><span data-stu-id="e2b08-256">macOSContentCachingType</span></span>](../resources/intune-deviceconfig-macoscontentcachingtype.md)|<span data-ttu-id="e2b08-257">Определяет, какой тип контента может кэшироваться службой кэширования контента Apple.</span><span class="sxs-lookup"><span data-stu-id="e2b08-257">Determines what type of content is allowed to be cached by Apple's content caching service.</span></span> <span data-ttu-id="e2b08-258">Возможные значения: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span><span class="sxs-lookup"><span data-stu-id="e2b08-258">Possible values are: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span></span>|
|<span data-ttu-id="e2b08-259">контенткачингмакссизебитес</span><span class="sxs-lookup"><span data-stu-id="e2b08-259">contentCachingMaxSizeBytes</span></span>|<span data-ttu-id="e2b08-260">Int32</span><span class="sxs-lookup"><span data-stu-id="e2b08-260">Int32</span></span>|<span data-ttu-id="e2b08-261">Максимальное количество байт дискового пространства, которое будет использоваться для кэша контента.</span><span class="sxs-lookup"><span data-stu-id="e2b08-261">The maximum number of bytes of disk space that will be used for the content cache.</span></span> <span data-ttu-id="e2b08-262">Значение 0 (по умолчанию) указывает на неограниченное дисковое пространство.</span><span class="sxs-lookup"><span data-stu-id="e2b08-262">A value of 0 (default) indicates unlimited disk space.</span></span> |
|<span data-ttu-id="e2b08-263">контенткачингдатапас</span><span class="sxs-lookup"><span data-stu-id="e2b08-263">contentCachingDataPath</span></span>|<span data-ttu-id="e2b08-264">String</span><span class="sxs-lookup"><span data-stu-id="e2b08-264">String</span></span>|<span data-ttu-id="e2b08-265">Путь к каталогу, используемому для хранения кэшированного содержимого.</span><span class="sxs-lookup"><span data-stu-id="e2b08-265">The path to the directory used to store cached content.</span></span> <span data-ttu-id="e2b08-266">Значение должно быть (или оканчиваться) поддержкой/Library/Application/Apple/Ассеткаче/Data</span><span class="sxs-lookup"><span data-stu-id="e2b08-266">The value must be (or end with) /Library/Application Support/Apple/AssetCache/Data</span></span>|
|<span data-ttu-id="e2b08-267">контенткачингдисаблеконнектионшаринг</span><span class="sxs-lookup"><span data-stu-id="e2b08-267">contentCachingDisableConnectionSharing</span></span>|<span data-ttu-id="e2b08-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-268">Boolean</span></span>|<span data-ttu-id="e2b08-269">Отключает общий доступ к подключению к Интернету.</span><span class="sxs-lookup"><span data-stu-id="e2b08-269">Disables internet connection sharing.</span></span>|
|<span data-ttu-id="e2b08-270">контенткачингфорцеконнектионшаринг</span><span class="sxs-lookup"><span data-stu-id="e2b08-270">contentCachingForceConnectionSharing</span></span>|<span data-ttu-id="e2b08-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-271">Boolean</span></span>|<span data-ttu-id="e2b08-272">Обеспечивает принудительное предоставление общего доступа к подключению к Интернету.</span><span class="sxs-lookup"><span data-stu-id="e2b08-272">Forces internet connection sharing.</span></span> <span data-ttu-id="e2b08-273">Контенткачингдисаблеконнектионшаринг переопределяет этот параметр.</span><span class="sxs-lookup"><span data-stu-id="e2b08-273">contentCachingDisableConnectionSharing overrides this setting.</span></span>|
|<span data-ttu-id="e2b08-274">контенткачингклиентполици</span><span class="sxs-lookup"><span data-stu-id="e2b08-274">contentCachingClientPolicy</span></span>|[<span data-ttu-id="e2b08-275">macOSContentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="e2b08-275">macOSContentCachingClientPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|<span data-ttu-id="e2b08-276">Определяет метод, используемый серверами кэширования контента для прослушивания клиентов.</span><span class="sxs-lookup"><span data-stu-id="e2b08-276">Determines the method in which content caching servers will listen for clients.</span></span> <span data-ttu-id="e2b08-277">Возможные значения: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span><span class="sxs-lookup"><span data-stu-id="e2b08-277">Possible values are: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span></span>|
|<span data-ttu-id="e2b08-278">контенткачингклиентлистенранжес</span><span class="sxs-lookup"><span data-stu-id="e2b08-278">contentCachingClientListenRanges</span></span>|<span data-ttu-id="e2b08-279">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e2b08-279">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="e2b08-280">Список настраиваемых диапазонов содержимого диапазонов IP-адресов будет использоваться для прослушивания клиентов.</span><span class="sxs-lookup"><span data-stu-id="e2b08-280">A list of custom IP ranges content caches will use to listen for clients.</span></span> <span data-ttu-id="e2b08-281">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e2b08-281">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e2b08-282">контенткачингпирполици</span><span class="sxs-lookup"><span data-stu-id="e2b08-282">contentCachingPeerPolicy</span></span>|[<span data-ttu-id="e2b08-283">macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="e2b08-283">macOSContentCachingPeerPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|<span data-ttu-id="e2b08-284">Определяет метод, в котором содержимое кэшируется на одноранговом узле с другими кэшами.</span><span class="sxs-lookup"><span data-stu-id="e2b08-284">Determines the method in which content caches peer with other caches.</span></span> <span data-ttu-id="e2b08-285">Возможные значения: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span><span class="sxs-lookup"><span data-stu-id="e2b08-285">Possible values are: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span></span>|
|<span data-ttu-id="e2b08-286">контенткачингпирлистенранжес</span><span class="sxs-lookup"><span data-stu-id="e2b08-286">contentCachingPeerListenRanges</span></span>|<span data-ttu-id="e2b08-287">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e2b08-287">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="e2b08-288">Список настраиваемых диапазонов содержимого диапазонов IP-адресов будет использоваться для прослушивания одноранговых кэшей.</span><span class="sxs-lookup"><span data-stu-id="e2b08-288">A list of custom IP ranges content caches will use to listen for peer caches.</span></span> <span data-ttu-id="e2b08-289">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e2b08-289">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e2b08-290">контенткачингпирфилтерранжес</span><span class="sxs-lookup"><span data-stu-id="e2b08-290">contentCachingPeerFilterRanges</span></span>|<span data-ttu-id="e2b08-291">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e2b08-291">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="e2b08-292">Список настраиваемых диапазонов содержимого диапазонов IP-адресов будет использоваться для запроса контента от кэш-памяти одноранговых узлов.</span><span class="sxs-lookup"><span data-stu-id="e2b08-292">A list of custom IP ranges content caches will use to query for content from peers caches.</span></span> <span data-ttu-id="e2b08-293">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e2b08-293">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e2b08-294">контенткачингпарентселектионполици</span><span class="sxs-lookup"><span data-stu-id="e2b08-294">contentCachingParentSelectionPolicy</span></span>|[<span data-ttu-id="e2b08-295">macOSContentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e2b08-295">macOSContentCachingParentSelectionPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|<span data-ttu-id="e2b08-296">Определяет метод, в котором серверы кэширования контента будут выбирать родительские элементы, если они есть.</span><span class="sxs-lookup"><span data-stu-id="e2b08-296">Determines the method in which content caching servers will select parents if multiple are present.</span></span> <span data-ttu-id="e2b08-297">Возможные значения: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span><span class="sxs-lookup"><span data-stu-id="e2b08-297">Possible values are: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span></span>|
|<span data-ttu-id="e2b08-298">контенткачингпарентс</span><span class="sxs-lookup"><span data-stu-id="e2b08-298">contentCachingParents</span></span>|<span data-ttu-id="e2b08-299">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e2b08-299">String collection</span></span>|<span data-ttu-id="e2b08-300">Список IP-адресов, представляющих родительские кэши контента.</span><span class="sxs-lookup"><span data-stu-id="e2b08-300">A list of IP addresses representing parent content caches.</span></span>|
|<span data-ttu-id="e2b08-301">контенткачинглогклиентидентитиес</span><span class="sxs-lookup"><span data-stu-id="e2b08-301">contentCachingLogClientIdentities</span></span>|<span data-ttu-id="e2b08-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-302">Boolean</span></span>|<span data-ttu-id="e2b08-303">Включает ведение журнала IP-адресов и портов клиентов, запрашивающих кэшированное содержимое.</span><span class="sxs-lookup"><span data-stu-id="e2b08-303">Enables logging of IP addresses and ports of clients that request cached content.</span></span>|
|<span data-ttu-id="e2b08-304">контенткачингпубликранжес</span><span class="sxs-lookup"><span data-stu-id="e2b08-304">contentCachingPublicRanges</span></span>|<span data-ttu-id="e2b08-305">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e2b08-305">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="e2b08-306">Список настраиваемых диапазонов IP-адресов, которые служба кэширования контента Apple должна использовать для согласования клиентов со кэшами контента.</span><span class="sxs-lookup"><span data-stu-id="e2b08-306">A list of custom IP ranges that Apple's content caching service should use to match clients to content caches.</span></span> <span data-ttu-id="e2b08-307">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="e2b08-307">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e2b08-308">контенткачингблоккделетион</span><span class="sxs-lookup"><span data-stu-id="e2b08-308">contentCachingBlockDeletion</span></span>|<span data-ttu-id="e2b08-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-309">Boolean</span></span>|<span data-ttu-id="e2b08-310">Предотвращает очистку содержимого кэшами, чтобы освободить место на диске для других приложений.</span><span class="sxs-lookup"><span data-stu-id="e2b08-310">Prevents content caches from purging content to free up disk space for other apps.</span></span>|
|<span data-ttu-id="e2b08-311">контенткачингшовалертс</span><span class="sxs-lookup"><span data-stu-id="e2b08-311">contentCachingShowAlerts</span></span>|<span data-ttu-id="e2b08-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-312">Boolean</span></span>|<span data-ttu-id="e2b08-313">Отображение оповещений о кэшировании содержимого как системных уведомлений.</span><span class="sxs-lookup"><span data-stu-id="e2b08-313">Display content caching alerts as system notifications.</span></span>|
|<span data-ttu-id="e2b08-314">контенткачингкипаваке</span><span class="sxs-lookup"><span data-stu-id="e2b08-314">contentCachingKeepAwake</span></span>|<span data-ttu-id="e2b08-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b08-315">Boolean</span></span>|<span data-ttu-id="e2b08-316">Запретите переустановку устройства в спящий режим, если включено кэширование содержимого.</span><span class="sxs-lookup"><span data-stu-id="e2b08-316">Prevent the device from sleeping if content caching is enabled.</span></span>|
|<span data-ttu-id="e2b08-317">контенткачингпорт</span><span class="sxs-lookup"><span data-stu-id="e2b08-317">contentCachingPort</span></span>|<span data-ttu-id="e2b08-318">Int32</span><span class="sxs-lookup"><span data-stu-id="e2b08-318">Int32</span></span>|<span data-ttu-id="e2b08-319">Задает порт, используемый для кэширования контента.</span><span class="sxs-lookup"><span data-stu-id="e2b08-319">Sets the port used for content caching.</span></span> <span data-ttu-id="e2b08-320">Если значение равно 0, будет выбран произвольный доступный порт.</span><span class="sxs-lookup"><span data-stu-id="e2b08-320">If the value is 0, a random available port will be selected.</span></span> <span data-ttu-id="e2b08-321">Допустимые значения — от 0 до 65535</span><span class="sxs-lookup"><span data-stu-id="e2b08-321">Valid values 0 to 65535</span></span>|



## <a name="response"></a><span data-ttu-id="e2b08-322">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2b08-322">Response</span></span>
<span data-ttu-id="e2b08-323">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e2b08-323">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2b08-324">Пример</span><span class="sxs-lookup"><span data-stu-id="e2b08-324">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2b08-325">Запрос</span><span class="sxs-lookup"><span data-stu-id="e2b08-325">Request</span></span>
<span data-ttu-id="e2b08-326">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e2b08-326">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5388

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
    "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
    "extensionIdentifier": "Extension Identifier value",
    "teamIdentifier": "Team Identifier value",
    "domains": [
      "Domains value"
    ],
    "realm": "Realm value",
    "configurations": [
      {
        "@odata.type": "microsoft.graph.keyStringValuePair",
        "key": "Key value",
        "value": "Value value"
      }
    ]
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  },
  "contentCachingEnabled": true,
  "contentCachingType": "userContentOnly",
  "contentCachingMaxSizeBytes": 10,
  "contentCachingDataPath": "Content Caching Data Path value",
  "contentCachingDisableConnectionSharing": true,
  "contentCachingForceConnectionSharing": true,
  "contentCachingClientPolicy": "clientsInLocalNetwork",
  "contentCachingClientListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerPolicy": "peersInLocalNetwork",
  "contentCachingPeerListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerFilterRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingParentSelectionPolicy": "roundRobin",
  "contentCachingParents": [
    "Content Caching Parents value"
  ],
  "contentCachingLogClientIdentities": true,
  "contentCachingPublicRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingBlockDeletion": true,
  "contentCachingShowAlerts": true,
  "contentCachingKeepAwake": true,
  "contentCachingPort": 2
}
```

### <a name="response"></a><span data-ttu-id="e2b08-327">Отклик</span><span class="sxs-lookup"><span data-stu-id="e2b08-327">Response</span></span>
<span data-ttu-id="e2b08-p129">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e2b08-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5560

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
    "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
    "extensionIdentifier": "Extension Identifier value",
    "teamIdentifier": "Team Identifier value",
    "domains": [
      "Domains value"
    ],
    "realm": "Realm value",
    "configurations": [
      {
        "@odata.type": "microsoft.graph.keyStringValuePair",
        "key": "Key value",
        "value": "Value value"
      }
    ]
  },
  "macOSSingleSignOnExtension": {
    "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
    "realm": "Realm value",
    "domains": [
      "Domains value"
    ],
    "blockAutomaticLogin": true,
    "cacheName": "Cache Name value",
    "credentialBundleIdAccessControlList": [
      "Credential Bundle Id Access Control List value"
    ],
    "domainRealms": [
      "Domain Realms value"
    ],
    "isDefaultRealm": true,
    "passwordBlockModification": true,
    "passwordExpirationDays": 6,
    "passwordExpirationNotificationDays": 2,
    "userPrincipalName": "User Principal Name value",
    "passwordRequireActiveDirectoryComplexity": true,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumLength": 5,
    "passwordMinimumAgeDays": 6,
    "passwordRequirementsDescription": "Password Requirements Description value",
    "requireUserPresence": true,
    "activeDirectorySiteCode": "Active Directory Site Code value",
    "passwordEnableLocalSync": true,
    "blockActiveDirectorySiteAutoDiscovery": true,
    "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
  },
  "contentCachingEnabled": true,
  "contentCachingType": "userContentOnly",
  "contentCachingMaxSizeBytes": 10,
  "contentCachingDataPath": "Content Caching Data Path value",
  "contentCachingDisableConnectionSharing": true,
  "contentCachingForceConnectionSharing": true,
  "contentCachingClientPolicy": "clientsInLocalNetwork",
  "contentCachingClientListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerPolicy": "peersInLocalNetwork",
  "contentCachingPeerListenRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingPeerFilterRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingParentSelectionPolicy": "roundRobin",
  "contentCachingParents": [
    "Content Caching Parents value"
  ],
  "contentCachingLogClientIdentities": true,
  "contentCachingPublicRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "Lower Address value",
      "upperAddress": "Upper Address value"
    }
  ],
  "contentCachingBlockDeletion": true,
  "contentCachingShowAlerts": true,
  "contentCachingKeepAwake": true,
  "contentCachingPort": 2
}
```






