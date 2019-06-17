---
title: Update managedAndroidStoreApp
description: Обновление свойств объекта managedAndroidStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e635cac001a7c4283da931845e314fcb5ff1406
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974939"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="0f7fe-103">Update managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="0f7fe-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="0f7fe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f7fe-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f7fe-106">Обновление свойств объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-106">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f7fe-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0f7fe-107">Prerequisites</span></span>
<span data-ttu-id="0f7fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f7fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f7fe-110">Permission type</span></span>|<span data-ttu-id="0f7fe-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f7fe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f7fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f7fe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f7fe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f7fe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f7fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f7fe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f7fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-115">Not supported.</span></span>|
|<span data-ttu-id="0f7fe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0f7fe-116">Application</span></span>|<span data-ttu-id="0f7fe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f7fe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f7fe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="0f7fe-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f7fe-119">Request headers</span></span>
|<span data-ttu-id="0f7fe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0f7fe-120">Header</span></span>|<span data-ttu-id="0f7fe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0f7fe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f7fe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f7fe-122">Authorization</span></span>|<span data-ttu-id="0f7fe-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f7fe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0f7fe-124">Accept</span></span>|<span data-ttu-id="0f7fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f7fe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f7fe-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0f7fe-126">Request body</span></span>
<span data-ttu-id="0f7fe-127">В теле запроса добавьте представление объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-127">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="0f7fe-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-128">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="0f7fe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f7fe-129">Property</span></span>|<span data-ttu-id="0f7fe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0f7fe-130">Type</span></span>|<span data-ttu-id="0f7fe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0f7fe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f7fe-132">id</span><span class="sxs-lookup"><span data-stu-id="0f7fe-132">id</span></span>|<span data-ttu-id="0f7fe-133">Строка</span><span class="sxs-lookup"><span data-stu-id="0f7fe-133">String</span></span>|<span data-ttu-id="0f7fe-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-134">Key of the entity.</span></span> <span data-ttu-id="0f7fe-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0f7fe-136">displayName</span></span>|<span data-ttu-id="0f7fe-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0f7fe-137">String</span></span>|<span data-ttu-id="0f7fe-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0f7fe-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-140">description</span><span class="sxs-lookup"><span data-stu-id="0f7fe-140">description</span></span>|<span data-ttu-id="0f7fe-141">String</span><span class="sxs-lookup"><span data-stu-id="0f7fe-141">String</span></span>|<span data-ttu-id="0f7fe-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-142">The description of the app.</span></span> <span data-ttu-id="0f7fe-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-144">publisher</span><span class="sxs-lookup"><span data-stu-id="0f7fe-144">publisher</span></span>|<span data-ttu-id="0f7fe-145">String</span><span class="sxs-lookup"><span data-stu-id="0f7fe-145">String</span></span>|<span data-ttu-id="0f7fe-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-146">The publisher of the app.</span></span> <span data-ttu-id="0f7fe-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0f7fe-148">largeIcon</span></span>|[<span data-ttu-id="0f7fe-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f7fe-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0f7fe-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0f7fe-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f7fe-152">createdDateTime</span></span>|<span data-ttu-id="0f7fe-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f7fe-153">DateTimeOffset</span></span>|<span data-ttu-id="0f7fe-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-154">The date and time the app was created.</span></span> <span data-ttu-id="0f7fe-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f7fe-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0f7fe-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f7fe-157">DateTimeOffset</span></span>|<span data-ttu-id="0f7fe-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0f7fe-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0f7fe-160">isFeatured</span></span>|<span data-ttu-id="0f7fe-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f7fe-161">Boolean</span></span>|<span data-ttu-id="0f7fe-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0f7fe-163">privacyInformationUrl</span></span>|<span data-ttu-id="0f7fe-164">String</span><span class="sxs-lookup"><span data-stu-id="0f7fe-164">String</span></span>|<span data-ttu-id="0f7fe-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-165">The privacy statement Url.</span></span> <span data-ttu-id="0f7fe-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0f7fe-167">informationUrl</span></span>|<span data-ttu-id="0f7fe-168">String</span><span class="sxs-lookup"><span data-stu-id="0f7fe-168">String</span></span>|<span data-ttu-id="0f7fe-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-169">The more information Url.</span></span> <span data-ttu-id="0f7fe-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-171">owner</span><span class="sxs-lookup"><span data-stu-id="0f7fe-171">owner</span></span>|<span data-ttu-id="0f7fe-172">String</span><span class="sxs-lookup"><span data-stu-id="0f7fe-172">String</span></span>|<span data-ttu-id="0f7fe-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-173">The owner of the app.</span></span> <span data-ttu-id="0f7fe-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-175">developer</span><span class="sxs-lookup"><span data-stu-id="0f7fe-175">developer</span></span>|<span data-ttu-id="0f7fe-176">String</span><span class="sxs-lookup"><span data-stu-id="0f7fe-176">String</span></span>|<span data-ttu-id="0f7fe-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-177">The developer of the app.</span></span> <span data-ttu-id="0f7fe-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-179">notes</span><span class="sxs-lookup"><span data-stu-id="0f7fe-179">notes</span></span>|<span data-ttu-id="0f7fe-180">String</span><span class="sxs-lookup"><span data-stu-id="0f7fe-180">String</span></span>|<span data-ttu-id="0f7fe-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-181">Notes for the app.</span></span> <span data-ttu-id="0f7fe-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="0f7fe-183">uploadState</span></span>|<span data-ttu-id="0f7fe-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0f7fe-184">Int32</span></span>|<span data-ttu-id="0f7fe-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-185">The upload state.</span></span> <span data-ttu-id="0f7fe-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="0f7fe-187">publishingState</span></span>|[<span data-ttu-id="0f7fe-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="0f7fe-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0f7fe-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-189">The publishing state for the app.</span></span> <span data-ttu-id="0f7fe-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0f7fe-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0f7fe-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0f7fe-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0f7fe-193">isAssigned</span></span>|<span data-ttu-id="0f7fe-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f7fe-194">Boolean</span></span>|<span data-ttu-id="0f7fe-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0f7fe-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f7fe-197">roleScopeTagIds</span></span>|<span data-ttu-id="0f7fe-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0f7fe-198">String collection</span></span>|<span data-ttu-id="0f7fe-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0f7fe-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="0f7fe-201">dependentAppCount</span></span>|<span data-ttu-id="0f7fe-202">Int32</span><span class="sxs-lookup"><span data-stu-id="0f7fe-202">Int32</span></span>|<span data-ttu-id="0f7fe-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="0f7fe-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f7fe-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="0f7fe-205">appAvailability</span></span>|[<span data-ttu-id="0f7fe-206">Манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="0f7fe-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="0f7fe-207">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-207">The Application's availability.</span></span> <span data-ttu-id="0f7fe-208">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="0f7fe-209">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="0f7fe-210">version</span><span class="sxs-lookup"><span data-stu-id="0f7fe-210">version</span></span>|<span data-ttu-id="0f7fe-211">String</span><span class="sxs-lookup"><span data-stu-id="0f7fe-211">String</span></span>|<span data-ttu-id="0f7fe-212">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-212">The Application's version.</span></span> <span data-ttu-id="0f7fe-213">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f7fe-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="0f7fe-214">packageId</span><span class="sxs-lookup"><span data-stu-id="0f7fe-214">packageId</span></span>|<span data-ttu-id="0f7fe-215">String</span><span class="sxs-lookup"><span data-stu-id="0f7fe-215">String</span></span>|<span data-ttu-id="0f7fe-216">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-216">The app's package ID.</span></span>|
|<span data-ttu-id="0f7fe-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0f7fe-217">appStoreUrl</span></span>|<span data-ttu-id="0f7fe-218">String</span><span class="sxs-lookup"><span data-stu-id="0f7fe-218">String</span></span>|<span data-ttu-id="0f7fe-219">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-219">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="0f7fe-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0f7fe-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0f7fe-221">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0f7fe-221">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="0f7fe-222">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-222">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="0f7fe-223">Ответ</span><span class="sxs-lookup"><span data-stu-id="0f7fe-223">Response</span></span>
<span data-ttu-id="0f7fe-224">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-224">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f7fe-225">Пример</span><span class="sxs-lookup"><span data-stu-id="0f7fe-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f7fe-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f7fe-226">Request</span></span>
<span data-ttu-id="0f7fe-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1264

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
  "dependentAppCount": 1,
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

### <a name="response"></a><span data-ttu-id="0f7fe-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f7fe-228">Response</span></span>
<span data-ttu-id="0f7fe-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0f7fe-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1436

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
  "dependentAppCount": 1,
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





