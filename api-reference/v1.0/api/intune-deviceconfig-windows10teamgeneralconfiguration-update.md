---
title: Обновление windows10TeamGeneralConfiguration
description: Обновление свойств объекта windows10TeamGeneralConfiguration.
author: tfitzmac
ms.openlocfilehash: 283e7211c98899b1c8eb02007c9b0d9b889f8ce5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334491"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="ed613-103">Обновление windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="ed613-103">Update windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="ed613-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ed613-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed613-105">Обновление свойств объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed613-105">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed613-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ed613-106">Prerequisites</span></span>
<span data-ttu-id="ed613-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed613-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed613-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed613-109">Permission type</span></span>|<span data-ttu-id="ed613-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ed613-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed613-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed613-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed613-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed613-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ed613-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed613-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed613-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed613-114">Not supported.</span></span>|
|<span data-ttu-id="ed613-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed613-115">Application</span></span>|<span data-ttu-id="ed613-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed613-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed613-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed613-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ed613-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed613-118">Request headers</span></span>
|<span data-ttu-id="ed613-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ed613-119">Header</span></span>|<span data-ttu-id="ed613-120">Значение</span><span class="sxs-lookup"><span data-stu-id="ed613-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed613-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ed613-121">Authorization</span></span>|<span data-ttu-id="ed613-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ed613-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed613-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ed613-123">Accept</span></span>|<span data-ttu-id="ed613-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ed613-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed613-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed613-125">Request body</span></span>
<span data-ttu-id="ed613-126">В теле запроса добавьте представление объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed613-126">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="ed613-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed613-127">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="ed613-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed613-128">Property</span></span>|<span data-ttu-id="ed613-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ed613-129">Type</span></span>|<span data-ttu-id="ed613-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ed613-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed613-131">id</span><span class="sxs-lookup"><span data-stu-id="ed613-131">id</span></span>|<span data-ttu-id="ed613-132">Строка</span><span class="sxs-lookup"><span data-stu-id="ed613-132">String</span></span>|<span data-ttu-id="ed613-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ed613-133">Key of the entity.</span></span> <span data-ttu-id="ed613-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed613-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed613-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ed613-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ed613-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed613-136">DateTimeOffset</span></span>|<span data-ttu-id="ed613-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ed613-137">DateTime the object was last modified.</span></span> <span data-ttu-id="ed613-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed613-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed613-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ed613-139">createdDateTime</span></span>|<span data-ttu-id="ed613-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed613-140">DateTimeOffset</span></span>|<span data-ttu-id="ed613-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ed613-141">DateTime the object was created.</span></span> <span data-ttu-id="ed613-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed613-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed613-143">описание</span><span class="sxs-lookup"><span data-stu-id="ed613-143">description</span></span>|<span data-ttu-id="ed613-144">Строка</span><span class="sxs-lookup"><span data-stu-id="ed613-144">String</span></span>|<span data-ttu-id="ed613-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ed613-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ed613-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed613-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed613-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ed613-147">displayName</span></span>|<span data-ttu-id="ed613-148">Строка</span><span class="sxs-lookup"><span data-stu-id="ed613-148">String</span></span>|<span data-ttu-id="ed613-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ed613-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ed613-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed613-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed613-151">version</span><span class="sxs-lookup"><span data-stu-id="ed613-151">version</span></span>|<span data-ttu-id="ed613-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ed613-152">Int32</span></span>|<span data-ttu-id="ed613-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ed613-153">Version of the device configuration.</span></span> <span data-ttu-id="ed613-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ed613-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ed613-155">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="ed613-155">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="ed613-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed613-156">Boolean</span></span>|<span data-ttu-id="ed613-157">Указывает, следует ли заблокировать оперативную аналитику Azure.</span><span class="sxs-lookup"><span data-stu-id="ed613-157">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="ed613-158">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="ed613-158">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="ed613-159">String</span><span class="sxs-lookup"><span data-stu-id="ed613-159">String</span></span>|<span data-ttu-id="ed613-160">Идентификатор рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="ed613-160">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="ed613-161">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="ed613-161">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="ed613-162">String</span><span class="sxs-lookup"><span data-stu-id="ed613-162">String</span></span>|<span data-ttu-id="ed613-163">Ключ рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="ed613-163">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="ed613-164">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="ed613-164">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="ed613-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed613-165">Boolean</span></span>|<span data-ttu-id="ed613-166">Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.</span><span class="sxs-lookup"><span data-stu-id="ed613-166">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="ed613-167">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="ed613-167">maintenanceWindowBlocked</span></span>|<span data-ttu-id="ed613-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed613-168">Boolean</span></span>|<span data-ttu-id="ed613-169">Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="ed613-169">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="ed613-170">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="ed613-170">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="ed613-171">Int32</span><span class="sxs-lookup"><span data-stu-id="ed613-171">Int32</span></span>|<span data-ttu-id="ed613-172">Длительность периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="ed613-172">Maintenance window duration for device updates.</span></span> <span data-ttu-id="ed613-173">Допустимые значения: от 0 до 5</span><span class="sxs-lookup"><span data-stu-id="ed613-173">Valid values 0 to 5</span></span>|
|<span data-ttu-id="ed613-174">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="ed613-174">maintenanceWindowStartTime</span></span>|<span data-ttu-id="ed613-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ed613-175">TimeOfDay</span></span>|<span data-ttu-id="ed613-176">Начало периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="ed613-176">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="ed613-177">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="ed613-177">miracastChannel</span></span>|[<span data-ttu-id="ed613-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="ed613-178">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="ed613-179">Канал.</span><span class="sxs-lookup"><span data-stu-id="ed613-179">The channel.</span></span> <span data-ttu-id="ed613-180">Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="ed613-180">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="ed613-181">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="ed613-181">miracastBlocked</span></span>|<span data-ttu-id="ed613-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed613-182">Boolean</span></span>|<span data-ttu-id="ed613-183">Указывает, следует ли заблокировать беспроводное проецирование.</span><span class="sxs-lookup"><span data-stu-id="ed613-183">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="ed613-184">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="ed613-184">miracastRequirePin</span></span>|<span data-ttu-id="ed613-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed613-185">Boolean</span></span>|<span data-ttu-id="ed613-186">Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.</span><span class="sxs-lookup"><span data-stu-id="ed613-186">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="ed613-187">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="ed613-187">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="ed613-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed613-188">Boolean</span></span>|<span data-ttu-id="ed613-189">Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.</span><span class="sxs-lookup"><span data-stu-id="ed613-189">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="ed613-190">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="ed613-190">settingsBlockSessionResume</span></span>|<span data-ttu-id="ed613-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed613-191">Boolean</span></span>|<span data-ttu-id="ed613-192">Указывает, следует ли разрешить возобновление сеанса после истечения времени.</span><span class="sxs-lookup"><span data-stu-id="ed613-192">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="ed613-193">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="ed613-193">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="ed613-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed613-194">Boolean</span></span>|<span data-ttu-id="ed613-195">Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.</span><span class="sxs-lookup"><span data-stu-id="ed613-195">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="ed613-196">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="ed613-196">settingsDefaultVolume</span></span>|<span data-ttu-id="ed613-197">Int32</span><span class="sxs-lookup"><span data-stu-id="ed613-197">Int32</span></span>|<span data-ttu-id="ed613-198">Задает объем нового сеанса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ed613-198">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="ed613-199">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="ed613-199">Permitted values are 0-100.</span></span> <span data-ttu-id="ed613-200">Значение по умолчанию — 45.</span><span class="sxs-lookup"><span data-stu-id="ed613-200">The default is 45.</span></span> <span data-ttu-id="ed613-201">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="ed613-201">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ed613-202">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="ed613-202">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="ed613-203">Int32</span><span class="sxs-lookup"><span data-stu-id="ed613-203">Int32</span></span>|<span data-ttu-id="ed613-204">Определяет время до отключения экрана Центра (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ed613-204">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="ed613-205">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="ed613-205">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="ed613-206">Int32</span><span class="sxs-lookup"><span data-stu-id="ed613-206">Int32</span></span>|<span data-ttu-id="ed613-207">Определяет время до истечения времени сеанса (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ed613-207">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="ed613-208">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="ed613-208">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="ed613-209">Int32</span><span class="sxs-lookup"><span data-stu-id="ed613-209">Int32</span></span>|<span data-ttu-id="ed613-210">Определяет время до перехода Центра в спящий режим (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ed613-210">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="ed613-211">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="ed613-211">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="ed613-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed613-212">Boolean</span></span>|<span data-ttu-id="ed613-213">Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.</span><span class="sxs-lookup"><span data-stu-id="ed613-213">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="ed613-214">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="ed613-214">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="ed613-215">String</span><span class="sxs-lookup"><span data-stu-id="ed613-215">String</span></span>|<span data-ttu-id="ed613-216">URL-адрес фонового изображения экрана приветствия.</span><span class="sxs-lookup"><span data-stu-id="ed613-216">The welcome screen background image URL.</span></span> <span data-ttu-id="ed613-217">URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.</span><span class="sxs-lookup"><span data-stu-id="ed613-217">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="ed613-218">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="ed613-218">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="ed613-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="ed613-219">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="ed613-220">Информация о собраниях, показываемая на экране приветствия.</span><span class="sxs-lookup"><span data-stu-id="ed613-220">The welcome screen meeting information shown.</span></span> <span data-ttu-id="ed613-221">Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="ed613-221">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="ed613-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed613-222">Response</span></span>
<span data-ttu-id="ed613-223">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ed613-223">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed613-224">Пример</span><span class="sxs-lookup"><span data-stu-id="ed613-224">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed613-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed613-225">Request</span></span>
<span data-ttu-id="ed613-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed613-226">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ed613-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed613-227">Response</span></span>
<span data-ttu-id="ed613-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ed613-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



