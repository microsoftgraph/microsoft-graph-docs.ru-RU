---
title: Update iosLobApp
description: Обновление свойств объекта iosLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 97e04e5895b97bfe514b6c787b93a2bc9ebf2c7a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445724"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="9ba15-103">Update iosLobApp</span><span class="sxs-lookup"><span data-stu-id="9ba15-103">Update iosLobApp</span></span>

<span data-ttu-id="9ba15-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9ba15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ba15-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ba15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ba15-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ba15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ba15-107">Обновление свойств объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-107">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ba15-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="9ba15-108">Prerequisites</span></span>
<span data-ttu-id="9ba15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ba15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ba15-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ba15-111">Permission type</span></span>|<span data-ttu-id="9ba15-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ba15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ba15-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ba15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ba15-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ba15-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ba15-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ba15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ba15-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ba15-116">Not supported.</span></span>|
|<span data-ttu-id="9ba15-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ba15-117">Application</span></span>|<span data-ttu-id="9ba15-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ba15-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ba15-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ba15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9ba15-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9ba15-120">Request headers</span></span>
|<span data-ttu-id="9ba15-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ba15-121">Header</span></span>|<span data-ttu-id="9ba15-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9ba15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ba15-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ba15-123">Authorization</span></span>|<span data-ttu-id="9ba15-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ba15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ba15-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9ba15-125">Accept</span></span>|<span data-ttu-id="9ba15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ba15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ba15-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ba15-127">Request body</span></span>
<span data-ttu-id="9ba15-128">В теле запроса добавьте представление объекта [iosLobApp](../resources/intune-apps-ioslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ba15-128">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="9ba15-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-129">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="9ba15-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ba15-130">Property</span></span>|<span data-ttu-id="9ba15-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9ba15-131">Type</span></span>|<span data-ttu-id="9ba15-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9ba15-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ba15-133">id</span><span class="sxs-lookup"><span data-stu-id="9ba15-133">id</span></span>|<span data-ttu-id="9ba15-134">Строка</span><span class="sxs-lookup"><span data-stu-id="9ba15-134">String</span></span>|<span data-ttu-id="9ba15-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9ba15-135">Key of the entity.</span></span> <span data-ttu-id="9ba15-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9ba15-137">displayName</span></span>|<span data-ttu-id="9ba15-138">Строка</span><span class="sxs-lookup"><span data-stu-id="9ba15-138">String</span></span>|<span data-ttu-id="9ba15-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9ba15-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9ba15-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-141">description</span><span class="sxs-lookup"><span data-stu-id="9ba15-141">description</span></span>|<span data-ttu-id="9ba15-142">Строка</span><span class="sxs-lookup"><span data-stu-id="9ba15-142">String</span></span>|<span data-ttu-id="9ba15-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-143">The description of the app.</span></span> <span data-ttu-id="9ba15-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-145">publisher</span><span class="sxs-lookup"><span data-stu-id="9ba15-145">publisher</span></span>|<span data-ttu-id="9ba15-146">String</span><span class="sxs-lookup"><span data-stu-id="9ba15-146">String</span></span>|<span data-ttu-id="9ba15-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-147">The publisher of the app.</span></span> <span data-ttu-id="9ba15-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9ba15-149">largeIcon</span></span>|[<span data-ttu-id="9ba15-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9ba15-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9ba15-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9ba15-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9ba15-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ba15-153">createdDateTime</span></span>|<span data-ttu-id="9ba15-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ba15-154">DateTimeOffset</span></span>|<span data-ttu-id="9ba15-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-155">The date and time the app was created.</span></span> <span data-ttu-id="9ba15-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ba15-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9ba15-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ba15-158">DateTimeOffset</span></span>|<span data-ttu-id="9ba15-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9ba15-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9ba15-161">isFeatured</span></span>|<span data-ttu-id="9ba15-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ba15-162">Boolean</span></span>|<span data-ttu-id="9ba15-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9ba15-164">privacyInformationUrl</span></span>|<span data-ttu-id="9ba15-165">String</span><span class="sxs-lookup"><span data-stu-id="9ba15-165">String</span></span>|<span data-ttu-id="9ba15-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9ba15-166">The privacy statement Url.</span></span> <span data-ttu-id="9ba15-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9ba15-168">informationUrl</span></span>|<span data-ttu-id="9ba15-169">String</span><span class="sxs-lookup"><span data-stu-id="9ba15-169">String</span></span>|<span data-ttu-id="9ba15-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9ba15-170">The more information Url.</span></span> <span data-ttu-id="9ba15-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-172">owner</span><span class="sxs-lookup"><span data-stu-id="9ba15-172">owner</span></span>|<span data-ttu-id="9ba15-173">String</span><span class="sxs-lookup"><span data-stu-id="9ba15-173">String</span></span>|<span data-ttu-id="9ba15-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-174">The owner of the app.</span></span> <span data-ttu-id="9ba15-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-176">developer</span><span class="sxs-lookup"><span data-stu-id="9ba15-176">developer</span></span>|<span data-ttu-id="9ba15-177">String</span><span class="sxs-lookup"><span data-stu-id="9ba15-177">String</span></span>|<span data-ttu-id="9ba15-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-178">The developer of the app.</span></span> <span data-ttu-id="9ba15-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-180">notes</span><span class="sxs-lookup"><span data-stu-id="9ba15-180">notes</span></span>|<span data-ttu-id="9ba15-181">String</span><span class="sxs-lookup"><span data-stu-id="9ba15-181">String</span></span>|<span data-ttu-id="9ba15-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-182">Notes for the app.</span></span> <span data-ttu-id="9ba15-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9ba15-184">uploadState</span></span>|<span data-ttu-id="9ba15-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9ba15-185">Int32</span></span>|<span data-ttu-id="9ba15-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="9ba15-186">The upload state.</span></span> <span data-ttu-id="9ba15-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="9ba15-188">publishingState</span></span>|[<span data-ttu-id="9ba15-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9ba15-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9ba15-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-190">The publishing state for the app.</span></span> <span data-ttu-id="9ba15-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9ba15-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9ba15-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="9ba15-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9ba15-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9ba15-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9ba15-194">isAssigned</span></span>|<span data-ttu-id="9ba15-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ba15-195">Boolean</span></span>|<span data-ttu-id="9ba15-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="9ba15-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9ba15-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ba15-198">roleScopeTagIds</span></span>|<span data-ttu-id="9ba15-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9ba15-199">String collection</span></span>|<span data-ttu-id="9ba15-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9ba15-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="9ba15-202">dependentAppCount</span></span>|<span data-ttu-id="9ba15-203">Int32</span><span class="sxs-lookup"><span data-stu-id="9ba15-203">Int32</span></span>|<span data-ttu-id="9ba15-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9ba15-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9ba15-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9ba15-206">committedContentVersion</span></span>|<span data-ttu-id="9ba15-207">String</span><span class="sxs-lookup"><span data-stu-id="9ba15-207">String</span></span>|<span data-ttu-id="9ba15-208">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="9ba15-208">The internal committed content version.</span></span> <span data-ttu-id="9ba15-209">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9ba15-210">fileName</span><span class="sxs-lookup"><span data-stu-id="9ba15-210">fileName</span></span>|<span data-ttu-id="9ba15-211">String</span><span class="sxs-lookup"><span data-stu-id="9ba15-211">String</span></span>|<span data-ttu-id="9ba15-212">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-212">The name of the main Lob application file.</span></span> <span data-ttu-id="9ba15-213">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9ba15-214">size</span><span class="sxs-lookup"><span data-stu-id="9ba15-214">size</span></span>|<span data-ttu-id="9ba15-215">Int64</span><span class="sxs-lookup"><span data-stu-id="9ba15-215">Int64</span></span>|<span data-ttu-id="9ba15-216">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="9ba15-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="9ba15-217">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9ba15-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9ba15-218">bundleId</span><span class="sxs-lookup"><span data-stu-id="9ba15-218">bundleId</span></span>|<span data-ttu-id="9ba15-219">String</span><span class="sxs-lookup"><span data-stu-id="9ba15-219">String</span></span>|<span data-ttu-id="9ba15-220">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-220">The Identity Name.</span></span>|
|<span data-ttu-id="9ba15-221">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9ba15-221">applicableDeviceType</span></span>|[<span data-ttu-id="9ba15-222">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9ba15-222">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="9ba15-223">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="9ba15-223">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="9ba15-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9ba15-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9ba15-225">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9ba15-225">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="9ba15-226">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="9ba15-226">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9ba15-227">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9ba15-227">expirationDateTime</span></span>|<span data-ttu-id="9ba15-228">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ba15-228">DateTimeOffset</span></span>|<span data-ttu-id="9ba15-229">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="9ba15-229">The expiration time.</span></span>|
|<span data-ttu-id="9ba15-230">versionNumber</span><span class="sxs-lookup"><span data-stu-id="9ba15-230">versionNumber</span></span>|<span data-ttu-id="9ba15-231">String</span><span class="sxs-lookup"><span data-stu-id="9ba15-231">String</span></span>|<span data-ttu-id="9ba15-232">Номер версии бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="9ba15-232">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9ba15-233">buildNumber</span><span class="sxs-lookup"><span data-stu-id="9ba15-233">buildNumber</span></span>|<span data-ttu-id="9ba15-234">String</span><span class="sxs-lookup"><span data-stu-id="9ba15-234">String</span></span>|<span data-ttu-id="9ba15-235">Номер сборки бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="9ba15-235">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9ba15-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9ba15-236">identityVersion</span></span>|<span data-ttu-id="9ba15-237">String</span><span class="sxs-lookup"><span data-stu-id="9ba15-237">String</span></span>|<span data-ttu-id="9ba15-238">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="9ba15-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="9ba15-239">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ba15-239">Response</span></span>
<span data-ttu-id="9ba15-240">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosLobApp](../resources/intune-apps-ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9ba15-240">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ba15-241">Пример</span><span class="sxs-lookup"><span data-stu-id="9ba15-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ba15-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ba15-242">Request</span></span>
<span data-ttu-id="9ba15-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ba15-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1411

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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

### <a name="response"></a><span data-ttu-id="9ba15-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ba15-244">Response</span></span>
<span data-ttu-id="9ba15-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ba15-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1583

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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





