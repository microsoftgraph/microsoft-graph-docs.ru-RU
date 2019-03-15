---
title: Обновление Виндовскиоскконфигуратион
description: Обновление свойств объекта Виндовскиоскконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b25f28e9ea87af0c6b6366fe43324c46114c0c5e
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571580"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="c577c-103">Обновление Виндовскиоскконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c577c-103">Update windowsKioskConfiguration</span></span>

> <span data-ttu-id="c577c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c577c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c577c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c577c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c577c-106">Обновление свойств объекта [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c577c-106">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c577c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c577c-107">Prerequisites</span></span>
<span data-ttu-id="c577c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c577c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c577c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c577c-110">Permission type</span></span>|<span data-ttu-id="c577c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c577c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c577c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c577c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c577c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c577c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c577c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c577c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c577c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c577c-115">Not supported.</span></span>|
|<span data-ttu-id="c577c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c577c-116">Application</span></span>|<span data-ttu-id="c577c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c577c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c577c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c577c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c577c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c577c-119">Request headers</span></span>
|<span data-ttu-id="c577c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c577c-120">Header</span></span>|<span data-ttu-id="c577c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c577c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c577c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c577c-122">Authorization</span></span>|<span data-ttu-id="c577c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c577c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c577c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c577c-124">Accept</span></span>|<span data-ttu-id="c577c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c577c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c577c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c577c-126">Request body</span></span>
<span data-ttu-id="c577c-127">В тексте запроса добавьте представление объекта [Виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c577c-127">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="c577c-128">В следующей таблице приведены свойства, необходимые при создании [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c577c-128">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="c577c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c577c-129">Property</span></span>|<span data-ttu-id="c577c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c577c-130">Type</span></span>|<span data-ttu-id="c577c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c577c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c577c-132">id</span><span class="sxs-lookup"><span data-stu-id="c577c-132">id</span></span>|<span data-ttu-id="c577c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c577c-133">String</span></span>|<span data-ttu-id="c577c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c577c-134">Key of the entity.</span></span> <span data-ttu-id="c577c-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c577c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c577c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c577c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c577c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c577c-137">DateTimeOffset</span></span>|<span data-ttu-id="c577c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="c577c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c577c-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c577c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c577c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c577c-140">roleScopeTagIds</span></span>|<span data-ttu-id="c577c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c577c-141">String collection</span></span>|<span data-ttu-id="c577c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="c577c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c577c-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c577c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c577c-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="c577c-144">supportsScopeTags</span></span>|<span data-ttu-id="c577c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c577c-145">Boolean</span></span>|<span data-ttu-id="c577c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="c577c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c577c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="c577c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c577c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c577c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c577c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c577c-149">This property is read-only.</span></span> <span data-ttu-id="c577c-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c577c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c577c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c577c-151">createdDateTime</span></span>|<span data-ttu-id="c577c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c577c-152">DateTimeOffset</span></span>|<span data-ttu-id="c577c-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="c577c-153">DateTime the object was created.</span></span> <span data-ttu-id="c577c-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c577c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c577c-155">description</span><span class="sxs-lookup"><span data-stu-id="c577c-155">description</span></span>|<span data-ttu-id="c577c-156">String</span><span class="sxs-lookup"><span data-stu-id="c577c-156">String</span></span>|<span data-ttu-id="c577c-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c577c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c577c-158">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c577c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c577c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c577c-159">displayName</span></span>|<span data-ttu-id="c577c-160">String</span><span class="sxs-lookup"><span data-stu-id="c577c-160">String</span></span>|<span data-ttu-id="c577c-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c577c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c577c-162">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c577c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c577c-163">version</span><span class="sxs-lookup"><span data-stu-id="c577c-163">version</span></span>|<span data-ttu-id="c577c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c577c-164">Int32</span></span>|<span data-ttu-id="c577c-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="c577c-165">Version of the device configuration.</span></span> <span data-ttu-id="c577c-166">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c577c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c577c-167">Киоскпрофилес</span><span class="sxs-lookup"><span data-stu-id="c577c-167">kioskProfiles</span></span>|<span data-ttu-id="c577c-168">Коллекция [виндовскиоскпрофиле](../resources/intune-deviceconfig-windowskioskprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c577c-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="c577c-169">Этот параметр политики позволяет определить список профилей киоска для конфигурации киоска.</span><span class="sxs-lookup"><span data-stu-id="c577c-169">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="c577c-170">Эта коллекция может содержать не более 3 элементов.</span><span class="sxs-lookup"><span data-stu-id="c577c-170">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="c577c-171">Киоскбровсердефаултурл</span><span class="sxs-lookup"><span data-stu-id="c577c-171">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="c577c-172">Строка</span><span class="sxs-lookup"><span data-stu-id="c577c-172">String</span></span>|<span data-ttu-id="c577c-173">Укажите URL-адрес по умолчанию, на который должен переходить браузер при запуске.</span><span class="sxs-lookup"><span data-stu-id="c577c-173">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="c577c-174">Киоскбровсеренаблехомебуттон</span><span class="sxs-lookup"><span data-stu-id="c577c-174">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="c577c-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="c577c-175">Boolean</span></span>|<span data-ttu-id="c577c-176">Включите кнопку Главная в браузере киоска.</span><span class="sxs-lookup"><span data-stu-id="c577c-176">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="c577c-177">По умолчанию кнопка "домой" отключена.</span><span class="sxs-lookup"><span data-stu-id="c577c-177">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="c577c-178">Киоскбровсеренабленавигатионбуттонс</span><span class="sxs-lookup"><span data-stu-id="c577c-178">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="c577c-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="c577c-179">Boolean</span></span>|<span data-ttu-id="c577c-180">Включение кнопок навигации в браузере киосков (вперед и назад).</span><span class="sxs-lookup"><span data-stu-id="c577c-180">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="c577c-181">По умолчанию кнопки навигации отключены.</span><span class="sxs-lookup"><span data-stu-id="c577c-181">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="c577c-182">Киоскбровсеренаблиндсессионбуттон</span><span class="sxs-lookup"><span data-stu-id="c577c-182">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="c577c-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="c577c-183">Boolean</span></span>|<span data-ttu-id="c577c-184">Включите кнопку End Session (завершить сеанс) в обозревателе киосков.</span><span class="sxs-lookup"><span data-stu-id="c577c-184">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="c577c-185">По умолчанию кнопка End Session отключена.</span><span class="sxs-lookup"><span data-stu-id="c577c-185">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="c577c-186">Киоскбровсеррестартонидлетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="c577c-186">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="c577c-187">Int32</span><span class="sxs-lookup"><span data-stu-id="c577c-187">Int32</span></span>|<span data-ttu-id="c577c-188">Укажите время в минутах, в течение которого сеанс простаивает до тех пор, пока обозреватель киоска не перезапустится в обновленном состоянии.</span><span class="sxs-lookup"><span data-stu-id="c577c-188">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="c577c-189">Допустимые значения: 1-1440.</span><span class="sxs-lookup"><span data-stu-id="c577c-189">Valid values are 1-1440.</span></span> <span data-ttu-id="c577c-190">Допустимые значения — от 1 до 1440</span><span class="sxs-lookup"><span data-stu-id="c577c-190">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="c577c-191">Киоскбровсерблоккедурлс</span><span class="sxs-lookup"><span data-stu-id="c577c-191">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="c577c-192">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c577c-192">String collection</span></span>|<span data-ttu-id="c577c-193">Указание URL-адресов, к которым не должны переходить браузеры киоска</span><span class="sxs-lookup"><span data-stu-id="c577c-193">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="c577c-194">Киоскбровсерблоккедурлексцептионс</span><span class="sxs-lookup"><span data-stu-id="c577c-194">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="c577c-195">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c577c-195">String collection</span></span>|<span data-ttu-id="c577c-196">Указание URL-адресов, на которые может перейти браузер с киоском</span><span class="sxs-lookup"><span data-stu-id="c577c-196">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="c577c-197">Еджекиоскенаблепубликбровсинг</span><span class="sxs-lookup"><span data-stu-id="c577c-197">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="c577c-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="c577c-198">Boolean</span></span>|<span data-ttu-id="c577c-199">Включение режима "общедоступный" в режиме киоска браузера для браузера Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="c577c-199">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="c577c-200">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="c577c-200">The Default is false.</span></span>|



## <a name="response"></a><span data-ttu-id="c577c-201">Ответ</span><span class="sxs-lookup"><span data-stu-id="c577c-201">Response</span></span>
<span data-ttu-id="c577c-202">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c577c-202">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c577c-203">Пример</span><span class="sxs-lookup"><span data-stu-id="c577c-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="c577c-204">Запрос</span><span class="sxs-lookup"><span data-stu-id="c577c-204">Request</span></span>
<span data-ttu-id="c577c-205">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c577c-205">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1753

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "edgeKioskEnablePublicBrowsing": true
}
```

### <a name="response"></a><span data-ttu-id="c577c-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="c577c-206">Response</span></span>
<span data-ttu-id="c577c-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c577c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1925

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "id": "146a990b-990b-146a-0b99-6a140b996a14",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "edgeKioskEnablePublicBrowsing": true
}
```




