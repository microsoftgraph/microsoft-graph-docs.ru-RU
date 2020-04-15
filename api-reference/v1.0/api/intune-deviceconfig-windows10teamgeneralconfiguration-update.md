---
title: Обновление windows10TeamGeneralConfiguration
description: Обновление свойств объекта windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a90858f35f0ae555ea8a74f2cfc4eed26cd7ea3a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442007"
---
# <a name="update-windows10teamgeneralconfiguration"></a><span data-ttu-id="ea665-103">Обновление windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea665-103">Update windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="ea665-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea665-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea665-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea665-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea665-106">Обновление свойств объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea665-106">Update the properties of a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea665-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ea665-107">Prerequisites</span></span>
<span data-ttu-id="ea665-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea665-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea665-110">Permission type</span></span>|<span data-ttu-id="ea665-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea665-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea665-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea665-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ea665-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea665-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ea665-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea665-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea665-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea665-115">Not supported.</span></span>|
|<span data-ttu-id="ea665-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea665-116">Application</span></span>|<span data-ttu-id="ea665-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea665-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea665-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea665-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ea665-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ea665-119">Request headers</span></span>
|<span data-ttu-id="ea665-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ea665-120">Header</span></span>|<span data-ttu-id="ea665-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ea665-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea665-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea665-122">Authorization</span></span>|<span data-ttu-id="ea665-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea665-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea665-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ea665-124">Accept</span></span>|<span data-ttu-id="ea665-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ea665-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea665-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ea665-126">Request body</span></span>
<span data-ttu-id="ea665-127">В теле запроса добавьте представление объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea665-127">In the request body, supply a JSON representation for the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

<span data-ttu-id="ea665-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea665-128">The following table shows the properties that are required when you create the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

