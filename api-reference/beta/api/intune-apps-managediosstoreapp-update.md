---
title: Обновление managedIOSStoreApp
description: Обновляет свойства объекта managedIOSStoreApp.
author: tfitzmac
ms.openlocfilehash: 27c91f6c22031ac7d4bfe9a69a339652104e025c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305105"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="e3a73-103">Обновление managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="e3a73-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="e3a73-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e3a73-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3a73-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3a73-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e3a73-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3a73-107">Обновляет свойства объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-107">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3a73-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e3a73-108">Prerequisites</span></span>
<span data-ttu-id="e3a73-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3a73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3a73-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3a73-111">Permission type</span></span>|<span data-ttu-id="e3a73-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3a73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3a73-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3a73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3a73-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3a73-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3a73-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3a73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3a73-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a73-116">Not supported.</span></span>|
|<span data-ttu-id="e3a73-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3a73-117">Application</span></span>|<span data-ttu-id="e3a73-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a73-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3a73-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3a73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e3a73-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3a73-120">Request headers</span></span>
|<span data-ttu-id="e3a73-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e3a73-121">Header</span></span>|<span data-ttu-id="e3a73-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e3a73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3a73-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3a73-123">Authorization</span></span>|<span data-ttu-id="e3a73-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e3a73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3a73-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3a73-125">Accept</span></span>|<span data-ttu-id="e3a73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3a73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3a73-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3a73-127">Request body</span></span>
<span data-ttu-id="e3a73-128">В теле запроса добавьте представление объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3a73-128">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="e3a73-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-129">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="e3a73-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3a73-130">Property</span></span>|<span data-ttu-id="e3a73-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e3a73-131">Type</span></span>|<span data-ttu-id="e3a73-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e3a73-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3a73-133">id</span><span class="sxs-lookup"><span data-stu-id="e3a73-133">id</span></span>|<span data-ttu-id="e3a73-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e3a73-134">String</span></span>|<span data-ttu-id="e3a73-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e3a73-135">Key of the entity.</span></span> <span data-ttu-id="e3a73-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e3a73-137">displayName</span></span>|<span data-ttu-id="e3a73-138">String</span><span class="sxs-lookup"><span data-stu-id="e3a73-138">String</span></span>|<span data-ttu-id="e3a73-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e3a73-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e3a73-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-141">описание</span><span class="sxs-lookup"><span data-stu-id="e3a73-141">description</span></span>|<span data-ttu-id="e3a73-142">String</span><span class="sxs-lookup"><span data-stu-id="e3a73-142">String</span></span>|<span data-ttu-id="e3a73-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e3a73-143">The description of the app.</span></span> <span data-ttu-id="e3a73-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e3a73-145">publisher</span></span>|<span data-ttu-id="e3a73-146">String</span><span class="sxs-lookup"><span data-stu-id="e3a73-146">String</span></span>|<span data-ttu-id="e3a73-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e3a73-147">The publisher of the app.</span></span> <span data-ttu-id="e3a73-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e3a73-149">largeIcon</span></span>|[<span data-ttu-id="e3a73-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e3a73-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e3a73-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e3a73-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e3a73-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3a73-153">createdDateTime</span></span>|<span data-ttu-id="e3a73-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3a73-154">DateTimeOffset</span></span>|<span data-ttu-id="e3a73-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e3a73-155">The date and time the app was created.</span></span> <span data-ttu-id="e3a73-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3a73-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e3a73-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3a73-158">DateTimeOffset</span></span>|<span data-ttu-id="e3a73-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e3a73-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e3a73-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e3a73-161">isFeatured</span></span>|<span data-ttu-id="e3a73-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3a73-162">Boolean</span></span>|<span data-ttu-id="e3a73-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e3a73-164">privacyInformationUrl</span></span>|<span data-ttu-id="e3a73-165">String</span><span class="sxs-lookup"><span data-stu-id="e3a73-165">String</span></span>|<span data-ttu-id="e3a73-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e3a73-166">The privacy statement Url.</span></span> <span data-ttu-id="e3a73-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e3a73-168">informationUrl</span></span>|<span data-ttu-id="e3a73-169">String</span><span class="sxs-lookup"><span data-stu-id="e3a73-169">String</span></span>|<span data-ttu-id="e3a73-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e3a73-170">The more information Url.</span></span> <span data-ttu-id="e3a73-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-172">owner</span><span class="sxs-lookup"><span data-stu-id="e3a73-172">owner</span></span>|<span data-ttu-id="e3a73-173">String</span><span class="sxs-lookup"><span data-stu-id="e3a73-173">String</span></span>|<span data-ttu-id="e3a73-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e3a73-174">The owner of the app.</span></span> <span data-ttu-id="e3a73-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-176">developer</span><span class="sxs-lookup"><span data-stu-id="e3a73-176">developer</span></span>|<span data-ttu-id="e3a73-177">String</span><span class="sxs-lookup"><span data-stu-id="e3a73-177">String</span></span>|<span data-ttu-id="e3a73-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e3a73-178">The developer of the app.</span></span> <span data-ttu-id="e3a73-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-180">notes</span><span class="sxs-lookup"><span data-stu-id="e3a73-180">notes</span></span>|<span data-ttu-id="e3a73-181">String</span><span class="sxs-lookup"><span data-stu-id="e3a73-181">String</span></span>|<span data-ttu-id="e3a73-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="e3a73-182">Notes for the app.</span></span> <span data-ttu-id="e3a73-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e3a73-184">uploadState</span></span>|<span data-ttu-id="e3a73-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e3a73-185">Int32</span></span>|<span data-ttu-id="e3a73-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="e3a73-186">The upload state.</span></span> <span data-ttu-id="e3a73-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e3a73-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="e3a73-188">publishingState</span></span>|[<span data-ttu-id="e3a73-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e3a73-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e3a73-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="e3a73-190">The publishing state for the app.</span></span> <span data-ttu-id="e3a73-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e3a73-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e3a73-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e3a73-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e3a73-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e3a73-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="e3a73-194">appAvailability</span></span>|[<span data-ttu-id="e3a73-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="e3a73-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="e3a73-196">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="e3a73-196">The Application's availability.</span></span> <span data-ttu-id="e3a73-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e3a73-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="e3a73-198">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="e3a73-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="e3a73-199">version</span><span class="sxs-lookup"><span data-stu-id="e3a73-199">version</span></span>|<span data-ttu-id="e3a73-200">String</span><span class="sxs-lookup"><span data-stu-id="e3a73-200">String</span></span>|<span data-ttu-id="e3a73-201">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="e3a73-201">The Application's version.</span></span> <span data-ttu-id="e3a73-202">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="e3a73-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="e3a73-203">bundleId</span><span class="sxs-lookup"><span data-stu-id="e3a73-203">bundleId</span></span>|<span data-ttu-id="e3a73-204">String</span><span class="sxs-lookup"><span data-stu-id="e3a73-204">String</span></span>|<span data-ttu-id="e3a73-205">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="e3a73-205">The app's Bundle ID.</span></span>|
|<span data-ttu-id="e3a73-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e3a73-206">appStoreUrl</span></span>|<span data-ttu-id="e3a73-207">String</span><span class="sxs-lookup"><span data-stu-id="e3a73-207">String</span></span>|<span data-ttu-id="e3a73-208">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="e3a73-208">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="e3a73-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="e3a73-209">applicableDeviceType</span></span>|[<span data-ttu-id="e3a73-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="e3a73-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="e3a73-211">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="e3a73-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="e3a73-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e3a73-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e3a73-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e3a73-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="e3a73-214">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e3a73-214">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="e3a73-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3a73-215">Response</span></span>
<span data-ttu-id="e3a73-216">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e3a73-216">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3a73-217">Пример</span><span class="sxs-lookup"><span data-stu-id="e3a73-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3a73-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3a73-218">Request</span></span>
<span data-ttu-id="e3a73-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e3a73-219">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e3a73-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3a73-220">Response</span></span>
<span data-ttu-id="e3a73-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e3a73-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





