---
title: Обновление windowsKioskConfiguration
description: Обновление свойства объекта windowsKioskConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 33fe6dc90fe6118dc8ca4aeb67bfc728f487a1b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983165"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="269ea-103">Обновление windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="269ea-103">Update windowsKioskConfiguration</span></span>

> <span data-ttu-id="269ea-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="269ea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="269ea-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="269ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="269ea-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="269ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="269ea-107">Обновление свойства объекта [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="269ea-107">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="269ea-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="269ea-108">Prerequisites</span></span>
<span data-ttu-id="269ea-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="269ea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="269ea-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="269ea-111">Permission type</span></span>|<span data-ttu-id="269ea-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="269ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="269ea-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="269ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="269ea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="269ea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="269ea-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="269ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="269ea-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="269ea-116">Not supported.</span></span>|
|<span data-ttu-id="269ea-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="269ea-117">Application</span></span>|<span data-ttu-id="269ea-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="269ea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="269ea-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="269ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="269ea-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="269ea-120">Request headers</span></span>
|<span data-ttu-id="269ea-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="269ea-121">Header</span></span>|<span data-ttu-id="269ea-122">Значение</span><span class="sxs-lookup"><span data-stu-id="269ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="269ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="269ea-123">Authorization</span></span>|<span data-ttu-id="269ea-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="269ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="269ea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="269ea-125">Accept</span></span>|<span data-ttu-id="269ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="269ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="269ea-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="269ea-127">Request body</span></span>
<span data-ttu-id="269ea-128">В тексте запроса укажите представление JSON для объекта [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="269ea-128">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="269ea-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="269ea-129">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="269ea-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="269ea-130">Property</span></span>|<span data-ttu-id="269ea-131">Тип</span><span class="sxs-lookup"><span data-stu-id="269ea-131">Type</span></span>|<span data-ttu-id="269ea-132">Описание</span><span class="sxs-lookup"><span data-stu-id="269ea-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="269ea-133">id</span><span class="sxs-lookup"><span data-stu-id="269ea-133">id</span></span>|<span data-ttu-id="269ea-134">Строка</span><span class="sxs-lookup"><span data-stu-id="269ea-134">String</span></span>|<span data-ttu-id="269ea-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="269ea-135">Key of the entity.</span></span> <span data-ttu-id="269ea-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="269ea-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="269ea-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="269ea-137">lastModifiedDateTime</span></span>|<span data-ttu-id="269ea-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="269ea-138">DateTimeOffset</span></span>|<span data-ttu-id="269ea-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="269ea-139">DateTime the object was last modified.</span></span> <span data-ttu-id="269ea-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="269ea-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="269ea-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="269ea-141">roleScopeTagIds</span></span>|<span data-ttu-id="269ea-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="269ea-142">String collection</span></span>|<span data-ttu-id="269ea-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="269ea-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="269ea-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="269ea-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="269ea-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="269ea-145">supportsScopeTags</span></span>|<span data-ttu-id="269ea-146">Логический</span><span class="sxs-lookup"><span data-stu-id="269ea-146">Boolean</span></span>|<span data-ttu-id="269ea-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="269ea-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="269ea-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="269ea-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="269ea-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="269ea-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="269ea-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="269ea-150">This property is read-only.</span></span> <span data-ttu-id="269ea-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="269ea-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="269ea-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="269ea-152">createdDateTime</span></span>|<span data-ttu-id="269ea-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="269ea-153">DateTimeOffset</span></span>|<span data-ttu-id="269ea-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="269ea-154">DateTime the object was created.</span></span> <span data-ttu-id="269ea-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="269ea-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="269ea-156">описание</span><span class="sxs-lookup"><span data-stu-id="269ea-156">description</span></span>|<span data-ttu-id="269ea-157">Строка</span><span class="sxs-lookup"><span data-stu-id="269ea-157">String</span></span>|<span data-ttu-id="269ea-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="269ea-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="269ea-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="269ea-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="269ea-160">displayName</span><span class="sxs-lookup"><span data-stu-id="269ea-160">displayName</span></span>|<span data-ttu-id="269ea-161">Строка</span><span class="sxs-lookup"><span data-stu-id="269ea-161">String</span></span>|<span data-ttu-id="269ea-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="269ea-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="269ea-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="269ea-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="269ea-164">version</span><span class="sxs-lookup"><span data-stu-id="269ea-164">version</span></span>|<span data-ttu-id="269ea-165">Int32</span><span class="sxs-lookup"><span data-stu-id="269ea-165">Int32</span></span>|<span data-ttu-id="269ea-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="269ea-166">Version of the device configuration.</span></span> <span data-ttu-id="269ea-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="269ea-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="269ea-168">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="269ea-168">kioskProfiles</span></span>|<span data-ttu-id="269ea-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="269ea-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="269ea-170">Этот параметр политики позволяет определить список профилей киоска для базовой конфигурации.</span><span class="sxs-lookup"><span data-stu-id="269ea-170">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="269ea-171">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="269ea-171">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="269ea-172">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="269ea-172">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="269ea-173">Строка</span><span class="sxs-lookup"><span data-stu-id="269ea-173">String</span></span>|<span data-ttu-id="269ea-174">Укажите URL-адрес по умолчанию, должен перейти браузер при запуске.</span><span class="sxs-lookup"><span data-stu-id="269ea-174">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="269ea-175">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="269ea-175">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="269ea-176">Логический</span><span class="sxs-lookup"><span data-stu-id="269ea-176">Boolean</span></span>|<span data-ttu-id="269ea-177">Кнопка браузера киоска Домашняя страница.</span><span class="sxs-lookup"><span data-stu-id="269ea-177">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="269ea-178">По умолчанию домашняя страница кнопка отключена.</span><span class="sxs-lookup"><span data-stu-id="269ea-178">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="269ea-179">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="269ea-179">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="269ea-180">Логический</span><span class="sxs-lookup"><span data-stu-id="269ea-180">Boolean</span></span>|<span data-ttu-id="269ea-181">Включите buttons(forward/back) навигации киоска браузера.</span><span class="sxs-lookup"><span data-stu-id="269ea-181">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="269ea-182">По умолчанию отключены кнопки перехода.</span><span class="sxs-lookup"><span data-stu-id="269ea-182">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="269ea-183">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="269ea-183">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="269ea-184">Логический</span><span class="sxs-lookup"><span data-stu-id="269ea-184">Boolean</span></span>|<span data-ttu-id="269ea-185">Кнопка браузера киоска окончания сеанса.</span><span class="sxs-lookup"><span data-stu-id="269ea-185">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="269ea-186">По умолчанию отключена кнопка окончания сеанса.</span><span class="sxs-lookup"><span data-stu-id="269ea-186">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="269ea-187">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="269ea-187">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="269ea-188">Int32</span><span class="sxs-lookup"><span data-stu-id="269ea-188">Int32</span></span>|<span data-ttu-id="269ea-189">Укажите время в минутах, сеанс находится в состоянии простоя до перезапуска браузера киоска новым состояние.</span><span class="sxs-lookup"><span data-stu-id="269ea-189">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="269ea-190">Допустимые значения: 1-1440.</span><span class="sxs-lookup"><span data-stu-id="269ea-190">Valid values are 1-1440.</span></span> <span data-ttu-id="269ea-191">Допустимые значения 1 до 1440</span><span class="sxs-lookup"><span data-stu-id="269ea-191">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="269ea-192">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="269ea-192">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="269ea-193">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="269ea-193">String collection</span></span>|<span data-ttu-id="269ea-194">Укажите URL-адреса, не должен перейти киоска браузеры</span><span class="sxs-lookup"><span data-stu-id="269ea-194">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="269ea-195">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="269ea-195">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="269ea-196">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="269ea-196">String collection</span></span>|<span data-ttu-id="269ea-197">Укажите URL-адресов, которые может киоска браузера перейдите на</span><span class="sxs-lookup"><span data-stu-id="269ea-197">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|



## <a name="response"></a><span data-ttu-id="269ea-198">Ответ</span><span class="sxs-lookup"><span data-stu-id="269ea-198">Response</span></span>
<span data-ttu-id="269ea-199">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="269ea-199">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="269ea-200">Пример</span><span class="sxs-lookup"><span data-stu-id="269ea-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="269ea-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="269ea-201">Request</span></span>
<span data-ttu-id="269ea-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="269ea-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1598

{
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

### <a name="response"></a><span data-ttu-id="269ea-203">Ответ</span><span class="sxs-lookup"><span data-stu-id="269ea-203">Response</span></span>
<span data-ttu-id="269ea-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="269ea-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





