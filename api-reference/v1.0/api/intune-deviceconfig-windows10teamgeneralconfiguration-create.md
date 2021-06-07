---
title: Создание объекта windows10TeamGeneralConfiguration
description: Создает объект windows10TeamGeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8286551f14d7fcedaa7233814240afe5c4610abe
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760449"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="c862e-103">Создание объекта windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="c862e-103">Create windows10TeamGeneralConfiguration</span></span>

<span data-ttu-id="c862e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c862e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c862e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c862e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c862e-106">Создает объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c862e-106">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c862e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c862e-107">Prerequisites</span></span>
<span data-ttu-id="c862e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c862e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c862e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c862e-110">Permission type</span></span>|<span data-ttu-id="c862e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c862e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c862e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c862e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c862e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c862e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c862e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c862e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c862e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c862e-115">Not supported.</span></span>|
|<span data-ttu-id="c862e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c862e-116">Application</span></span>|<span data-ttu-id="c862e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c862e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c862e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c862e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c862e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c862e-119">Request headers</span></span>
|<span data-ttu-id="c862e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c862e-120">Header</span></span>|<span data-ttu-id="c862e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c862e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c862e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c862e-122">Authorization</span></span>|<span data-ttu-id="c862e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c862e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c862e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c862e-124">Accept</span></span>|<span data-ttu-id="c862e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c862e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c862e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c862e-126">Request body</span></span>
<span data-ttu-id="c862e-127">В теле запроса добавьте представление объекта windows10TeamGeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c862e-127">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="c862e-128">Ниже показаны свойства, которые необходимо указывать при создании объекта windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c862e-128">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="c862e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c862e-129">Property</span></span>|<span data-ttu-id="c862e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c862e-130">Type</span></span>|<span data-ttu-id="c862e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c862e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c862e-132">id</span><span class="sxs-lookup"><span data-stu-id="c862e-132">id</span></span>|<span data-ttu-id="c862e-133">String</span><span class="sxs-lookup"><span data-stu-id="c862e-133">String</span></span>|<span data-ttu-id="c862e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c862e-134">Key of the entity.</span></span> <span data-ttu-id="c862e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c862e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c862e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c862e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c862e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c862e-137">DateTimeOffset</span></span>|<span data-ttu-id="c862e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c862e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c862e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c862e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c862e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c862e-140">createdDateTime</span></span>|<span data-ttu-id="c862e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c862e-141">DateTimeOffset</span></span>|<span data-ttu-id="c862e-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c862e-142">DateTime the object was created.</span></span> <span data-ttu-id="c862e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c862e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c862e-144">description</span><span class="sxs-lookup"><span data-stu-id="c862e-144">description</span></span>|<span data-ttu-id="c862e-145">String</span><span class="sxs-lookup"><span data-stu-id="c862e-145">String</span></span>|<span data-ttu-id="c862e-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c862e-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c862e-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c862e-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c862e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="c862e-148">displayName</span></span>|<span data-ttu-id="c862e-149">String</span><span class="sxs-lookup"><span data-stu-id="c862e-149">String</span></span>|<span data-ttu-id="c862e-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c862e-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c862e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c862e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c862e-152">version</span><span class="sxs-lookup"><span data-stu-id="c862e-152">version</span></span>|<span data-ttu-id="c862e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c862e-153">Int32</span></span>|<span data-ttu-id="c862e-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c862e-154">Version of the device configuration.</span></span> <span data-ttu-id="c862e-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c862e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c862e-156">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="c862e-156">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="c862e-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="c862e-157">Boolean</span></span>|<span data-ttu-id="c862e-158">Указывает, следует ли заблокировать оперативную аналитику Azure.</span><span class="sxs-lookup"><span data-stu-id="c862e-158">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="c862e-159">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="c862e-159">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="c862e-160">String</span><span class="sxs-lookup"><span data-stu-id="c862e-160">String</span></span>|<span data-ttu-id="c862e-161">Идентификатор рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="c862e-161">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="c862e-162">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="c862e-162">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="c862e-163">String</span><span class="sxs-lookup"><span data-stu-id="c862e-163">String</span></span>|<span data-ttu-id="c862e-164">Ключ рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="c862e-164">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="c862e-165">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="c862e-165">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="c862e-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="c862e-166">Boolean</span></span>|<span data-ttu-id="c862e-167">Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.</span><span class="sxs-lookup"><span data-stu-id="c862e-167">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="c862e-168">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="c862e-168">maintenanceWindowBlocked</span></span>|<span data-ttu-id="c862e-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="c862e-169">Boolean</span></span>|<span data-ttu-id="c862e-170">Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="c862e-170">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="c862e-171">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="c862e-171">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="c862e-172">Int32</span><span class="sxs-lookup"><span data-stu-id="c862e-172">Int32</span></span>|<span data-ttu-id="c862e-173">Длительность периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="c862e-173">Maintenance window duration for device updates.</span></span> <span data-ttu-id="c862e-174">Допустимые значения: от 0 до 5</span><span class="sxs-lookup"><span data-stu-id="c862e-174">Valid values 0 to 5</span></span>|
|<span data-ttu-id="c862e-175">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="c862e-175">maintenanceWindowStartTime</span></span>|<span data-ttu-id="c862e-176">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="c862e-176">TimeOfDay</span></span>|<span data-ttu-id="c862e-177">Начало периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="c862e-177">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="c862e-178">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="c862e-178">miracastChannel</span></span>|[<span data-ttu-id="c862e-179">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="c862e-179">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="c862e-180">Канал.</span><span class="sxs-lookup"><span data-stu-id="c862e-180">The channel.</span></span> <span data-ttu-id="c862e-181">Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="c862e-181">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="c862e-182">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="c862e-182">miracastBlocked</span></span>|<span data-ttu-id="c862e-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="c862e-183">Boolean</span></span>|<span data-ttu-id="c862e-184">Указывает, следует ли заблокировать беспроводное проецирование.</span><span class="sxs-lookup"><span data-stu-id="c862e-184">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="c862e-185">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="c862e-185">miracastRequirePin</span></span>|<span data-ttu-id="c862e-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="c862e-186">Boolean</span></span>|<span data-ttu-id="c862e-187">Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.</span><span class="sxs-lookup"><span data-stu-id="c862e-187">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="c862e-188">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="c862e-188">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="c862e-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="c862e-189">Boolean</span></span>|<span data-ttu-id="c862e-190">Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.</span><span class="sxs-lookup"><span data-stu-id="c862e-190">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="c862e-191">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="c862e-191">settingsBlockSessionResume</span></span>|<span data-ttu-id="c862e-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="c862e-192">Boolean</span></span>|<span data-ttu-id="c862e-193">Указывает, следует ли разрешить возобновление сеанса после истечения времени.</span><span class="sxs-lookup"><span data-stu-id="c862e-193">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="c862e-194">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="c862e-194">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="c862e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c862e-195">Boolean</span></span>|<span data-ttu-id="c862e-196">Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.</span><span class="sxs-lookup"><span data-stu-id="c862e-196">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="c862e-197">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="c862e-197">settingsDefaultVolume</span></span>|<span data-ttu-id="c862e-198">Int32</span><span class="sxs-lookup"><span data-stu-id="c862e-198">Int32</span></span>|<span data-ttu-id="c862e-199">Задает объем нового сеанса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c862e-199">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="c862e-200">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="c862e-200">Permitted values are 0-100.</span></span> <span data-ttu-id="c862e-201">Значение по умолчанию — 45.</span><span class="sxs-lookup"><span data-stu-id="c862e-201">The default is 45.</span></span> <span data-ttu-id="c862e-202">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="c862e-202">Valid values 0 to 100</span></span>|
|<span data-ttu-id="c862e-203">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c862e-203">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="c862e-204">Int32</span><span class="sxs-lookup"><span data-stu-id="c862e-204">Int32</span></span>|<span data-ttu-id="c862e-205">Определяет время до отключения экрана Центра (в минутах).</span><span class="sxs-lookup"><span data-stu-id="c862e-205">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="c862e-206">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c862e-206">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="c862e-207">Int32</span><span class="sxs-lookup"><span data-stu-id="c862e-207">Int32</span></span>|<span data-ttu-id="c862e-208">Определяет время до истечения времени сеанса (в минутах).</span><span class="sxs-lookup"><span data-stu-id="c862e-208">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="c862e-209">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c862e-209">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="c862e-210">Int32</span><span class="sxs-lookup"><span data-stu-id="c862e-210">Int32</span></span>|<span data-ttu-id="c862e-211">Определяет время до перехода Центра в спящий режим (в минутах).</span><span class="sxs-lookup"><span data-stu-id="c862e-211">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="c862e-212">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="c862e-212">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="c862e-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="c862e-213">Boolean</span></span>|<span data-ttu-id="c862e-214">Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.</span><span class="sxs-lookup"><span data-stu-id="c862e-214">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="c862e-215">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="c862e-215">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="c862e-216">String</span><span class="sxs-lookup"><span data-stu-id="c862e-216">String</span></span>|<span data-ttu-id="c862e-217">URL-адрес фонового изображения экрана приветствия.</span><span class="sxs-lookup"><span data-stu-id="c862e-217">The welcome screen background image URL.</span></span> <span data-ttu-id="c862e-218">URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.</span><span class="sxs-lookup"><span data-stu-id="c862e-218">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="c862e-219">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="c862e-219">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="c862e-220">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="c862e-220">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="c862e-221">Информация о собраниях, показываемая на экране приветствия.</span><span class="sxs-lookup"><span data-stu-id="c862e-221">The welcome screen meeting information shown.</span></span> <span data-ttu-id="c862e-222">Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="c862e-222">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="c862e-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="c862e-223">Response</span></span>
<span data-ttu-id="c862e-224">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c862e-224">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c862e-225">Пример</span><span class="sxs-lookup"><span data-stu-id="c862e-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="c862e-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="c862e-226">Request</span></span>
<span data-ttu-id="c862e-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c862e-227">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c862e-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="c862e-228">Response</span></span>
<span data-ttu-id="c862e-p113">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c862e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




