---
title: Обновление managedIOSStoreApp
description: Обновляет свойства объекта managedIOSStoreApp.
ms.openlocfilehash: f65cfb1c45b376db753c73c3fe1fa58b0f5af309
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075007"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="9b64c-103">Обновление managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="9b64c-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="9b64c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9b64c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9b64c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b64c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9b64c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9b64c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b64c-107">Обновляет свойства объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-107">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b64c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9b64c-108">Prerequisites</span></span>
<span data-ttu-id="9b64c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b64c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b64c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b64c-111">Permission type</span></span>|<span data-ttu-id="9b64c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b64c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b64c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b64c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9b64c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b64c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9b64c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b64c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b64c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b64c-116">Not supported.</span></span>|
|<span data-ttu-id="9b64c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b64c-117">Application</span></span>|<span data-ttu-id="9b64c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b64c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b64c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b64c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9b64c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b64c-120">Request headers</span></span>
|<span data-ttu-id="9b64c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b64c-121">Header</span></span>|<span data-ttu-id="9b64c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9b64c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b64c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b64c-123">Authorization</span></span>|<span data-ttu-id="9b64c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9b64c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b64c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9b64c-125">Accept</span></span>|<span data-ttu-id="9b64c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9b64c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b64c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b64c-127">Request body</span></span>
<span data-ttu-id="9b64c-128">В теле запроса добавьте представление объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b64c-128">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="9b64c-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-129">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="9b64c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b64c-130">Property</span></span>|<span data-ttu-id="9b64c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9b64c-131">Type</span></span>|<span data-ttu-id="9b64c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9b64c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b64c-133">id</span><span class="sxs-lookup"><span data-stu-id="9b64c-133">id</span></span>|<span data-ttu-id="9b64c-134">String</span><span class="sxs-lookup"><span data-stu-id="9b64c-134">String</span></span>|<span data-ttu-id="9b64c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9b64c-135">Key of the entity.</span></span> <span data-ttu-id="9b64c-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9b64c-137">displayName</span></span>|<span data-ttu-id="9b64c-138">String</span><span class="sxs-lookup"><span data-stu-id="9b64c-138">String</span></span>|<span data-ttu-id="9b64c-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9b64c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9b64c-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-141">описание</span><span class="sxs-lookup"><span data-stu-id="9b64c-141">description</span></span>|<span data-ttu-id="9b64c-142">String</span><span class="sxs-lookup"><span data-stu-id="9b64c-142">String</span></span>|<span data-ttu-id="9b64c-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9b64c-143">The description of the app.</span></span> <span data-ttu-id="9b64c-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-145">publisher</span><span class="sxs-lookup"><span data-stu-id="9b64c-145">publisher</span></span>|<span data-ttu-id="9b64c-146">String</span><span class="sxs-lookup"><span data-stu-id="9b64c-146">String</span></span>|<span data-ttu-id="9b64c-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9b64c-147">The publisher of the app.</span></span> <span data-ttu-id="9b64c-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9b64c-149">largeIcon</span></span>|[<span data-ttu-id="9b64c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9b64c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9b64c-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9b64c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9b64c-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b64c-153">createdDateTime</span></span>|<span data-ttu-id="9b64c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b64c-154">DateTimeOffset</span></span>|<span data-ttu-id="9b64c-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9b64c-155">The date and time the app was created.</span></span> <span data-ttu-id="9b64c-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b64c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9b64c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b64c-158">DateTimeOffset</span></span>|<span data-ttu-id="9b64c-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9b64c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9b64c-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9b64c-161">isFeatured</span></span>|<span data-ttu-id="9b64c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b64c-162">Boolean</span></span>|<span data-ttu-id="9b64c-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9b64c-164">privacyInformationUrl</span></span>|<span data-ttu-id="9b64c-165">String</span><span class="sxs-lookup"><span data-stu-id="9b64c-165">String</span></span>|<span data-ttu-id="9b64c-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9b64c-166">The privacy statement Url.</span></span> <span data-ttu-id="9b64c-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9b64c-168">informationUrl</span></span>|<span data-ttu-id="9b64c-169">String</span><span class="sxs-lookup"><span data-stu-id="9b64c-169">String</span></span>|<span data-ttu-id="9b64c-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9b64c-170">The more information Url.</span></span> <span data-ttu-id="9b64c-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-172">owner</span><span class="sxs-lookup"><span data-stu-id="9b64c-172">owner</span></span>|<span data-ttu-id="9b64c-173">String</span><span class="sxs-lookup"><span data-stu-id="9b64c-173">String</span></span>|<span data-ttu-id="9b64c-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9b64c-174">The owner of the app.</span></span> <span data-ttu-id="9b64c-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-176">developer</span><span class="sxs-lookup"><span data-stu-id="9b64c-176">developer</span></span>|<span data-ttu-id="9b64c-177">String</span><span class="sxs-lookup"><span data-stu-id="9b64c-177">String</span></span>|<span data-ttu-id="9b64c-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9b64c-178">The developer of the app.</span></span> <span data-ttu-id="9b64c-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-180">notes</span><span class="sxs-lookup"><span data-stu-id="9b64c-180">notes</span></span>|<span data-ttu-id="9b64c-181">String</span><span class="sxs-lookup"><span data-stu-id="9b64c-181">String</span></span>|<span data-ttu-id="9b64c-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="9b64c-182">Notes for the app.</span></span> <span data-ttu-id="9b64c-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9b64c-184">uploadState</span></span>|<span data-ttu-id="9b64c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9b64c-185">Int32</span></span>|<span data-ttu-id="9b64c-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="9b64c-186">The upload state.</span></span> <span data-ttu-id="9b64c-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9b64c-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="9b64c-188">publishingState</span></span>|[<span data-ttu-id="9b64c-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9b64c-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9b64c-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="9b64c-190">The publishing state for the app.</span></span> <span data-ttu-id="9b64c-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9b64c-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9b64c-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9b64c-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9b64c-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9b64c-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="9b64c-194">appAvailability</span></span>|[<span data-ttu-id="9b64c-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="9b64c-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="9b64c-196">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="9b64c-196">The Application's availability.</span></span> <span data-ttu-id="9b64c-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9b64c-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="9b64c-198">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="9b64c-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="9b64c-199">version</span><span class="sxs-lookup"><span data-stu-id="9b64c-199">version</span></span>|<span data-ttu-id="9b64c-200">String</span><span class="sxs-lookup"><span data-stu-id="9b64c-200">String</span></span>|<span data-ttu-id="9b64c-201">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="9b64c-201">The Application's version.</span></span> <span data-ttu-id="9b64c-202">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="9b64c-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="9b64c-203">bundleId</span><span class="sxs-lookup"><span data-stu-id="9b64c-203">bundleId</span></span>|<span data-ttu-id="9b64c-204">String</span><span class="sxs-lookup"><span data-stu-id="9b64c-204">String</span></span>|<span data-ttu-id="9b64c-205">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="9b64c-205">The app's Bundle ID.</span></span>|
|<span data-ttu-id="9b64c-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9b64c-206">appStoreUrl</span></span>|<span data-ttu-id="9b64c-207">String</span><span class="sxs-lookup"><span data-stu-id="9b64c-207">String</span></span>|<span data-ttu-id="9b64c-208">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="9b64c-208">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="9b64c-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9b64c-209">applicableDeviceType</span></span>|[<span data-ttu-id="9b64c-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9b64c-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="9b64c-211">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="9b64c-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="9b64c-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9b64c-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9b64c-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9b64c-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="9b64c-214">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="9b64c-214">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="9b64c-215">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b64c-215">Response</span></span>
<span data-ttu-id="9b64c-216">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9b64c-216">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b64c-217">Пример</span><span class="sxs-lookup"><span data-stu-id="9b64c-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b64c-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b64c-218">Request</span></span>
<span data-ttu-id="9b64c-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b64c-219">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9b64c-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="9b64c-220">Response</span></span>
<span data-ttu-id="9b64c-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9b64c-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





