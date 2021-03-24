---
title: Создание объекта macOSDeviceFeaturesConfiguration
description: Создание объекта macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9d85d2ff96b4da0dea48bce3f8148a7bd93a71fd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147708"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="14eec-103">Создание объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="14eec-103">Create macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="14eec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14eec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14eec-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14eec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14eec-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14eec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14eec-107">Создание объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eec-107">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14eec-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="14eec-108">Prerequisites</span></span>
<span data-ttu-id="14eec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14eec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14eec-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14eec-111">Permission type</span></span>|<span data-ttu-id="14eec-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14eec-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14eec-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14eec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14eec-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14eec-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14eec-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14eec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14eec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14eec-116">Not supported.</span></span>|
|<span data-ttu-id="14eec-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="14eec-117">Application</span></span>|<span data-ttu-id="14eec-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14eec-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14eec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14eec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="14eec-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="14eec-120">Request headers</span></span>
|<span data-ttu-id="14eec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14eec-121">Header</span></span>|<span data-ttu-id="14eec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="14eec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14eec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14eec-123">Authorization</span></span>|<span data-ttu-id="14eec-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14eec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14eec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14eec-125">Accept</span></span>|<span data-ttu-id="14eec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14eec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14eec-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14eec-127">Request body</span></span>
<span data-ttu-id="14eec-128">В теле запроса добавьте представление объекта macOSDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14eec-128">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="14eec-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="14eec-129">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="14eec-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="14eec-130">Property</span></span>|<span data-ttu-id="14eec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="14eec-131">Type</span></span>|<span data-ttu-id="14eec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="14eec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14eec-133">id</span><span class="sxs-lookup"><span data-stu-id="14eec-133">id</span></span>|<span data-ttu-id="14eec-134">Строка</span><span class="sxs-lookup"><span data-stu-id="14eec-134">String</span></span>|<span data-ttu-id="14eec-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="14eec-135">Key of the entity.</span></span> <span data-ttu-id="14eec-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eec-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eec-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14eec-137">lastModifiedDateTime</span></span>|<span data-ttu-id="14eec-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14eec-138">DateTimeOffset</span></span>|<span data-ttu-id="14eec-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="14eec-139">DateTime the object was last modified.</span></span> <span data-ttu-id="14eec-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eec-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eec-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="14eec-141">roleScopeTagIds</span></span>|<span data-ttu-id="14eec-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="14eec-142">String collection</span></span>|<span data-ttu-id="14eec-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="14eec-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="14eec-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eec-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eec-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="14eec-145">supportsScopeTags</span></span>|<span data-ttu-id="14eec-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-146">Boolean</span></span>|<span data-ttu-id="14eec-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="14eec-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="14eec-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="14eec-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="14eec-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="14eec-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="14eec-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="14eec-150">This property is read-only.</span></span> <span data-ttu-id="14eec-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eec-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eec-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="14eec-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="14eec-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="14eec-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="14eec-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="14eec-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="14eec-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eec-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eec-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="14eec-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="14eec-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="14eec-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="14eec-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="14eec-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="14eec-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eec-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eec-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="14eec-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="14eec-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="14eec-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="14eec-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="14eec-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="14eec-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eec-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eec-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14eec-164">createdDateTime</span></span>|<span data-ttu-id="14eec-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14eec-165">DateTimeOffset</span></span>|<span data-ttu-id="14eec-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="14eec-166">DateTime the object was created.</span></span> <span data-ttu-id="14eec-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eec-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eec-168">description</span><span class="sxs-lookup"><span data-stu-id="14eec-168">description</span></span>|<span data-ttu-id="14eec-169">Строка</span><span class="sxs-lookup"><span data-stu-id="14eec-169">String</span></span>|<span data-ttu-id="14eec-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14eec-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="14eec-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eec-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eec-172">displayName</span><span class="sxs-lookup"><span data-stu-id="14eec-172">displayName</span></span>|<span data-ttu-id="14eec-173">Строка</span><span class="sxs-lookup"><span data-stu-id="14eec-173">String</span></span>|<span data-ttu-id="14eec-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14eec-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="14eec-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eec-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eec-176">version</span><span class="sxs-lookup"><span data-stu-id="14eec-176">version</span></span>|<span data-ttu-id="14eec-177">Int32</span><span class="sxs-lookup"><span data-stu-id="14eec-177">Int32</span></span>|<span data-ttu-id="14eec-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="14eec-178">Version of the device configuration.</span></span> <span data-ttu-id="14eec-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="14eec-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14eec-180">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="14eec-180">airPrintDestinations</span></span>|<span data-ttu-id="14eec-181">[коллекция airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="14eec-181">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="14eec-182">Массив принтеров AirPrint, которые всегда должны быть показаны.</span><span class="sxs-lookup"><span data-stu-id="14eec-182">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="14eec-183">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="14eec-183">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="14eec-184">Унаследованный от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="14eec-184">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="14eec-185">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="14eec-185">autoLaunchItems</span></span>|<span data-ttu-id="14eec-186">[коллекция macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="14eec-186">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="14eec-187">Список приложений, файлов, папок и других элементов, которые необходимо запустить при входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="14eec-187">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="14eec-188">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="14eec-188">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="14eec-189">adminShowHostInfo</span><span class="sxs-lookup"><span data-stu-id="14eec-189">adminShowHostInfo</span></span>|<span data-ttu-id="14eec-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-190">Boolean</span></span>|<span data-ttu-id="14eec-191">Следует ли показывать сведения о хост-администраторе в окне входа.</span><span class="sxs-lookup"><span data-stu-id="14eec-191">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="14eec-192">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="14eec-192">loginWindowText</span></span>|<span data-ttu-id="14eec-193">Строка</span><span class="sxs-lookup"><span data-stu-id="14eec-193">String</span></span>|<span data-ttu-id="14eec-194">Пользовательский текст, отображаемый в окне входа.</span><span class="sxs-lookup"><span data-stu-id="14eec-194">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="14eec-195">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="14eec-195">authorizedUsersListHidden</span></span>|<span data-ttu-id="14eec-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-196">Boolean</span></span>|<span data-ttu-id="14eec-197">Следует ли показывать диалоговое окно имени и пароля или список пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="14eec-197">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="14eec-198">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="14eec-198">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="14eec-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-199">Boolean</span></span>|<span data-ttu-id="14eec-200">Следует ли показывать только сетевых и системных пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="14eec-200">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="14eec-201">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="14eec-201">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="14eec-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-202">Boolean</span></span>|<span data-ttu-id="14eec-203">Следует ли скрывать мобильных пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="14eec-203">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="14eec-204">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="14eec-204">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="14eec-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-205">Boolean</span></span>|<span data-ttu-id="14eec-206">Следует ли показывать сетевых пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="14eec-206">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="14eec-207">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="14eec-207">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="14eec-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-208">Boolean</span></span>|<span data-ttu-id="14eec-209">Следует ли скрывать пользователей администратора в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="14eec-209">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="14eec-210">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="14eec-210">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="14eec-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-211">Boolean</span></span>|<span data-ttu-id="14eec-212">Следует ли показывать других пользователей в списке авторизованного пользователя в окне входа.</span><span class="sxs-lookup"><span data-stu-id="14eec-212">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="14eec-213">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="14eec-213">shutDownDisabled</span></span>|<span data-ttu-id="14eec-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-214">Boolean</span></span>|<span data-ttu-id="14eec-215">Следует ли скрывать элемент кнопки Shut Down в окне входа.</span><span class="sxs-lookup"><span data-stu-id="14eec-215">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="14eec-216">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="14eec-216">restartDisabled</span></span>|<span data-ttu-id="14eec-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-217">Boolean</span></span>|<span data-ttu-id="14eec-218">Следует ли скрывать элемент кнопки Перезапуска в окне входа.</span><span class="sxs-lookup"><span data-stu-id="14eec-218">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="14eec-219">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="14eec-219">sleepDisabled</span></span>|<span data-ttu-id="14eec-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-220">Boolean</span></span>|<span data-ttu-id="14eec-221">Следует ли скрывать элемент меню Sleep в окне входа.</span><span class="sxs-lookup"><span data-stu-id="14eec-221">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="14eec-222">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="14eec-222">consoleAccessDisabled</span></span>|<span data-ttu-id="14eec-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-223">Boolean</span></span>|<span data-ttu-id="14eec-224">Будет ли другой пользователь игнорировать использование>консоли> имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="14eec-224">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="14eec-225">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="14eec-225">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="14eec-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-226">Boolean</span></span>|<span data-ttu-id="14eec-227">Будет ли отключен элемент меню Shut Down в окне входа во время входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="14eec-227">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="14eec-228">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="14eec-228">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="14eec-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-229">Boolean</span></span>|<span data-ttu-id="14eec-230">Будет ли элемент меню Перезапуска в окне входа отключен во время входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="14eec-230">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="14eec-231">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="14eec-231">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="14eec-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-232">Boolean</span></span>|<span data-ttu-id="14eec-233">Будет ли отключен элемент меню Power Off в окне входа во время входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="14eec-233">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="14eec-234">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="14eec-234">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="14eec-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-235">Boolean</span></span>|<span data-ttu-id="14eec-236">Будет ли отключен элемент меню Log Out в окне входа во время входа пользователя.</span><span class="sxs-lookup"><span data-stu-id="14eec-236">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="14eec-237">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="14eec-237">screenLockDisableImmediate</span></span>|<span data-ttu-id="14eec-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-238">Boolean</span></span>|<span data-ttu-id="14eec-239">Следует ли отключить функции немедленной блокировки экрана.</span><span class="sxs-lookup"><span data-stu-id="14eec-239">Whether to disable the immediate screen lock functions.</span></span>|
|<span data-ttu-id="14eec-240">associatedDomains</span><span class="sxs-lookup"><span data-stu-id="14eec-240">associatedDomains</span></span>|<span data-ttu-id="14eec-241">Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="14eec-241">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="14eec-242">DEPRECATED: вместо этого используйте appAssociatedDomains.</span><span class="sxs-lookup"><span data-stu-id="14eec-242">DEPRECATED: use appAssociatedDomains instead.</span></span> <span data-ttu-id="14eec-243">Получает или задает список, который сопополагает приложения с связанными доменами.</span><span class="sxs-lookup"><span data-stu-id="14eec-243">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="14eec-244">Ключ должен соответствовать ID приложения, а значение должно быть строкой в виде "service:domain", где домен является полнокровным имям хост-сайта (например, webcredentials:example.com).</span><span class="sxs-lookup"><span data-stu-id="14eec-244">The key should match the app's ID, and the value should be a string in the form of "service:domain" where domain is a fully qualified hostname (e.g. webcredentials:example.com).</span></span> <span data-ttu-id="14eec-245">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="14eec-245">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="14eec-246">appAssociatedDomains</span><span class="sxs-lookup"><span data-stu-id="14eec-246">appAssociatedDomains</span></span>|<span data-ttu-id="14eec-247">[коллекция macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md)</span><span class="sxs-lookup"><span data-stu-id="14eec-247">[macOSAssociatedDomainsItem](../resources/intune-deviceconfig-macosassociateddomainsitem.md) collection</span></span>|<span data-ttu-id="14eec-248">Получает или задает список, который сопополагает приложения с связанными доменами.</span><span class="sxs-lookup"><span data-stu-id="14eec-248">Gets or sets a list that maps apps to their associated domains.</span></span> <span data-ttu-id="14eec-249">Идентификаторы приложений должны быть уникальными.</span><span class="sxs-lookup"><span data-stu-id="14eec-249">Application identifiers must be unique.</span></span> <span data-ttu-id="14eec-250">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="14eec-250">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="14eec-251">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="14eec-251">singleSignOnExtension</span></span>|[<span data-ttu-id="14eec-252">singleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="14eec-252">singleSignOnExtension</span></span>](../resources/intune-deviceconfig-singlesignonextension.md)|<span data-ttu-id="14eec-253">Получает или задает один профиль расширения для входов.</span><span class="sxs-lookup"><span data-stu-id="14eec-253">Gets or sets a single sign-on extension profile.</span></span> <span data-ttu-id="14eec-254">Неуловимый: вместо этого используйте MacOSSingleSignOnExtension.</span><span class="sxs-lookup"><span data-stu-id="14eec-254">Deprecated: use MacOSSingleSignOnExtension instead.</span></span>|
|<span data-ttu-id="14eec-255">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="14eec-255">macOSSingleSignOnExtension</span></span>|[<span data-ttu-id="14eec-256">macOSSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="14eec-256">macOSSingleSignOnExtension</span></span>](../resources/intune-deviceconfig-macossinglesignonextension.md)|<span data-ttu-id="14eec-257">Получает или задает один профиль расширения для входов.</span><span class="sxs-lookup"><span data-stu-id="14eec-257">Gets or sets a single sign-on extension profile.</span></span>|
|<span data-ttu-id="14eec-258">contentCachingEnabled</span><span class="sxs-lookup"><span data-stu-id="14eec-258">contentCachingEnabled</span></span>|<span data-ttu-id="14eec-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-259">Boolean</span></span>|<span data-ttu-id="14eec-260">Включает кэшинг контента и предотвращает его отключение пользователем.</span><span class="sxs-lookup"><span data-stu-id="14eec-260">Enables content caching and prevents it from being disabled by the user.</span></span>|
|<span data-ttu-id="14eec-261">contentCachingType</span><span class="sxs-lookup"><span data-stu-id="14eec-261">contentCachingType</span></span>|[<span data-ttu-id="14eec-262">macOSContentCachingType</span><span class="sxs-lookup"><span data-stu-id="14eec-262">macOSContentCachingType</span></span>](../resources/intune-deviceconfig-macoscontentcachingtype.md)|<span data-ttu-id="14eec-263">Определяет, какой тип контента разрешен кэшировали службой кэшинга контента Apple.</span><span class="sxs-lookup"><span data-stu-id="14eec-263">Determines what type of content is allowed to be cached by Apple's content caching service.</span></span> <span data-ttu-id="14eec-264">Возможные значения: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span><span class="sxs-lookup"><span data-stu-id="14eec-264">Possible values are: `notConfigured`, `userContentOnly`, `sharedContentOnly`.</span></span>|
|<span data-ttu-id="14eec-265">contentCachingMaxSizeBytes</span><span class="sxs-lookup"><span data-stu-id="14eec-265">contentCachingMaxSizeBytes</span></span>|<span data-ttu-id="14eec-266">Int32</span><span class="sxs-lookup"><span data-stu-id="14eec-266">Int32</span></span>|<span data-ttu-id="14eec-267">Максимальное количество bytes дискового пространства, которое будет использоваться для кэша контента.</span><span class="sxs-lookup"><span data-stu-id="14eec-267">The maximum number of bytes of disk space that will be used for the content cache.</span></span> <span data-ttu-id="14eec-268">Значение 0 (по умолчанию) указывает на неограниченное пространство диска.</span><span class="sxs-lookup"><span data-stu-id="14eec-268">A value of 0 (default) indicates unlimited disk space.</span></span> |
|<span data-ttu-id="14eec-269">contentCachingDataPath</span><span class="sxs-lookup"><span data-stu-id="14eec-269">contentCachingDataPath</span></span>|<span data-ttu-id="14eec-270">Строка</span><span class="sxs-lookup"><span data-stu-id="14eec-270">String</span></span>|<span data-ttu-id="14eec-271">Путь к каталогу, используемый для хранения кэшного контента.</span><span class="sxs-lookup"><span data-stu-id="14eec-271">The path to the directory used to store cached content.</span></span> <span data-ttu-id="14eec-272">Значение должно быть (или заканчивается) /Library/Application Support/Apple/AssetCache/Data</span><span class="sxs-lookup"><span data-stu-id="14eec-272">The value must be (or end with) /Library/Application Support/Apple/AssetCache/Data</span></span>|
|<span data-ttu-id="14eec-273">contentCachingDisableConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="14eec-273">contentCachingDisableConnectionSharing</span></span>|<span data-ttu-id="14eec-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-274">Boolean</span></span>|<span data-ttu-id="14eec-275">Отключение общего доступа к Интернету.</span><span class="sxs-lookup"><span data-stu-id="14eec-275">Disables internet connection sharing.</span></span>|
|<span data-ttu-id="14eec-276">contentCachingForceConnectionSharing</span><span class="sxs-lookup"><span data-stu-id="14eec-276">contentCachingForceConnectionSharing</span></span>|<span data-ttu-id="14eec-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-277">Boolean</span></span>|<span data-ttu-id="14eec-278">Заставляет совместное использование подключения к Интернету.</span><span class="sxs-lookup"><span data-stu-id="14eec-278">Forces internet connection sharing.</span></span> <span data-ttu-id="14eec-279">contentCachingDisableConnectionSharing переопределяет этот параметр.</span><span class="sxs-lookup"><span data-stu-id="14eec-279">contentCachingDisableConnectionSharing overrides this setting.</span></span>|
|<span data-ttu-id="14eec-280">contentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="14eec-280">contentCachingClientPolicy</span></span>|[<span data-ttu-id="14eec-281">macOSContentCachingClientPolicy</span><span class="sxs-lookup"><span data-stu-id="14eec-281">macOSContentCachingClientPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingclientpolicy.md)|<span data-ttu-id="14eec-282">Определяет метод, с помощью которого серверы кэшинга контента будут прослушивать клиентов.</span><span class="sxs-lookup"><span data-stu-id="14eec-282">Determines the method in which content caching servers will listen for clients.</span></span> <span data-ttu-id="14eec-283">Возможные значения: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span><span class="sxs-lookup"><span data-stu-id="14eec-283">Possible values are: `notConfigured`, `clientsInLocalNetwork`, `clientsWithSamePublicIpAddress`, `clientsInCustomLocalNetworks`, `clientsInCustomLocalNetworksWithFallback`.</span></span>|
|<span data-ttu-id="14eec-284">contentCachingClientListenRanges</span><span class="sxs-lookup"><span data-stu-id="14eec-284">contentCachingClientListenRanges</span></span>|<span data-ttu-id="14eec-285">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="14eec-285">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="14eec-286">Список пользовательских кэшей контента диапазонов IP будет использовать для прослушивания для клиентов.</span><span class="sxs-lookup"><span data-stu-id="14eec-286">A list of custom IP ranges content caches will use to listen for clients.</span></span> <span data-ttu-id="14eec-287">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="14eec-287">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="14eec-288">contentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="14eec-288">contentCachingPeerPolicy</span></span>|[<span data-ttu-id="14eec-289">macOSContentCachingPeerPolicy</span><span class="sxs-lookup"><span data-stu-id="14eec-289">macOSContentCachingPeerPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingpeerpolicy.md)|<span data-ttu-id="14eec-290">Определяет метод, в котором кэши контента соединяют с другими кэшами.</span><span class="sxs-lookup"><span data-stu-id="14eec-290">Determines the method in which content caches peer with other caches.</span></span> <span data-ttu-id="14eec-291">Возможные значения: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span><span class="sxs-lookup"><span data-stu-id="14eec-291">Possible values are: `notConfigured`, `peersInLocalNetwork`, `peersWithSamePublicIpAddress`, `peersInCustomLocalNetworks`.</span></span>|
|<span data-ttu-id="14eec-292">contentCachingPeerListenRanges</span><span class="sxs-lookup"><span data-stu-id="14eec-292">contentCachingPeerListenRanges</span></span>|<span data-ttu-id="14eec-293">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="14eec-293">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="14eec-294">Список пользовательских кэшей контента диапазонов IP будет использовать для прослушивания одноранговых кэшей.</span><span class="sxs-lookup"><span data-stu-id="14eec-294">A list of custom IP ranges content caches will use to listen for peer caches.</span></span> <span data-ttu-id="14eec-295">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="14eec-295">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="14eec-296">contentCachingPeerFilterRanges</span><span class="sxs-lookup"><span data-stu-id="14eec-296">contentCachingPeerFilterRanges</span></span>|<span data-ttu-id="14eec-297">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="14eec-297">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="14eec-298">Список пользовательских кэшей контента диапазонов IP будет использовать для запроса контента из кэшей одноранговых.</span><span class="sxs-lookup"><span data-stu-id="14eec-298">A list of custom IP ranges content caches will use to query for content from peers caches.</span></span> <span data-ttu-id="14eec-299">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="14eec-299">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="14eec-300">contentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="14eec-300">contentCachingParentSelectionPolicy</span></span>|[<span data-ttu-id="14eec-301">macOSContentCachingParentSelectionPolicy</span><span class="sxs-lookup"><span data-stu-id="14eec-301">macOSContentCachingParentSelectionPolicy</span></span>](../resources/intune-deviceconfig-macoscontentcachingparentselectionpolicy.md)|<span data-ttu-id="14eec-302">Определяет метод, при котором серверы кэшинга контента будут выбирать родителей, если их несколько.</span><span class="sxs-lookup"><span data-stu-id="14eec-302">Determines the method in which content caching servers will select parents if multiple are present.</span></span> <span data-ttu-id="14eec-303">Возможные значения: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span><span class="sxs-lookup"><span data-stu-id="14eec-303">Possible values are: `notConfigured`, `roundRobin`, `firstAvailable`, `urlPathHash`, `random`, `stickyAvailable`.</span></span>|
|<span data-ttu-id="14eec-304">contentCachingParents</span><span class="sxs-lookup"><span data-stu-id="14eec-304">contentCachingParents</span></span>|<span data-ttu-id="14eec-305">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="14eec-305">String collection</span></span>|<span data-ttu-id="14eec-306">Список IP-адресов, представляющих кэши родительского контента.</span><span class="sxs-lookup"><span data-stu-id="14eec-306">A list of IP addresses representing parent content caches.</span></span>|
|<span data-ttu-id="14eec-307">contentCachingLogClientIdentities</span><span class="sxs-lookup"><span data-stu-id="14eec-307">contentCachingLogClientIdentities</span></span>|<span data-ttu-id="14eec-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-308">Boolean</span></span>|<span data-ttu-id="14eec-309">Включает ведение журнала IP-адресов и портов клиентов, запрашивает кэширование контента.</span><span class="sxs-lookup"><span data-stu-id="14eec-309">Enables logging of IP addresses and ports of clients that request cached content.</span></span>|
|<span data-ttu-id="14eec-310">contentCachingPublicRanges</span><span class="sxs-lookup"><span data-stu-id="14eec-310">contentCachingPublicRanges</span></span>|<span data-ttu-id="14eec-311">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="14eec-311">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="14eec-312">Список пользовательских диапазонов IP-адресов, которые служба кэшинга контента Apple должна использовать для совпадения клиентов с кэшами контента.</span><span class="sxs-lookup"><span data-stu-id="14eec-312">A list of custom IP ranges that Apple's content caching service should use to match clients to content caches.</span></span> <span data-ttu-id="14eec-313">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="14eec-313">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="14eec-314">contentCachingBlockDeletion</span><span class="sxs-lookup"><span data-stu-id="14eec-314">contentCachingBlockDeletion</span></span>|<span data-ttu-id="14eec-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-315">Boolean</span></span>|<span data-ttu-id="14eec-316">Предотвращает очистку содержимого от кэшей контента, чтобы освободить пространство диска для других приложений.</span><span class="sxs-lookup"><span data-stu-id="14eec-316">Prevents content caches from purging content to free up disk space for other apps.</span></span>|
|<span data-ttu-id="14eec-317">contentCachingShowAlerts</span><span class="sxs-lookup"><span data-stu-id="14eec-317">contentCachingShowAlerts</span></span>|<span data-ttu-id="14eec-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-318">Boolean</span></span>|<span data-ttu-id="14eec-319">Отображение оповещений кэшинга контента в качестве системных уведомлений.</span><span class="sxs-lookup"><span data-stu-id="14eec-319">Display content caching alerts as system notifications.</span></span>|
|<span data-ttu-id="14eec-320">contentCachingKeepAwake</span><span class="sxs-lookup"><span data-stu-id="14eec-320">contentCachingKeepAwake</span></span>|<span data-ttu-id="14eec-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="14eec-321">Boolean</span></span>|<span data-ttu-id="14eec-322">Запретить устройству спать, если включен кэшинг контента.</span><span class="sxs-lookup"><span data-stu-id="14eec-322">Prevent the device from sleeping if content caching is enabled.</span></span>|
|<span data-ttu-id="14eec-323">contentCachingPort</span><span class="sxs-lookup"><span data-stu-id="14eec-323">contentCachingPort</span></span>|<span data-ttu-id="14eec-324">Int32</span><span class="sxs-lookup"><span data-stu-id="14eec-324">Int32</span></span>|<span data-ttu-id="14eec-325">Задает порт, используемый для кэшинга контента.</span><span class="sxs-lookup"><span data-stu-id="14eec-325">Sets the port used for content caching.</span></span> <span data-ttu-id="14eec-326">Если значение 0, будет выбран случайный доступный порт.</span><span class="sxs-lookup"><span data-stu-id="14eec-326">If the value is 0, a random available port will be selected.</span></span> <span data-ttu-id="14eec-327">Допустимые значения от 0 до 65535</span><span class="sxs-lookup"><span data-stu-id="14eec-327">Valid values 0 to 65535</span></span>|



## <a name="response"></a><span data-ttu-id="14eec-328">Отклик</span><span class="sxs-lookup"><span data-stu-id="14eec-328">Response</span></span>
<span data-ttu-id="14eec-329">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="14eec-329">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14eec-330">Пример</span><span class="sxs-lookup"><span data-stu-id="14eec-330">Example</span></span>

### <a name="request"></a><span data-ttu-id="14eec-331">Запрос</span><span class="sxs-lookup"><span data-stu-id="14eec-331">Request</span></span>
<span data-ttu-id="14eec-332">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14eec-332">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 5662

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
  "appAssociatedDomains": [
    {
      "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
      "applicationIdentifier": "Application Identifier value",
      "domains": [
        "Domains value"
      ],
      "directDownloadsEnabled": true
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

### <a name="response"></a><span data-ttu-id="14eec-333">Отклик</span><span class="sxs-lookup"><span data-stu-id="14eec-333">Response</span></span>
<span data-ttu-id="14eec-p130">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="14eec-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 5834

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
  "appAssociatedDomains": [
    {
      "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
      "applicationIdentifier": "Application Identifier value",
      "domains": [
        "Domains value"
      ],
      "directDownloadsEnabled": true
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




