---
title: Создание объекта windows10TeamGeneralConfiguration
description: Создание объекта windows10TeamGeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b1b1061e1aba8f1f3aaccc8cdc2d85565a52dadf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836619"
---
# <a name="create-windows10teamgeneralconfiguration"></a><span data-ttu-id="ca386-103">Создание объекта windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca386-103">Create windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="ca386-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca386-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca386-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca386-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca386-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ca386-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca386-107">Создает объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca386-107">Create a new [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca386-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ca386-108">Prerequisites</span></span>
<span data-ttu-id="ca386-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca386-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca386-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ca386-111">Permission type</span></span>|<span data-ttu-id="ca386-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ca386-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca386-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ca386-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca386-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca386-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca386-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ca386-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca386-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca386-116">Not supported.</span></span>|
|<span data-ttu-id="ca386-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ca386-117">Application</span></span>|<span data-ttu-id="ca386-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca386-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca386-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ca386-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ca386-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ca386-120">Request headers</span></span>
|<span data-ttu-id="ca386-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ca386-121">Header</span></span>|<span data-ttu-id="ca386-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ca386-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca386-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca386-123">Authorization</span></span>|<span data-ttu-id="ca386-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ca386-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca386-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ca386-125">Accept</span></span>|<span data-ttu-id="ca386-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca386-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca386-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ca386-127">Request body</span></span>
<span data-ttu-id="ca386-128">В теле запроса добавьте представление объекта windows10TeamGeneralConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca386-128">In the request body, supply a JSON representation for the windows10TeamGeneralConfiguration object.</span></span>

<span data-ttu-id="ca386-129">Ниже показаны свойства, которые необходимо указывать при создании объекта windows10TeamGeneralConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ca386-129">The following table shows the properties that are required when you create the windows10TeamGeneralConfiguration.</span></span>

