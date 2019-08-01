---
title: Создание объекта windows10TeamGeneralConfiguration
description: Создает объект windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b4083c1bc0c9673c1cf8d773e4ce836cc2243ea3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997192"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="0028d-103">Создание объекта windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="0028d-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="0028d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0028d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0028d-105">Создает объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0028d-105">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0028d-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0028d-106">Prerequisites</span></span>
<span data-ttu-id="0028d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0028d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0028d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0028d-109">Permission type</span></span>|<span data-ttu-id="0028d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0028d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0028d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0028d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0028d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0028d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0028d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0028d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0028d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0028d-114">Not supported.</span></span>|
|<span data-ttu-id="0028d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0028d-115">Application</span></span>|<span data-ttu-id="0028d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0028d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0028d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0028d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0028d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0028d-118">Request headers</span></span>
|<span data-ttu-id="0028d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0028d-119">Header</span></span>|<span data-ttu-id="0028d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0028d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0028d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0028d-121">Authorization</span></span>|<span data-ttu-id="0028d-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0028d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0028d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0028d-123">Accept</span></span>|<span data-ttu-id="0028d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0028d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0028d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0028d-125">Request body</span></span>
<span data-ttu-id="0028d-126">В теле запроса добавьте представление объекта windows10TeamGeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0028d-126">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="0028d-127">Ниже показаны свойства, которые необходимо указывать при создании объекта windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0028d-127">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="0028d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0028d-128">Property</span></span>|<span data-ttu-id="0028d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0028d-129">Type</span></span>|<span data-ttu-id="0028d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0028d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0028d-131">id</span><span class="sxs-lookup"><span data-stu-id="0028d-131">id</span></span>|<span data-ttu-id="0028d-132">Строка</span><span class="sxs-lookup"><span data-stu-id="0028d-132">String</span></span>|<span data-ttu-id="0028d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0028d-133">Key of the entity.</span></span> <span data-ttu-id="0028d-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0028d-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0028d-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0028d-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0028d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0028d-136">DateTimeOffset</span></span>|<span data-ttu-id="0028d-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0028d-137">DateTime the object was last modified.</span></span> <span data-ttu-id="0028d-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0028d-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0028d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0028d-139">createdDateTime</span></span>|<span data-ttu-id="0028d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0028d-140">DateTimeOffset</span></span>|<span data-ttu-id="0028d-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0028d-141">DateTime the object was created.</span></span> <span data-ttu-id="0028d-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0028d-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0028d-143">description</span><span class="sxs-lookup"><span data-stu-id="0028d-143">description</span></span>|<span data-ttu-id="0028d-144">String</span><span class="sxs-lookup"><span data-stu-id="0028d-144">String</span></span>|<span data-ttu-id="0028d-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0028d-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0028d-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0028d-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0028d-147">displayName</span><span class="sxs-lookup"><span data-stu-id="0028d-147">displayName</span></span>|<span data-ttu-id="0028d-148">Строка</span><span class="sxs-lookup"><span data-stu-id="0028d-148">String</span></span>|<span data-ttu-id="0028d-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0028d-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0028d-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0028d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0028d-151">version</span><span class="sxs-lookup"><span data-stu-id="0028d-151">version</span></span>|<span data-ttu-id="0028d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0028d-152">Int32</span></span>|<span data-ttu-id="0028d-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0028d-153">Version of the device configuration.</span></span> <span data-ttu-id="0028d-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0028d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0028d-155">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="0028d-155">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="0028d-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="0028d-156">Boolean</span></span>|<span data-ttu-id="0028d-157">Указывает, следует ли заблокировать оперативную аналитику Azure.</span><span class="sxs-lookup"><span data-stu-id="0028d-157">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="0028d-158">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="0028d-158">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="0028d-159">String</span><span class="sxs-lookup"><span data-stu-id="0028d-159">String</span></span>|<span data-ttu-id="0028d-160">Идентификатор рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="0028d-160">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="0028d-161">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="0028d-161">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="0028d-162">String</span><span class="sxs-lookup"><span data-stu-id="0028d-162">String</span></span>|<span data-ttu-id="0028d-163">Ключ рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="0028d-163">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="0028d-164">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="0028d-164">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="0028d-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="0028d-165">Boolean</span></span>|<span data-ttu-id="0028d-166">Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.</span><span class="sxs-lookup"><span data-stu-id="0028d-166">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="0028d-167">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="0028d-167">maintenanceWindowBlocked</span></span>|<span data-ttu-id="0028d-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="0028d-168">Boolean</span></span>|<span data-ttu-id="0028d-169">Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="0028d-169">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="0028d-170">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="0028d-170">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="0028d-171">Int32</span><span class="sxs-lookup"><span data-stu-id="0028d-171">Int32</span></span>|<span data-ttu-id="0028d-172">Длительность периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="0028d-172">Maintenance window duration for device updates.</span></span> <span data-ttu-id="0028d-173">Допустимые значения: от 0 до 5</span><span class="sxs-lookup"><span data-stu-id="0028d-173">Valid values 0 to 5</span></span>|
|<span data-ttu-id="0028d-174">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="0028d-174">maintenanceWindowStartTime</span></span>|<span data-ttu-id="0028d-175">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0028d-175">TimeOfDay</span></span>|<span data-ttu-id="0028d-176">Начало периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="0028d-176">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="0028d-177">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="0028d-177">miracastChannel</span></span>|[<span data-ttu-id="0028d-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="0028d-178">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="0028d-179">Канал.</span><span class="sxs-lookup"><span data-stu-id="0028d-179">The channel.</span></span> <span data-ttu-id="0028d-180">Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="0028d-180">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="0028d-181">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="0028d-181">miracastBlocked</span></span>|<span data-ttu-id="0028d-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="0028d-182">Boolean</span></span>|<span data-ttu-id="0028d-183">Указывает, следует ли заблокировать беспроводное проецирование.</span><span class="sxs-lookup"><span data-stu-id="0028d-183">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="0028d-184">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="0028d-184">miracastRequirePin</span></span>|<span data-ttu-id="0028d-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="0028d-185">Boolean</span></span>|<span data-ttu-id="0028d-186">Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.</span><span class="sxs-lookup"><span data-stu-id="0028d-186">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="0028d-187">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="0028d-187">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="0028d-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="0028d-188">Boolean</span></span>|<span data-ttu-id="0028d-189">Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.</span><span class="sxs-lookup"><span data-stu-id="0028d-189">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="0028d-190">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="0028d-190">settingsBlockSessionResume</span></span>|<span data-ttu-id="0028d-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="0028d-191">Boolean</span></span>|<span data-ttu-id="0028d-192">Указывает, следует ли разрешить возобновление сеанса после истечения времени.</span><span class="sxs-lookup"><span data-stu-id="0028d-192">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="0028d-193">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="0028d-193">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="0028d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0028d-194">Boolean</span></span>|<span data-ttu-id="0028d-195">Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.</span><span class="sxs-lookup"><span data-stu-id="0028d-195">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="0028d-196">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="0028d-196">settingsDefaultVolume</span></span>|<span data-ttu-id="0028d-197">Int32</span><span class="sxs-lookup"><span data-stu-id="0028d-197">Int32</span></span>|<span data-ttu-id="0028d-198">Задает объем нового сеанса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0028d-198">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="0028d-199">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="0028d-199">Permitted values are 0-100.</span></span> <span data-ttu-id="0028d-200">Значение по умолчанию — 45.</span><span class="sxs-lookup"><span data-stu-id="0028d-200">The default is 45.</span></span> <span data-ttu-id="0028d-201">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="0028d-201">Valid values 0 to 100</span></span>|
|<span data-ttu-id="0028d-202">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="0028d-202">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="0028d-203">Int32</span><span class="sxs-lookup"><span data-stu-id="0028d-203">Int32</span></span>|<span data-ttu-id="0028d-204">Определяет время до отключения экрана Центра (в минутах).</span><span class="sxs-lookup"><span data-stu-id="0028d-204">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="0028d-205">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="0028d-205">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="0028d-206">Int32</span><span class="sxs-lookup"><span data-stu-id="0028d-206">Int32</span></span>|<span data-ttu-id="0028d-207">Определяет время до истечения времени сеанса (в минутах).</span><span class="sxs-lookup"><span data-stu-id="0028d-207">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="0028d-208">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="0028d-208">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="0028d-209">Int32</span><span class="sxs-lookup"><span data-stu-id="0028d-209">Int32</span></span>|<span data-ttu-id="0028d-210">Определяет время до перехода Центра в спящий режим (в минутах).</span><span class="sxs-lookup"><span data-stu-id="0028d-210">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="0028d-211">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="0028d-211">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="0028d-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="0028d-212">Boolean</span></span>|<span data-ttu-id="0028d-213">Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.</span><span class="sxs-lookup"><span data-stu-id="0028d-213">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="0028d-214">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="0028d-214">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="0028d-215">String</span><span class="sxs-lookup"><span data-stu-id="0028d-215">String</span></span>|<span data-ttu-id="0028d-216">URL-адрес фонового изображения экрана приветствия.</span><span class="sxs-lookup"><span data-stu-id="0028d-216">The welcome screen background image URL.</span></span> <span data-ttu-id="0028d-217">URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.</span><span class="sxs-lookup"><span data-stu-id="0028d-217">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="0028d-218">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="0028d-218">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="0028d-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="0028d-219">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="0028d-220">Информация о собраниях, показываемая на экране приветствия.</span><span class="sxs-lookup"><span data-stu-id="0028d-220">The welcome screen meeting information shown.</span></span> <span data-ttu-id="0028d-221">Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="0028d-221">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="0028d-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="0028d-222">Response</span></span>
<span data-ttu-id="0028d-223">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0028d-223">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0028d-224">Пример</span><span class="sxs-lookup"><span data-stu-id="0028d-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="0028d-225">Запрос</span><span class="sxs-lookup"><span data-stu-id="0028d-225">Request</span></span>
<span data-ttu-id="0028d-226">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0028d-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="0028d-227">Отклик</span><span class="sxs-lookup"><span data-stu-id="0028d-227">Response</span></span>
<span data-ttu-id="0028d-p113">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0028d-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



