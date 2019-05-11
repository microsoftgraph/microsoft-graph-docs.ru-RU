---
title: Обновление win32LobApp
description: Обновление свойств объекта win32LobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca694f762de48ee2afdcbb49ebaf70d9dfe11ebf
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934805"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="51da1-103">Обновление win32LobApp</span><span class="sxs-lookup"><span data-stu-id="51da1-103">Update win32LobApp</span></span>

> <span data-ttu-id="51da1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51da1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51da1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51da1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51da1-106">Обновление свойств объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="51da1-106">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51da1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51da1-107">Prerequisites</span></span>
<span data-ttu-id="51da1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51da1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51da1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51da1-110">Permission type</span></span>|<span data-ttu-id="51da1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51da1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51da1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51da1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="51da1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51da1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51da1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51da1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51da1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51da1-115">Not supported.</span></span>|
|<span data-ttu-id="51da1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51da1-116">Application</span></span>|<span data-ttu-id="51da1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51da1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51da1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51da1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="51da1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51da1-119">Request headers</span></span>
|<span data-ttu-id="51da1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51da1-120">Header</span></span>|<span data-ttu-id="51da1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="51da1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51da1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="51da1-122">Authorization</span></span>|<span data-ttu-id="51da1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51da1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51da1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="51da1-124">Accept</span></span>|<span data-ttu-id="51da1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="51da1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51da1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51da1-126">Request body</span></span>
<span data-ttu-id="51da1-127">В тексте запроса добавьте представление объекта [Win32LobApp](../resources/intune-apps-win32lobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51da1-127">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="51da1-128">В следующей таблице приведены свойства, необходимые при создании [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-128">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="51da1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="51da1-129">Property</span></span>|<span data-ttu-id="51da1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="51da1-130">Type</span></span>|<span data-ttu-id="51da1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="51da1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51da1-132">id</span><span class="sxs-lookup"><span data-stu-id="51da1-132">id</span></span>|<span data-ttu-id="51da1-133">Строка</span><span class="sxs-lookup"><span data-stu-id="51da1-133">String</span></span>|<span data-ttu-id="51da1-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="51da1-134">Key of the entity.</span></span> <span data-ttu-id="51da1-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="51da1-136">displayName</span></span>|<span data-ttu-id="51da1-137">Строка</span><span class="sxs-lookup"><span data-stu-id="51da1-137">String</span></span>|<span data-ttu-id="51da1-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="51da1-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="51da1-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-140">description</span><span class="sxs-lookup"><span data-stu-id="51da1-140">description</span></span>|<span data-ttu-id="51da1-141">Строка</span><span class="sxs-lookup"><span data-stu-id="51da1-141">String</span></span>|<span data-ttu-id="51da1-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-142">The description of the app.</span></span> <span data-ttu-id="51da1-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-144">publisher</span><span class="sxs-lookup"><span data-stu-id="51da1-144">publisher</span></span>|<span data-ttu-id="51da1-145">Строка</span><span class="sxs-lookup"><span data-stu-id="51da1-145">String</span></span>|<span data-ttu-id="51da1-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-146">The publisher of the app.</span></span> <span data-ttu-id="51da1-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="51da1-148">largeIcon</span></span>|[<span data-ttu-id="51da1-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="51da1-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="51da1-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="51da1-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="51da1-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51da1-152">createdDateTime</span></span>|<span data-ttu-id="51da1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51da1-153">DateTimeOffset</span></span>|<span data-ttu-id="51da1-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-154">The date and time the app was created.</span></span> <span data-ttu-id="51da1-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51da1-156">lastModifiedDateTime</span></span>|<span data-ttu-id="51da1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51da1-157">DateTimeOffset</span></span>|<span data-ttu-id="51da1-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-158">The date and time the app was last modified.</span></span> <span data-ttu-id="51da1-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="51da1-160">isFeatured</span></span>|<span data-ttu-id="51da1-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="51da1-161">Boolean</span></span>|<span data-ttu-id="51da1-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="51da1-163">privacyInformationUrl</span></span>|<span data-ttu-id="51da1-164">Строка</span><span class="sxs-lookup"><span data-stu-id="51da1-164">String</span></span>|<span data-ttu-id="51da1-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="51da1-165">The privacy statement Url.</span></span> <span data-ttu-id="51da1-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="51da1-167">informationUrl</span></span>|<span data-ttu-id="51da1-168">Строка</span><span class="sxs-lookup"><span data-stu-id="51da1-168">String</span></span>|<span data-ttu-id="51da1-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="51da1-169">The more information Url.</span></span> <span data-ttu-id="51da1-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-171">owner</span><span class="sxs-lookup"><span data-stu-id="51da1-171">owner</span></span>|<span data-ttu-id="51da1-172">String</span><span class="sxs-lookup"><span data-stu-id="51da1-172">String</span></span>|<span data-ttu-id="51da1-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-173">The owner of the app.</span></span> <span data-ttu-id="51da1-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-175">developer</span><span class="sxs-lookup"><span data-stu-id="51da1-175">developer</span></span>|<span data-ttu-id="51da1-176">Строка</span><span class="sxs-lookup"><span data-stu-id="51da1-176">String</span></span>|<span data-ttu-id="51da1-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-177">The developer of the app.</span></span> <span data-ttu-id="51da1-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-179">notes</span><span class="sxs-lookup"><span data-stu-id="51da1-179">notes</span></span>|<span data-ttu-id="51da1-180">Строка</span><span class="sxs-lookup"><span data-stu-id="51da1-180">String</span></span>|<span data-ttu-id="51da1-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-181">Notes for the app.</span></span> <span data-ttu-id="51da1-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="51da1-183">uploadState</span></span>|<span data-ttu-id="51da1-184">Int32</span><span class="sxs-lookup"><span data-stu-id="51da1-184">Int32</span></span>|<span data-ttu-id="51da1-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="51da1-185">The upload state.</span></span> <span data-ttu-id="51da1-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="51da1-187">publishingState</span></span>|[<span data-ttu-id="51da1-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="51da1-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="51da1-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-189">The publishing state for the app.</span></span> <span data-ttu-id="51da1-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="51da1-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="51da1-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="51da1-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="51da1-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="51da1-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="51da1-193">isAssigned</span></span>|<span data-ttu-id="51da1-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="51da1-194">Boolean</span></span>|<span data-ttu-id="51da1-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="51da1-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="51da1-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51da1-197">roleScopeTagIds</span></span>|<span data-ttu-id="51da1-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="51da1-198">String collection</span></span>|<span data-ttu-id="51da1-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="51da1-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="51da1-201">dependentAppCount</span></span>|<span data-ttu-id="51da1-202">Int32</span><span class="sxs-lookup"><span data-stu-id="51da1-202">Int32</span></span>|<span data-ttu-id="51da1-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="51da1-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51da1-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="51da1-205">committedContentVersion</span></span>|<span data-ttu-id="51da1-206">Строка</span><span class="sxs-lookup"><span data-stu-id="51da1-206">String</span></span>|<span data-ttu-id="51da1-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="51da1-207">The internal committed content version.</span></span> <span data-ttu-id="51da1-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="51da1-209">fileName</span><span class="sxs-lookup"><span data-stu-id="51da1-209">fileName</span></span>|<span data-ttu-id="51da1-210">String</span><span class="sxs-lookup"><span data-stu-id="51da1-210">String</span></span>|<span data-ttu-id="51da1-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-211">The name of the main Lob application file.</span></span> <span data-ttu-id="51da1-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="51da1-213">size</span><span class="sxs-lookup"><span data-stu-id="51da1-213">size</span></span>|<span data-ttu-id="51da1-214">Int64</span><span class="sxs-lookup"><span data-stu-id="51da1-214">Int64</span></span>|<span data-ttu-id="51da1-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="51da1-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="51da1-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="51da1-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="51da1-217">Инсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="51da1-217">installCommandLine</span></span>|<span data-ttu-id="51da1-218">Строка</span><span class="sxs-lookup"><span data-stu-id="51da1-218">String</span></span>|<span data-ttu-id="51da1-219">Командная строка для установки приложения</span><span class="sxs-lookup"><span data-stu-id="51da1-219">The command line to install this app</span></span>|
|<span data-ttu-id="51da1-220">Унинсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="51da1-220">uninstallCommandLine</span></span>|<span data-ttu-id="51da1-221">Строка</span><span class="sxs-lookup"><span data-stu-id="51da1-221">String</span></span>|<span data-ttu-id="51da1-222">Командная строка для удаления приложения</span><span class="sxs-lookup"><span data-stu-id="51da1-222">The command line to uninstall this app</span></span>|
|<span data-ttu-id="51da1-223">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="51da1-223">applicableArchitectures</span></span>|[<span data-ttu-id="51da1-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="51da1-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="51da1-225">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="51da1-225">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="51da1-226">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="51da1-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="51da1-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="51da1-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="51da1-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="51da1-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="51da1-229">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="51da1-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="51da1-230">Минимумфридискспацеинмб</span><span class="sxs-lookup"><span data-stu-id="51da1-230">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="51da1-231">Int32</span><span class="sxs-lookup"><span data-stu-id="51da1-231">Int32</span></span>|<span data-ttu-id="51da1-232">Минимальное свободное место на диске, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-232">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="51da1-233">Минимуммеморинмб</span><span class="sxs-lookup"><span data-stu-id="51da1-233">minimumMemoryInMB</span></span>|<span data-ttu-id="51da1-234">Int32</span><span class="sxs-lookup"><span data-stu-id="51da1-234">Int32</span></span>|<span data-ttu-id="51da1-235">Значение минимальной физической памяти, необходимой для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-235">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="51da1-236">Минимумнумберофпроцессорс</span><span class="sxs-lookup"><span data-stu-id="51da1-236">minimumNumberOfProcessors</span></span>|<span data-ttu-id="51da1-237">Int32</span><span class="sxs-lookup"><span data-stu-id="51da1-237">Int32</span></span>|<span data-ttu-id="51da1-238">Значение минимального числа процессоров, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-238">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="51da1-239">Минимумкпуспидинмхз</span><span class="sxs-lookup"><span data-stu-id="51da1-239">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="51da1-240">Int32</span><span class="sxs-lookup"><span data-stu-id="51da1-240">Int32</span></span>|<span data-ttu-id="51da1-241">Значение минимальной скорости ЦП, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-241">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="51da1-242">Детектионрулес</span><span class="sxs-lookup"><span data-stu-id="51da1-242">detectionRules</span></span>|<span data-ttu-id="51da1-243">Коллекция [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="51da1-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="51da1-244">Правила обнаружения для определения бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="51da1-244">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="51da1-245">Рекуирементрулес</span><span class="sxs-lookup"><span data-stu-id="51da1-245">requirementRules</span></span>|<span data-ttu-id="51da1-246">Коллекция [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="51da1-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="51da1-247">Правила требований для обнаружения бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="51da1-247">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="51da1-248">Инсталлекспериенце</span><span class="sxs-lookup"><span data-stu-id="51da1-248">installExperience</span></span>|[<span data-ttu-id="51da1-249">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="51da1-249">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="51da1-250">Установка приложения.</span><span class="sxs-lookup"><span data-stu-id="51da1-250">The install experience for this app.</span></span>|
|<span data-ttu-id="51da1-251">Ретурнкодес</span><span class="sxs-lookup"><span data-stu-id="51da1-251">returnCodes</span></span>|<span data-ttu-id="51da1-252">Коллекция [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="51da1-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="51da1-253">Коды возврата для поведения после установки.</span><span class="sxs-lookup"><span data-stu-id="51da1-253">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="51da1-254">Мсиинформатион</span><span class="sxs-lookup"><span data-stu-id="51da1-254">msiInformation</span></span>|[<span data-ttu-id="51da1-255">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="51da1-255">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="51da1-256">Сведения о MSI, если это приложение Win32 является приложением MSI.</span><span class="sxs-lookup"><span data-stu-id="51da1-256">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="51da1-257">Сетупфилепас</span><span class="sxs-lookup"><span data-stu-id="51da1-257">setupFilePath</span></span>|<span data-ttu-id="51da1-258">Строка</span><span class="sxs-lookup"><span data-stu-id="51da1-258">String</span></span>|<span data-ttu-id="51da1-259">Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="51da1-259">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="51da1-260">Отклик</span><span class="sxs-lookup"><span data-stu-id="51da1-260">Response</span></span>
<span data-ttu-id="51da1-261">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51da1-261">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51da1-262">Пример</span><span class="sxs-lookup"><span data-stu-id="51da1-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="51da1-263">Запрос</span><span class="sxs-lookup"><span data-stu-id="51da1-263">Request</span></span>
<span data-ttu-id="51da1-264">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51da1-264">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2732

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="51da1-265">Отклик</span><span class="sxs-lookup"><span data-stu-id="51da1-265">Response</span></span>
<span data-ttu-id="51da1-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51da1-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2904

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value"
}
```




