---
title: Обновление managedIOSStoreApp
description: Обновляет свойства объекта managedIOSStoreApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e7f46d334eb1842b96d764d1e7865a6840978965
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825062"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="e4ec8-103">Обновление managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="e4ec8-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="e4ec8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4ec8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4ec8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4ec8-107">Обновляет свойства объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-107">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4ec8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e4ec8-108">Prerequisites</span></span>
<span data-ttu-id="e4ec8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4ec8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4ec8-111">Permission type</span></span>|<span data-ttu-id="e4ec8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4ec8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4ec8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4ec8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4ec8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4ec8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e4ec8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4ec8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4ec8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-116">Not supported.</span></span>|
|<span data-ttu-id="e4ec8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4ec8-117">Application</span></span>|<span data-ttu-id="e4ec8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4ec8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4ec8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e4ec8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4ec8-120">Request headers</span></span>
|<span data-ttu-id="e4ec8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4ec8-121">Header</span></span>|<span data-ttu-id="e4ec8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e4ec8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4ec8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4ec8-123">Authorization</span></span>|<span data-ttu-id="e4ec8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e4ec8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4ec8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4ec8-125">Accept</span></span>|<span data-ttu-id="e4ec8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4ec8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4ec8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4ec8-127">Request body</span></span>
<span data-ttu-id="e4ec8-128">В теле запроса добавьте представление объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-128">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="e4ec8-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-129">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="e4ec8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4ec8-130">Property</span></span>|<span data-ttu-id="e4ec8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e4ec8-131">Type</span></span>|<span data-ttu-id="e4ec8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e4ec8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4ec8-133">id</span><span class="sxs-lookup"><span data-stu-id="e4ec8-133">id</span></span>|<span data-ttu-id="e4ec8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e4ec8-134">String</span></span>|<span data-ttu-id="e4ec8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-135">Key of the entity.</span></span> <span data-ttu-id="e4ec8-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e4ec8-137">displayName</span></span>|<span data-ttu-id="e4ec8-138">String</span><span class="sxs-lookup"><span data-stu-id="e4ec8-138">String</span></span>|<span data-ttu-id="e4ec8-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e4ec8-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-141">описание</span><span class="sxs-lookup"><span data-stu-id="e4ec8-141">description</span></span>|<span data-ttu-id="e4ec8-142">String</span><span class="sxs-lookup"><span data-stu-id="e4ec8-142">String</span></span>|<span data-ttu-id="e4ec8-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-143">The description of the app.</span></span> <span data-ttu-id="e4ec8-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e4ec8-145">publisher</span></span>|<span data-ttu-id="e4ec8-146">String</span><span class="sxs-lookup"><span data-stu-id="e4ec8-146">String</span></span>|<span data-ttu-id="e4ec8-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-147">The publisher of the app.</span></span> <span data-ttu-id="e4ec8-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e4ec8-149">largeIcon</span></span>|[<span data-ttu-id="e4ec8-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e4ec8-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e4ec8-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e4ec8-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4ec8-153">createdDateTime</span></span>|<span data-ttu-id="e4ec8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4ec8-154">DateTimeOffset</span></span>|<span data-ttu-id="e4ec8-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-155">The date and time the app was created.</span></span> <span data-ttu-id="e4ec8-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4ec8-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e4ec8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4ec8-158">DateTimeOffset</span></span>|<span data-ttu-id="e4ec8-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e4ec8-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e4ec8-161">isFeatured</span></span>|<span data-ttu-id="e4ec8-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4ec8-162">Boolean</span></span>|<span data-ttu-id="e4ec8-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e4ec8-164">privacyInformationUrl</span></span>|<span data-ttu-id="e4ec8-165">String</span><span class="sxs-lookup"><span data-stu-id="e4ec8-165">String</span></span>|<span data-ttu-id="e4ec8-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-166">The privacy statement Url.</span></span> <span data-ttu-id="e4ec8-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e4ec8-168">informationUrl</span></span>|<span data-ttu-id="e4ec8-169">String</span><span class="sxs-lookup"><span data-stu-id="e4ec8-169">String</span></span>|<span data-ttu-id="e4ec8-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-170">The more information Url.</span></span> <span data-ttu-id="e4ec8-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-172">owner</span><span class="sxs-lookup"><span data-stu-id="e4ec8-172">owner</span></span>|<span data-ttu-id="e4ec8-173">String</span><span class="sxs-lookup"><span data-stu-id="e4ec8-173">String</span></span>|<span data-ttu-id="e4ec8-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-174">The owner of the app.</span></span> <span data-ttu-id="e4ec8-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-176">developer</span><span class="sxs-lookup"><span data-stu-id="e4ec8-176">developer</span></span>|<span data-ttu-id="e4ec8-177">String</span><span class="sxs-lookup"><span data-stu-id="e4ec8-177">String</span></span>|<span data-ttu-id="e4ec8-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-178">The developer of the app.</span></span> <span data-ttu-id="e4ec8-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-180">notes</span><span class="sxs-lookup"><span data-stu-id="e4ec8-180">notes</span></span>|<span data-ttu-id="e4ec8-181">String</span><span class="sxs-lookup"><span data-stu-id="e4ec8-181">String</span></span>|<span data-ttu-id="e4ec8-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-182">Notes for the app.</span></span> <span data-ttu-id="e4ec8-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e4ec8-184">uploadState</span></span>|<span data-ttu-id="e4ec8-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ec8-185">Int32</span></span>|<span data-ttu-id="e4ec8-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-186">The upload state.</span></span> <span data-ttu-id="e4ec8-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e4ec8-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="e4ec8-188">publishingState</span></span>|[<span data-ttu-id="e4ec8-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e4ec8-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e4ec8-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-190">The publishing state for the app.</span></span> <span data-ttu-id="e4ec8-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e4ec8-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e4ec8-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e4ec8-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="e4ec8-194">appAvailability</span></span>|[<span data-ttu-id="e4ec8-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="e4ec8-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="e4ec8-196">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-196">The Application's availability.</span></span> <span data-ttu-id="e4ec8-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e4ec8-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="e4ec8-198">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="e4ec8-199">version</span><span class="sxs-lookup"><span data-stu-id="e4ec8-199">version</span></span>|<span data-ttu-id="e4ec8-200">String</span><span class="sxs-lookup"><span data-stu-id="e4ec8-200">String</span></span>|<span data-ttu-id="e4ec8-201">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-201">The Application's version.</span></span> <span data-ttu-id="e4ec8-202">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4ec8-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="e4ec8-203">bundleId</span><span class="sxs-lookup"><span data-stu-id="e4ec8-203">bundleId</span></span>|<span data-ttu-id="e4ec8-204">String</span><span class="sxs-lookup"><span data-stu-id="e4ec8-204">String</span></span>|<span data-ttu-id="e4ec8-205">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-205">The app's Bundle ID.</span></span>|
|<span data-ttu-id="e4ec8-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e4ec8-206">appStoreUrl</span></span>|<span data-ttu-id="e4ec8-207">String</span><span class="sxs-lookup"><span data-stu-id="e4ec8-207">String</span></span>|<span data-ttu-id="e4ec8-208">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-208">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="e4ec8-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="e4ec8-209">applicableDeviceType</span></span>|[<span data-ttu-id="e4ec8-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="e4ec8-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="e4ec8-211">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="e4ec8-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e4ec8-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e4ec8-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e4ec8-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="e4ec8-214">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-214">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="e4ec8-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4ec8-215">Response</span></span>
<span data-ttu-id="e4ec8-216">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-216">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4ec8-217">Пример</span><span class="sxs-lookup"><span data-stu-id="e4ec8-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4ec8-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4ec8-218">Request</span></span>
<span data-ttu-id="e4ec8-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1113

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="e4ec8-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4ec8-220">Response</span></span>
<span data-ttu-id="e4ec8-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e4ec8-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1278

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```





