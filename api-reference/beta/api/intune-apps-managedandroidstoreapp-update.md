---
title: Update managedAndroidStoreApp
description: Обновление свойств объекта managedAndroidStoreApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 07cd1d7ca6bbec237a853e8670437e07a06cb2a9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421048"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="cce13-103">Update managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="cce13-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="cce13-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cce13-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cce13-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cce13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cce13-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cce13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cce13-107">Обновление свойств объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-107">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cce13-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cce13-108">Prerequisites</span></span>
<span data-ttu-id="cce13-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cce13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cce13-111">Permission type</span></span>|<span data-ttu-id="cce13-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cce13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cce13-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cce13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cce13-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cce13-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cce13-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cce13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cce13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cce13-116">Not supported.</span></span>|
|<span data-ttu-id="cce13-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cce13-117">Application</span></span>|<span data-ttu-id="cce13-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cce13-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cce13-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cce13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="cce13-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cce13-120">Request headers</span></span>
|<span data-ttu-id="cce13-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cce13-121">Header</span></span>|<span data-ttu-id="cce13-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cce13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cce13-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cce13-123">Authorization</span></span>|<span data-ttu-id="cce13-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cce13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cce13-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cce13-125">Accept</span></span>|<span data-ttu-id="cce13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cce13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cce13-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cce13-127">Request body</span></span>
<span data-ttu-id="cce13-128">В теле запроса добавьте представление объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cce13-128">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="cce13-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-129">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="cce13-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cce13-130">Property</span></span>|<span data-ttu-id="cce13-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cce13-131">Type</span></span>|<span data-ttu-id="cce13-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cce13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cce13-133">id</span><span class="sxs-lookup"><span data-stu-id="cce13-133">id</span></span>|<span data-ttu-id="cce13-134">String</span><span class="sxs-lookup"><span data-stu-id="cce13-134">String</span></span>|<span data-ttu-id="cce13-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cce13-135">Key of the entity.</span></span> <span data-ttu-id="cce13-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cce13-137">displayName</span></span>|<span data-ttu-id="cce13-138">String</span><span class="sxs-lookup"><span data-stu-id="cce13-138">String</span></span>|<span data-ttu-id="cce13-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="cce13-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cce13-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-141">description</span><span class="sxs-lookup"><span data-stu-id="cce13-141">description</span></span>|<span data-ttu-id="cce13-142">String</span><span class="sxs-lookup"><span data-stu-id="cce13-142">String</span></span>|<span data-ttu-id="cce13-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="cce13-143">The description of the app.</span></span> <span data-ttu-id="cce13-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-145">publisher</span><span class="sxs-lookup"><span data-stu-id="cce13-145">publisher</span></span>|<span data-ttu-id="cce13-146">String</span><span class="sxs-lookup"><span data-stu-id="cce13-146">String</span></span>|<span data-ttu-id="cce13-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="cce13-147">The publisher of the app.</span></span> <span data-ttu-id="cce13-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cce13-149">largeIcon</span></span>|[<span data-ttu-id="cce13-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cce13-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cce13-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="cce13-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cce13-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cce13-153">createdDateTime</span></span>|<span data-ttu-id="cce13-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cce13-154">DateTimeOffset</span></span>|<span data-ttu-id="cce13-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="cce13-155">The date and time the app was created.</span></span> <span data-ttu-id="cce13-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cce13-157">lastModifiedDateTime</span></span>|<span data-ttu-id="cce13-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cce13-158">DateTimeOffset</span></span>|<span data-ttu-id="cce13-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="cce13-159">The date and time the app was last modified.</span></span> <span data-ttu-id="cce13-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cce13-161">isFeatured</span></span>|<span data-ttu-id="cce13-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="cce13-162">Boolean</span></span>|<span data-ttu-id="cce13-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cce13-164">privacyInformationUrl</span></span>|<span data-ttu-id="cce13-165">String</span><span class="sxs-lookup"><span data-stu-id="cce13-165">String</span></span>|<span data-ttu-id="cce13-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="cce13-166">The privacy statement Url.</span></span> <span data-ttu-id="cce13-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cce13-168">informationUrl</span></span>|<span data-ttu-id="cce13-169">String</span><span class="sxs-lookup"><span data-stu-id="cce13-169">String</span></span>|<span data-ttu-id="cce13-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="cce13-170">The more information Url.</span></span> <span data-ttu-id="cce13-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-172">owner</span><span class="sxs-lookup"><span data-stu-id="cce13-172">owner</span></span>|<span data-ttu-id="cce13-173">String</span><span class="sxs-lookup"><span data-stu-id="cce13-173">String</span></span>|<span data-ttu-id="cce13-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="cce13-174">The owner of the app.</span></span> <span data-ttu-id="cce13-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-176">developer</span><span class="sxs-lookup"><span data-stu-id="cce13-176">developer</span></span>|<span data-ttu-id="cce13-177">String</span><span class="sxs-lookup"><span data-stu-id="cce13-177">String</span></span>|<span data-ttu-id="cce13-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="cce13-178">The developer of the app.</span></span> <span data-ttu-id="cce13-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-180">notes</span><span class="sxs-lookup"><span data-stu-id="cce13-180">notes</span></span>|<span data-ttu-id="cce13-181">String</span><span class="sxs-lookup"><span data-stu-id="cce13-181">String</span></span>|<span data-ttu-id="cce13-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="cce13-182">Notes for the app.</span></span> <span data-ttu-id="cce13-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="cce13-184">uploadState</span></span>|<span data-ttu-id="cce13-185">Int32</span><span class="sxs-lookup"><span data-stu-id="cce13-185">Int32</span></span>|<span data-ttu-id="cce13-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="cce13-186">The upload state.</span></span> <span data-ttu-id="cce13-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="cce13-188">publishingState</span></span>|[<span data-ttu-id="cce13-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cce13-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cce13-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="cce13-190">The publishing state for the app.</span></span> <span data-ttu-id="cce13-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="cce13-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cce13-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cce13-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="cce13-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cce13-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cce13-194">isAssigned</span></span>|<span data-ttu-id="cce13-195">Логический</span><span class="sxs-lookup"><span data-stu-id="cce13-195">Boolean</span></span>|<span data-ttu-id="cce13-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="cce13-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cce13-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cce13-198">roleScopeTagIds</span></span>|<span data-ttu-id="cce13-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="cce13-199">String collection</span></span>|<span data-ttu-id="cce13-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="cce13-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cce13-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cce13-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="cce13-202">appAvailability</span></span>|[<span data-ttu-id="cce13-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="cce13-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="cce13-204">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="cce13-204">The Application's availability.</span></span> <span data-ttu-id="cce13-205">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="cce13-206">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="cce13-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="cce13-207">version</span><span class="sxs-lookup"><span data-stu-id="cce13-207">version</span></span>|<span data-ttu-id="cce13-208">String</span><span class="sxs-lookup"><span data-stu-id="cce13-208">String</span></span>|<span data-ttu-id="cce13-209">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="cce13-209">The Application's version.</span></span> <span data-ttu-id="cce13-210">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="cce13-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="cce13-211">packageId</span><span class="sxs-lookup"><span data-stu-id="cce13-211">packageId</span></span>|<span data-ttu-id="cce13-212">String</span><span class="sxs-lookup"><span data-stu-id="cce13-212">String</span></span>|<span data-ttu-id="cce13-213">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="cce13-213">The app's package ID.</span></span>|
|<span data-ttu-id="cce13-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="cce13-214">appStoreUrl</span></span>|<span data-ttu-id="cce13-215">String</span><span class="sxs-lookup"><span data-stu-id="cce13-215">String</span></span>|<span data-ttu-id="cce13-216">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="cce13-216">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="cce13-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cce13-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cce13-218">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cce13-218">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="cce13-219">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="cce13-219">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="cce13-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="cce13-220">Response</span></span>
<span data-ttu-id="cce13-221">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cce13-221">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cce13-222">Пример</span><span class="sxs-lookup"><span data-stu-id="cce13-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="cce13-223">Запрос</span><span class="sxs-lookup"><span data-stu-id="cce13-223">Request</span></span>
<span data-ttu-id="cce13-224">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cce13-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1237

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="cce13-225">Отклик</span><span class="sxs-lookup"><span data-stu-id="cce13-225">Response</span></span>
<span data-ttu-id="cce13-p121">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cce13-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1409

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```




