---
title: Update androidLobApp
description: Обновление свойств объекта androidLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 928620e0ac689d139fe1ae953b7697efd2371119
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952270"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="fbb67-103">Update androidLobApp</span><span class="sxs-lookup"><span data-stu-id="fbb67-103">Update androidLobApp</span></span>

> <span data-ttu-id="fbb67-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbb67-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbb67-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbb67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbb67-106">Обновление свойств объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbb67-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="fbb67-107">Prerequisites</span></span>
<span data-ttu-id="fbb67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbb67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbb67-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbb67-110">Permission type</span></span>|<span data-ttu-id="fbb67-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbb67-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbb67-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbb67-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fbb67-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbb67-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fbb67-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbb67-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbb67-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbb67-115">Not supported.</span></span>|
|<span data-ttu-id="fbb67-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbb67-116">Application</span></span>|<span data-ttu-id="fbb67-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbb67-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbb67-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbb67-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="fbb67-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbb67-119">Request headers</span></span>
|<span data-ttu-id="fbb67-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbb67-120">Header</span></span>|<span data-ttu-id="fbb67-121">Значение</span><span class="sxs-lookup"><span data-stu-id="fbb67-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbb67-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbb67-122">Authorization</span></span>|<span data-ttu-id="fbb67-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbb67-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbb67-124">Accept</span><span class="sxs-lookup"><span data-stu-id="fbb67-124">Accept</span></span>|<span data-ttu-id="fbb67-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fbb67-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbb67-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fbb67-126">Request body</span></span>
<span data-ttu-id="fbb67-127">В теле запроса добавьте представление объекта [androidLobApp](../resources/intune-apps-androidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbb67-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="fbb67-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="fbb67-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbb67-129">Property</span></span>|<span data-ttu-id="fbb67-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fbb67-130">Type</span></span>|<span data-ttu-id="fbb67-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fbb67-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbb67-132">id</span><span class="sxs-lookup"><span data-stu-id="fbb67-132">id</span></span>|<span data-ttu-id="fbb67-133">Строка</span><span class="sxs-lookup"><span data-stu-id="fbb67-133">String</span></span>|<span data-ttu-id="fbb67-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fbb67-134">Key of the entity.</span></span> <span data-ttu-id="fbb67-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fbb67-136">displayName</span></span>|<span data-ttu-id="fbb67-137">Строка</span><span class="sxs-lookup"><span data-stu-id="fbb67-137">String</span></span>|<span data-ttu-id="fbb67-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="fbb67-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fbb67-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-140">description</span><span class="sxs-lookup"><span data-stu-id="fbb67-140">description</span></span>|<span data-ttu-id="fbb67-141">Строка</span><span class="sxs-lookup"><span data-stu-id="fbb67-141">String</span></span>|<span data-ttu-id="fbb67-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-142">The description of the app.</span></span> <span data-ttu-id="fbb67-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-144">publisher</span><span class="sxs-lookup"><span data-stu-id="fbb67-144">publisher</span></span>|<span data-ttu-id="fbb67-145">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-145">String</span></span>|<span data-ttu-id="fbb67-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-146">The publisher of the app.</span></span> <span data-ttu-id="fbb67-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fbb67-148">largeIcon</span></span>|[<span data-ttu-id="fbb67-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fbb67-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fbb67-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="fbb67-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fbb67-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbb67-152">createdDateTime</span></span>|<span data-ttu-id="fbb67-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbb67-153">DateTimeOffset</span></span>|<span data-ttu-id="fbb67-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-154">The date and time the app was created.</span></span> <span data-ttu-id="fbb67-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbb67-156">lastModifiedDateTime</span></span>|<span data-ttu-id="fbb67-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbb67-157">DateTimeOffset</span></span>|<span data-ttu-id="fbb67-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-158">The date and time the app was last modified.</span></span> <span data-ttu-id="fbb67-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fbb67-160">isFeatured</span></span>|<span data-ttu-id="fbb67-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbb67-161">Boolean</span></span>|<span data-ttu-id="fbb67-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fbb67-163">privacyInformationUrl</span></span>|<span data-ttu-id="fbb67-164">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-164">String</span></span>|<span data-ttu-id="fbb67-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="fbb67-165">The privacy statement Url.</span></span> <span data-ttu-id="fbb67-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fbb67-167">informationUrl</span></span>|<span data-ttu-id="fbb67-168">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-168">String</span></span>|<span data-ttu-id="fbb67-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="fbb67-169">The more information Url.</span></span> <span data-ttu-id="fbb67-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-171">owner</span><span class="sxs-lookup"><span data-stu-id="fbb67-171">owner</span></span>|<span data-ttu-id="fbb67-172">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-172">String</span></span>|<span data-ttu-id="fbb67-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-173">The owner of the app.</span></span> <span data-ttu-id="fbb67-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-175">developer</span><span class="sxs-lookup"><span data-stu-id="fbb67-175">developer</span></span>|<span data-ttu-id="fbb67-176">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-176">String</span></span>|<span data-ttu-id="fbb67-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-177">The developer of the app.</span></span> <span data-ttu-id="fbb67-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-179">notes</span><span class="sxs-lookup"><span data-stu-id="fbb67-179">notes</span></span>|<span data-ttu-id="fbb67-180">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-180">String</span></span>|<span data-ttu-id="fbb67-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-181">Notes for the app.</span></span> <span data-ttu-id="fbb67-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="fbb67-183">uploadState</span></span>|<span data-ttu-id="fbb67-184">Int32</span><span class="sxs-lookup"><span data-stu-id="fbb67-184">Int32</span></span>|<span data-ttu-id="fbb67-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="fbb67-185">The upload state.</span></span> <span data-ttu-id="fbb67-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="fbb67-187">publishingState</span></span>|[<span data-ttu-id="fbb67-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="fbb67-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fbb67-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-189">The publishing state for the app.</span></span> <span data-ttu-id="fbb67-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="fbb67-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fbb67-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="fbb67-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fbb67-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fbb67-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fbb67-193">isAssigned</span></span>|<span data-ttu-id="fbb67-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbb67-194">Boolean</span></span>|<span data-ttu-id="fbb67-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="fbb67-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="fbb67-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fbb67-197">roleScopeTagIds</span></span>|<span data-ttu-id="fbb67-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="fbb67-198">String collection</span></span>|<span data-ttu-id="fbb67-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="fbb67-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="fbb67-201">dependentAppCount</span></span>|<span data-ttu-id="fbb67-202">Int32</span><span class="sxs-lookup"><span data-stu-id="fbb67-202">Int32</span></span>|<span data-ttu-id="fbb67-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="fbb67-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbb67-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fbb67-205">committedContentVersion</span></span>|<span data-ttu-id="fbb67-206">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-206">String</span></span>|<span data-ttu-id="fbb67-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="fbb67-207">The internal committed content version.</span></span> <span data-ttu-id="fbb67-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fbb67-209">fileName</span><span class="sxs-lookup"><span data-stu-id="fbb67-209">fileName</span></span>|<span data-ttu-id="fbb67-210">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-210">String</span></span>|<span data-ttu-id="fbb67-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-211">The name of the main Lob application file.</span></span> <span data-ttu-id="fbb67-212">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fbb67-213">size</span><span class="sxs-lookup"><span data-stu-id="fbb67-213">size</span></span>|<span data-ttu-id="fbb67-214">Int64</span><span class="sxs-lookup"><span data-stu-id="fbb67-214">Int64</span></span>|<span data-ttu-id="fbb67-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="fbb67-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="fbb67-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbb67-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fbb67-217">packageId</span><span class="sxs-lookup"><span data-stu-id="fbb67-217">packageId</span></span>|<span data-ttu-id="fbb67-218">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-218">String</span></span>|<span data-ttu-id="fbb67-219">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="fbb67-219">The package identifier.</span></span>|
|<span data-ttu-id="fbb67-220">identityName</span><span class="sxs-lookup"><span data-stu-id="fbb67-220">identityName</span></span>|<span data-ttu-id="fbb67-221">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-221">String</span></span>|<span data-ttu-id="fbb67-222">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-222">The Identity Name.</span></span>|
|<span data-ttu-id="fbb67-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fbb67-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fbb67-224">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fbb67-224">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="fbb67-225">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="fbb67-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="fbb67-226">versionName</span><span class="sxs-lookup"><span data-stu-id="fbb67-226">versionName</span></span>|<span data-ttu-id="fbb67-227">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-227">String</span></span>|<span data-ttu-id="fbb67-228">Имя версии бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="fbb67-228">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="fbb67-229">versionCode</span><span class="sxs-lookup"><span data-stu-id="fbb67-229">versionCode</span></span>|<span data-ttu-id="fbb67-230">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-230">String</span></span>|<span data-ttu-id="fbb67-231">Код версии бизнес-приложения Android.</span><span class="sxs-lookup"><span data-stu-id="fbb67-231">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="fbb67-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="fbb67-232">identityVersion</span></span>|<span data-ttu-id="fbb67-233">String</span><span class="sxs-lookup"><span data-stu-id="fbb67-233">String</span></span>|<span data-ttu-id="fbb67-234">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="fbb67-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="fbb67-235">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbb67-235">Response</span></span>
<span data-ttu-id="fbb67-236">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidLobApp](../resources/intune-apps-androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fbb67-236">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbb67-237">Пример</span><span class="sxs-lookup"><span data-stu-id="fbb67-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbb67-238">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbb67-238">Request</span></span>
<span data-ttu-id="fbb67-239">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbb67-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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

### <a name="response"></a><span data-ttu-id="fbb67-240">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbb67-240">Response</span></span>
<span data-ttu-id="fbb67-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbb67-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1585

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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





