---
title: Обновление Виндовскиоскконфигуратион
description: Обновление свойств объекта Виндовскиоскконфигуратион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 110bc99ab677c940adc35b5266b1b34323d3748d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42475574"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="03f2e-103">Обновление Виндовскиоскконфигуратион</span><span class="sxs-lookup"><span data-stu-id="03f2e-103">Update windowsKioskConfiguration</span></span>

<span data-ttu-id="03f2e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="03f2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03f2e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03f2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03f2e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03f2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03f2e-107">Обновление свойств объекта [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="03f2e-107">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03f2e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="03f2e-108">Prerequisites</span></span>
<span data-ttu-id="03f2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03f2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03f2e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03f2e-111">Permission type</span></span>|<span data-ttu-id="03f2e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03f2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03f2e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03f2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03f2e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03f2e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03f2e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03f2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03f2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03f2e-116">Not supported.</span></span>|
|<span data-ttu-id="03f2e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03f2e-117">Application</span></span>|<span data-ttu-id="03f2e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03f2e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03f2e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03f2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="03f2e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="03f2e-120">Request headers</span></span>
|<span data-ttu-id="03f2e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03f2e-121">Header</span></span>|<span data-ttu-id="03f2e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="03f2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03f2e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03f2e-123">Authorization</span></span>|<span data-ttu-id="03f2e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03f2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03f2e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="03f2e-125">Accept</span></span>|<span data-ttu-id="03f2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03f2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03f2e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03f2e-127">Request body</span></span>
<span data-ttu-id="03f2e-128">В тексте запроса добавьте представление объекта [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03f2e-128">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="03f2e-129">В следующей таблице приведены свойства, необходимые при создании [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03f2e-129">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="03f2e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="03f2e-130">Property</span></span>|<span data-ttu-id="03f2e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="03f2e-131">Type</span></span>|<span data-ttu-id="03f2e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="03f2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03f2e-133">id</span><span class="sxs-lookup"><span data-stu-id="03f2e-133">id</span></span>|<span data-ttu-id="03f2e-134">String</span><span class="sxs-lookup"><span data-stu-id="03f2e-134">String</span></span>|<span data-ttu-id="03f2e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="03f2e-135">Key of the entity.</span></span> <span data-ttu-id="03f2e-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03f2e-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03f2e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03f2e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="03f2e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03f2e-138">DateTimeOffset</span></span>|<span data-ttu-id="03f2e-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="03f2e-139">DateTime the object was last modified.</span></span> <span data-ttu-id="03f2e-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03f2e-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03f2e-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="03f2e-141">roleScopeTagIds</span></span>|<span data-ttu-id="03f2e-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="03f2e-142">String collection</span></span>|<span data-ttu-id="03f2e-143">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="03f2e-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="03f2e-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03f2e-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03f2e-145">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="03f2e-145">supportsScopeTags</span></span>|<span data-ttu-id="03f2e-146">Логический</span><span class="sxs-lookup"><span data-stu-id="03f2e-146">Boolean</span></span>|<span data-ttu-id="03f2e-147">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="03f2e-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="03f2e-148">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="03f2e-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="03f2e-149">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="03f2e-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="03f2e-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="03f2e-150">This property is read-only.</span></span> <span data-ttu-id="03f2e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03f2e-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03f2e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="03f2e-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="03f2e-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="03f2e-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="03f2e-154">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="03f2e-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="03f2e-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03f2e-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03f2e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="03f2e-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="03f2e-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="03f2e-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="03f2e-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="03f2e-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="03f2e-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03f2e-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03f2e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="03f2e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="03f2e-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="03f2e-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="03f2e-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="03f2e-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="03f2e-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03f2e-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03f2e-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03f2e-164">createdDateTime</span></span>|<span data-ttu-id="03f2e-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03f2e-165">DateTimeOffset</span></span>|<span data-ttu-id="03f2e-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="03f2e-166">DateTime the object was created.</span></span> <span data-ttu-id="03f2e-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03f2e-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03f2e-168">description</span><span class="sxs-lookup"><span data-stu-id="03f2e-168">description</span></span>|<span data-ttu-id="03f2e-169">String</span><span class="sxs-lookup"><span data-stu-id="03f2e-169">String</span></span>|<span data-ttu-id="03f2e-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03f2e-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="03f2e-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03f2e-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03f2e-172">displayName</span><span class="sxs-lookup"><span data-stu-id="03f2e-172">displayName</span></span>|<span data-ttu-id="03f2e-173">Строка</span><span class="sxs-lookup"><span data-stu-id="03f2e-173">String</span></span>|<span data-ttu-id="03f2e-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03f2e-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="03f2e-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03f2e-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03f2e-176">version</span><span class="sxs-lookup"><span data-stu-id="03f2e-176">version</span></span>|<span data-ttu-id="03f2e-177">Int32</span><span class="sxs-lookup"><span data-stu-id="03f2e-177">Int32</span></span>|<span data-ttu-id="03f2e-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="03f2e-178">Version of the device configuration.</span></span> <span data-ttu-id="03f2e-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="03f2e-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="03f2e-180">киоскпрофилес</span><span class="sxs-lookup"><span data-stu-id="03f2e-180">kioskProfiles</span></span>|<span data-ttu-id="03f2e-181">Коллекция [виндовскиоскпрофиле](../resources/intune-deviceconfig-windowskioskprofile.md)</span><span class="sxs-lookup"><span data-stu-id="03f2e-181">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="03f2e-182">Этот параметр политики позволяет определить список профилей киоска для конфигурации киоска.</span><span class="sxs-lookup"><span data-stu-id="03f2e-182">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="03f2e-183">Эта коллекция может содержать не более 3 элементов.</span><span class="sxs-lookup"><span data-stu-id="03f2e-183">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="03f2e-184">киоскбровсердефаултурл</span><span class="sxs-lookup"><span data-stu-id="03f2e-184">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="03f2e-185">String</span><span class="sxs-lookup"><span data-stu-id="03f2e-185">String</span></span>|<span data-ttu-id="03f2e-186">Укажите URL-адрес по умолчанию, на который должен переходить браузер при запуске.</span><span class="sxs-lookup"><span data-stu-id="03f2e-186">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="03f2e-187">киоскбровсеренаблехомебуттон</span><span class="sxs-lookup"><span data-stu-id="03f2e-187">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="03f2e-188">Логический</span><span class="sxs-lookup"><span data-stu-id="03f2e-188">Boolean</span></span>|<span data-ttu-id="03f2e-189">Включите кнопку Главная в браузере киоска.</span><span class="sxs-lookup"><span data-stu-id="03f2e-189">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="03f2e-190">По умолчанию кнопка "домой" отключена.</span><span class="sxs-lookup"><span data-stu-id="03f2e-190">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="03f2e-191">киоскбровсеренабленавигатионбуттонс</span><span class="sxs-lookup"><span data-stu-id="03f2e-191">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="03f2e-192">Логический</span><span class="sxs-lookup"><span data-stu-id="03f2e-192">Boolean</span></span>|<span data-ttu-id="03f2e-193">Включение кнопок навигации в браузере киосков (вперед и назад).</span><span class="sxs-lookup"><span data-stu-id="03f2e-193">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="03f2e-194">По умолчанию кнопки навигации отключены.</span><span class="sxs-lookup"><span data-stu-id="03f2e-194">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="03f2e-195">киоскбровсеренаблиндсессионбуттон</span><span class="sxs-lookup"><span data-stu-id="03f2e-195">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="03f2e-196">Логический</span><span class="sxs-lookup"><span data-stu-id="03f2e-196">Boolean</span></span>|<span data-ttu-id="03f2e-197">Включите кнопку End Session (завершить сеанс) в обозревателе киосков.</span><span class="sxs-lookup"><span data-stu-id="03f2e-197">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="03f2e-198">По умолчанию кнопка End Session отключена.</span><span class="sxs-lookup"><span data-stu-id="03f2e-198">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="03f2e-199">киоскбровсеррестартонидлетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="03f2e-199">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="03f2e-200">Int32</span><span class="sxs-lookup"><span data-stu-id="03f2e-200">Int32</span></span>|<span data-ttu-id="03f2e-201">Укажите время в минутах, в течение которого сеанс простаивает до тех пор, пока обозреватель киоска не перезапустится в обновленном состоянии.</span><span class="sxs-lookup"><span data-stu-id="03f2e-201">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="03f2e-202">Допустимые значения: 1-1440.</span><span class="sxs-lookup"><span data-stu-id="03f2e-202">Valid values are 1-1440.</span></span> <span data-ttu-id="03f2e-203">Допустимые значения — от 1 до 1440</span><span class="sxs-lookup"><span data-stu-id="03f2e-203">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="03f2e-204">киоскбровсерблоккедурлс</span><span class="sxs-lookup"><span data-stu-id="03f2e-204">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="03f2e-205">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="03f2e-205">String collection</span></span>|<span data-ttu-id="03f2e-206">Указание URL-адресов, к которым не должны переходить браузеры киоска</span><span class="sxs-lookup"><span data-stu-id="03f2e-206">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="03f2e-207">киоскбровсерблоккедурлексцептионс</span><span class="sxs-lookup"><span data-stu-id="03f2e-207">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="03f2e-208">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="03f2e-208">String collection</span></span>|<span data-ttu-id="03f2e-209">Указание URL-адресов, на которые может перейти браузер с киоском</span><span class="sxs-lookup"><span data-stu-id="03f2e-209">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="03f2e-210">еджекиоскенаблепубликбровсинг</span><span class="sxs-lookup"><span data-stu-id="03f2e-210">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="03f2e-211">Логический</span><span class="sxs-lookup"><span data-stu-id="03f2e-211">Boolean</span></span>|<span data-ttu-id="03f2e-212">Включение режима "общедоступный" в режиме киоска браузера для браузера Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="03f2e-212">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="03f2e-213">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="03f2e-213">The Default is false.</span></span>|
|<span data-ttu-id="03f2e-214">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="03f2e-214">windowsKioskForceUpdateSchedule</span></span>|[<span data-ttu-id="03f2e-215">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="03f2e-215">windowsKioskForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windowskioskforceupdateschedule.md)|<span data-ttu-id="03f2e-216">принудительное обновление расписания для устройств киоска.</span><span class="sxs-lookup"><span data-stu-id="03f2e-216">force update schedule for Kiosk devices.</span></span>|



## <a name="response"></a><span data-ttu-id="03f2e-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="03f2e-217">Response</span></span>
<span data-ttu-id="03f2e-218">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="03f2e-218">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03f2e-219">Пример</span><span class="sxs-lookup"><span data-stu-id="03f2e-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="03f2e-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="03f2e-220">Request</span></span>
<span data-ttu-id="03f2e-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03f2e-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2829

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
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
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "Profile Id value",
      "profileName": "Profile Name value",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "small",
            "name": "Name value",
            "appType": "store",
            "autoLaunch": true,
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
        "allowAccessToDownloadsFolder": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 6,
  "kioskBrowserBlockedURLs": [
    "Kiosk Browser Blocked URLs value"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "Kiosk Browser Blocked Url Exceptions value"
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "windowsKioskForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "dayofWeek": "monday",
    "dayofMonth": 10,
    "runImmediatelyIfAfterStartDateTime": true
  }
}
```

### <a name="response"></a><span data-ttu-id="03f2e-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="03f2e-222">Response</span></span>
<span data-ttu-id="03f2e-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03f2e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3001

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "id": "146a990b-990b-146a-0b99-6a140b996a14",
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
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "Profile Id value",
      "profileName": "Profile Name value",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "small",
            "name": "Name value",
            "appType": "store",
            "autoLaunch": true,
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
        "allowAccessToDownloadsFolder": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 6,
  "kioskBrowserBlockedURLs": [
    "Kiosk Browser Blocked URLs value"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "Kiosk Browser Blocked Url Exceptions value"
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "windowsKioskForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "dayofWeek": "monday",
    "dayofMonth": 10,
    "runImmediatelyIfAfterStartDateTime": true
  }
}
```





