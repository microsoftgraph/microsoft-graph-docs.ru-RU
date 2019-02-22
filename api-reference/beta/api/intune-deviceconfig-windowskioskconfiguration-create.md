---
title: Создание Виндовскиоскконфигуратион
description: Создание нового объекта Виндовскиоскконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dd32b23626c027cfc4a9cdac60b5a5a4a6c37973
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160748"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="8787c-103">Создание Виндовскиоскконфигуратион</span><span class="sxs-lookup"><span data-stu-id="8787c-103">Create windowsKioskConfiguration</span></span>

> <span data-ttu-id="8787c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8787c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8787c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8787c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8787c-106">Создание нового объекта [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8787c-106">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8787c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8787c-107">Prerequisites</span></span>
<span data-ttu-id="8787c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8787c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8787c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8787c-110">Permission type</span></span>|<span data-ttu-id="8787c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8787c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8787c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8787c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8787c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8787c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8787c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8787c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8787c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8787c-115">Not supported.</span></span>|
|<span data-ttu-id="8787c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8787c-116">Application</span></span>|<span data-ttu-id="8787c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8787c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8787c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8787c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8787c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8787c-119">Request headers</span></span>
|<span data-ttu-id="8787c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8787c-120">Header</span></span>|<span data-ttu-id="8787c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8787c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8787c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8787c-122">Authorization</span></span>|<span data-ttu-id="8787c-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8787c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8787c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8787c-124">Accept</span></span>|<span data-ttu-id="8787c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8787c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8787c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8787c-126">Request body</span></span>
<span data-ttu-id="8787c-127">В тексте запроса добавьте представление объекта Виндовскиоскконфигуратион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8787c-127">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="8787c-128">В следующей таблице приведены свойства, необходимые при создании Виндовскиоскконфигуратион.</span><span class="sxs-lookup"><span data-stu-id="8787c-128">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="8787c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8787c-129">Property</span></span>|<span data-ttu-id="8787c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8787c-130">Type</span></span>|<span data-ttu-id="8787c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8787c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8787c-132">id</span><span class="sxs-lookup"><span data-stu-id="8787c-132">id</span></span>|<span data-ttu-id="8787c-133">String</span><span class="sxs-lookup"><span data-stu-id="8787c-133">String</span></span>|<span data-ttu-id="8787c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8787c-134">Key of the entity.</span></span> <span data-ttu-id="8787c-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8787c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8787c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8787c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8787c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8787c-137">DateTimeOffset</span></span>|<span data-ttu-id="8787c-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8787c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8787c-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8787c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8787c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8787c-140">roleScopeTagIds</span></span>|<span data-ttu-id="8787c-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8787c-141">String collection</span></span>|<span data-ttu-id="8787c-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="8787c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8787c-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8787c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8787c-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="8787c-144">supportsScopeTags</span></span>|<span data-ttu-id="8787c-145">Логический</span><span class="sxs-lookup"><span data-stu-id="8787c-145">Boolean</span></span>|<span data-ttu-id="8787c-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="8787c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8787c-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="8787c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8787c-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8787c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8787c-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8787c-149">This property is read-only.</span></span> <span data-ttu-id="8787c-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8787c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8787c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8787c-151">createdDateTime</span></span>|<span data-ttu-id="8787c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8787c-152">DateTimeOffset</span></span>|<span data-ttu-id="8787c-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8787c-153">DateTime the object was created.</span></span> <span data-ttu-id="8787c-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8787c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8787c-155">description</span><span class="sxs-lookup"><span data-stu-id="8787c-155">description</span></span>|<span data-ttu-id="8787c-156">String</span><span class="sxs-lookup"><span data-stu-id="8787c-156">String</span></span>|<span data-ttu-id="8787c-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8787c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8787c-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8787c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8787c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8787c-159">displayName</span></span>|<span data-ttu-id="8787c-160">String</span><span class="sxs-lookup"><span data-stu-id="8787c-160">String</span></span>|<span data-ttu-id="8787c-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8787c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8787c-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8787c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8787c-163">version</span><span class="sxs-lookup"><span data-stu-id="8787c-163">version</span></span>|<span data-ttu-id="8787c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8787c-164">Int32</span></span>|<span data-ttu-id="8787c-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8787c-165">Version of the device configuration.</span></span> <span data-ttu-id="8787c-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8787c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8787c-167">Киоскпрофилес</span><span class="sxs-lookup"><span data-stu-id="8787c-167">kioskProfiles</span></span>|<span data-ttu-id="8787c-168">Коллекция [виндовскиоскпрофиле](../resources/intune-deviceconfig-windowskioskprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8787c-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="8787c-169">Этот параметр политики позволяет определить список профилей киоска для конфигурации киоска.</span><span class="sxs-lookup"><span data-stu-id="8787c-169">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="8787c-170">Эта коллекция может содержать не более 3 элементов.</span><span class="sxs-lookup"><span data-stu-id="8787c-170">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="8787c-171">Киоскбровсердефаултурл</span><span class="sxs-lookup"><span data-stu-id="8787c-171">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="8787c-172">String</span><span class="sxs-lookup"><span data-stu-id="8787c-172">String</span></span>|<span data-ttu-id="8787c-173">Укажите URL-адрес по умолчанию, на который должен переходить браузер при запуске.</span><span class="sxs-lookup"><span data-stu-id="8787c-173">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="8787c-174">Киоскбровсеренаблехомебуттон</span><span class="sxs-lookup"><span data-stu-id="8787c-174">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="8787c-175">Логический</span><span class="sxs-lookup"><span data-stu-id="8787c-175">Boolean</span></span>|<span data-ttu-id="8787c-176">Включите кнопку Главная в браузере киоска.</span><span class="sxs-lookup"><span data-stu-id="8787c-176">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="8787c-177">По умолчанию кнопка "домой" отключена.</span><span class="sxs-lookup"><span data-stu-id="8787c-177">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="8787c-178">Киоскбровсеренабленавигатионбуттонс</span><span class="sxs-lookup"><span data-stu-id="8787c-178">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="8787c-179">Логический</span><span class="sxs-lookup"><span data-stu-id="8787c-179">Boolean</span></span>|<span data-ttu-id="8787c-180">Включение кнопок навигации в браузере киосков (вперед и назад).</span><span class="sxs-lookup"><span data-stu-id="8787c-180">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="8787c-181">По умолчанию кнопки навигации отключены.</span><span class="sxs-lookup"><span data-stu-id="8787c-181">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="8787c-182">Киоскбровсеренаблиндсессионбуттон</span><span class="sxs-lookup"><span data-stu-id="8787c-182">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="8787c-183">Логический</span><span class="sxs-lookup"><span data-stu-id="8787c-183">Boolean</span></span>|<span data-ttu-id="8787c-184">Включите кнопку End Session (завершить сеанс) в обозревателе киосков.</span><span class="sxs-lookup"><span data-stu-id="8787c-184">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="8787c-185">По умолчанию кнопка End Session отключена.</span><span class="sxs-lookup"><span data-stu-id="8787c-185">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="8787c-186">Киоскбровсеррестартонидлетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="8787c-186">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="8787c-187">Int32</span><span class="sxs-lookup"><span data-stu-id="8787c-187">Int32</span></span>|<span data-ttu-id="8787c-188">Укажите время в минутах, в течение которого сеанс простаивает до тех пор, пока обозреватель киоска не перезапустится в обновленном состоянии.</span><span class="sxs-lookup"><span data-stu-id="8787c-188">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="8787c-189">Допустимые значения: 1-1440.</span><span class="sxs-lookup"><span data-stu-id="8787c-189">Valid values are 1-1440.</span></span> <span data-ttu-id="8787c-190">Допустимые значения — от 1 до 1440</span><span class="sxs-lookup"><span data-stu-id="8787c-190">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="8787c-191">Киоскбровсерблоккедурлс</span><span class="sxs-lookup"><span data-stu-id="8787c-191">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="8787c-192">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8787c-192">String collection</span></span>|<span data-ttu-id="8787c-193">Указание URL-адресов, к которым не должны переходить браузеры киоска</span><span class="sxs-lookup"><span data-stu-id="8787c-193">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="8787c-194">Киоскбровсерблоккедурлексцептионс</span><span class="sxs-lookup"><span data-stu-id="8787c-194">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="8787c-195">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8787c-195">String collection</span></span>|<span data-ttu-id="8787c-196">Указание URL-адресов, на которые может перейти браузер с киоском</span><span class="sxs-lookup"><span data-stu-id="8787c-196">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="8787c-197">Еджекиоскенаблепубликбровсинг</span><span class="sxs-lookup"><span data-stu-id="8787c-197">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="8787c-198">Логический</span><span class="sxs-lookup"><span data-stu-id="8787c-198">Boolean</span></span>|<span data-ttu-id="8787c-199">Включение режима "общедоступный" в режиме киоска браузера для браузера Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="8787c-199">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="8787c-200">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="8787c-200">The Default is false.</span></span>|
|<span data-ttu-id="8787c-201">Еджекиоскресетафтеридлетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="8787c-201">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="8787c-202">Int32</span><span class="sxs-lookup"><span data-stu-id="8787c-202">Int32</span></span>|<span data-ttu-id="8787c-203">Задает время (в минутах) от последнего действия пользователя до сброса Microsoft Edge киоска.</span><span class="sxs-lookup"><span data-stu-id="8787c-203">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="8787c-204">Допустимые значения: 0-1440.</span><span class="sxs-lookup"><span data-stu-id="8787c-204">Valid values are 0-1440.</span></span> <span data-ttu-id="8787c-205">Значение по умолчанию — 5.</span><span class="sxs-lookup"><span data-stu-id="8787c-205">The default is 5.</span></span> <span data-ttu-id="8787c-206">0 указывает на отсутствие сброса.</span><span class="sxs-lookup"><span data-stu-id="8787c-206">0 indicates no reset.</span></span> <span data-ttu-id="8787c-207">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="8787c-207">Valid values 0 to 1440</span></span>|



## <a name="response"></a><span data-ttu-id="8787c-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="8787c-208">Response</span></span>
<span data-ttu-id="8787c-209">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8787c-209">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8787c-210">Пример</span><span class="sxs-lookup"><span data-stu-id="8787c-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="8787c-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="8787c-211">Request</span></span>
<span data-ttu-id="8787c-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8787c-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="8787c-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="8787c-213">Response</span></span>
<span data-ttu-id="8787c-p117">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8787c-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




