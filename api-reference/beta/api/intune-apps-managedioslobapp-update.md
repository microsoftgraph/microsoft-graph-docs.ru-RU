---
title: Update managedIOSLobApp
description: Обновление свойств объекта managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b86a843e2202297809ffc4036f2ea2a001be87ea
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43405711"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="8b533-103">Update managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="8b533-103">Update managedIOSLobApp</span></span>

<span data-ttu-id="8b533-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b533-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b533-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b533-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b533-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b533-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b533-107">Обновление свойств объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b533-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8b533-108">Prerequisites</span></span>
<span data-ttu-id="8b533-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b533-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b533-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b533-111">Permission type</span></span>|<span data-ttu-id="8b533-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b533-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b533-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b533-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b533-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b533-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8b533-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b533-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b533-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b533-116">Not supported.</span></span>|
|<span data-ttu-id="8b533-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8b533-117">Application</span></span>|<span data-ttu-id="8b533-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b533-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b533-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b533-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8b533-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8b533-120">Request headers</span></span>
|<span data-ttu-id="8b533-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b533-121">Header</span></span>|<span data-ttu-id="8b533-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8b533-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b533-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b533-123">Authorization</span></span>|<span data-ttu-id="8b533-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b533-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b533-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8b533-125">Accept</span></span>|<span data-ttu-id="8b533-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b533-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b533-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b533-127">Request body</span></span>
<span data-ttu-id="8b533-128">В теле запроса добавьте представление объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b533-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="8b533-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="8b533-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b533-130">Property</span></span>|<span data-ttu-id="8b533-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8b533-131">Type</span></span>|<span data-ttu-id="8b533-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8b533-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b533-133">id</span><span class="sxs-lookup"><span data-stu-id="8b533-133">id</span></span>|<span data-ttu-id="8b533-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8b533-134">String</span></span>|<span data-ttu-id="8b533-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8b533-135">Key of the entity.</span></span> <span data-ttu-id="8b533-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8b533-137">displayName</span></span>|<span data-ttu-id="8b533-138">Строка</span><span class="sxs-lookup"><span data-stu-id="8b533-138">String</span></span>|<span data-ttu-id="8b533-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="8b533-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8b533-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-141">description</span><span class="sxs-lookup"><span data-stu-id="8b533-141">description</span></span>|<span data-ttu-id="8b533-142">String</span><span class="sxs-lookup"><span data-stu-id="8b533-142">String</span></span>|<span data-ttu-id="8b533-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-143">The description of the app.</span></span> <span data-ttu-id="8b533-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8b533-145">publisher</span></span>|<span data-ttu-id="8b533-146">String</span><span class="sxs-lookup"><span data-stu-id="8b533-146">String</span></span>|<span data-ttu-id="8b533-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-147">The publisher of the app.</span></span> <span data-ttu-id="8b533-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8b533-149">largeIcon</span></span>|[<span data-ttu-id="8b533-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8b533-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8b533-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="8b533-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8b533-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b533-153">createdDateTime</span></span>|<span data-ttu-id="8b533-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b533-154">DateTimeOffset</span></span>|<span data-ttu-id="8b533-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-155">The date and time the app was created.</span></span> <span data-ttu-id="8b533-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b533-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8b533-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b533-158">DateTimeOffset</span></span>|<span data-ttu-id="8b533-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8b533-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8b533-161">isFeatured</span></span>|<span data-ttu-id="8b533-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b533-162">Boolean</span></span>|<span data-ttu-id="8b533-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8b533-164">privacyInformationUrl</span></span>|<span data-ttu-id="8b533-165">String</span><span class="sxs-lookup"><span data-stu-id="8b533-165">String</span></span>|<span data-ttu-id="8b533-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8b533-166">The privacy statement Url.</span></span> <span data-ttu-id="8b533-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8b533-168">informationUrl</span></span>|<span data-ttu-id="8b533-169">String</span><span class="sxs-lookup"><span data-stu-id="8b533-169">String</span></span>|<span data-ttu-id="8b533-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="8b533-170">The more information Url.</span></span> <span data-ttu-id="8b533-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-172">owner</span><span class="sxs-lookup"><span data-stu-id="8b533-172">owner</span></span>|<span data-ttu-id="8b533-173">String</span><span class="sxs-lookup"><span data-stu-id="8b533-173">String</span></span>|<span data-ttu-id="8b533-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-174">The owner of the app.</span></span> <span data-ttu-id="8b533-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-176">developer</span><span class="sxs-lookup"><span data-stu-id="8b533-176">developer</span></span>|<span data-ttu-id="8b533-177">String</span><span class="sxs-lookup"><span data-stu-id="8b533-177">String</span></span>|<span data-ttu-id="8b533-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-178">The developer of the app.</span></span> <span data-ttu-id="8b533-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-180">notes</span><span class="sxs-lookup"><span data-stu-id="8b533-180">notes</span></span>|<span data-ttu-id="8b533-181">String</span><span class="sxs-lookup"><span data-stu-id="8b533-181">String</span></span>|<span data-ttu-id="8b533-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-182">Notes for the app.</span></span> <span data-ttu-id="8b533-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8b533-184">uploadState</span></span>|<span data-ttu-id="8b533-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8b533-185">Int32</span></span>|<span data-ttu-id="8b533-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="8b533-186">The upload state.</span></span> <span data-ttu-id="8b533-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8b533-188">publishingState</span></span>|[<span data-ttu-id="8b533-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="8b533-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8b533-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-190">The publishing state for the app.</span></span> <span data-ttu-id="8b533-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="8b533-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8b533-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8b533-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8b533-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8b533-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8b533-194">isAssigned</span></span>|<span data-ttu-id="8b533-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b533-195">Boolean</span></span>|<span data-ttu-id="8b533-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="8b533-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8b533-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8b533-198">roleScopeTagIds</span></span>|<span data-ttu-id="8b533-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8b533-199">String collection</span></span>|<span data-ttu-id="8b533-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8b533-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="8b533-202">dependentAppCount</span></span>|<span data-ttu-id="8b533-203">Int32</span><span class="sxs-lookup"><span data-stu-id="8b533-203">Int32</span></span>|<span data-ttu-id="8b533-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8b533-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8b533-206">appAvailability</span><span class="sxs-lookup"><span data-stu-id="8b533-206">appAvailability</span></span>|[<span data-ttu-id="8b533-207">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="8b533-207">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="8b533-208">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-208">The Application's availability.</span></span> <span data-ttu-id="8b533-209">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="8b533-210">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="8b533-210">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="8b533-211">version</span><span class="sxs-lookup"><span data-stu-id="8b533-211">version</span></span>|<span data-ttu-id="8b533-212">String</span><span class="sxs-lookup"><span data-stu-id="8b533-212">String</span></span>|<span data-ttu-id="8b533-213">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-213">The Application's version.</span></span> <span data-ttu-id="8b533-214">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-214">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="8b533-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8b533-215">committedContentVersion</span></span>|<span data-ttu-id="8b533-216">String</span><span class="sxs-lookup"><span data-stu-id="8b533-216">String</span></span>|<span data-ttu-id="8b533-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="8b533-217">The internal committed content version.</span></span> <span data-ttu-id="8b533-218">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8b533-219">fileName</span><span class="sxs-lookup"><span data-stu-id="8b533-219">fileName</span></span>|<span data-ttu-id="8b533-220">String</span><span class="sxs-lookup"><span data-stu-id="8b533-220">String</span></span>|<span data-ttu-id="8b533-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="8b533-221">The name of the main Lob application file.</span></span> <span data-ttu-id="8b533-222">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8b533-223">size</span><span class="sxs-lookup"><span data-stu-id="8b533-223">size</span></span>|<span data-ttu-id="8b533-224">Int64</span><span class="sxs-lookup"><span data-stu-id="8b533-224">Int64</span></span>|<span data-ttu-id="8b533-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="8b533-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="8b533-226">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8b533-226">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8b533-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="8b533-227">bundleId</span></span>|<span data-ttu-id="8b533-228">String</span><span class="sxs-lookup"><span data-stu-id="8b533-228">String</span></span>|<span data-ttu-id="8b533-229">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="8b533-229">The Identity Name.</span></span>|
|<span data-ttu-id="8b533-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="8b533-230">applicableDeviceType</span></span>|[<span data-ttu-id="8b533-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="8b533-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="8b533-232">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="8b533-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="8b533-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8b533-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8b533-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8b533-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="8b533-235">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="8b533-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8b533-236">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8b533-236">expirationDateTime</span></span>|<span data-ttu-id="8b533-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b533-237">DateTimeOffset</span></span>|<span data-ttu-id="8b533-238">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="8b533-238">The expiration time.</span></span>|
|<span data-ttu-id="8b533-239">versionNumber</span><span class="sxs-lookup"><span data-stu-id="8b533-239">versionNumber</span></span>|<span data-ttu-id="8b533-240">String</span><span class="sxs-lookup"><span data-stu-id="8b533-240">String</span></span>|<span data-ttu-id="8b533-241">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="8b533-241">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8b533-242">buildNumber</span><span class="sxs-lookup"><span data-stu-id="8b533-242">buildNumber</span></span>|<span data-ttu-id="8b533-243">String</span><span class="sxs-lookup"><span data-stu-id="8b533-243">String</span></span>|<span data-ttu-id="8b533-244">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="8b533-244">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8b533-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="8b533-245">identityVersion</span></span>|<span data-ttu-id="8b533-246">String</span><span class="sxs-lookup"><span data-stu-id="8b533-246">String</span></span>|<span data-ttu-id="8b533-247">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="8b533-247">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="8b533-248">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b533-248">Response</span></span>
<span data-ttu-id="8b533-249">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8b533-249">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b533-250">Пример</span><span class="sxs-lookup"><span data-stu-id="8b533-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b533-251">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b533-251">Request</span></span>
<span data-ttu-id="8b533-252">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b533-252">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1489

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "bundleId": "Bundle Id value",
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
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="8b533-253">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b533-253">Response</span></span>
<span data-ttu-id="8b533-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b533-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1661

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "bundleId": "Bundle Id value",
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
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```



