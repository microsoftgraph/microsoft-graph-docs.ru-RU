---
title: Создание объекта windows10TeamGeneralConfiguration
description: Создает объект windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df58cd9c0ee316743b876882cbda57495c8d1cda
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980539"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="a215e-103">Создание объекта windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="a215e-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="a215e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a215e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a215e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a215e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a215e-106">Создает объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a215e-106">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a215e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a215e-107">Prerequisites</span></span>
<span data-ttu-id="a215e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a215e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a215e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a215e-110">Permission type</span></span>|<span data-ttu-id="a215e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a215e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a215e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a215e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a215e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a215e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a215e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a215e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a215e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a215e-115">Not supported.</span></span>|
|<span data-ttu-id="a215e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a215e-116">Application</span></span>|<span data-ttu-id="a215e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a215e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a215e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a215e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a215e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a215e-119">Request headers</span></span>
|<span data-ttu-id="a215e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a215e-120">Header</span></span>|<span data-ttu-id="a215e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a215e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a215e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a215e-122">Authorization</span></span>|<span data-ttu-id="a215e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a215e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a215e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a215e-124">Accept</span></span>|<span data-ttu-id="a215e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a215e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a215e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a215e-126">Request body</span></span>
<span data-ttu-id="a215e-127">В теле запроса добавьте представление объекта windows10TeamGeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a215e-127">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="a215e-128">Ниже показаны свойства, которые необходимо указывать при создании объекта windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a215e-128">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="a215e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a215e-129">Property</span></span>|<span data-ttu-id="a215e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a215e-130">Type</span></span>|<span data-ttu-id="a215e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a215e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a215e-132">id</span><span class="sxs-lookup"><span data-stu-id="a215e-132">id</span></span>|<span data-ttu-id="a215e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a215e-133">String</span></span>|<span data-ttu-id="a215e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a215e-134">Key of the entity.</span></span> <span data-ttu-id="a215e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a215e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a215e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a215e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a215e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a215e-137">DateTimeOffset</span></span>|<span data-ttu-id="a215e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a215e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a215e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a215e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a215e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a215e-140">roleScopeTagIds</span></span>|<span data-ttu-id="a215e-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a215e-141">String collection</span></span>|<span data-ttu-id="a215e-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="a215e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a215e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a215e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a215e-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="a215e-144">supportsScopeTags</span></span>|<span data-ttu-id="a215e-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a215e-145">Boolean</span></span>|<span data-ttu-id="a215e-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="a215e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a215e-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="a215e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a215e-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="a215e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a215e-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a215e-149">This property is read-only.</span></span> <span data-ttu-id="a215e-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a215e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a215e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a215e-151">createdDateTime</span></span>|<span data-ttu-id="a215e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a215e-152">DateTimeOffset</span></span>|<span data-ttu-id="a215e-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a215e-153">DateTime the object was created.</span></span> <span data-ttu-id="a215e-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a215e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a215e-155">description</span><span class="sxs-lookup"><span data-stu-id="a215e-155">description</span></span>|<span data-ttu-id="a215e-156">String</span><span class="sxs-lookup"><span data-stu-id="a215e-156">String</span></span>|<span data-ttu-id="a215e-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a215e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a215e-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a215e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a215e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a215e-159">displayName</span></span>|<span data-ttu-id="a215e-160">Строка</span><span class="sxs-lookup"><span data-stu-id="a215e-160">String</span></span>|<span data-ttu-id="a215e-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a215e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a215e-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a215e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a215e-163">version</span><span class="sxs-lookup"><span data-stu-id="a215e-163">version</span></span>|<span data-ttu-id="a215e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a215e-164">Int32</span></span>|<span data-ttu-id="a215e-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a215e-165">Version of the device configuration.</span></span> <span data-ttu-id="a215e-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a215e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a215e-167">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="a215e-167">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="a215e-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="a215e-168">Boolean</span></span>|<span data-ttu-id="a215e-169">Указывает, следует ли заблокировать оперативную аналитику Azure.</span><span class="sxs-lookup"><span data-stu-id="a215e-169">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="a215e-170">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="a215e-170">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="a215e-171">String</span><span class="sxs-lookup"><span data-stu-id="a215e-171">String</span></span>|<span data-ttu-id="a215e-172">Идентификатор рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="a215e-172">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="a215e-173">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="a215e-173">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="a215e-174">String</span><span class="sxs-lookup"><span data-stu-id="a215e-174">String</span></span>|<span data-ttu-id="a215e-175">Ключ рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="a215e-175">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="a215e-176">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="a215e-176">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="a215e-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="a215e-177">Boolean</span></span>|<span data-ttu-id="a215e-178">Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.</span><span class="sxs-lookup"><span data-stu-id="a215e-178">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="a215e-179">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="a215e-179">maintenanceWindowBlocked</span></span>|<span data-ttu-id="a215e-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="a215e-180">Boolean</span></span>|<span data-ttu-id="a215e-181">Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="a215e-181">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="a215e-182">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="a215e-182">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="a215e-183">Int32</span><span class="sxs-lookup"><span data-stu-id="a215e-183">Int32</span></span>|<span data-ttu-id="a215e-184">Длительность периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="a215e-184">Maintenance window duration for device updates.</span></span> <span data-ttu-id="a215e-185">Допустимые значения: от 0 до 5</span><span class="sxs-lookup"><span data-stu-id="a215e-185">Valid values 0 to 5</span></span>|
|<span data-ttu-id="a215e-186">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="a215e-186">maintenanceWindowStartTime</span></span>|<span data-ttu-id="a215e-187">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a215e-187">TimeOfDay</span></span>|<span data-ttu-id="a215e-188">Начало периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="a215e-188">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="a215e-189">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="a215e-189">miracastChannel</span></span>|[<span data-ttu-id="a215e-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="a215e-190">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="a215e-191">Канал.</span><span class="sxs-lookup"><span data-stu-id="a215e-191">The channel.</span></span> <span data-ttu-id="a215e-192">Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="a215e-192">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="a215e-193">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="a215e-193">miracastBlocked</span></span>|<span data-ttu-id="a215e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a215e-194">Boolean</span></span>|<span data-ttu-id="a215e-195">Указывает, следует ли заблокировать беспроводное проецирование.</span><span class="sxs-lookup"><span data-stu-id="a215e-195">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="a215e-196">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="a215e-196">miracastRequirePin</span></span>|<span data-ttu-id="a215e-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="a215e-197">Boolean</span></span>|<span data-ttu-id="a215e-198">Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.</span><span class="sxs-lookup"><span data-stu-id="a215e-198">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="a215e-199">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="a215e-199">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="a215e-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a215e-200">Boolean</span></span>|<span data-ttu-id="a215e-201">Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.</span><span class="sxs-lookup"><span data-stu-id="a215e-201">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="a215e-202">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="a215e-202">settingsBlockSessionResume</span></span>|<span data-ttu-id="a215e-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="a215e-203">Boolean</span></span>|<span data-ttu-id="a215e-204">Указывает, следует ли разрешить возобновление сеанса после истечения времени.</span><span class="sxs-lookup"><span data-stu-id="a215e-204">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="a215e-205">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="a215e-205">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="a215e-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="a215e-206">Boolean</span></span>|<span data-ttu-id="a215e-207">Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.</span><span class="sxs-lookup"><span data-stu-id="a215e-207">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="a215e-208">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="a215e-208">settingsDefaultVolume</span></span>|<span data-ttu-id="a215e-209">Int32</span><span class="sxs-lookup"><span data-stu-id="a215e-209">Int32</span></span>|<span data-ttu-id="a215e-210">Задает объем нового сеанса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a215e-210">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="a215e-211">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="a215e-211">Permitted values are 0-100.</span></span> <span data-ttu-id="a215e-212">Значение по умолчанию — 45.</span><span class="sxs-lookup"><span data-stu-id="a215e-212">The default is 45.</span></span> <span data-ttu-id="a215e-213">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="a215e-213">Valid values 0 to 100</span></span>|
|<span data-ttu-id="a215e-214">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="a215e-214">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="a215e-215">Int32</span><span class="sxs-lookup"><span data-stu-id="a215e-215">Int32</span></span>|<span data-ttu-id="a215e-216">Определяет время до отключения экрана Центра (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a215e-216">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="a215e-217">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="a215e-217">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="a215e-218">Int32</span><span class="sxs-lookup"><span data-stu-id="a215e-218">Int32</span></span>|<span data-ttu-id="a215e-219">Определяет время до истечения времени сеанса (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a215e-219">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="a215e-220">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="a215e-220">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="a215e-221">Int32</span><span class="sxs-lookup"><span data-stu-id="a215e-221">Int32</span></span>|<span data-ttu-id="a215e-222">Определяет время до перехода Центра в спящий режим (в минутах).</span><span class="sxs-lookup"><span data-stu-id="a215e-222">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="a215e-223">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="a215e-223">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="a215e-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="a215e-224">Boolean</span></span>|<span data-ttu-id="a215e-225">Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.</span><span class="sxs-lookup"><span data-stu-id="a215e-225">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="a215e-226">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="a215e-226">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="a215e-227">String</span><span class="sxs-lookup"><span data-stu-id="a215e-227">String</span></span>|<span data-ttu-id="a215e-228">URL-адрес фонового изображения экрана приветствия.</span><span class="sxs-lookup"><span data-stu-id="a215e-228">The welcome screen background image URL.</span></span> <span data-ttu-id="a215e-229">URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.</span><span class="sxs-lookup"><span data-stu-id="a215e-229">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="a215e-230">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="a215e-230">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="a215e-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="a215e-231">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="a215e-232">Информация о собраниях, показываемая на экране приветствия.</span><span class="sxs-lookup"><span data-stu-id="a215e-232">The welcome screen meeting information shown.</span></span> <span data-ttu-id="a215e-233">Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="a215e-233">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="a215e-234">Отклик</span><span class="sxs-lookup"><span data-stu-id="a215e-234">Response</span></span>
<span data-ttu-id="a215e-235">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a215e-235">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a215e-236">Пример</span><span class="sxs-lookup"><span data-stu-id="a215e-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="a215e-237">Запрос</span><span class="sxs-lookup"><span data-stu-id="a215e-237">Request</span></span>
<span data-ttu-id="a215e-238">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a215e-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1242

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```

### <a name="response"></a><span data-ttu-id="a215e-239">Отклик</span><span class="sxs-lookup"><span data-stu-id="a215e-239">Response</span></span>
<span data-ttu-id="a215e-p115">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a215e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1414

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "azureOperationalInsightsBlockTelemetry": true,
  "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
  "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
  "connectAppBlockAutoLaunch": true,
  "maintenanceWindowBlocked": true,
  "maintenanceWindowDurationInHours": 0,
  "maintenanceWindowStartTime": "11:59:09.3130000",
  "miracastChannel": "one",
  "miracastBlocked": true,
  "miracastRequirePin": true,
  "settingsBlockMyMeetingsAndFiles": true,
  "settingsBlockSessionResume": true,
  "settingsBlockSigninSuggestions": true,
  "settingsDefaultVolume": 5,
  "settingsScreenTimeoutInMinutes": 14,
  "settingsSessionTimeoutInMinutes": 15,
  "settingsSleepTimeoutInMinutes": 13,
  "welcomeScreenBlockAutomaticWakeUp": true,
  "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
  "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
}
```




