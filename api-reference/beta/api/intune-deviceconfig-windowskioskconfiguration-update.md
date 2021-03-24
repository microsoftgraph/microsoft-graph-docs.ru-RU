---
title: Обновление windowsKioskConfiguration
description: Обновление свойств объекта WindowsKioskConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 653511dcb6782b953e985a2bacb24f891ffda51f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132361"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="9e857-103">Обновление windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e857-103">Update windowsKioskConfiguration</span></span>

<span data-ttu-id="9e857-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e857-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e857-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e857-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e857-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9e857-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e857-107">Обновление свойств объекта [WindowsKioskConfiguration.](../resources/intune-deviceconfig-windowskioskconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e857-107">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e857-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9e857-108">Prerequisites</span></span>
<span data-ttu-id="9e857-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e857-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e857-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e857-111">Permission type</span></span>|<span data-ttu-id="9e857-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e857-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e857-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e857-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e857-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e857-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e857-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e857-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e857-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e857-116">Not supported.</span></span>|
|<span data-ttu-id="9e857-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9e857-117">Application</span></span>|<span data-ttu-id="9e857-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e857-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e857-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e857-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9e857-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9e857-120">Request headers</span></span>
|<span data-ttu-id="9e857-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9e857-121">Header</span></span>|<span data-ttu-id="9e857-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9e857-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e857-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e857-123">Authorization</span></span>|<span data-ttu-id="9e857-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e857-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e857-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9e857-125">Accept</span></span>|<span data-ttu-id="9e857-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e857-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e857-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e857-127">Request body</span></span>
<span data-ttu-id="9e857-128">В теле запроса предоставляем представление JSON для [объекта WindowsKioskConfiguration.](../resources/intune-deviceconfig-windowskioskconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e857-128">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="9e857-129">В следующей таблице показаны свойства, необходимые при создании [windowsKioskConfiguration.](../resources/intune-deviceconfig-windowskioskconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e857-129">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="9e857-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e857-130">Property</span></span>|<span data-ttu-id="9e857-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9e857-131">Type</span></span>|<span data-ttu-id="9e857-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9e857-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e857-133">id</span><span class="sxs-lookup"><span data-stu-id="9e857-133">id</span></span>|<span data-ttu-id="9e857-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9e857-134">String</span></span>|<span data-ttu-id="9e857-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9e857-135">Key of the entity.</span></span> <span data-ttu-id="9e857-136">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e857-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e857-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e857-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9e857-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e857-138">DateTimeOffset</span></span>|<span data-ttu-id="9e857-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9e857-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9e857-140">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e857-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e857-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e857-141">roleScopeTagIds</span></span>|<span data-ttu-id="9e857-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9e857-142">String collection</span></span>|<span data-ttu-id="9e857-143">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="9e857-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9e857-144">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e857-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e857-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9e857-145">supportsScopeTags</span></span>|<span data-ttu-id="9e857-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e857-146">Boolean</span></span>|<span data-ttu-id="9e857-147">Указывает, поддерживает ли вся конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="9e857-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9e857-148">Назначение свойства ScopeTags не допускается, если это значение является ложным и объекты не будут видны пользователям с охватом.</span><span class="sxs-lookup"><span data-stu-id="9e857-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9e857-149">Это происходит для политик Legacy, созданных в Silverlight, и их можно разрешить путем удаления и воссоздания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="9e857-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9e857-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e857-150">This property is read-only.</span></span> <span data-ttu-id="9e857-151">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e857-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e857-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9e857-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9e857-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9e857-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9e857-154">Применимость к выпуску ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9e857-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9e857-155">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e857-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e857-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9e857-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9e857-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9e857-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9e857-158">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9e857-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9e857-159">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e857-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e857-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9e857-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9e857-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="9e857-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9e857-162">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="9e857-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9e857-163">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e857-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e857-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e857-164">createdDateTime</span></span>|<span data-ttu-id="9e857-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e857-165">DateTimeOffset</span></span>|<span data-ttu-id="9e857-166">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9e857-166">DateTime the object was created.</span></span> <span data-ttu-id="9e857-167">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e857-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e857-168">description</span><span class="sxs-lookup"><span data-stu-id="9e857-168">description</span></span>|<span data-ttu-id="9e857-169">Строка</span><span class="sxs-lookup"><span data-stu-id="9e857-169">String</span></span>|<span data-ttu-id="9e857-170">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9e857-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9e857-171">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e857-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e857-172">displayName</span><span class="sxs-lookup"><span data-stu-id="9e857-172">displayName</span></span>|<span data-ttu-id="9e857-173">Строка</span><span class="sxs-lookup"><span data-stu-id="9e857-173">String</span></span>|<span data-ttu-id="9e857-174">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9e857-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9e857-175">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e857-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e857-176">version</span><span class="sxs-lookup"><span data-stu-id="9e857-176">version</span></span>|<span data-ttu-id="9e857-177">Int32</span><span class="sxs-lookup"><span data-stu-id="9e857-177">Int32</span></span>|<span data-ttu-id="9e857-178">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9e857-178">Version of the device configuration.</span></span> <span data-ttu-id="9e857-179">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9e857-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e857-180">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="9e857-180">kioskProfiles</span></span>|<span data-ttu-id="9e857-181">[коллекция windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9e857-181">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="9e857-182">Этот параметр политики позволяет определить список профилей киоска для конфигурации киоска.</span><span class="sxs-lookup"><span data-stu-id="9e857-182">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="9e857-183">Эта коллекция может содержать не более 3 элементов.</span><span class="sxs-lookup"><span data-stu-id="9e857-183">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="9e857-184">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="9e857-184">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="9e857-185">Строка</span><span class="sxs-lookup"><span data-stu-id="9e857-185">String</span></span>|<span data-ttu-id="9e857-186">Укажите URL-адрес по умолчанию, в который браузер должен перейти при запуске.</span><span class="sxs-lookup"><span data-stu-id="9e857-186">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="9e857-187">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="9e857-187">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="9e857-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e857-188">Boolean</span></span>|<span data-ttu-id="9e857-189">Включить домашняя кнопка браузера киоска.</span><span class="sxs-lookup"><span data-stu-id="9e857-189">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="9e857-190">По умолчанию кнопка home отключена.</span><span class="sxs-lookup"><span data-stu-id="9e857-190">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="9e857-191">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="9e857-191">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="9e857-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e857-192">Boolean</span></span>|<span data-ttu-id="9e857-193">Включить кнопки навигации браузера киоска (вперед/назад).</span><span class="sxs-lookup"><span data-stu-id="9e857-193">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="9e857-194">По умолчанию отключены кнопки навигации.</span><span class="sxs-lookup"><span data-stu-id="9e857-194">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="9e857-195">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="9e857-195">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="9e857-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e857-196">Boolean</span></span>|<span data-ttu-id="9e857-197">Включить кнопку окончания сеанса браузера киоска.</span><span class="sxs-lookup"><span data-stu-id="9e857-197">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="9e857-198">По умолчанию отключена кнопка окончания сеанса.</span><span class="sxs-lookup"><span data-stu-id="9e857-198">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="9e857-199">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="9e857-199">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="9e857-200">Int32</span><span class="sxs-lookup"><span data-stu-id="9e857-200">Int32</span></span>|<span data-ttu-id="9e857-201">Укажите количество минут ожидания сеанса, пока браузер киоска не перезапустится в свежем состоянии.</span><span class="sxs-lookup"><span data-stu-id="9e857-201">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="9e857-202">Допустимые значения : 1-1440.</span><span class="sxs-lookup"><span data-stu-id="9e857-202">Valid values are 1-1440.</span></span> <span data-ttu-id="9e857-203">Допустимые значения от 1 до 1440</span><span class="sxs-lookup"><span data-stu-id="9e857-203">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="9e857-204">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="9e857-204">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="9e857-205">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9e857-205">String collection</span></span>|<span data-ttu-id="9e857-206">Укажите URL-адреса, в которые браузеры киосков не должны переходить</span><span class="sxs-lookup"><span data-stu-id="9e857-206">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="9e857-207">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="9e857-207">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="9e857-208">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9e857-208">String collection</span></span>|<span data-ttu-id="9e857-209">Укажите URL-адреса, в которые браузеру киоска разрешено перемещаться</span><span class="sxs-lookup"><span data-stu-id="9e857-209">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="9e857-210">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="9e857-210">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="9e857-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e857-211">Boolean</span></span>|<span data-ttu-id="9e857-212">Включить общедоступный режим просмотра киоска для браузера Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="9e857-212">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="9e857-213">Значение По умолчанию является ложным.</span><span class="sxs-lookup"><span data-stu-id="9e857-213">The Default is false.</span></span>|
|<span data-ttu-id="9e857-214">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="9e857-214">windowsKioskForceUpdateSchedule</span></span>|[<span data-ttu-id="9e857-215">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="9e857-215">windowsKioskForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windowskioskforceupdateschedule.md)|<span data-ttu-id="9e857-216">расписание принудительного обновления для устройств Киоска.</span><span class="sxs-lookup"><span data-stu-id="9e857-216">force update schedule for Kiosk devices.</span></span>|



## <a name="response"></a><span data-ttu-id="9e857-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e857-217">Response</span></span>
<span data-ttu-id="9e857-218">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9e857-218">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e857-219">Пример</span><span class="sxs-lookup"><span data-stu-id="9e857-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e857-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e857-220">Request</span></span>
<span data-ttu-id="9e857-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e857-221">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9e857-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e857-222">Response</span></span>
<span data-ttu-id="9e857-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e857-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




