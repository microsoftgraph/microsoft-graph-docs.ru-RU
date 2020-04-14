---
title: Update managedAndroidLobApp
description: Обновление свойств объекта managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0c1c29bcd318d1f3a089397ed4ef65e637ab00d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43409754"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="99f31-103">Update managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="99f31-103">Update managedAndroidLobApp</span></span>

<span data-ttu-id="99f31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99f31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99f31-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99f31-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99f31-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99f31-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99f31-107">Обновление свойств объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-107">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99f31-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="99f31-108">Prerequisites</span></span>
<span data-ttu-id="99f31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99f31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99f31-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99f31-111">Permission type</span></span>|<span data-ttu-id="99f31-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="99f31-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99f31-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99f31-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99f31-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99f31-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="99f31-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99f31-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99f31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99f31-116">Not supported.</span></span>|
|<span data-ttu-id="99f31-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="99f31-117">Application</span></span>|<span data-ttu-id="99f31-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99f31-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99f31-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99f31-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="99f31-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="99f31-120">Request headers</span></span>
|<span data-ttu-id="99f31-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99f31-121">Header</span></span>|<span data-ttu-id="99f31-122">Значение</span><span class="sxs-lookup"><span data-stu-id="99f31-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99f31-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99f31-123">Authorization</span></span>|<span data-ttu-id="99f31-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99f31-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99f31-125">Accept</span><span class="sxs-lookup"><span data-stu-id="99f31-125">Accept</span></span>|<span data-ttu-id="99f31-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99f31-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99f31-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99f31-127">Request body</span></span>
<span data-ttu-id="99f31-128">В теле запроса добавьте представление объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99f31-128">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="99f31-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-129">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="99f31-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="99f31-130">Property</span></span>|<span data-ttu-id="99f31-131">Тип</span><span class="sxs-lookup"><span data-stu-id="99f31-131">Type</span></span>|<span data-ttu-id="99f31-132">Описание</span><span class="sxs-lookup"><span data-stu-id="99f31-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99f31-133">id</span><span class="sxs-lookup"><span data-stu-id="99f31-133">id</span></span>|<span data-ttu-id="99f31-134">Строка</span><span class="sxs-lookup"><span data-stu-id="99f31-134">String</span></span>|<span data-ttu-id="99f31-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="99f31-135">Key of the entity.</span></span> <span data-ttu-id="99f31-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-137">displayName</span><span class="sxs-lookup"><span data-stu-id="99f31-137">displayName</span></span>|<span data-ttu-id="99f31-138">Строка</span><span class="sxs-lookup"><span data-stu-id="99f31-138">String</span></span>|<span data-ttu-id="99f31-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="99f31-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="99f31-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-141">description</span><span class="sxs-lookup"><span data-stu-id="99f31-141">description</span></span>|<span data-ttu-id="99f31-142">String</span><span class="sxs-lookup"><span data-stu-id="99f31-142">String</span></span>|<span data-ttu-id="99f31-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-143">The description of the app.</span></span> <span data-ttu-id="99f31-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-145">publisher</span><span class="sxs-lookup"><span data-stu-id="99f31-145">publisher</span></span>|<span data-ttu-id="99f31-146">String</span><span class="sxs-lookup"><span data-stu-id="99f31-146">String</span></span>|<span data-ttu-id="99f31-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-147">The publisher of the app.</span></span> <span data-ttu-id="99f31-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="99f31-149">largeIcon</span></span>|[<span data-ttu-id="99f31-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="99f31-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="99f31-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="99f31-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="99f31-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99f31-153">createdDateTime</span></span>|<span data-ttu-id="99f31-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99f31-154">DateTimeOffset</span></span>|<span data-ttu-id="99f31-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-155">The date and time the app was created.</span></span> <span data-ttu-id="99f31-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99f31-157">lastModifiedDateTime</span></span>|<span data-ttu-id="99f31-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99f31-158">DateTimeOffset</span></span>|<span data-ttu-id="99f31-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-159">The date and time the app was last modified.</span></span> <span data-ttu-id="99f31-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="99f31-161">isFeatured</span></span>|<span data-ttu-id="99f31-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="99f31-162">Boolean</span></span>|<span data-ttu-id="99f31-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="99f31-164">privacyInformationUrl</span></span>|<span data-ttu-id="99f31-165">String</span><span class="sxs-lookup"><span data-stu-id="99f31-165">String</span></span>|<span data-ttu-id="99f31-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="99f31-166">The privacy statement Url.</span></span> <span data-ttu-id="99f31-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="99f31-168">informationUrl</span></span>|<span data-ttu-id="99f31-169">String</span><span class="sxs-lookup"><span data-stu-id="99f31-169">String</span></span>|<span data-ttu-id="99f31-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="99f31-170">The more information Url.</span></span> <span data-ttu-id="99f31-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-172">owner</span><span class="sxs-lookup"><span data-stu-id="99f31-172">owner</span></span>|<span data-ttu-id="99f31-173">String</span><span class="sxs-lookup"><span data-stu-id="99f31-173">String</span></span>|<span data-ttu-id="99f31-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-174">The owner of the app.</span></span> <span data-ttu-id="99f31-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-176">developer</span><span class="sxs-lookup"><span data-stu-id="99f31-176">developer</span></span>|<span data-ttu-id="99f31-177">String</span><span class="sxs-lookup"><span data-stu-id="99f31-177">String</span></span>|<span data-ttu-id="99f31-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-178">The developer of the app.</span></span> <span data-ttu-id="99f31-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-180">notes</span><span class="sxs-lookup"><span data-stu-id="99f31-180">notes</span></span>|<span data-ttu-id="99f31-181">String</span><span class="sxs-lookup"><span data-stu-id="99f31-181">String</span></span>|<span data-ttu-id="99f31-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-182">Notes for the app.</span></span> <span data-ttu-id="99f31-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="99f31-184">uploadState</span></span>|<span data-ttu-id="99f31-185">Int32</span><span class="sxs-lookup"><span data-stu-id="99f31-185">Int32</span></span>|<span data-ttu-id="99f31-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="99f31-186">The upload state.</span></span> <span data-ttu-id="99f31-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="99f31-188">publishingState</span></span>|[<span data-ttu-id="99f31-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="99f31-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="99f31-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-190">The publishing state for the app.</span></span> <span data-ttu-id="99f31-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="99f31-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="99f31-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="99f31-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="99f31-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="99f31-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="99f31-194">isAssigned</span></span>|<span data-ttu-id="99f31-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="99f31-195">Boolean</span></span>|<span data-ttu-id="99f31-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="99f31-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="99f31-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="99f31-198">roleScopeTagIds</span></span>|<span data-ttu-id="99f31-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="99f31-199">String collection</span></span>|<span data-ttu-id="99f31-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="99f31-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="99f31-202">dependentAppCount</span></span>|<span data-ttu-id="99f31-203">Int32</span><span class="sxs-lookup"><span data-stu-id="99f31-203">Int32</span></span>|<span data-ttu-id="99f31-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="99f31-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="99f31-206">appAvailability</span><span class="sxs-lookup"><span data-stu-id="99f31-206">appAvailability</span></span>|[<span data-ttu-id="99f31-207">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="99f31-207">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="99f31-208">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-208">The Application's availability.</span></span> <span data-ttu-id="99f31-209">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="99f31-210">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="99f31-210">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="99f31-211">version</span><span class="sxs-lookup"><span data-stu-id="99f31-211">version</span></span>|<span data-ttu-id="99f31-212">String</span><span class="sxs-lookup"><span data-stu-id="99f31-212">String</span></span>|<span data-ttu-id="99f31-213">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-213">The Application's version.</span></span> <span data-ttu-id="99f31-214">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-214">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="99f31-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="99f31-215">committedContentVersion</span></span>|<span data-ttu-id="99f31-216">String</span><span class="sxs-lookup"><span data-stu-id="99f31-216">String</span></span>|<span data-ttu-id="99f31-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="99f31-217">The internal committed content version.</span></span> <span data-ttu-id="99f31-218">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="99f31-219">fileName</span><span class="sxs-lookup"><span data-stu-id="99f31-219">fileName</span></span>|<span data-ttu-id="99f31-220">String</span><span class="sxs-lookup"><span data-stu-id="99f31-220">String</span></span>|<span data-ttu-id="99f31-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="99f31-221">The name of the main Lob application file.</span></span> <span data-ttu-id="99f31-222">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="99f31-223">size</span><span class="sxs-lookup"><span data-stu-id="99f31-223">size</span></span>|<span data-ttu-id="99f31-224">Int64</span><span class="sxs-lookup"><span data-stu-id="99f31-224">Int64</span></span>|<span data-ttu-id="99f31-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="99f31-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="99f31-226">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="99f31-226">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="99f31-227">packageId</span><span class="sxs-lookup"><span data-stu-id="99f31-227">packageId</span></span>|<span data-ttu-id="99f31-228">String</span><span class="sxs-lookup"><span data-stu-id="99f31-228">String</span></span>|<span data-ttu-id="99f31-229">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="99f31-229">The package identifier.</span></span>|
|<span data-ttu-id="99f31-230">identityName</span><span class="sxs-lookup"><span data-stu-id="99f31-230">identityName</span></span>|<span data-ttu-id="99f31-231">String</span><span class="sxs-lookup"><span data-stu-id="99f31-231">String</span></span>|<span data-ttu-id="99f31-232">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="99f31-232">The Identity Name.</span></span>|
|<span data-ttu-id="99f31-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="99f31-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="99f31-234">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="99f31-234">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="99f31-235">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="99f31-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="99f31-236">versionName</span><span class="sxs-lookup"><span data-stu-id="99f31-236">versionName</span></span>|<span data-ttu-id="99f31-237">String</span><span class="sxs-lookup"><span data-stu-id="99f31-237">String</span></span>|<span data-ttu-id="99f31-238">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="99f31-238">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="99f31-239">versionCode</span><span class="sxs-lookup"><span data-stu-id="99f31-239">versionCode</span></span>|<span data-ttu-id="99f31-240">String</span><span class="sxs-lookup"><span data-stu-id="99f31-240">String</span></span>|<span data-ttu-id="99f31-241">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="99f31-241">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="99f31-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="99f31-242">identityVersion</span></span>|<span data-ttu-id="99f31-243">String</span><span class="sxs-lookup"><span data-stu-id="99f31-243">String</span></span>|<span data-ttu-id="99f31-244">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="99f31-244">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="99f31-245">Ответ</span><span class="sxs-lookup"><span data-stu-id="99f31-245">Response</span></span>
<span data-ttu-id="99f31-246">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="99f31-246">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99f31-247">Пример</span><span class="sxs-lookup"><span data-stu-id="99f31-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="99f31-248">Запрос</span><span class="sxs-lookup"><span data-stu-id="99f31-248">Request</span></span>
<span data-ttu-id="99f31-249">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99f31-249">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1491

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="99f31-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="99f31-250">Response</span></span>
<span data-ttu-id="99f31-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="99f31-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1663

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```



