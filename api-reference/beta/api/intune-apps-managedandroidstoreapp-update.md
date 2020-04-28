---
title: Update managedAndroidStoreApp
description: Обновление свойств объекта managedAndroidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b4d8f56f54d464f7323d641c730ef85d8a16acbe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406245"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="56bdd-103">Update managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="56bdd-103">Update managedAndroidStoreApp</span></span>

<span data-ttu-id="56bdd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56bdd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56bdd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56bdd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56bdd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56bdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56bdd-107">Обновление свойств объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-107">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56bdd-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="56bdd-108">Prerequisites</span></span>
<span data-ttu-id="56bdd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56bdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56bdd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56bdd-111">Permission type</span></span>|<span data-ttu-id="56bdd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="56bdd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56bdd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56bdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56bdd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56bdd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="56bdd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56bdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56bdd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56bdd-116">Not supported.</span></span>|
|<span data-ttu-id="56bdd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56bdd-117">Application</span></span>|<span data-ttu-id="56bdd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56bdd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56bdd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56bdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="56bdd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="56bdd-120">Request headers</span></span>
|<span data-ttu-id="56bdd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="56bdd-121">Header</span></span>|<span data-ttu-id="56bdd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="56bdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56bdd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56bdd-123">Authorization</span></span>|<span data-ttu-id="56bdd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56bdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56bdd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="56bdd-125">Accept</span></span>|<span data-ttu-id="56bdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56bdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56bdd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56bdd-127">Request body</span></span>
<span data-ttu-id="56bdd-128">В теле запроса добавьте представление объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56bdd-128">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="56bdd-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-129">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="56bdd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="56bdd-130">Property</span></span>|<span data-ttu-id="56bdd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="56bdd-131">Type</span></span>|<span data-ttu-id="56bdd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="56bdd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56bdd-133">id</span><span class="sxs-lookup"><span data-stu-id="56bdd-133">id</span></span>|<span data-ttu-id="56bdd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="56bdd-134">String</span></span>|<span data-ttu-id="56bdd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="56bdd-135">Key of the entity.</span></span> <span data-ttu-id="56bdd-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="56bdd-137">displayName</span></span>|<span data-ttu-id="56bdd-138">Строка</span><span class="sxs-lookup"><span data-stu-id="56bdd-138">String</span></span>|<span data-ttu-id="56bdd-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="56bdd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="56bdd-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-141">description</span><span class="sxs-lookup"><span data-stu-id="56bdd-141">description</span></span>|<span data-ttu-id="56bdd-142">String</span><span class="sxs-lookup"><span data-stu-id="56bdd-142">String</span></span>|<span data-ttu-id="56bdd-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-143">The description of the app.</span></span> <span data-ttu-id="56bdd-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-145">publisher</span><span class="sxs-lookup"><span data-stu-id="56bdd-145">publisher</span></span>|<span data-ttu-id="56bdd-146">String</span><span class="sxs-lookup"><span data-stu-id="56bdd-146">String</span></span>|<span data-ttu-id="56bdd-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-147">The publisher of the app.</span></span> <span data-ttu-id="56bdd-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="56bdd-149">largeIcon</span></span>|[<span data-ttu-id="56bdd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="56bdd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="56bdd-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="56bdd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="56bdd-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56bdd-153">createdDateTime</span></span>|<span data-ttu-id="56bdd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56bdd-154">DateTimeOffset</span></span>|<span data-ttu-id="56bdd-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-155">The date and time the app was created.</span></span> <span data-ttu-id="56bdd-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56bdd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="56bdd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56bdd-158">DateTimeOffset</span></span>|<span data-ttu-id="56bdd-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="56bdd-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="56bdd-161">isFeatured</span></span>|<span data-ttu-id="56bdd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="56bdd-162">Boolean</span></span>|<span data-ttu-id="56bdd-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="56bdd-164">privacyInformationUrl</span></span>|<span data-ttu-id="56bdd-165">String</span><span class="sxs-lookup"><span data-stu-id="56bdd-165">String</span></span>|<span data-ttu-id="56bdd-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="56bdd-166">The privacy statement Url.</span></span> <span data-ttu-id="56bdd-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="56bdd-168">informationUrl</span></span>|<span data-ttu-id="56bdd-169">String</span><span class="sxs-lookup"><span data-stu-id="56bdd-169">String</span></span>|<span data-ttu-id="56bdd-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="56bdd-170">The more information Url.</span></span> <span data-ttu-id="56bdd-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-172">owner</span><span class="sxs-lookup"><span data-stu-id="56bdd-172">owner</span></span>|<span data-ttu-id="56bdd-173">String</span><span class="sxs-lookup"><span data-stu-id="56bdd-173">String</span></span>|<span data-ttu-id="56bdd-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-174">The owner of the app.</span></span> <span data-ttu-id="56bdd-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-176">developer</span><span class="sxs-lookup"><span data-stu-id="56bdd-176">developer</span></span>|<span data-ttu-id="56bdd-177">String</span><span class="sxs-lookup"><span data-stu-id="56bdd-177">String</span></span>|<span data-ttu-id="56bdd-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-178">The developer of the app.</span></span> <span data-ttu-id="56bdd-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-180">notes</span><span class="sxs-lookup"><span data-stu-id="56bdd-180">notes</span></span>|<span data-ttu-id="56bdd-181">String</span><span class="sxs-lookup"><span data-stu-id="56bdd-181">String</span></span>|<span data-ttu-id="56bdd-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-182">Notes for the app.</span></span> <span data-ttu-id="56bdd-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="56bdd-184">uploadState</span></span>|<span data-ttu-id="56bdd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="56bdd-185">Int32</span></span>|<span data-ttu-id="56bdd-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="56bdd-186">The upload state.</span></span> <span data-ttu-id="56bdd-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="56bdd-188">publishingState</span></span>|[<span data-ttu-id="56bdd-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="56bdd-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="56bdd-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-190">The publishing state for the app.</span></span> <span data-ttu-id="56bdd-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="56bdd-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="56bdd-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="56bdd-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="56bdd-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="56bdd-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="56bdd-194">isAssigned</span></span>|<span data-ttu-id="56bdd-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="56bdd-195">Boolean</span></span>|<span data-ttu-id="56bdd-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="56bdd-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="56bdd-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="56bdd-198">roleScopeTagIds</span></span>|<span data-ttu-id="56bdd-199">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="56bdd-199">String collection</span></span>|<span data-ttu-id="56bdd-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="56bdd-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="56bdd-202">dependentAppCount</span></span>|<span data-ttu-id="56bdd-203">Int32</span><span class="sxs-lookup"><span data-stu-id="56bdd-203">Int32</span></span>|<span data-ttu-id="56bdd-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="56bdd-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="56bdd-206">appAvailability</span><span class="sxs-lookup"><span data-stu-id="56bdd-206">appAvailability</span></span>|[<span data-ttu-id="56bdd-207">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="56bdd-207">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="56bdd-208">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-208">The Application's availability.</span></span> <span data-ttu-id="56bdd-209">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="56bdd-210">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="56bdd-210">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="56bdd-211">version</span><span class="sxs-lookup"><span data-stu-id="56bdd-211">version</span></span>|<span data-ttu-id="56bdd-212">String</span><span class="sxs-lookup"><span data-stu-id="56bdd-212">String</span></span>|<span data-ttu-id="56bdd-213">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-213">The Application's version.</span></span> <span data-ttu-id="56bdd-214">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="56bdd-214">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="56bdd-215">packageId</span><span class="sxs-lookup"><span data-stu-id="56bdd-215">packageId</span></span>|<span data-ttu-id="56bdd-216">String</span><span class="sxs-lookup"><span data-stu-id="56bdd-216">String</span></span>|<span data-ttu-id="56bdd-217">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="56bdd-217">The app's package ID.</span></span>|
|<span data-ttu-id="56bdd-218">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="56bdd-218">appStoreUrl</span></span>|<span data-ttu-id="56bdd-219">String</span><span class="sxs-lookup"><span data-stu-id="56bdd-219">String</span></span>|<span data-ttu-id="56bdd-220">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="56bdd-220">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="56bdd-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="56bdd-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="56bdd-222">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="56bdd-222">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="56bdd-223">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="56bdd-223">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="56bdd-224">Ответ</span><span class="sxs-lookup"><span data-stu-id="56bdd-224">Response</span></span>
<span data-ttu-id="56bdd-225">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="56bdd-225">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56bdd-226">Пример</span><span class="sxs-lookup"><span data-stu-id="56bdd-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="56bdd-227">Запрос</span><span class="sxs-lookup"><span data-stu-id="56bdd-227">Request</span></span>
<span data-ttu-id="56bdd-228">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56bdd-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="56bdd-229">Отклик</span><span class="sxs-lookup"><span data-stu-id="56bdd-229">Response</span></span>
<span data-ttu-id="56bdd-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56bdd-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



