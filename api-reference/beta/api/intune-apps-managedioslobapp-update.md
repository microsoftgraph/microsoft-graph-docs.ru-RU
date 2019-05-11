---
title: Update managedIOSLobApp
description: Обновление свойств объекта managedIOSLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a538add4f2ee45a0b74f56129a448a190bc263d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935519"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="423e0-103">Update managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="423e0-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="423e0-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="423e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="423e0-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="423e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="423e0-106">Обновление свойств объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-106">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="423e0-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="423e0-107">Prerequisites</span></span>
<span data-ttu-id="423e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="423e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="423e0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="423e0-110">Permission type</span></span>|<span data-ttu-id="423e0-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="423e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="423e0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="423e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="423e0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="423e0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="423e0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="423e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="423e0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="423e0-115">Not supported.</span></span>|
|<span data-ttu-id="423e0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="423e0-116">Application</span></span>|<span data-ttu-id="423e0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="423e0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="423e0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="423e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="423e0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="423e0-119">Request headers</span></span>
|<span data-ttu-id="423e0-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="423e0-120">Header</span></span>|<span data-ttu-id="423e0-121">Значение</span><span class="sxs-lookup"><span data-stu-id="423e0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="423e0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="423e0-122">Authorization</span></span>|<span data-ttu-id="423e0-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="423e0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="423e0-124">Accept</span><span class="sxs-lookup"><span data-stu-id="423e0-124">Accept</span></span>|<span data-ttu-id="423e0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="423e0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="423e0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="423e0-126">Request body</span></span>
<span data-ttu-id="423e0-127">В теле запроса добавьте представление объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="423e0-127">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="423e0-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-128">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="423e0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="423e0-129">Property</span></span>|<span data-ttu-id="423e0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="423e0-130">Type</span></span>|<span data-ttu-id="423e0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="423e0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="423e0-132">id</span><span class="sxs-lookup"><span data-stu-id="423e0-132">id</span></span>|<span data-ttu-id="423e0-133">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-133">String</span></span>|<span data-ttu-id="423e0-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="423e0-134">Key of the entity.</span></span> <span data-ttu-id="423e0-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="423e0-136">displayName</span></span>|<span data-ttu-id="423e0-137">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-137">String</span></span>|<span data-ttu-id="423e0-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="423e0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="423e0-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-140">description</span><span class="sxs-lookup"><span data-stu-id="423e0-140">description</span></span>|<span data-ttu-id="423e0-141">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-141">String</span></span>|<span data-ttu-id="423e0-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-142">The description of the app.</span></span> <span data-ttu-id="423e0-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-144">publisher</span><span class="sxs-lookup"><span data-stu-id="423e0-144">publisher</span></span>|<span data-ttu-id="423e0-145">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-145">String</span></span>|<span data-ttu-id="423e0-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-146">The publisher of the app.</span></span> <span data-ttu-id="423e0-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="423e0-148">largeIcon</span></span>|[<span data-ttu-id="423e0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="423e0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="423e0-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="423e0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="423e0-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="423e0-152">createdDateTime</span></span>|<span data-ttu-id="423e0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="423e0-153">DateTimeOffset</span></span>|<span data-ttu-id="423e0-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-154">The date and time the app was created.</span></span> <span data-ttu-id="423e0-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="423e0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="423e0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="423e0-157">DateTimeOffset</span></span>|<span data-ttu-id="423e0-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="423e0-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="423e0-160">isFeatured</span></span>|<span data-ttu-id="423e0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="423e0-161">Boolean</span></span>|<span data-ttu-id="423e0-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="423e0-163">privacyInformationUrl</span></span>|<span data-ttu-id="423e0-164">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-164">String</span></span>|<span data-ttu-id="423e0-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="423e0-165">The privacy statement Url.</span></span> <span data-ttu-id="423e0-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="423e0-167">informationUrl</span></span>|<span data-ttu-id="423e0-168">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-168">String</span></span>|<span data-ttu-id="423e0-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="423e0-169">The more information Url.</span></span> <span data-ttu-id="423e0-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-171">owner</span><span class="sxs-lookup"><span data-stu-id="423e0-171">owner</span></span>|<span data-ttu-id="423e0-172">String</span><span class="sxs-lookup"><span data-stu-id="423e0-172">String</span></span>|<span data-ttu-id="423e0-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-173">The owner of the app.</span></span> <span data-ttu-id="423e0-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-175">developer</span><span class="sxs-lookup"><span data-stu-id="423e0-175">developer</span></span>|<span data-ttu-id="423e0-176">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-176">String</span></span>|<span data-ttu-id="423e0-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-177">The developer of the app.</span></span> <span data-ttu-id="423e0-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-179">notes</span><span class="sxs-lookup"><span data-stu-id="423e0-179">notes</span></span>|<span data-ttu-id="423e0-180">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-180">String</span></span>|<span data-ttu-id="423e0-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-181">Notes for the app.</span></span> <span data-ttu-id="423e0-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="423e0-183">uploadState</span></span>|<span data-ttu-id="423e0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="423e0-184">Int32</span></span>|<span data-ttu-id="423e0-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="423e0-185">The upload state.</span></span> <span data-ttu-id="423e0-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="423e0-187">publishingState</span></span>|[<span data-ttu-id="423e0-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="423e0-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="423e0-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-189">The publishing state for the app.</span></span> <span data-ttu-id="423e0-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="423e0-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="423e0-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="423e0-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="423e0-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="423e0-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="423e0-193">isAssigned</span></span>|<span data-ttu-id="423e0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="423e0-194">Boolean</span></span>|<span data-ttu-id="423e0-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="423e0-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="423e0-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="423e0-197">roleScopeTagIds</span></span>|<span data-ttu-id="423e0-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="423e0-198">String collection</span></span>|<span data-ttu-id="423e0-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="423e0-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="423e0-201">dependentAppCount</span></span>|<span data-ttu-id="423e0-202">Int32</span><span class="sxs-lookup"><span data-stu-id="423e0-202">Int32</span></span>|<span data-ttu-id="423e0-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="423e0-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="423e0-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="423e0-205">appAvailability</span></span>|[<span data-ttu-id="423e0-206">Манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="423e0-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="423e0-207">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-207">The Application's availability.</span></span> <span data-ttu-id="423e0-208">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="423e0-209">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="423e0-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="423e0-210">version</span><span class="sxs-lookup"><span data-stu-id="423e0-210">version</span></span>|<span data-ttu-id="423e0-211">String</span><span class="sxs-lookup"><span data-stu-id="423e0-211">String</span></span>|<span data-ttu-id="423e0-212">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-212">The Application's version.</span></span> <span data-ttu-id="423e0-213">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="423e0-214">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="423e0-214">committedContentVersion</span></span>|<span data-ttu-id="423e0-215">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-215">String</span></span>|<span data-ttu-id="423e0-216">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="423e0-216">The internal committed content version.</span></span> <span data-ttu-id="423e0-217">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="423e0-218">fileName</span><span class="sxs-lookup"><span data-stu-id="423e0-218">fileName</span></span>|<span data-ttu-id="423e0-219">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-219">String</span></span>|<span data-ttu-id="423e0-220">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="423e0-220">The name of the main Lob application file.</span></span> <span data-ttu-id="423e0-221">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="423e0-222">size</span><span class="sxs-lookup"><span data-stu-id="423e0-222">size</span></span>|<span data-ttu-id="423e0-223">Int64</span><span class="sxs-lookup"><span data-stu-id="423e0-223">Int64</span></span>|<span data-ttu-id="423e0-224">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="423e0-224">The total size, including all uploaded files.</span></span> <span data-ttu-id="423e0-225">Наследуется от [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="423e0-225">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="423e0-226">bundleId</span><span class="sxs-lookup"><span data-stu-id="423e0-226">bundleId</span></span>|<span data-ttu-id="423e0-227">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-227">String</span></span>|<span data-ttu-id="423e0-228">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="423e0-228">The Identity Name.</span></span>|
|<span data-ttu-id="423e0-229">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="423e0-229">applicableDeviceType</span></span>|[<span data-ttu-id="423e0-230">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="423e0-230">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="423e0-231">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="423e0-231">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="423e0-232">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="423e0-232">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="423e0-233">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="423e0-233">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="423e0-234">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="423e0-234">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="423e0-235">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="423e0-235">expirationDateTime</span></span>|<span data-ttu-id="423e0-236">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="423e0-236">DateTimeOffset</span></span>|<span data-ttu-id="423e0-237">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="423e0-237">The expiration time.</span></span>|
|<span data-ttu-id="423e0-238">versionNumber</span><span class="sxs-lookup"><span data-stu-id="423e0-238">versionNumber</span></span>|<span data-ttu-id="423e0-239">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-239">String</span></span>|<span data-ttu-id="423e0-240">Номер версии управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="423e0-240">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="423e0-241">buildNumber</span><span class="sxs-lookup"><span data-stu-id="423e0-241">buildNumber</span></span>|<span data-ttu-id="423e0-242">Строка</span><span class="sxs-lookup"><span data-stu-id="423e0-242">String</span></span>|<span data-ttu-id="423e0-243">Номер сборки управляемого бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="423e0-243">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="423e0-244">identityVersion</span><span class="sxs-lookup"><span data-stu-id="423e0-244">identityVersion</span></span>|<span data-ttu-id="423e0-245">String</span><span class="sxs-lookup"><span data-stu-id="423e0-245">String</span></span>|<span data-ttu-id="423e0-246">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="423e0-246">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="423e0-247">Ответ</span><span class="sxs-lookup"><span data-stu-id="423e0-247">Response</span></span>
<span data-ttu-id="423e0-248">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="423e0-248">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="423e0-249">Пример</span><span class="sxs-lookup"><span data-stu-id="423e0-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="423e0-250">Запрос</span><span class="sxs-lookup"><span data-stu-id="423e0-250">Request</span></span>
<span data-ttu-id="423e0-251">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="423e0-251">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1469

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
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="423e0-252">Отклик</span><span class="sxs-lookup"><span data-stu-id="423e0-252">Response</span></span>
<span data-ttu-id="423e0-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="423e0-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1641

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
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