|<span data-ttu-id="ca386-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca386-130">Property</span></span>|<span data-ttu-id="ca386-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ca386-131">Type</span></span>|<span data-ttu-id="ca386-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ca386-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca386-133">id</span><span class="sxs-lookup"><span data-stu-id="ca386-133">id</span></span>|<span data-ttu-id="ca386-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ca386-134">String</span></span>|<span data-ttu-id="ca386-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ca386-135">Key of the entity.</span></span> <span data-ttu-id="ca386-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca386-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca386-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ca386-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ca386-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca386-138">DateTimeOffset</span></span>|<span data-ttu-id="ca386-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ca386-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ca386-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca386-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca386-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca386-141">roleScopeTagIds</span></span>|<span data-ttu-id="ca386-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ca386-142">String collection</span></span>|<span data-ttu-id="ca386-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ca386-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ca386-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca386-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca386-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ca386-145">supportsScopeTags</span></span>|<span data-ttu-id="ca386-146">Логический</span><span class="sxs-lookup"><span data-stu-id="ca386-146">Boolean</span></span>|<span data-ttu-id="ca386-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="ca386-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ca386-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="ca386-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ca386-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="ca386-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ca386-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca386-150">This property is read-only.</span></span> <span data-ttu-id="ca386-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca386-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca386-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca386-152">createdDateTime</span></span>|<span data-ttu-id="ca386-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca386-153">DateTimeOffset</span></span>|<span data-ttu-id="ca386-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ca386-154">DateTime the object was created.</span></span> <span data-ttu-id="ca386-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca386-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca386-156">описание</span><span class="sxs-lookup"><span data-stu-id="ca386-156">description</span></span>|<span data-ttu-id="ca386-157">Строка</span><span class="sxs-lookup"><span data-stu-id="ca386-157">String</span></span>|<span data-ttu-id="ca386-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ca386-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ca386-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca386-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca386-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ca386-160">displayName</span></span>|<span data-ttu-id="ca386-161">Строка</span><span class="sxs-lookup"><span data-stu-id="ca386-161">String</span></span>|<span data-ttu-id="ca386-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ca386-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ca386-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca386-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca386-164">version</span><span class="sxs-lookup"><span data-stu-id="ca386-164">version</span></span>|<span data-ttu-id="ca386-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ca386-165">Int32</span></span>|<span data-ttu-id="ca386-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ca386-166">Version of the device configuration.</span></span> <span data-ttu-id="ca386-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ca386-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ca386-168">azureOperationalInsightsBlockTelemetry</span><span class="sxs-lookup"><span data-stu-id="ca386-168">azureOperationalInsightsBlockTelemetry</span></span>|<span data-ttu-id="ca386-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca386-169">Boolean</span></span>|<span data-ttu-id="ca386-170">Указывает, следует ли заблокировать оперативную аналитику Azure.</span><span class="sxs-lookup"><span data-stu-id="ca386-170">Indicates whether or not to Block Azure Operational Insights.</span></span>|
|<span data-ttu-id="ca386-171">azureOperationalInsightsWorkspaceId</span><span class="sxs-lookup"><span data-stu-id="ca386-171">azureOperationalInsightsWorkspaceId</span></span>|<span data-ttu-id="ca386-172">String</span><span class="sxs-lookup"><span data-stu-id="ca386-172">String</span></span>|<span data-ttu-id="ca386-173">Идентификатор рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="ca386-173">The Azure Operational Insights workspace id.</span></span>|
|<span data-ttu-id="ca386-174">azureOperationalInsightsWorkspaceKey</span><span class="sxs-lookup"><span data-stu-id="ca386-174">azureOperationalInsightsWorkspaceKey</span></span>|<span data-ttu-id="ca386-175">String</span><span class="sxs-lookup"><span data-stu-id="ca386-175">String</span></span>|<span data-ttu-id="ca386-176">Ключ рабочей области оперативной аналитики Azure.</span><span class="sxs-lookup"><span data-stu-id="ca386-176">The Azure Operational Insights Workspace key.</span></span>|
|<span data-ttu-id="ca386-177">connectAppBlockAutoLaunch</span><span class="sxs-lookup"><span data-stu-id="ca386-177">connectAppBlockAutoLaunch</span></span>|<span data-ttu-id="ca386-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca386-178">Boolean</span></span>|<span data-ttu-id="ca386-179">Указывает, следует ли автоматически запускать приложение Connect, когда начинается проекция.</span><span class="sxs-lookup"><span data-stu-id="ca386-179">Specifies whether to automatically launch the Connect app whenever a projection is initiated.</span></span>|
|<span data-ttu-id="ca386-180">maintenanceWindowBlocked</span><span class="sxs-lookup"><span data-stu-id="ca386-180">maintenanceWindowBlocked</span></span>|<span data-ttu-id="ca386-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca386-181">Boolean</span></span>|<span data-ttu-id="ca386-182">Указывает, следует ли запретить устанавливать период обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="ca386-182">Indicates whether or not to Block setting a maintenance window for device updates.</span></span>|
|<span data-ttu-id="ca386-183">maintenanceWindowDurationInHours</span><span class="sxs-lookup"><span data-stu-id="ca386-183">maintenanceWindowDurationInHours</span></span>|<span data-ttu-id="ca386-184">Int32</span><span class="sxs-lookup"><span data-stu-id="ca386-184">Int32</span></span>|<span data-ttu-id="ca386-185">Длительность периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="ca386-185">Maintenance window duration for device updates.</span></span> <span data-ttu-id="ca386-186">Допустимые значения: от 0 до 5</span><span class="sxs-lookup"><span data-stu-id="ca386-186">Valid values 0 to 5</span></span>|
|<span data-ttu-id="ca386-187">maintenanceWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="ca386-187">maintenanceWindowStartTime</span></span>|<span data-ttu-id="ca386-188">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="ca386-188">TimeOfDay</span></span>|<span data-ttu-id="ca386-189">Начало периода обслуживания для обновлений устройства.</span><span class="sxs-lookup"><span data-stu-id="ca386-189">Maintenance window start time for device updates.</span></span>|
|<span data-ttu-id="ca386-190">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="ca386-190">miracastChannel</span></span>|[<span data-ttu-id="ca386-191">miracastChannel</span><span class="sxs-lookup"><span data-stu-id="ca386-191">miracastChannel</span></span>](../resources/intune-deviceconfig-miracastchannel.md)|<span data-ttu-id="ca386-192">Канал.</span><span class="sxs-lookup"><span data-stu-id="ca386-192">The channel.</span></span> <span data-ttu-id="ca386-193">Возможные значения: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span><span class="sxs-lookup"><span data-stu-id="ca386-193">Possible values are: `userDefined`, `one`, `two`, `three`, `four`, `five`, `six`, `seven`, `eight`, `nine`, `ten`, `eleven`, `thirtySix`, `forty`, `fortyFour`, `fortyEight`, `oneHundredFortyNine`, `oneHundredFiftyThree`, `oneHundredFiftySeven`, `oneHundredSixtyOne`, `oneHundredSixtyFive`.</span></span>|
|<span data-ttu-id="ca386-194">miracastBlocked</span><span class="sxs-lookup"><span data-stu-id="ca386-194">miracastBlocked</span></span>|<span data-ttu-id="ca386-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca386-195">Boolean</span></span>|<span data-ttu-id="ca386-196">Указывает, следует ли заблокировать беспроводное проецирование.</span><span class="sxs-lookup"><span data-stu-id="ca386-196">Indicates whether or not to Block wireless projection.</span></span>|
|<span data-ttu-id="ca386-197">miracastRequirePin</span><span class="sxs-lookup"><span data-stu-id="ca386-197">miracastRequirePin</span></span>|<span data-ttu-id="ca386-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca386-198">Boolean</span></span>|<span data-ttu-id="ca386-199">Указывает, обязательно ли использовать ПИН-код для беспроводного проецирования.</span><span class="sxs-lookup"><span data-stu-id="ca386-199">Indicates whether or not to require a pin for wireless projection.</span></span>|
|<span data-ttu-id="ca386-200">settingsBlockMyMeetingsAndFiles</span><span class="sxs-lookup"><span data-stu-id="ca386-200">settingsBlockMyMeetingsAndFiles</span></span>|<span data-ttu-id="ca386-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca386-201">Boolean</span></span>|<span data-ttu-id="ca386-202">Указывает, следует ли отключить функцию "Мои встречи и файлы" в меню "Пуск", которая показывает собрания и файлы вошедшего пользователя из Office 365.</span><span class="sxs-lookup"><span data-stu-id="ca386-202">Specifies whether to disable the "My meetings and files" feature in the Start menu, which shows the signed-in user's meetings and files from Office 365.</span></span>|
|<span data-ttu-id="ca386-203">settingsBlockSessionResume</span><span class="sxs-lookup"><span data-stu-id="ca386-203">settingsBlockSessionResume</span></span>|<span data-ttu-id="ca386-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca386-204">Boolean</span></span>|<span data-ttu-id="ca386-205">Указывает, следует ли разрешить возобновление сеанса после истечения времени.</span><span class="sxs-lookup"><span data-stu-id="ca386-205">Specifies whether to allow the ability to resume a session when the session times out.</span></span>|
|<span data-ttu-id="ca386-206">settingsBlockSigninSuggestions</span><span class="sxs-lookup"><span data-stu-id="ca386-206">settingsBlockSigninSuggestions</span></span>|<span data-ttu-id="ca386-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca386-207">Boolean</span></span>|<span data-ttu-id="ca386-208">Указывает, следует ли отключить автоматическое добавление в диалоговое окно входа приглашенных из запланированных собраний.</span><span class="sxs-lookup"><span data-stu-id="ca386-208">Specifies whether to disable auto-populating of the sign-in dialog with invitees from scheduled meetings.</span></span>|
|<span data-ttu-id="ca386-209">settingsDefaultVolume</span><span class="sxs-lookup"><span data-stu-id="ca386-209">settingsDefaultVolume</span></span>|<span data-ttu-id="ca386-210">Int32</span><span class="sxs-lookup"><span data-stu-id="ca386-210">Int32</span></span>|<span data-ttu-id="ca386-211">Задает объем нового сеанса по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ca386-211">Specifies the default volume value for a new session.</span></span> <span data-ttu-id="ca386-212">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="ca386-212">Permitted values are 0-100.</span></span> <span data-ttu-id="ca386-213">Значение по умолчанию — 45.</span><span class="sxs-lookup"><span data-stu-id="ca386-213">The default is 45.</span></span> <span data-ttu-id="ca386-214">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="ca386-214">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ca386-215">settingsScreenTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="ca386-215">settingsScreenTimeoutInMinutes</span></span>|<span data-ttu-id="ca386-216">Int32</span><span class="sxs-lookup"><span data-stu-id="ca386-216">Int32</span></span>|<span data-ttu-id="ca386-217">Определяет время до отключения экрана Центра (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ca386-217">Specifies the number of minutes until the Hub screen turns off.</span></span>|
|<span data-ttu-id="ca386-218">settingsSessionTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="ca386-218">settingsSessionTimeoutInMinutes</span></span>|<span data-ttu-id="ca386-219">Int32</span><span class="sxs-lookup"><span data-stu-id="ca386-219">Int32</span></span>|<span data-ttu-id="ca386-220">Определяет время до истечения времени сеанса (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ca386-220">Specifies the number of minutes until the session times out.</span></span>|
|<span data-ttu-id="ca386-221">settingsSleepTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="ca386-221">settingsSleepTimeoutInMinutes</span></span>|<span data-ttu-id="ca386-222">Int32</span><span class="sxs-lookup"><span data-stu-id="ca386-222">Int32</span></span>|<span data-ttu-id="ca386-223">Определяет время до перехода Центра в спящий режим (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ca386-223">Specifies the number of minutes until the Hub enters sleep mode.</span></span>|
|<span data-ttu-id="ca386-224">welcomeScreenBlockAutomaticWakeUp</span><span class="sxs-lookup"><span data-stu-id="ca386-224">welcomeScreenBlockAutomaticWakeUp</span></span>|<span data-ttu-id="ca386-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca386-225">Boolean</span></span>|<span data-ttu-id="ca386-226">Указывает, следует ли заблокировать автоматический вывод экрана приветствия из спящего режима, когда кто-то входит в комнату.</span><span class="sxs-lookup"><span data-stu-id="ca386-226">Indicates whether or not to Block the welcome screen from waking up automatically when someone enters the room.</span></span>|
|<span data-ttu-id="ca386-227">welcomeScreenBackgroundImageUrl</span><span class="sxs-lookup"><span data-stu-id="ca386-227">welcomeScreenBackgroundImageUrl</span></span>|<span data-ttu-id="ca386-228">String</span><span class="sxs-lookup"><span data-stu-id="ca386-228">String</span></span>|<span data-ttu-id="ca386-229">URL-адрес фонового изображения экрана приветствия.</span><span class="sxs-lookup"><span data-stu-id="ca386-229">The welcome screen background image URL.</span></span> <span data-ttu-id="ca386-230">URL-адрес должен начинаться с протокола HTTPS и возвращать PNG-изображение.</span><span class="sxs-lookup"><span data-stu-id="ca386-230">The URL must use the HTTPS protocol and return a PNG image.</span></span>|
|<span data-ttu-id="ca386-231">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="ca386-231">welcomeScreenMeetingInformation</span></span>|[<span data-ttu-id="ca386-232">welcomeScreenMeetingInformation</span><span class="sxs-lookup"><span data-stu-id="ca386-232">welcomeScreenMeetingInformation</span></span>](../resources/intune-deviceconfig-welcomescreenmeetinginformation.md)|<span data-ttu-id="ca386-233">Информация о собраниях, показываемая на экране приветствия.</span><span class="sxs-lookup"><span data-stu-id="ca386-233">The welcome screen meeting information shown.</span></span> <span data-ttu-id="ca386-234">Возможные значения: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span><span class="sxs-lookup"><span data-stu-id="ca386-234">Possible values are: `userDefined`, `showOrganizerAndTimeOnly`, `showOrganizerAndTimeAndSubject`.</span></span>|



## <a name="response"></a><span data-ttu-id="ca386-235">Отклик</span><span class="sxs-lookup"><span data-stu-id="ca386-235">Response</span></span>
<span data-ttu-id="ca386-236">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ca386-236">If successful, this method returns a `201 Created` response code and a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca386-237">Пример</span><span class="sxs-lookup"><span data-stu-id="ca386-237">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca386-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="ca386-238">Request</span></span>
<span data-ttu-id="ca386-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ca386-239">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ca386-240">Ответ</span><span class="sxs-lookup"><span data-stu-id="ca386-240">Response</span></span>
<span data-ttu-id="ca386-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ca386-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





