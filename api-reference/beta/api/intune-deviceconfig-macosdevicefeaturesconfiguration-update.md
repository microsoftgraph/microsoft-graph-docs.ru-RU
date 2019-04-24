---
title: Обновление объекта macOSDeviceFeaturesConfiguration
description: Обновление свойств объекта macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d3d583d894a11edc6d95a95f2b1869b08467689
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518739"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="577b6-103">Обновление объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="577b6-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="577b6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="577b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="577b6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="577b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="577b6-106">Обновление свойств объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="577b6-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="577b6-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="577b6-107">Prerequisites</span></span>
<span data-ttu-id="577b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="577b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="577b6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="577b6-110">Permission type</span></span>|<span data-ttu-id="577b6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="577b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="577b6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="577b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="577b6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="577b6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="577b6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="577b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="577b6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="577b6-115">Not supported.</span></span>|
|<span data-ttu-id="577b6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="577b6-116">Application</span></span>|<span data-ttu-id="577b6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="577b6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="577b6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="577b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="577b6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="577b6-119">Request headers</span></span>
|<span data-ttu-id="577b6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="577b6-120">Header</span></span>|<span data-ttu-id="577b6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="577b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="577b6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="577b6-122">Authorization</span></span>|<span data-ttu-id="577b6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="577b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="577b6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="577b6-124">Accept</span></span>|<span data-ttu-id="577b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="577b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="577b6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="577b6-126">Request body</span></span>
<span data-ttu-id="577b6-127">В теле запроса добавьте представление объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="577b6-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="577b6-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="577b6-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="577b6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="577b6-129">Property</span></span>|<span data-ttu-id="577b6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="577b6-130">Type</span></span>|<span data-ttu-id="577b6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="577b6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="577b6-132">id</span><span class="sxs-lookup"><span data-stu-id="577b6-132">id</span></span>|<span data-ttu-id="577b6-133">Строка</span><span class="sxs-lookup"><span data-stu-id="577b6-133">String</span></span>|<span data-ttu-id="577b6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="577b6-134">Key of the entity.</span></span> <span data-ttu-id="577b6-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="577b6-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="577b6-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="577b6-136">lastModifiedDateTime</span></span>|<span data-ttu-id="577b6-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="577b6-137">DateTimeOffset</span></span>|<span data-ttu-id="577b6-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="577b6-138">DateTime the object was last modified.</span></span> <span data-ttu-id="577b6-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="577b6-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="577b6-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="577b6-140">roleScopeTagIds</span></span>|<span data-ttu-id="577b6-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="577b6-141">String collection</span></span>|<span data-ttu-id="577b6-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="577b6-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="577b6-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="577b6-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="577b6-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="577b6-144">supportsScopeTags</span></span>|<span data-ttu-id="577b6-145">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-145">Boolean</span></span>|<span data-ttu-id="577b6-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="577b6-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="577b6-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="577b6-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="577b6-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="577b6-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="577b6-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="577b6-149">This property is read-only.</span></span> <span data-ttu-id="577b6-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="577b6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="577b6-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="577b6-151">createdDateTime</span></span>|<span data-ttu-id="577b6-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="577b6-152">DateTimeOffset</span></span>|<span data-ttu-id="577b6-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="577b6-153">DateTime the object was created.</span></span> <span data-ttu-id="577b6-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="577b6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="577b6-155">description</span><span class="sxs-lookup"><span data-stu-id="577b6-155">description</span></span>|<span data-ttu-id="577b6-156">String</span><span class="sxs-lookup"><span data-stu-id="577b6-156">String</span></span>|<span data-ttu-id="577b6-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="577b6-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="577b6-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="577b6-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="577b6-159">displayName</span><span class="sxs-lookup"><span data-stu-id="577b6-159">displayName</span></span>|<span data-ttu-id="577b6-160">String</span><span class="sxs-lookup"><span data-stu-id="577b6-160">String</span></span>|<span data-ttu-id="577b6-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="577b6-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="577b6-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="577b6-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="577b6-163">version</span><span class="sxs-lookup"><span data-stu-id="577b6-163">version</span></span>|<span data-ttu-id="577b6-164">Int32</span><span class="sxs-lookup"><span data-stu-id="577b6-164">Int32</span></span>|<span data-ttu-id="577b6-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="577b6-165">Version of the device configuration.</span></span> <span data-ttu-id="577b6-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="577b6-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="577b6-167">Аирпринтдестинатионс</span><span class="sxs-lookup"><span data-stu-id="577b6-167">airPrintDestinations</span></span>|<span data-ttu-id="577b6-168">Коллекция [аирпринтдестинатион](../resources/intune-deviceconfig-airprintdestination.md)</span><span class="sxs-lookup"><span data-stu-id="577b6-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="577b6-169">Массив принтеров Аирпринт, которые должны отображаться всегда.</span><span class="sxs-lookup"><span data-stu-id="577b6-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="577b6-170">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="577b6-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="577b6-171">НаСледуется от [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="577b6-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="577b6-172">Аутолаунчитемс</span><span class="sxs-lookup"><span data-stu-id="577b6-172">autoLaunchItems</span></span>|<span data-ttu-id="577b6-173">Коллекция [макослаунчитем](../resources/intune-deviceconfig-macoslaunchitem.md)</span><span class="sxs-lookup"><span data-stu-id="577b6-173">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="577b6-174">Список приложений, файлов, папок и других элементов, которые запускаются при входе пользователя.</span><span class="sxs-lookup"><span data-stu-id="577b6-174">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="577b6-175">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="577b6-175">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="577b6-176">Админшовхостинфо</span><span class="sxs-lookup"><span data-stu-id="577b6-176">adminShowHostInfo</span></span>|<span data-ttu-id="577b6-177">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-177">Boolean</span></span>|<span data-ttu-id="577b6-178">Показывать ли сведения об узле администратора в окне входа.</span><span class="sxs-lookup"><span data-stu-id="577b6-178">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="577b6-179">Логинвиндовтекст</span><span class="sxs-lookup"><span data-stu-id="577b6-179">loginWindowText</span></span>|<span data-ttu-id="577b6-180">String</span><span class="sxs-lookup"><span data-stu-id="577b6-180">String</span></span>|<span data-ttu-id="577b6-181">Настраиваемый текст, отображаемый в окне входа.</span><span class="sxs-lookup"><span data-stu-id="577b6-181">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="577b6-182">Аусоризедусерслиссидден</span><span class="sxs-lookup"><span data-stu-id="577b6-182">authorizedUsersListHidden</span></span>|<span data-ttu-id="577b6-183">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-183">Boolean</span></span>|<span data-ttu-id="577b6-184">Указывает, следует ли отображать диалоговое окно имя и пароль или список пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="577b6-184">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="577b6-185">Аусоризедусерслиссиделокалусерс</span><span class="sxs-lookup"><span data-stu-id="577b6-185">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="577b6-186">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-186">Boolean</span></span>|<span data-ttu-id="577b6-187">Отображение только сетевых и системных пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="577b6-187">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="577b6-188">Аусоризедусерслиссидемобилеаккаунтс</span><span class="sxs-lookup"><span data-stu-id="577b6-188">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="577b6-189">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-189">Boolean</span></span>|<span data-ttu-id="577b6-190">Следует ли скрыть пользователей для мобильных устройств в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="577b6-190">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="577b6-191">Аусоризедусерслистинклуденетворкусерс</span><span class="sxs-lookup"><span data-stu-id="577b6-191">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="577b6-192">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-192">Boolean</span></span>|<span data-ttu-id="577b6-193">Показывать ли пользователей сети в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="577b6-193">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="577b6-194">Аусоризедусерслиссидеадминусерс</span><span class="sxs-lookup"><span data-stu-id="577b6-194">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="577b6-195">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-195">Boolean</span></span>|<span data-ttu-id="577b6-196">Указывает, следует ли скрыть пользователей Admin в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="577b6-196">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="577b6-197">Аусоризедусерслистшовосерманажедусерс</span><span class="sxs-lookup"><span data-stu-id="577b6-197">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="577b6-198">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-198">Boolean</span></span>|<span data-ttu-id="577b6-199">Указывает, следует ли показывать других пользователей в списке авторизованных пользователей в окне входа.</span><span class="sxs-lookup"><span data-stu-id="577b6-199">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="577b6-200">Шутдовндисаблед</span><span class="sxs-lookup"><span data-stu-id="577b6-200">shutDownDisabled</span></span>|<span data-ttu-id="577b6-201">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-201">Boolean</span></span>|<span data-ttu-id="577b6-202">Указывает, следует ли скрыть элемент кнопка "завершение работы" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="577b6-202">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="577b6-203">Рестартдисаблед</span><span class="sxs-lookup"><span data-stu-id="577b6-203">restartDisabled</span></span>|<span data-ttu-id="577b6-204">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-204">Boolean</span></span>|<span data-ttu-id="577b6-205">Указывает, следует ли скрыть элемент "кнопка переЗапуска" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="577b6-205">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="577b6-206">Слипдисаблед</span><span class="sxs-lookup"><span data-stu-id="577b6-206">sleepDisabled</span></span>|<span data-ttu-id="577b6-207">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-207">Boolean</span></span>|<span data-ttu-id="577b6-208">Указывает, следует ли скрыть пункт меню "сон" в окне входа.</span><span class="sxs-lookup"><span data-stu-id="577b6-208">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="577b6-209">Консолеакцессдисаблед</span><span class="sxs-lookup"><span data-stu-id="577b6-209">consoleAccessDisabled</span></span>|<span data-ttu-id="577b6-210">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-210">Boolean</span></span>|<span data-ttu-id="577b6-211">Будет ли другой пользователь игнорировать использование специального имени пользователя "_Гт_консоле_гт_".</span><span class="sxs-lookup"><span data-stu-id="577b6-211">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="577b6-212">Шутдовндисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="577b6-212">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="577b6-213">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-213">Boolean</span></span>|<span data-ttu-id="577b6-214">Будет ли отключен элемент меню "завершение работы" в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="577b6-214">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="577b6-215">Рестартдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="577b6-215">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="577b6-216">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-216">Boolean</span></span>|<span data-ttu-id="577b6-217">Будет ли отключен элемент меню переЗапуска в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="577b6-217">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="577b6-218">Повероффдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="577b6-218">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="577b6-219">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-219">Boolean</span></span>|<span data-ttu-id="577b6-220">Будет ли отключен элемент меню Power of Power в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="577b6-220">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="577b6-221">Логаутдисабледвхилелогжедин</span><span class="sxs-lookup"><span data-stu-id="577b6-221">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="577b6-222">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-222">Boolean</span></span>|<span data-ttu-id="577b6-223">Будет ли отключен элемент меню журнала в окне входа, когда пользователь вошел в систему.</span><span class="sxs-lookup"><span data-stu-id="577b6-223">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="577b6-224">Скринлоккдисаблеиммедиате</span><span class="sxs-lookup"><span data-stu-id="577b6-224">screenLockDisableImmediate</span></span>|<span data-ttu-id="577b6-225">Логический</span><span class="sxs-lookup"><span data-stu-id="577b6-225">Boolean</span></span>|<span data-ttu-id="577b6-226">Следует ли отключить функции немедленной блокировки экрана.</span><span class="sxs-lookup"><span data-stu-id="577b6-226">Whether to disable the immediate screen lock functions.</span></span>|



## <a name="response"></a><span data-ttu-id="577b6-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="577b6-227">Response</span></span>
<span data-ttu-id="577b6-228">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="577b6-228">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="577b6-229">Пример</span><span class="sxs-lookup"><span data-stu-id="577b6-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="577b6-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="577b6-230">Request</span></span>
<span data-ttu-id="577b6-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="577b6-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1334

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="577b6-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="577b6-232">Response</span></span>
<span data-ttu-id="577b6-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="577b6-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1506

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





