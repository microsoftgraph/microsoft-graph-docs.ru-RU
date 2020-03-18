---
title: Создание Виндовскиоскконфигуратион
description: Создание нового объекта Виндовскиоскконфигуратион.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f159decfd00f39af2d619613a6419acfdd532494
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42735144"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="71bd9-103">Создание Виндовскиоскконфигуратион</span><span class="sxs-lookup"><span data-stu-id="71bd9-103">Create windowsKioskConfiguration</span></span>

> <span data-ttu-id="71bd9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71bd9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71bd9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71bd9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71bd9-106">Создание нового объекта [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="71bd9-106">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71bd9-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="71bd9-107">Prerequisites</span></span>
<span data-ttu-id="71bd9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71bd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71bd9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71bd9-110">Permission type</span></span>|<span data-ttu-id="71bd9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71bd9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71bd9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71bd9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71bd9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71bd9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71bd9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71bd9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71bd9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71bd9-115">Not supported.</span></span>|
|<span data-ttu-id="71bd9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="71bd9-116">Application</span></span>|<span data-ttu-id="71bd9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71bd9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71bd9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71bd9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="71bd9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="71bd9-119">Request headers</span></span>
|<span data-ttu-id="71bd9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="71bd9-120">Header</span></span>|<span data-ttu-id="71bd9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="71bd9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71bd9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71bd9-122">Authorization</span></span>|<span data-ttu-id="71bd9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71bd9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71bd9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="71bd9-124">Accept</span></span>|<span data-ttu-id="71bd9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71bd9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71bd9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71bd9-126">Request body</span></span>
<span data-ttu-id="71bd9-127">В тексте запроса добавьте представление объекта Виндовскиоскконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71bd9-127">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="71bd9-128">В следующей таблице приведены свойства, необходимые при создании Виндовскиоскконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="71bd9-128">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="71bd9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="71bd9-129">Property</span></span>|<span data-ttu-id="71bd9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="71bd9-130">Type</span></span>|<span data-ttu-id="71bd9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="71bd9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71bd9-132">id</span><span class="sxs-lookup"><span data-stu-id="71bd9-132">id</span></span>|<span data-ttu-id="71bd9-133">String</span><span class="sxs-lookup"><span data-stu-id="71bd9-133">String</span></span>|<span data-ttu-id="71bd9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="71bd9-134">Key of the entity.</span></span> <span data-ttu-id="71bd9-135">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71bd9-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71bd9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71bd9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="71bd9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71bd9-137">DateTimeOffset</span></span>|<span data-ttu-id="71bd9-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="71bd9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="71bd9-139">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71bd9-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71bd9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="71bd9-140">roleScopeTagIds</span></span>|<span data-ttu-id="71bd9-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="71bd9-141">String collection</span></span>|<span data-ttu-id="71bd9-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="71bd9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="71bd9-143">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71bd9-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71bd9-144">суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="71bd9-144">supportsScopeTags</span></span>|<span data-ttu-id="71bd9-145">Логический</span><span class="sxs-lookup"><span data-stu-id="71bd9-145">Boolean</span></span>|<span data-ttu-id="71bd9-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="71bd9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="71bd9-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="71bd9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="71bd9-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="71bd9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="71bd9-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="71bd9-149">This property is read-only.</span></span> <span data-ttu-id="71bd9-150">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71bd9-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71bd9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="71bd9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="71bd9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="71bd9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="71bd9-153">Применимость выпусков ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="71bd9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="71bd9-154">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71bd9-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71bd9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="71bd9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="71bd9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="71bd9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="71bd9-157">Правило применимости версии ОС для этой политики.</span><span class="sxs-lookup"><span data-stu-id="71bd9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="71bd9-158">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71bd9-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71bd9-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="71bd9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="71bd9-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="71bd9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="71bd9-161">Правило применимости режима устройства для этой политики.</span><span class="sxs-lookup"><span data-stu-id="71bd9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="71bd9-162">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71bd9-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71bd9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71bd9-163">createdDateTime</span></span>|<span data-ttu-id="71bd9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71bd9-164">DateTimeOffset</span></span>|<span data-ttu-id="71bd9-165">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="71bd9-165">DateTime the object was created.</span></span> <span data-ttu-id="71bd9-166">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71bd9-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71bd9-167">description</span><span class="sxs-lookup"><span data-stu-id="71bd9-167">description</span></span>|<span data-ttu-id="71bd9-168">String</span><span class="sxs-lookup"><span data-stu-id="71bd9-168">String</span></span>|<span data-ttu-id="71bd9-169">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="71bd9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71bd9-170">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71bd9-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71bd9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="71bd9-171">displayName</span></span>|<span data-ttu-id="71bd9-172">Строка</span><span class="sxs-lookup"><span data-stu-id="71bd9-172">String</span></span>|<span data-ttu-id="71bd9-173">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="71bd9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71bd9-174">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71bd9-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71bd9-175">version</span><span class="sxs-lookup"><span data-stu-id="71bd9-175">version</span></span>|<span data-ttu-id="71bd9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="71bd9-176">Int32</span></span>|<span data-ttu-id="71bd9-177">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="71bd9-177">Version of the device configuration.</span></span> <span data-ttu-id="71bd9-178">Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="71bd9-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71bd9-179">киоскпрофилес</span><span class="sxs-lookup"><span data-stu-id="71bd9-179">kioskProfiles</span></span>|<span data-ttu-id="71bd9-180">Коллекция [виндовскиоскпрофиле](../resources/intune-deviceconfig-windowskioskprofile.md)</span><span class="sxs-lookup"><span data-stu-id="71bd9-180">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="71bd9-181">Этот параметр политики позволяет определить список профилей киоска для конфигурации киоска.</span><span class="sxs-lookup"><span data-stu-id="71bd9-181">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="71bd9-182">Эта коллекция может содержать не более 3 элементов.</span><span class="sxs-lookup"><span data-stu-id="71bd9-182">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="71bd9-183">киоскбровсердефаултурл</span><span class="sxs-lookup"><span data-stu-id="71bd9-183">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="71bd9-184">String</span><span class="sxs-lookup"><span data-stu-id="71bd9-184">String</span></span>|<span data-ttu-id="71bd9-185">Укажите URL-адрес по умолчанию, на который должен переходить браузер при запуске.</span><span class="sxs-lookup"><span data-stu-id="71bd9-185">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="71bd9-186">киоскбровсеренаблехомебуттон</span><span class="sxs-lookup"><span data-stu-id="71bd9-186">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="71bd9-187">Логический</span><span class="sxs-lookup"><span data-stu-id="71bd9-187">Boolean</span></span>|<span data-ttu-id="71bd9-188">Включите кнопку Главная в браузере киоска.</span><span class="sxs-lookup"><span data-stu-id="71bd9-188">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="71bd9-189">По умолчанию кнопка "домой" отключена.</span><span class="sxs-lookup"><span data-stu-id="71bd9-189">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="71bd9-190">киоскбровсеренабленавигатионбуттонс</span><span class="sxs-lookup"><span data-stu-id="71bd9-190">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="71bd9-191">Логический</span><span class="sxs-lookup"><span data-stu-id="71bd9-191">Boolean</span></span>|<span data-ttu-id="71bd9-192">Включение кнопок навигации в браузере киосков (вперед и назад).</span><span class="sxs-lookup"><span data-stu-id="71bd9-192">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="71bd9-193">По умолчанию кнопки навигации отключены.</span><span class="sxs-lookup"><span data-stu-id="71bd9-193">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="71bd9-194">киоскбровсеренаблиндсессионбуттон</span><span class="sxs-lookup"><span data-stu-id="71bd9-194">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="71bd9-195">Логический</span><span class="sxs-lookup"><span data-stu-id="71bd9-195">Boolean</span></span>|<span data-ttu-id="71bd9-196">Включите кнопку End Session (завершить сеанс) в обозревателе киосков.</span><span class="sxs-lookup"><span data-stu-id="71bd9-196">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="71bd9-197">По умолчанию кнопка End Session отключена.</span><span class="sxs-lookup"><span data-stu-id="71bd9-197">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="71bd9-198">киоскбровсеррестартонидлетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="71bd9-198">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="71bd9-199">Int32</span><span class="sxs-lookup"><span data-stu-id="71bd9-199">Int32</span></span>|<span data-ttu-id="71bd9-200">Укажите время в минутах, в течение которого сеанс простаивает до тех пор, пока обозреватель киоска не перезапустится в обновленном состоянии.</span><span class="sxs-lookup"><span data-stu-id="71bd9-200">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="71bd9-201">Допустимые значения: 1-1440.</span><span class="sxs-lookup"><span data-stu-id="71bd9-201">Valid values are 1-1440.</span></span> <span data-ttu-id="71bd9-202">Допустимые значения — от 1 до 1440</span><span class="sxs-lookup"><span data-stu-id="71bd9-202">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="71bd9-203">киоскбровсерблоккедурлс</span><span class="sxs-lookup"><span data-stu-id="71bd9-203">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="71bd9-204">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="71bd9-204">String collection</span></span>|<span data-ttu-id="71bd9-205">Указание URL-адресов, к которым не должны переходить браузеры киоска</span><span class="sxs-lookup"><span data-stu-id="71bd9-205">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="71bd9-206">киоскбровсерблоккедурлексцептионс</span><span class="sxs-lookup"><span data-stu-id="71bd9-206">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="71bd9-207">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="71bd9-207">String collection</span></span>|<span data-ttu-id="71bd9-208">Указание URL-адресов, на которые может перейти браузер с киоском</span><span class="sxs-lookup"><span data-stu-id="71bd9-208">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="71bd9-209">еджекиоскенаблепубликбровсинг</span><span class="sxs-lookup"><span data-stu-id="71bd9-209">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="71bd9-210">Логический</span><span class="sxs-lookup"><span data-stu-id="71bd9-210">Boolean</span></span>|<span data-ttu-id="71bd9-211">Включение режима "общедоступный" в режиме киоска браузера для браузера Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="71bd9-211">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="71bd9-212">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="71bd9-212">The Default is false.</span></span>|
|<span data-ttu-id="71bd9-213">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="71bd9-213">windowsKioskForceUpdateSchedule</span></span>|[<span data-ttu-id="71bd9-214">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="71bd9-214">windowsKioskForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windowskioskforceupdateschedule.md)|<span data-ttu-id="71bd9-215">принудительное обновление расписания для устройств киоска.</span><span class="sxs-lookup"><span data-stu-id="71bd9-215">force update schedule for Kiosk devices.</span></span>|



## <a name="response"></a><span data-ttu-id="71bd9-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="71bd9-216">Response</span></span>
<span data-ttu-id="71bd9-217">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="71bd9-217">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71bd9-218">Пример</span><span class="sxs-lookup"><span data-stu-id="71bd9-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="71bd9-219">Запрос</span><span class="sxs-lookup"><span data-stu-id="71bd9-219">Request</span></span>
<span data-ttu-id="71bd9-220">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71bd9-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="71bd9-221">Отклик</span><span class="sxs-lookup"><span data-stu-id="71bd9-221">Response</span></span>
<span data-ttu-id="71bd9-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71bd9-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




