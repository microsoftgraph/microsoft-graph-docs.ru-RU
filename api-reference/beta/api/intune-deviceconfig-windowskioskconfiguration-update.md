---
title: Обновление windowsKioskConfiguration
description: Обновление свойства объекта windowsKioskConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 767acd4136226e2687977cf09d2c08f6c413fcb8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414888"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="f634c-103">Обновление windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="f634c-103">Update windowsKioskConfiguration</span></span>

> <span data-ttu-id="f634c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f634c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f634c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f634c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f634c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f634c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f634c-107">Обновление свойства объекта [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f634c-107">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f634c-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="f634c-108">Prerequisites</span></span>
<span data-ttu-id="f634c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f634c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f634c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f634c-111">Permission type</span></span>|<span data-ttu-id="f634c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f634c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f634c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f634c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f634c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f634c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f634c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f634c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f634c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f634c-116">Not supported.</span></span>|
|<span data-ttu-id="f634c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f634c-117">Application</span></span>|<span data-ttu-id="f634c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f634c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f634c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f634c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f634c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f634c-120">Request headers</span></span>
|<span data-ttu-id="f634c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f634c-121">Header</span></span>|<span data-ttu-id="f634c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f634c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f634c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f634c-123">Authorization</span></span>|<span data-ttu-id="f634c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f634c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f634c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f634c-125">Accept</span></span>|<span data-ttu-id="f634c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f634c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f634c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f634c-127">Request body</span></span>
<span data-ttu-id="f634c-128">В тексте запроса укажите представление JSON для объекта [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f634c-128">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="f634c-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f634c-129">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="f634c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f634c-130">Property</span></span>|<span data-ttu-id="f634c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f634c-131">Type</span></span>|<span data-ttu-id="f634c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f634c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f634c-133">id</span><span class="sxs-lookup"><span data-stu-id="f634c-133">id</span></span>|<span data-ttu-id="f634c-134">String</span><span class="sxs-lookup"><span data-stu-id="f634c-134">String</span></span>|<span data-ttu-id="f634c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f634c-135">Key of the entity.</span></span> <span data-ttu-id="f634c-136">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f634c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f634c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f634c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f634c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f634c-138">DateTimeOffset</span></span>|<span data-ttu-id="f634c-139">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f634c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f634c-140">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f634c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f634c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f634c-141">roleScopeTagIds</span></span>|<span data-ttu-id="f634c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f634c-142">String collection</span></span>|<span data-ttu-id="f634c-143">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="f634c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f634c-144">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f634c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f634c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f634c-145">supportsScopeTags</span></span>|<span data-ttu-id="f634c-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f634c-146">Boolean</span></span>|<span data-ttu-id="f634c-147">Указывает, поддерживает ли базовой конфигурации устройства назначения тегов области действия.</span><span class="sxs-lookup"><span data-stu-id="f634c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f634c-148">Присвоение свойства ScopeTags не допускается, если это значение равно false и сущности не будут недоступны пользователям с заданной областью.</span><span class="sxs-lookup"><span data-stu-id="f634c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f634c-149">Это происходит для политик прежних версий, созданные в Silverlight и можно устранить, удаление и повторное создание политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="f634c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f634c-150">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f634c-150">This property is read-only.</span></span> <span data-ttu-id="f634c-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f634c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f634c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f634c-152">createdDateTime</span></span>|<span data-ttu-id="f634c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f634c-153">DateTimeOffset</span></span>|<span data-ttu-id="f634c-154">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f634c-154">DateTime the object was created.</span></span> <span data-ttu-id="f634c-155">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f634c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f634c-156">description</span><span class="sxs-lookup"><span data-stu-id="f634c-156">description</span></span>|<span data-ttu-id="f634c-157">String</span><span class="sxs-lookup"><span data-stu-id="f634c-157">String</span></span>|<span data-ttu-id="f634c-158">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f634c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f634c-159">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f634c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f634c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f634c-160">displayName</span></span>|<span data-ttu-id="f634c-161">String</span><span class="sxs-lookup"><span data-stu-id="f634c-161">String</span></span>|<span data-ttu-id="f634c-162">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f634c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f634c-163">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f634c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f634c-164">version</span><span class="sxs-lookup"><span data-stu-id="f634c-164">version</span></span>|<span data-ttu-id="f634c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f634c-165">Int32</span></span>|<span data-ttu-id="f634c-166">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f634c-166">Version of the device configuration.</span></span> <span data-ttu-id="f634c-167">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f634c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f634c-168">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="f634c-168">kioskProfiles</span></span>|<span data-ttu-id="f634c-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="f634c-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="f634c-170">Этот параметр политики позволяет определить список профилей киоска для базовой конфигурации.</span><span class="sxs-lookup"><span data-stu-id="f634c-170">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="f634c-171">В этом семействе может содержать не более 3 элементы.</span><span class="sxs-lookup"><span data-stu-id="f634c-171">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="f634c-172">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="f634c-172">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="f634c-173">String</span><span class="sxs-lookup"><span data-stu-id="f634c-173">String</span></span>|<span data-ttu-id="f634c-174">Укажите URL-адрес по умолчанию, должен перейти браузер при запуске.</span><span class="sxs-lookup"><span data-stu-id="f634c-174">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="f634c-175">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="f634c-175">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="f634c-176">Логический</span><span class="sxs-lookup"><span data-stu-id="f634c-176">Boolean</span></span>|<span data-ttu-id="f634c-177">Кнопка браузера киоска Домашняя страница.</span><span class="sxs-lookup"><span data-stu-id="f634c-177">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="f634c-178">По умолчанию домашняя страница кнопка отключена.</span><span class="sxs-lookup"><span data-stu-id="f634c-178">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="f634c-179">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="f634c-179">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="f634c-180">Логический</span><span class="sxs-lookup"><span data-stu-id="f634c-180">Boolean</span></span>|<span data-ttu-id="f634c-181">Включите buttons(forward/back) навигации киоска браузера.</span><span class="sxs-lookup"><span data-stu-id="f634c-181">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="f634c-182">По умолчанию отключены кнопки перехода.</span><span class="sxs-lookup"><span data-stu-id="f634c-182">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="f634c-183">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="f634c-183">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="f634c-184">Логический</span><span class="sxs-lookup"><span data-stu-id="f634c-184">Boolean</span></span>|<span data-ttu-id="f634c-185">Кнопка браузера киоска окончания сеанса.</span><span class="sxs-lookup"><span data-stu-id="f634c-185">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="f634c-186">По умолчанию отключена кнопка окончания сеанса.</span><span class="sxs-lookup"><span data-stu-id="f634c-186">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="f634c-187">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="f634c-187">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="f634c-188">Int32</span><span class="sxs-lookup"><span data-stu-id="f634c-188">Int32</span></span>|<span data-ttu-id="f634c-189">Укажите время в минутах, сеанс находится в состоянии простоя до перезапуска браузера киоска новым состояние.</span><span class="sxs-lookup"><span data-stu-id="f634c-189">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="f634c-190">Допустимые значения: 1-1440.</span><span class="sxs-lookup"><span data-stu-id="f634c-190">Valid values are 1-1440.</span></span> <span data-ttu-id="f634c-191">Допустимые значения 1 до 1440</span><span class="sxs-lookup"><span data-stu-id="f634c-191">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="f634c-192">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="f634c-192">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="f634c-193">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f634c-193">String collection</span></span>|<span data-ttu-id="f634c-194">Укажите URL-адреса, не должен перейти киоска браузеры</span><span class="sxs-lookup"><span data-stu-id="f634c-194">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="f634c-195">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="f634c-195">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="f634c-196">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f634c-196">String collection</span></span>|<span data-ttu-id="f634c-197">Укажите URL-адресов, которые может киоска браузера перейдите на</span><span class="sxs-lookup"><span data-stu-id="f634c-197">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="f634c-198">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="f634c-198">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="f634c-199">Логический</span><span class="sxs-lookup"><span data-stu-id="f634c-199">Boolean</span></span>|<span data-ttu-id="f634c-200">Включение общей обзора полноэкранном режиме для браузера Microsoft пограничного сервера.</span><span class="sxs-lookup"><span data-stu-id="f634c-200">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="f634c-201">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="f634c-201">The Default is false.</span></span>|
|<span data-ttu-id="f634c-202">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="f634c-202">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="f634c-203">Int32</span><span class="sxs-lookup"><span data-stu-id="f634c-203">Int32</span></span>|<span data-ttu-id="f634c-204">Задает время в минутах из последнего действия пользователя перед базовая Подписка пограничного сервера Microsoft восстанавливаются значения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f634c-204">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="f634c-205">Допустимые значения: 0-1440.</span><span class="sxs-lookup"><span data-stu-id="f634c-205">Valid values are 0-1440.</span></span> <span data-ttu-id="f634c-206">Значение по умолчанию равно 5.</span><span class="sxs-lookup"><span data-stu-id="f634c-206">The default is 5.</span></span> <span data-ttu-id="f634c-207">0 указывает не reset.</span><span class="sxs-lookup"><span data-stu-id="f634c-207">0 indicates no reset.</span></span> <span data-ttu-id="f634c-208">Допустимые значения 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="f634c-208">Valid values 0 to 1440</span></span>|



## <a name="response"></a><span data-ttu-id="f634c-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="f634c-209">Response</span></span>
<span data-ttu-id="f634c-210">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f634c-210">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f634c-211">Пример</span><span class="sxs-lookup"><span data-stu-id="f634c-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="f634c-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="f634c-212">Request</span></span>
<span data-ttu-id="f634c-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f634c-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1719

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
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "edgeKioskResetAfterIdleTimeInMinutes": 4
}
```

### <a name="response"></a><span data-ttu-id="f634c-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="f634c-214">Response</span></span>
<span data-ttu-id="f634c-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f634c-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1891

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
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "edgeKioskResetAfterIdleTimeInMinutes": 4
}
```