|<span data-ttu-id="ea665-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea665-129">Property</span></span>|<span data-ttu-id="ea665-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ea665-130">Type</span></span>|<span data-ttu-id="ea665-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ea665-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea665-132">id</span><span class="sxs-lookup"><span data-stu-id="ea665-132">id</span></span>|<span data-ttu-id="ea665-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ea665-133">String</span></span>|<span data-ttu-id="ea665-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ea665-134">Key of the entity.</span></span> <span data-ttu-id="ea665-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea665-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea665-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea665-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ea665-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea665-137">DateTimeOffset</span></span>|<span data-ttu-id="ea665-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ea665-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ea665-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea665-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea665-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea665-140">createdDateTime</span></span>|<span data-ttu-id="ea665-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea665-141">DateTimeOffset</span></span>|<span data-ttu-id="ea665-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ea665-142">DateTime the object was created.</span></span> <span data-ttu-id="ea665-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea665-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea665-144">description</span><span class="sxs-lookup"><span data-stu-id="ea665-144">description</span></span>|<span data-ttu-id="ea665-145">String</span><span class="sxs-lookup"><span data-stu-id="ea665-145">String</span></span>|<span data-ttu-id="ea665-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ea665-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ea665-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea665-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea665-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ea665-148">displayName</span></span>|<span data-ttu-id="ea665-149">Строка</span><span class="sxs-lookup"><span data-stu-id="ea665-149">String</span></span>|<span data-ttu-id="ea665-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ea665-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ea665-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea665-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea665-152">version</span><span class="sxs-lookup"><span data-stu-id="ea665-152">version</span></span>|<span data-ttu-id="ea665-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ea665-153">Int32</span></span>|<span data-ttu-id="ea665-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ea665-154">Version of the device configuration.</span></span> <span data-ttu-id="ea665-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea665-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ea665-156">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="ea665-156">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="ea665-157">Логический</span><span class="sxs-lookup"><span data-stu-id="ea665-157">Boolean</span></span>|<span data-ttu-id="ea665-158">Указывает, следует ли заблокировать оперативную аналитику Azure.</span><span class="sxs-lookup"><span data-stu-id="ea665-158">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="ea665-159">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="ea665-159">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="ea665-160">String</span><span class="sxs-lookup"><span data-stu-id="ea665-160">String</span></span>|<span data-ttu-id="ea665-161">Идентификатор рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="ea665-161">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="ea665-162">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="ea665-162">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="ea665-163">String</span><span class="sxs-lookup"><span data-stu-id="ea665-163">String</span></span>|<span data-ttu-id="ea665-164">Ключ рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="ea665-164">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="ea665-165">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="ea665-165">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="ea665-166">Логический</span><span class="sxs-lookup"><span data-stu-id="ea665-166">Boolean</span></span>|<span data-ttu-id="ea665-167">Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.</span><span class="sxs-lookup"><span data-stu-id="ea665-167">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="ea665-168">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="ea665-168">maintenanceWindowBlocked</span></span>|<span data-ttu-id="ea665-169">Логический</span><span class="sxs-lookup"><span data-stu-id="ea665-169">Boolean</span></span>|<span data-ttu-id="ea665-170">Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="ea665-170">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="ea665-171">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="ea665-171">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="ea665-172">Int32</span><span class="sxs-lookup"><span data-stu-id="ea665-172">Int32</span></span>|<span data-ttu-id="ea665-173">Длительность периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="ea665-173">Maintenance window duration for device updates.</span></span> <span data-ttu-id="ea665-174">Допустимые значения: от 0 до 5</span><span class="sxs-lookup"><span data-stu-id="ea665-174">Valid values 0 to 5</span></span>|
|<span data-ttu-id="ea665-175">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="ea665-175">maintenanceWindowStartTime</span></span>|<span data-ttu-id="ea665-176">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ea665-176">TimeOfDay</span></span>|<span data-ttu-id="ea665-177">Начало периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="ea665-177">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="ea665-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="ea665-178">miracastChannel</span></span>|[<span data-ttu-id="ea665-179">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="ea665-179">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="ea665-180">Канал.</span><span class="sxs-lookup"><span data-stu-id="ea665-180">The channel.</span></span> <span data-ttu-id="ea665-181">Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="ea665-181">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="ea665-182">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="ea665-182">miracastBlocked</span></span>|<span data-ttu-id="ea665-183">Логический</span><span class="sxs-lookup"><span data-stu-id="ea665-183">Boolean</span></span>|<span data-ttu-id="ea665-184">Указывает, следует ли заблокировать беспроводное проецирование.</span><span class="sxs-lookup"><span data-stu-id="ea665-184">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="ea665-185">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="ea665-185">miracastRequirePin</span></span>|<span data-ttu-id="ea665-186">Логический</span><span class="sxs-lookup"><span data-stu-id="ea665-186">Boolean</span></span>|<span data-ttu-id="ea665-187">Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.</span><span class="sxs-lookup"><span data-stu-id="ea665-187">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="ea665-188">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="ea665-188">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="ea665-189">Логический</span><span class="sxs-lookup"><span data-stu-id="ea665-189">Boolean</span></span>|<span data-ttu-id="ea665-190">Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.</span><span class="sxs-lookup"><span data-stu-id="ea665-190">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="ea665-191">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="ea665-191">settingsBlockSessionResume</span></span>|<span data-ttu-id="ea665-192">Логический</span><span class="sxs-lookup"><span data-stu-id="ea665-192">Boolean</span></span>|<span data-ttu-id="ea665-193">Указывает, следует ли разрешить возобновление сеанса после истечения времени.</span><span class="sxs-lookup"><span data-stu-id="ea665-193">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="ea665-194">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="ea665-194">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="ea665-195">Логический</span><span class="sxs-lookup"><span data-stu-id="ea665-195">Boolean</span></span>|<span data-ttu-id="ea665-196">Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.</span><span class="sxs-lookup"><span data-stu-id="ea665-196">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="ea665-197">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="ea665-197">settingsDefaultVolume</span></span>|<span data-ttu-id="ea665-198">Int32</span><span class="sxs-lookup"><span data-stu-id="ea665-198">Int32</span></span>|<span data-ttu-id="ea665-199">Задает объем нового сеанса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ea665-199">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="ea665-200">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="ea665-200">Permitted values are 0-100.</span></span> <span data-ttu-id="ea665-201">Значение по умолчанию — 45.</span><span class="sxs-lookup"><span data-stu-id="ea665-201">The default is 45.</span></span> <span data-ttu-id="ea665-202">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="ea665-202">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ea665-203">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="ea665-203">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="ea665-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ea665-204">Int32</span></span>|<span data-ttu-id="ea665-205">Определяет время до отключения экрана Центра (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ea665-205">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="ea665-206">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="ea665-206">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="ea665-207">Int32</span><span class="sxs-lookup"><span data-stu-id="ea665-207">Int32</span></span>|<span data-ttu-id="ea665-208">Определяет время до истечения времени сеанса (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ea665-208">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="ea665-209">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="ea665-209">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="ea665-210">Int32</span><span class="sxs-lookup"><span data-stu-id="ea665-210">Int32</span></span>|<span data-ttu-id="ea665-211">Определяет время до перехода Центра в спящий режим (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ea665-211">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="ea665-212">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="ea665-212">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="ea665-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea665-213">Boolean</span></span>|<span data-ttu-id="ea665-214">Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.</span><span class="sxs-lookup"><span data-stu-id="ea665-214">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="ea665-215">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="ea665-215">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="ea665-216">String</span><span class="sxs-lookup"><span data-stu-id="ea665-216">String</span></span>|<span data-ttu-id="ea665-217">URL-адрес фонового изображения экрана приветствия.</span><span class="sxs-lookup"><span data-stu-id="ea665-217">The welcome screen background image URL.</span></span> <span data-ttu-id="ea665-218">URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.</span><span class="sxs-lookup"><span data-stu-id="ea665-218">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="ea665-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="ea665-219">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="ea665-220">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="ea665-220">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="ea665-221">Информация о собраниях, показываемая на экране приветствия.</span><span class="sxs-lookup"><span data-stu-id="ea665-221">The welcome screen meeting information shown.</span></span> <span data-ttu-id="ea665-222">Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="ea665-222">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="ea665-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea665-223">Response</span></span>
<span data-ttu-id="ea665-224">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ea665-224">If successful, this method returns a `200 OK` response code and an updated [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea665-225">Пример</span><span class="sxs-lookup"><span data-stu-id="ea665-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea665-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea665-226">Request</span></span>
<span data-ttu-id="ea665-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea665-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ea665-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea665-228">Response</span></span>
<span data-ttu-id="ea665-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea665-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






