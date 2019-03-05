---
title: Обновление windows10TeamGeneralConfiguration
description: Обновление свойств объекта windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab049fecd546462123796aff2fd3ac975e71932f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251022"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="89cbb-103">Обновление windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="89cbb-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="89cbb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89cbb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89cbb-105">Обновление свойств объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89cbb-105">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89cbb-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="89cbb-106">Prerequisites</span></span>
<span data-ttu-id="89cbb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="89cbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="89cbb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89cbb-109">Permission type</span></span>|<span data-ttu-id="89cbb-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="89cbb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89cbb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89cbb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="89cbb-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89cbb-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89cbb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89cbb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89cbb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89cbb-114">Not supported.</span></span>|
|<span data-ttu-id="89cbb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="89cbb-115">Application</span></span>|<span data-ttu-id="89cbb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89cbb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89cbb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89cbb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="89cbb-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89cbb-118">Request headers</span></span>
|<span data-ttu-id="89cbb-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89cbb-119">Header</span></span>|<span data-ttu-id="89cbb-120">Значение</span><span class="sxs-lookup"><span data-stu-id="89cbb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89cbb-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89cbb-121">Authorization</span></span>|<span data-ttu-id="89cbb-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="89cbb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89cbb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="89cbb-123">Accept</span></span>|<span data-ttu-id="89cbb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="89cbb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89cbb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="89cbb-125">Request body</span></span>
<span data-ttu-id="89cbb-126">В теле запроса добавьте представление объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89cbb-126">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="89cbb-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89cbb-127">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="89cbb-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="89cbb-128">Property</span></span>|<span data-ttu-id="89cbb-129">Тип</span><span class="sxs-lookup"><span data-stu-id="89cbb-129">Type</span></span>|<span data-ttu-id="89cbb-130">Описание</span><span class="sxs-lookup"><span data-stu-id="89cbb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89cbb-131">id</span><span class="sxs-lookup"><span data-stu-id="89cbb-131">id</span></span>|<span data-ttu-id="89cbb-132">String</span><span class="sxs-lookup"><span data-stu-id="89cbb-132">String</span></span>|<span data-ttu-id="89cbb-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="89cbb-133">Key of the entity.</span></span> <span data-ttu-id="89cbb-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89cbb-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89cbb-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89cbb-135">lastModifiedDateTime</span></span>|<span data-ttu-id="89cbb-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89cbb-136">DateTimeOffset</span></span>|<span data-ttu-id="89cbb-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="89cbb-137">DateTime the object was last modified.</span></span> <span data-ttu-id="89cbb-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89cbb-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89cbb-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89cbb-139">createdDateTime</span></span>|<span data-ttu-id="89cbb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89cbb-140">DateTimeOffset</span></span>|<span data-ttu-id="89cbb-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="89cbb-141">DateTime the object was created.</span></span> <span data-ttu-id="89cbb-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89cbb-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89cbb-143">description</span><span class="sxs-lookup"><span data-stu-id="89cbb-143">description</span></span>|<span data-ttu-id="89cbb-144">Строка</span><span class="sxs-lookup"><span data-stu-id="89cbb-144">String</span></span>|<span data-ttu-id="89cbb-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89cbb-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="89cbb-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89cbb-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89cbb-147">displayName</span><span class="sxs-lookup"><span data-stu-id="89cbb-147">displayName</span></span>|<span data-ttu-id="89cbb-148">Строка</span><span class="sxs-lookup"><span data-stu-id="89cbb-148">String</span></span>|<span data-ttu-id="89cbb-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89cbb-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="89cbb-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="89cbb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89cbb-151">version</span><span class="sxs-lookup"><span data-stu-id="89cbb-151">version</span></span>|<span data-ttu-id="89cbb-152">Int32</span><span class="sxs-lookup"><span data-stu-id="89cbb-152">Int32</span></span>|<span data-ttu-id="89cbb-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89cbb-153">Version of the device configuration.</span></span> <span data-ttu-id="89cbb-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="89cbb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="89cbb-155">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="89cbb-155">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="89cbb-156">Логический</span><span class="sxs-lookup"><span data-stu-id="89cbb-156">Boolean</span></span>|<span data-ttu-id="89cbb-157">Указывает, следует ли заблокировать оперативную аналитику Azure.</span><span class="sxs-lookup"><span data-stu-id="89cbb-157">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="89cbb-158">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="89cbb-158">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="89cbb-159">String</span><span class="sxs-lookup"><span data-stu-id="89cbb-159">String</span></span>|<span data-ttu-id="89cbb-160">Идентификатор рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="89cbb-160">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="89cbb-161">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="89cbb-161">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="89cbb-162">String</span><span class="sxs-lookup"><span data-stu-id="89cbb-162">String</span></span>|<span data-ttu-id="89cbb-163">Ключ рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="89cbb-163">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="89cbb-164">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="89cbb-164">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="89cbb-165">Логический</span><span class="sxs-lookup"><span data-stu-id="89cbb-165">Boolean</span></span>|<span data-ttu-id="89cbb-166">Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.</span><span class="sxs-lookup"><span data-stu-id="89cbb-166">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="89cbb-167">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="89cbb-167">maintenanceWindowBlocked</span></span>|<span data-ttu-id="89cbb-168">Логический</span><span class="sxs-lookup"><span data-stu-id="89cbb-168">Boolean</span></span>|<span data-ttu-id="89cbb-169">Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="89cbb-169">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="89cbb-170">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="89cbb-170">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="89cbb-171">Int32</span><span class="sxs-lookup"><span data-stu-id="89cbb-171">Int32</span></span>|<span data-ttu-id="89cbb-172">Длительность периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="89cbb-172">Maintenance window duration for device updates.</span></span> <span data-ttu-id="89cbb-173">Допустимые значения: от 0 до 5</span><span class="sxs-lookup"><span data-stu-id="89cbb-173">Valid values 0 to 5</span></span>|
|<span data-ttu-id="89cbb-174">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="89cbb-174">maintenanceWindowStartTime</span></span>|<span data-ttu-id="89cbb-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="89cbb-175">TimeOfDay</span></span>|<span data-ttu-id="89cbb-176">Начало периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="89cbb-176">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="89cbb-177">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="89cbb-177">miracastChannel</span></span>|[<span data-ttu-id="89cbb-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="89cbb-178">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="89cbb-179">Канал.</span><span class="sxs-lookup"><span data-stu-id="89cbb-179">The channel.</span></span> <span data-ttu-id="89cbb-180">Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="89cbb-180">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="89cbb-181">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="89cbb-181">miracastBlocked</span></span>|<span data-ttu-id="89cbb-182">Логический</span><span class="sxs-lookup"><span data-stu-id="89cbb-182">Boolean</span></span>|<span data-ttu-id="89cbb-183">Указывает, следует ли заблокировать беспроводное проецирование.</span><span class="sxs-lookup"><span data-stu-id="89cbb-183">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="89cbb-184">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="89cbb-184">miracastRequirePin</span></span>|<span data-ttu-id="89cbb-185">Логический</span><span class="sxs-lookup"><span data-stu-id="89cbb-185">Boolean</span></span>|<span data-ttu-id="89cbb-186">Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.</span><span class="sxs-lookup"><span data-stu-id="89cbb-186">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="89cbb-187">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="89cbb-187">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="89cbb-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="89cbb-188">Boolean</span></span>|<span data-ttu-id="89cbb-189">Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.</span><span class="sxs-lookup"><span data-stu-id="89cbb-189">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="89cbb-190">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="89cbb-190">settingsBlockSessionResume</span></span>|<span data-ttu-id="89cbb-191">Логический</span><span class="sxs-lookup"><span data-stu-id="89cbb-191">Boolean</span></span>|<span data-ttu-id="89cbb-192">Указывает, следует ли разрешить возобновление сеанса после истечения времени.</span><span class="sxs-lookup"><span data-stu-id="89cbb-192">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="89cbb-193">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="89cbb-193">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="89cbb-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="89cbb-194">Boolean</span></span>|<span data-ttu-id="89cbb-195">Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.</span><span class="sxs-lookup"><span data-stu-id="89cbb-195">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="89cbb-196">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="89cbb-196">settingsDefaultVolume</span></span>|<span data-ttu-id="89cbb-197">Int32</span><span class="sxs-lookup"><span data-stu-id="89cbb-197">Int32</span></span>|<span data-ttu-id="89cbb-198">Задает объем нового сеанса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="89cbb-198">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="89cbb-199">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="89cbb-199">Permitted values are 0-100.</span></span> <span data-ttu-id="89cbb-200">Значение по умолчанию — 45.</span><span class="sxs-lookup"><span data-stu-id="89cbb-200">The default is 45.</span></span> <span data-ttu-id="89cbb-201">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="89cbb-201">Valid values 0 to 100</span></span>|
|<span data-ttu-id="89cbb-202">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="89cbb-202">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="89cbb-203">Int32</span><span class="sxs-lookup"><span data-stu-id="89cbb-203">Int32</span></span>|<span data-ttu-id="89cbb-204">Определяет время до отключения экрана Центра (в минутах).</span><span class="sxs-lookup"><span data-stu-id="89cbb-204">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="89cbb-205">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="89cbb-205">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="89cbb-206">Int32</span><span class="sxs-lookup"><span data-stu-id="89cbb-206">Int32</span></span>|<span data-ttu-id="89cbb-207">Определяет время до истечения времени сеанса (в минутах).</span><span class="sxs-lookup"><span data-stu-id="89cbb-207">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="89cbb-208">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="89cbb-208">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="89cbb-209">Int32</span><span class="sxs-lookup"><span data-stu-id="89cbb-209">Int32</span></span>|<span data-ttu-id="89cbb-210">Определяет время до перехода Центра в спящий режим (в минутах).</span><span class="sxs-lookup"><span data-stu-id="89cbb-210">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="89cbb-211">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="89cbb-211">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="89cbb-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="89cbb-212">Boolean</span></span>|<span data-ttu-id="89cbb-213">Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.</span><span class="sxs-lookup"><span data-stu-id="89cbb-213">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="89cbb-214">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="89cbb-214">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="89cbb-215">String</span><span class="sxs-lookup"><span data-stu-id="89cbb-215">String</span></span>|<span data-ttu-id="89cbb-216">URL-адрес фонового изображения экрана приветствия.</span><span class="sxs-lookup"><span data-stu-id="89cbb-216">The welcome screen background image URL.</span></span> <span data-ttu-id="89cbb-217">URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.</span><span class="sxs-lookup"><span data-stu-id="89cbb-217">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="89cbb-218">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="89cbb-218">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="89cbb-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="89cbb-219">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="89cbb-220">Информация о собраниях, показываемая на экране приветствия.</span><span class="sxs-lookup"><span data-stu-id="89cbb-220">The welcome screen meeting information shown.</span></span> <span data-ttu-id="89cbb-221">Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="89cbb-221">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="89cbb-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="89cbb-222">Response</span></span>
<span data-ttu-id="89cbb-223">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="89cbb-223">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89cbb-224">Пример</span><span class="sxs-lookup"><span data-stu-id="89cbb-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="89cbb-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="89cbb-225">Request</span></span>
<span data-ttu-id="89cbb-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89cbb-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1150

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="89cbb-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="89cbb-227">Response</span></span>
<span data-ttu-id="89cbb-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89cbb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1322

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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



