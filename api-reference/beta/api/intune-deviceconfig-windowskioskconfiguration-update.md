---
title: Обновление Виндовскиоскконфигуратион
description: Обновление свойств объекта Виндовскиоскконфигуратион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cee7c118ba4e78670c0fdef8dd512bcfdc063d5c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160545"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="58a3e-103">Обновление Виндовскиоскконфигуратион</span><span class="sxs-lookup"><span data-stu-id="58a3e-103">Update windowsKioskConfiguration</span></span>

> <span data-ttu-id="58a3e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58a3e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58a3e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58a3e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58a3e-106">Обновление свойств объекта [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="58a3e-106">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58a3e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="58a3e-107">Prerequisites</span></span>
<span data-ttu-id="58a3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="58a3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="58a3e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58a3e-110">Permission type</span></span>|<span data-ttu-id="58a3e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58a3e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58a3e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58a3e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58a3e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58a3e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="58a3e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58a3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58a3e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58a3e-115">Not supported.</span></span>|
|<span data-ttu-id="58a3e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58a3e-116">Application</span></span>|<span data-ttu-id="58a3e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58a3e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58a3e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58a3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="58a3e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58a3e-119">Request headers</span></span>
|<span data-ttu-id="58a3e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58a3e-120">Header</span></span>|<span data-ttu-id="58a3e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="58a3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58a3e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58a3e-122">Authorization</span></span>|<span data-ttu-id="58a3e-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="58a3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58a3e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="58a3e-124">Accept</span></span>|<span data-ttu-id="58a3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58a3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58a3e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58a3e-126">Request body</span></span>
<span data-ttu-id="58a3e-127">В тексте запроса добавьте представление объекта [Виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58a3e-127">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="58a3e-128">В следующей таблице приведены свойства, необходимые при создании [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58a3e-128">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="58a3e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="58a3e-129">Property</span></span>|<span data-ttu-id="58a3e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="58a3e-130">Type</span></span>|<span data-ttu-id="58a3e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="58a3e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58a3e-132">id</span><span class="sxs-lookup"><span data-stu-id="58a3e-132">id</span></span>|<span data-ttu-id="58a3e-133">String</span><span class="sxs-lookup"><span data-stu-id="58a3e-133">String</span></span>|<span data-ttu-id="58a3e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="58a3e-134">Key of the entity.</span></span> <span data-ttu-id="58a3e-135">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58a3e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58a3e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58a3e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="58a3e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a3e-137">DateTimeOffset</span></span>|<span data-ttu-id="58a3e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="58a3e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="58a3e-139">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58a3e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58a3e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="58a3e-140">roleScopeTagIds</span></span>|<span data-ttu-id="58a3e-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="58a3e-141">String collection</span></span>|<span data-ttu-id="58a3e-142">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="58a3e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="58a3e-143">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58a3e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58a3e-144">Суппортсскопетагс</span><span class="sxs-lookup"><span data-stu-id="58a3e-144">supportsScopeTags</span></span>|<span data-ttu-id="58a3e-145">Логический</span><span class="sxs-lookup"><span data-stu-id="58a3e-145">Boolean</span></span>|<span data-ttu-id="58a3e-146">Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области.</span><span class="sxs-lookup"><span data-stu-id="58a3e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="58a3e-147">Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия.</span><span class="sxs-lookup"><span data-stu-id="58a3e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="58a3e-148">Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="58a3e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="58a3e-149">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="58a3e-149">This property is read-only.</span></span> <span data-ttu-id="58a3e-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58a3e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58a3e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58a3e-151">createdDateTime</span></span>|<span data-ttu-id="58a3e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a3e-152">DateTimeOffset</span></span>|<span data-ttu-id="58a3e-153">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="58a3e-153">DateTime the object was created.</span></span> <span data-ttu-id="58a3e-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58a3e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58a3e-155">description</span><span class="sxs-lookup"><span data-stu-id="58a3e-155">description</span></span>|<span data-ttu-id="58a3e-156">String</span><span class="sxs-lookup"><span data-stu-id="58a3e-156">String</span></span>|<span data-ttu-id="58a3e-157">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="58a3e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="58a3e-158">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58a3e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58a3e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="58a3e-159">displayName</span></span>|<span data-ttu-id="58a3e-160">String</span><span class="sxs-lookup"><span data-stu-id="58a3e-160">String</span></span>|<span data-ttu-id="58a3e-161">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="58a3e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="58a3e-162">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58a3e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58a3e-163">version</span><span class="sxs-lookup"><span data-stu-id="58a3e-163">version</span></span>|<span data-ttu-id="58a3e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="58a3e-164">Int32</span></span>|<span data-ttu-id="58a3e-165">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="58a3e-165">Version of the device configuration.</span></span> <span data-ttu-id="58a3e-166">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="58a3e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="58a3e-167">Киоскпрофилес</span><span class="sxs-lookup"><span data-stu-id="58a3e-167">kioskProfiles</span></span>|<span data-ttu-id="58a3e-168">Коллекция [виндовскиоскпрофиле](../resources/intune-deviceconfig-windowskioskprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a3e-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="58a3e-169">Этот параметр политики позволяет определить список профилей киоска для конфигурации киоска.</span><span class="sxs-lookup"><span data-stu-id="58a3e-169">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="58a3e-170">Эта коллекция может содержать не более 3 элементов.</span><span class="sxs-lookup"><span data-stu-id="58a3e-170">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="58a3e-171">Киоскбровсердефаултурл</span><span class="sxs-lookup"><span data-stu-id="58a3e-171">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="58a3e-172">String</span><span class="sxs-lookup"><span data-stu-id="58a3e-172">String</span></span>|<span data-ttu-id="58a3e-173">Укажите URL-адрес по умолчанию, на который должен переходить браузер при запуске.</span><span class="sxs-lookup"><span data-stu-id="58a3e-173">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="58a3e-174">Киоскбровсеренаблехомебуттон</span><span class="sxs-lookup"><span data-stu-id="58a3e-174">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="58a3e-175">Логический</span><span class="sxs-lookup"><span data-stu-id="58a3e-175">Boolean</span></span>|<span data-ttu-id="58a3e-176">Включите кнопку Главная в браузере киоска.</span><span class="sxs-lookup"><span data-stu-id="58a3e-176">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="58a3e-177">По умолчанию кнопка "домой" отключена.</span><span class="sxs-lookup"><span data-stu-id="58a3e-177">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="58a3e-178">Киоскбровсеренабленавигатионбуттонс</span><span class="sxs-lookup"><span data-stu-id="58a3e-178">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="58a3e-179">Логический</span><span class="sxs-lookup"><span data-stu-id="58a3e-179">Boolean</span></span>|<span data-ttu-id="58a3e-180">Включение кнопок навигации в браузере киосков (вперед и назад).</span><span class="sxs-lookup"><span data-stu-id="58a3e-180">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="58a3e-181">По умолчанию кнопки навигации отключены.</span><span class="sxs-lookup"><span data-stu-id="58a3e-181">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="58a3e-182">Киоскбровсеренаблиндсессионбуттон</span><span class="sxs-lookup"><span data-stu-id="58a3e-182">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="58a3e-183">Логический</span><span class="sxs-lookup"><span data-stu-id="58a3e-183">Boolean</span></span>|<span data-ttu-id="58a3e-184">Включите кнопку End Session (завершить сеанс) в обозревателе киосков.</span><span class="sxs-lookup"><span data-stu-id="58a3e-184">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="58a3e-185">По умолчанию кнопка End Session отключена.</span><span class="sxs-lookup"><span data-stu-id="58a3e-185">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="58a3e-186">Киоскбровсеррестартонидлетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="58a3e-186">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="58a3e-187">Int32</span><span class="sxs-lookup"><span data-stu-id="58a3e-187">Int32</span></span>|<span data-ttu-id="58a3e-188">Укажите время в минутах, в течение которого сеанс простаивает до тех пор, пока обозреватель киоска не перезапустится в обновленном состоянии.</span><span class="sxs-lookup"><span data-stu-id="58a3e-188">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="58a3e-189">Допустимые значения: 1-1440.</span><span class="sxs-lookup"><span data-stu-id="58a3e-189">Valid values are 1-1440.</span></span> <span data-ttu-id="58a3e-190">Допустимые значения — от 1 до 1440</span><span class="sxs-lookup"><span data-stu-id="58a3e-190">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="58a3e-191">Киоскбровсерблоккедурлс</span><span class="sxs-lookup"><span data-stu-id="58a3e-191">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="58a3e-192">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="58a3e-192">String collection</span></span>|<span data-ttu-id="58a3e-193">Указание URL-адресов, к которым не должны переходить браузеры киоска</span><span class="sxs-lookup"><span data-stu-id="58a3e-193">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="58a3e-194">Киоскбровсерблоккедурлексцептионс</span><span class="sxs-lookup"><span data-stu-id="58a3e-194">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="58a3e-195">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="58a3e-195">String collection</span></span>|<span data-ttu-id="58a3e-196">Указание URL-адресов, на которые может перейти браузер с киоском</span><span class="sxs-lookup"><span data-stu-id="58a3e-196">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="58a3e-197">Еджекиоскенаблепубликбровсинг</span><span class="sxs-lookup"><span data-stu-id="58a3e-197">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="58a3e-198">Логический</span><span class="sxs-lookup"><span data-stu-id="58a3e-198">Boolean</span></span>|<span data-ttu-id="58a3e-199">Включение режима "общедоступный" в режиме киоска браузера для браузера Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="58a3e-199">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="58a3e-200">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="58a3e-200">The Default is false.</span></span>|
|<span data-ttu-id="58a3e-201">Еджекиоскресетафтеридлетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="58a3e-201">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="58a3e-202">Int32</span><span class="sxs-lookup"><span data-stu-id="58a3e-202">Int32</span></span>|<span data-ttu-id="58a3e-203">Задает время (в минутах) от последнего действия пользователя до сброса Microsoft Edge киоска.</span><span class="sxs-lookup"><span data-stu-id="58a3e-203">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="58a3e-204">Допустимые значения: 0-1440.</span><span class="sxs-lookup"><span data-stu-id="58a3e-204">Valid values are 0-1440.</span></span> <span data-ttu-id="58a3e-205">Значение по умолчанию — 5.</span><span class="sxs-lookup"><span data-stu-id="58a3e-205">The default is 5.</span></span> <span data-ttu-id="58a3e-206">0 указывает на отсутствие сброса.</span><span class="sxs-lookup"><span data-stu-id="58a3e-206">0 indicates no reset.</span></span> <span data-ttu-id="58a3e-207">Допустимые значения — от 0 до 1440</span><span class="sxs-lookup"><span data-stu-id="58a3e-207">Valid values 0 to 1440</span></span>|



## <a name="response"></a><span data-ttu-id="58a3e-208">Отклик</span><span class="sxs-lookup"><span data-stu-id="58a3e-208">Response</span></span>
<span data-ttu-id="58a3e-209">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовскиоскконфигуратион](../resources/intune-deviceconfig-windowskioskconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="58a3e-209">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a3e-210">Пример</span><span class="sxs-lookup"><span data-stu-id="58a3e-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="58a3e-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="58a3e-211">Request</span></span>
<span data-ttu-id="58a3e-212">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="58a3e-212">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58a3e-213">Отклик</span><span class="sxs-lookup"><span data-stu-id="58a3e-213">Response</span></span>
<span data-ttu-id="58a3e-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="58a3e-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




