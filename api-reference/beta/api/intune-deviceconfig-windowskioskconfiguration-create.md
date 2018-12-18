---
title: Создание windowsKioskConfiguration
description: Создание нового объекта windowsKioskConfiguration.
author: tfitzmac
ms.openlocfilehash: 35630494206a234e248935a75483afa2da969ed4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327540"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="39ef9-103">Создание windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="39ef9-103">Create windowsKioskConfiguration</span></span>

> <span data-ttu-id="39ef9-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="39ef9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39ef9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39ef9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39ef9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="39ef9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39ef9-107">Создание нового объекта [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="39ef9-107">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39ef9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="39ef9-108">Prerequisites</span></span>
<span data-ttu-id="39ef9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39ef9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39ef9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39ef9-111">Permission type</span></span>|<span data-ttu-id="39ef9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39ef9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39ef9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39ef9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39ef9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39ef9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="39ef9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39ef9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39ef9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39ef9-116">Not supported.</span></span>|
|<span data-ttu-id="39ef9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39ef9-117">Application</span></span>|<span data-ttu-id="39ef9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39ef9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39ef9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39ef9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="39ef9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39ef9-120">Request headers</span></span>
|<span data-ttu-id="39ef9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39ef9-121">Header</span></span>|<span data-ttu-id="39ef9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="39ef9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39ef9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39ef9-123">Authorization</span></span>|<span data-ttu-id="39ef9-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="39ef9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39ef9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="39ef9-125">Accept</span></span>|<span data-ttu-id="39ef9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39ef9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39ef9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39ef9-127">Request body</span></span>
<span data-ttu-id="39ef9-128">В тексте запроса укажите представление JSON для объекта windowsKioskConfiguration.</span><span class="sxs-lookup"><span data-stu-id="39ef9-128">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="39ef9-129">В следующей таблице показаны свойства, которые необходимы для создания windowsKioskConfiguration.</span><span class="sxs-lookup"><span data-stu-id="39ef9-129">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="39ef9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="39ef9-130">Property</span></span>|<span data-ttu-id="39ef9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="39ef9-131">Type</span></span>|<span data-ttu-id="39ef9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="39ef9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ef9-133">id</span><span class="sxs-lookup"><span data-stu-id="39ef9-133">id</span></span>|<span data-ttu-id="39ef9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="39ef9-134">String</span></span>|<span data-ttu-id="39ef9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="39ef9-135">Key of the entity.</span></span> <span data-ttu-id="39ef9-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ef9-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ef9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39ef9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="39ef9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ef9-138">DateTimeOffset</span></span>|<span data-ttu-id="39ef9-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="39ef9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="39ef9-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ef9-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ef9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39ef9-141">roleScopeTagIds</span></span>|<span data-ttu-id="39ef9-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="39ef9-142">String collection</span></span>|<span data-ttu-id="39ef9-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="39ef9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="39ef9-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ef9-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ef9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="39ef9-145">supportsScopeTags</span></span>|<span data-ttu-id="39ef9-146">Boolean.</span><span class="sxs-lookup"><span data-stu-id="39ef9-146">Boolean</span></span>|<span data-ttu-id="39ef9-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="39ef9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="39ef9-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="39ef9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="39ef9-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="39ef9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="39ef9-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="39ef9-150">This property is read-only.</span></span> <span data-ttu-id="39ef9-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ef9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ef9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39ef9-152">createdDateTime</span></span>|<span data-ttu-id="39ef9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39ef9-153">DateTimeOffset</span></span>|<span data-ttu-id="39ef9-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="39ef9-154">DateTime the object was created.</span></span> <span data-ttu-id="39ef9-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ef9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ef9-156">описание</span><span class="sxs-lookup"><span data-stu-id="39ef9-156">description</span></span>|<span data-ttu-id="39ef9-157">Строка</span><span class="sxs-lookup"><span data-stu-id="39ef9-157">String</span></span>|<span data-ttu-id="39ef9-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39ef9-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="39ef9-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ef9-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ef9-160">displayName</span><span class="sxs-lookup"><span data-stu-id="39ef9-160">displayName</span></span>|<span data-ttu-id="39ef9-161">Строка</span><span class="sxs-lookup"><span data-stu-id="39ef9-161">String</span></span>|<span data-ttu-id="39ef9-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39ef9-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="39ef9-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ef9-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ef9-164">version</span><span class="sxs-lookup"><span data-stu-id="39ef9-164">version</span></span>|<span data-ttu-id="39ef9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="39ef9-165">Int32</span></span>|<span data-ttu-id="39ef9-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="39ef9-166">Version of the device configuration.</span></span> <span data-ttu-id="39ef9-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="39ef9-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="39ef9-168">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="39ef9-168">kioskProfiles</span></span>|<span data-ttu-id="39ef9-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="39ef9-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="39ef9-170">Этот параметр политики позволяет определить список профилей киоска для базовой конфигурации.</span><span class="sxs-lookup"><span data-stu-id="39ef9-170">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="39ef9-171">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="39ef9-171">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="39ef9-172">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="39ef9-172">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="39ef9-173">String.</span><span class="sxs-lookup"><span data-stu-id="39ef9-173">String</span></span>|<span data-ttu-id="39ef9-174">Укажите URL-адрес по умолчанию, должен перейти браузер при запуске.</span><span class="sxs-lookup"><span data-stu-id="39ef9-174">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="39ef9-175">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="39ef9-175">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="39ef9-176">Boolean.</span><span class="sxs-lookup"><span data-stu-id="39ef9-176">Boolean</span></span>|<span data-ttu-id="39ef9-177">Кнопка браузера киоска Домашняя страница.</span><span class="sxs-lookup"><span data-stu-id="39ef9-177">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="39ef9-178">По умолчанию домашняя страница кнопка отключена.</span><span class="sxs-lookup"><span data-stu-id="39ef9-178">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="39ef9-179">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="39ef9-179">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="39ef9-180">Boolean.</span><span class="sxs-lookup"><span data-stu-id="39ef9-180">Boolean</span></span>|<span data-ttu-id="39ef9-181">Включите buttons(forward/back) навигации киоска браузера.</span><span class="sxs-lookup"><span data-stu-id="39ef9-181">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="39ef9-182">По умолчанию отключены кнопки перехода.</span><span class="sxs-lookup"><span data-stu-id="39ef9-182">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="39ef9-183">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="39ef9-183">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="39ef9-184">Boolean.</span><span class="sxs-lookup"><span data-stu-id="39ef9-184">Boolean</span></span>|<span data-ttu-id="39ef9-185">Кнопка браузера киоска окончания сеанса.</span><span class="sxs-lookup"><span data-stu-id="39ef9-185">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="39ef9-186">По умолчанию отключена кнопка окончания сеанса.</span><span class="sxs-lookup"><span data-stu-id="39ef9-186">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="39ef9-187">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="39ef9-187">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="39ef9-188">Int32</span><span class="sxs-lookup"><span data-stu-id="39ef9-188">Int32</span></span>|<span data-ttu-id="39ef9-189">Укажите время в минутах, сеанс находится в состоянии простоя до перезапуска браузера киоска новым состояние.</span><span class="sxs-lookup"><span data-stu-id="39ef9-189">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="39ef9-190">Допустимые значения: 1-1440.</span><span class="sxs-lookup"><span data-stu-id="39ef9-190">Valid values are 1-1440.</span></span> <span data-ttu-id="39ef9-191">Допустимые значения 1 до 1440</span><span class="sxs-lookup"><span data-stu-id="39ef9-191">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="39ef9-192">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="39ef9-192">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="39ef9-193">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="39ef9-193">String collection</span></span>|<span data-ttu-id="39ef9-194">Укажите URL-адреса, не должен перейти киоска браузеры</span><span class="sxs-lookup"><span data-stu-id="39ef9-194">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="39ef9-195">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="39ef9-195">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="39ef9-196">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="39ef9-196">String collection</span></span>|<span data-ttu-id="39ef9-197">Укажите URL-адресов, которые может киоска браузера перейдите на</span><span class="sxs-lookup"><span data-stu-id="39ef9-197">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|



## <a name="response"></a><span data-ttu-id="39ef9-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="39ef9-198">Response</span></span>
<span data-ttu-id="39ef9-199">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="39ef9-199">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39ef9-200">Пример</span><span class="sxs-lookup"><span data-stu-id="39ef9-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="39ef9-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="39ef9-201">Request</span></span>
<span data-ttu-id="39ef9-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39ef9-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1662

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="39ef9-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="39ef9-203">Response</span></span>
<span data-ttu-id="39ef9-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="39ef9-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1770

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
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
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
  ]
}
```





