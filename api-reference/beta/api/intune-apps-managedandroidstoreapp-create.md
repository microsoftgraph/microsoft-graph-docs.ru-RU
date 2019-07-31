---
title: Create managedAndroidStoreApp
description: Создание нового объекта managedAndroidStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f70421792c76b9cbfdd08caf74a5cc63016c1949
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961821"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="422c6-103">Create managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="422c6-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="422c6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="422c6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="422c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="422c6-106">Создание нового объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-106">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="422c6-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="422c6-107">Prerequisites</span></span>
<span data-ttu-id="422c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="422c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="422c6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="422c6-110">Permission type</span></span>|<span data-ttu-id="422c6-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="422c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="422c6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="422c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="422c6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="422c6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="422c6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="422c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="422c6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422c6-115">Not supported.</span></span>|
|<span data-ttu-id="422c6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="422c6-116">Application</span></span>|<span data-ttu-id="422c6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="422c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="422c6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="422c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="422c6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="422c6-119">Request headers</span></span>
|<span data-ttu-id="422c6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="422c6-120">Header</span></span>|<span data-ttu-id="422c6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="422c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="422c6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="422c6-122">Authorization</span></span>|<span data-ttu-id="422c6-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="422c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="422c6-124">Accept</span><span class="sxs-lookup"><span data-stu-id="422c6-124">Accept</span></span>|<span data-ttu-id="422c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="422c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="422c6-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="422c6-126">Request body</span></span>
<span data-ttu-id="422c6-127">В теле запроса добавьте представление объекта managedAndroidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="422c6-127">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="422c6-128">Ниже показаны свойства, которые необходимо указывать при создании объекта managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="422c6-128">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="422c6-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="422c6-129">Property</span></span>|<span data-ttu-id="422c6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="422c6-130">Type</span></span>|<span data-ttu-id="422c6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="422c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="422c6-132">id</span><span class="sxs-lookup"><span data-stu-id="422c6-132">id</span></span>|<span data-ttu-id="422c6-133">Строка</span><span class="sxs-lookup"><span data-stu-id="422c6-133">String</span></span>|<span data-ttu-id="422c6-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="422c6-134">Key of the entity.</span></span> <span data-ttu-id="422c6-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="422c6-136">displayName</span></span>|<span data-ttu-id="422c6-137">Строка</span><span class="sxs-lookup"><span data-stu-id="422c6-137">String</span></span>|<span data-ttu-id="422c6-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="422c6-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="422c6-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-140">description</span><span class="sxs-lookup"><span data-stu-id="422c6-140">description</span></span>|<span data-ttu-id="422c6-141">String</span><span class="sxs-lookup"><span data-stu-id="422c6-141">String</span></span>|<span data-ttu-id="422c6-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-142">The description of the app.</span></span> <span data-ttu-id="422c6-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-144">publisher</span><span class="sxs-lookup"><span data-stu-id="422c6-144">publisher</span></span>|<span data-ttu-id="422c6-145">String</span><span class="sxs-lookup"><span data-stu-id="422c6-145">String</span></span>|<span data-ttu-id="422c6-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-146">The publisher of the app.</span></span> <span data-ttu-id="422c6-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="422c6-148">largeIcon</span></span>|[<span data-ttu-id="422c6-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="422c6-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="422c6-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="422c6-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="422c6-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="422c6-152">createdDateTime</span></span>|<span data-ttu-id="422c6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="422c6-153">DateTimeOffset</span></span>|<span data-ttu-id="422c6-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-154">The date and time the app was created.</span></span> <span data-ttu-id="422c6-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="422c6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="422c6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="422c6-157">DateTimeOffset</span></span>|<span data-ttu-id="422c6-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-158">The date and time the app was last modified.</span></span> <span data-ttu-id="422c6-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="422c6-160">isFeatured</span></span>|<span data-ttu-id="422c6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="422c6-161">Boolean</span></span>|<span data-ttu-id="422c6-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="422c6-163">privacyInformationUrl</span></span>|<span data-ttu-id="422c6-164">String</span><span class="sxs-lookup"><span data-stu-id="422c6-164">String</span></span>|<span data-ttu-id="422c6-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="422c6-165">The privacy statement Url.</span></span> <span data-ttu-id="422c6-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="422c6-167">informationUrl</span></span>|<span data-ttu-id="422c6-168">String</span><span class="sxs-lookup"><span data-stu-id="422c6-168">String</span></span>|<span data-ttu-id="422c6-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="422c6-169">The more information Url.</span></span> <span data-ttu-id="422c6-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-171">owner</span><span class="sxs-lookup"><span data-stu-id="422c6-171">owner</span></span>|<span data-ttu-id="422c6-172">String</span><span class="sxs-lookup"><span data-stu-id="422c6-172">String</span></span>|<span data-ttu-id="422c6-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-173">The owner of the app.</span></span> <span data-ttu-id="422c6-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-175">developer</span><span class="sxs-lookup"><span data-stu-id="422c6-175">developer</span></span>|<span data-ttu-id="422c6-176">String</span><span class="sxs-lookup"><span data-stu-id="422c6-176">String</span></span>|<span data-ttu-id="422c6-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-177">The developer of the app.</span></span> <span data-ttu-id="422c6-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-179">notes</span><span class="sxs-lookup"><span data-stu-id="422c6-179">notes</span></span>|<span data-ttu-id="422c6-180">String</span><span class="sxs-lookup"><span data-stu-id="422c6-180">String</span></span>|<span data-ttu-id="422c6-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-181">Notes for the app.</span></span> <span data-ttu-id="422c6-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="422c6-183">uploadState</span></span>|<span data-ttu-id="422c6-184">Int32</span><span class="sxs-lookup"><span data-stu-id="422c6-184">Int32</span></span>|<span data-ttu-id="422c6-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="422c6-185">The upload state.</span></span> <span data-ttu-id="422c6-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="422c6-187">publishingState</span></span>|[<span data-ttu-id="422c6-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="422c6-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="422c6-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-189">The publishing state for the app.</span></span> <span data-ttu-id="422c6-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="422c6-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="422c6-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="422c6-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="422c6-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="422c6-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="422c6-193">isAssigned</span></span>|<span data-ttu-id="422c6-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="422c6-194">Boolean</span></span>|<span data-ttu-id="422c6-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="422c6-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="422c6-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="422c6-197">roleScopeTagIds</span></span>|<span data-ttu-id="422c6-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="422c6-198">String collection</span></span>|<span data-ttu-id="422c6-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="422c6-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="422c6-201">dependentAppCount</span></span>|<span data-ttu-id="422c6-202">Int32</span><span class="sxs-lookup"><span data-stu-id="422c6-202">Int32</span></span>|<span data-ttu-id="422c6-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="422c6-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="422c6-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="422c6-205">appAvailability</span></span>|[<span data-ttu-id="422c6-206">Манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="422c6-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="422c6-207">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-207">The Application's availability.</span></span> <span data-ttu-id="422c6-208">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="422c6-209">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="422c6-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="422c6-210">version</span><span class="sxs-lookup"><span data-stu-id="422c6-210">version</span></span>|<span data-ttu-id="422c6-211">String</span><span class="sxs-lookup"><span data-stu-id="422c6-211">String</span></span>|<span data-ttu-id="422c6-212">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-212">The Application's version.</span></span> <span data-ttu-id="422c6-213">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="422c6-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="422c6-214">packageId</span><span class="sxs-lookup"><span data-stu-id="422c6-214">packageId</span></span>|<span data-ttu-id="422c6-215">String</span><span class="sxs-lookup"><span data-stu-id="422c6-215">String</span></span>|<span data-ttu-id="422c6-216">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="422c6-216">The app's package ID.</span></span>|
|<span data-ttu-id="422c6-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="422c6-217">appStoreUrl</span></span>|<span data-ttu-id="422c6-218">String</span><span class="sxs-lookup"><span data-stu-id="422c6-218">String</span></span>|<span data-ttu-id="422c6-219">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="422c6-219">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="422c6-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="422c6-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="422c6-221">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="422c6-221">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="422c6-222">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="422c6-222">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="422c6-223">Ответ</span><span class="sxs-lookup"><span data-stu-id="422c6-223">Response</span></span>
<span data-ttu-id="422c6-224">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="422c6-224">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="422c6-225">Пример</span><span class="sxs-lookup"><span data-stu-id="422c6-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="422c6-226">Запрос</span><span class="sxs-lookup"><span data-stu-id="422c6-226">Request</span></span>
<span data-ttu-id="422c6-227">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="422c6-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="422c6-228">Отклик</span><span class="sxs-lookup"><span data-stu-id="422c6-228">Response</span></span>
<span data-ttu-id="422c6-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="422c6-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





