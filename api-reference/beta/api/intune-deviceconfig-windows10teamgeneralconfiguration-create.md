---
title: Создание объекта windows10TeamGeneralConfiguration
description: Создание объекта windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3ae4ff125219d470b4ae8bc8462f6b234adb0714
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986000"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="91452-103">Создание объекта windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="91452-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="91452-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91452-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91452-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91452-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91452-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="91452-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91452-107">Создает объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91452-107">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="91452-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="91452-108">Prerequisites</span></span>
<span data-ttu-id="91452-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91452-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91452-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91452-111">Permission type</span></span>|<span data-ttu-id="91452-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="91452-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91452-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91452-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91452-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91452-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="91452-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91452-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91452-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91452-116">Not supported.</span></span>|
|<span data-ttu-id="91452-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91452-117">Application</span></span>|<span data-ttu-id="91452-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91452-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91452-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91452-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="91452-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91452-120">Request headers</span></span>
|<span data-ttu-id="91452-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91452-121">Header</span></span>|<span data-ttu-id="91452-122">Значение</span><span class="sxs-lookup"><span data-stu-id="91452-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91452-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91452-123">Authorization</span></span>|<span data-ttu-id="91452-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="91452-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91452-125">Accept</span><span class="sxs-lookup"><span data-stu-id="91452-125">Accept</span></span>|<span data-ttu-id="91452-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91452-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91452-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91452-127">Request body</span></span>
<span data-ttu-id="91452-128">В теле запроса добавьте представление объекта windows10TeamGeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91452-128">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="91452-129">Ниже показаны свойства, которые необходимо указывать при создании объекта windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="91452-129">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="91452-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="91452-130">Property</span></span>|<span data-ttu-id="91452-131">Тип</span><span class="sxs-lookup"><span data-stu-id="91452-131">Type</span></span>|<span data-ttu-id="91452-132">Описание</span><span class="sxs-lookup"><span data-stu-id="91452-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91452-133">id</span><span class="sxs-lookup"><span data-stu-id="91452-133">id</span></span>|<span data-ttu-id="91452-134">Строка</span><span class="sxs-lookup"><span data-stu-id="91452-134">String</span></span>|<span data-ttu-id="91452-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="91452-135">Key of the entity.</span></span> <span data-ttu-id="91452-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91452-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91452-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91452-137">lastModifiedDateTime</span></span>|<span data-ttu-id="91452-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91452-138">DateTimeOffset</span></span>|<span data-ttu-id="91452-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="91452-139">DateTime the object was last modified.</span></span> <span data-ttu-id="91452-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91452-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91452-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="91452-141">roleScopeTagIds</span></span>|<span data-ttu-id="91452-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="91452-142">String collection</span></span>|<span data-ttu-id="91452-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="91452-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="91452-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91452-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91452-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="91452-145">supportsScopeTags</span></span>|<span data-ttu-id="91452-146">Логический</span><span class="sxs-lookup"><span data-stu-id="91452-146">Boolean</span></span>|<span data-ttu-id="91452-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="91452-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="91452-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="91452-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="91452-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="91452-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="91452-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="91452-150">This property is read-only.</span></span> <span data-ttu-id="91452-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91452-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91452-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91452-152">createdDateTime</span></span>|<span data-ttu-id="91452-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91452-153">DateTimeOffset</span></span>|<span data-ttu-id="91452-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="91452-154">DateTime the object was created.</span></span> <span data-ttu-id="91452-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91452-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91452-156">описание</span><span class="sxs-lookup"><span data-stu-id="91452-156">description</span></span>|<span data-ttu-id="91452-157">Строка</span><span class="sxs-lookup"><span data-stu-id="91452-157">String</span></span>|<span data-ttu-id="91452-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="91452-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="91452-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91452-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91452-160">displayName</span><span class="sxs-lookup"><span data-stu-id="91452-160">displayName</span></span>|<span data-ttu-id="91452-161">Строка</span><span class="sxs-lookup"><span data-stu-id="91452-161">String</span></span>|<span data-ttu-id="91452-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="91452-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="91452-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91452-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91452-164">version</span><span class="sxs-lookup"><span data-stu-id="91452-164">version</span></span>|<span data-ttu-id="91452-165">Int32</span><span class="sxs-lookup"><span data-stu-id="91452-165">Int32</span></span>|<span data-ttu-id="91452-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="91452-166">Version of the device configuration.</span></span> <span data-ttu-id="91452-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="91452-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="91452-168">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="91452-168">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="91452-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="91452-169">Boolean</span></span>|<span data-ttu-id="91452-170">Указывает, следует ли заблокировать оперативную аналитику Azure.</span><span class="sxs-lookup"><span data-stu-id="91452-170">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="91452-171">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="91452-171">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="91452-172">String</span><span class="sxs-lookup"><span data-stu-id="91452-172">String</span></span>|<span data-ttu-id="91452-173">Идентификатор рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="91452-173">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="91452-174">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="91452-174">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="91452-175">String</span><span class="sxs-lookup"><span data-stu-id="91452-175">String</span></span>|<span data-ttu-id="91452-176">Ключ рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="91452-176">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="91452-177">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="91452-177">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="91452-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="91452-178">Boolean</span></span>|<span data-ttu-id="91452-179">Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.</span><span class="sxs-lookup"><span data-stu-id="91452-179">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="91452-180">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="91452-180">maintenanceWindowBlocked</span></span>|<span data-ttu-id="91452-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="91452-181">Boolean</span></span>|<span data-ttu-id="91452-182">Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="91452-182">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="91452-183">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="91452-183">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="91452-184">Int32</span><span class="sxs-lookup"><span data-stu-id="91452-184">Int32</span></span>|<span data-ttu-id="91452-185">Длительность периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="91452-185">Maintenance window duration for device updates.</span></span> <span data-ttu-id="91452-186">Допустимые значения: от 0 до 5</span><span class="sxs-lookup"><span data-stu-id="91452-186">Valid values 0 to 5</span></span>|
|<span data-ttu-id="91452-187">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="91452-187">maintenanceWindowStartTime</span></span>|<span data-ttu-id="91452-188">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="91452-188">TimeOfDay</span></span>|<span data-ttu-id="91452-189">Начало периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="91452-189">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="91452-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="91452-190">miracastChannel</span></span>|[<span data-ttu-id="91452-191">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="91452-191">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="91452-192">Канал.</span><span class="sxs-lookup"><span data-stu-id="91452-192">The channel.</span></span> <span data-ttu-id="91452-193">Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="91452-193">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="91452-194">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="91452-194">miracastBlocked</span></span>|<span data-ttu-id="91452-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="91452-195">Boolean</span></span>|<span data-ttu-id="91452-196">Указывает, следует ли заблокировать беспроводное проецирование.</span><span class="sxs-lookup"><span data-stu-id="91452-196">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="91452-197">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="91452-197">miracastRequirePin</span></span>|<span data-ttu-id="91452-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="91452-198">Boolean</span></span>|<span data-ttu-id="91452-199">Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.</span><span class="sxs-lookup"><span data-stu-id="91452-199">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="91452-200">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="91452-200">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="91452-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="91452-201">Boolean</span></span>|<span data-ttu-id="91452-202">Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.</span><span class="sxs-lookup"><span data-stu-id="91452-202">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="91452-203">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="91452-203">settingsBlockSessionResume</span></span>|<span data-ttu-id="91452-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="91452-204">Boolean</span></span>|<span data-ttu-id="91452-205">Указывает, следует ли разрешить возобновление сеанса после истечения времени.</span><span class="sxs-lookup"><span data-stu-id="91452-205">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="91452-206">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="91452-206">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="91452-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="91452-207">Boolean</span></span>|<span data-ttu-id="91452-208">Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.</span><span class="sxs-lookup"><span data-stu-id="91452-208">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="91452-209">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="91452-209">settingsDefaultVolume</span></span>|<span data-ttu-id="91452-210">Int32</span><span class="sxs-lookup"><span data-stu-id="91452-210">Int32</span></span>|<span data-ttu-id="91452-211">Задает объем нового сеанса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="91452-211">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="91452-212">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="91452-212">Permitted values are 0-100.</span></span> <span data-ttu-id="91452-213">Значение по умолчанию — 45.</span><span class="sxs-lookup"><span data-stu-id="91452-213">The default is 45.</span></span> <span data-ttu-id="91452-214">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="91452-214">Valid values 0 to 100</span></span>|
|<span data-ttu-id="91452-215">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="91452-215">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="91452-216">Int32</span><span class="sxs-lookup"><span data-stu-id="91452-216">Int32</span></span>|<span data-ttu-id="91452-217">Определяет время до отключения экрана Центра (в минутах).</span><span class="sxs-lookup"><span data-stu-id="91452-217">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="91452-218">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="91452-218">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="91452-219">Int32</span><span class="sxs-lookup"><span data-stu-id="91452-219">Int32</span></span>|<span data-ttu-id="91452-220">Определяет время до истечения времени сеанса (в минутах).</span><span class="sxs-lookup"><span data-stu-id="91452-220">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="91452-221">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="91452-221">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="91452-222">Int32</span><span class="sxs-lookup"><span data-stu-id="91452-222">Int32</span></span>|<span data-ttu-id="91452-223">Определяет время до перехода Центра в спящий режим (в минутах).</span><span class="sxs-lookup"><span data-stu-id="91452-223">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="91452-224">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="91452-224">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="91452-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="91452-225">Boolean</span></span>|<span data-ttu-id="91452-226">Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.</span><span class="sxs-lookup"><span data-stu-id="91452-226">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="91452-227">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="91452-227">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="91452-228">String</span><span class="sxs-lookup"><span data-stu-id="91452-228">String</span></span>|<span data-ttu-id="91452-229">URL-адрес фонового изображения экрана приветствия.</span><span class="sxs-lookup"><span data-stu-id="91452-229">The welcome screen background image URL.</span></span> <span data-ttu-id="91452-230">URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.</span><span class="sxs-lookup"><span data-stu-id="91452-230">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="91452-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="91452-231">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="91452-232">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="91452-232">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="91452-233">Информация о собраниях, показываемая на экране приветствия.</span><span class="sxs-lookup"><span data-stu-id="91452-233">The welcome screen meeting information shown.</span></span> <span data-ttu-id="91452-234">Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="91452-234">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="91452-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="91452-235">Response</span></span>
<span data-ttu-id="91452-236">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="91452-236">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91452-237">Пример</span><span class="sxs-lookup"><span data-stu-id="91452-237">Example</span></span>
### <a name="request"></a><span data-ttu-id="91452-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="91452-238">Request</span></span>
<span data-ttu-id="91452-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91452-239">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1306

{
  "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="91452-240">Ответ</span><span class="sxs-lookup"><span data-stu-id="91452-240">Response</span></span>
<span data-ttu-id="91452-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="91452-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





