---
title: Обновление win32LobApp
description: Обновление свойств объекта win32LobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8ba1e1be5a6fb5bf13cdb900cfc2bf4a6da07358
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760965"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="7923a-103">Обновление win32LobApp</span><span class="sxs-lookup"><span data-stu-id="7923a-103">Update win32LobApp</span></span>

> <span data-ttu-id="7923a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7923a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7923a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7923a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7923a-106">Обновление свойств объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7923a-106">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7923a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7923a-107">Prerequisites</span></span>
<span data-ttu-id="7923a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7923a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7923a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7923a-110">Permission type</span></span>|<span data-ttu-id="7923a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7923a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7923a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7923a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7923a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7923a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7923a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7923a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7923a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7923a-115">Not supported.</span></span>|
|<span data-ttu-id="7923a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7923a-116">Application</span></span>|<span data-ttu-id="7923a-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7923a-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7923a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7923a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="7923a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7923a-119">Request headers</span></span>
|<span data-ttu-id="7923a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7923a-120">Header</span></span>|<span data-ttu-id="7923a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7923a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7923a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7923a-122">Authorization</span></span>|<span data-ttu-id="7923a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7923a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7923a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7923a-124">Accept</span></span>|<span data-ttu-id="7923a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7923a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7923a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7923a-126">Request body</span></span>
<span data-ttu-id="7923a-127">В тексте запроса добавьте представление объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7923a-127">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="7923a-128">В следующей таблице приведены свойства, необходимые при создании [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-128">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="7923a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7923a-129">Property</span></span>|<span data-ttu-id="7923a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7923a-130">Type</span></span>|<span data-ttu-id="7923a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7923a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7923a-132">id</span><span class="sxs-lookup"><span data-stu-id="7923a-132">id</span></span>|<span data-ttu-id="7923a-133">Строка</span><span class="sxs-lookup"><span data-stu-id="7923a-133">String</span></span>|<span data-ttu-id="7923a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7923a-134">Key of the entity.</span></span> <span data-ttu-id="7923a-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7923a-136">displayName</span></span>|<span data-ttu-id="7923a-137">Строка</span><span class="sxs-lookup"><span data-stu-id="7923a-137">String</span></span>|<span data-ttu-id="7923a-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="7923a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7923a-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-140">description</span><span class="sxs-lookup"><span data-stu-id="7923a-140">description</span></span>|<span data-ttu-id="7923a-141">Строка</span><span class="sxs-lookup"><span data-stu-id="7923a-141">String</span></span>|<span data-ttu-id="7923a-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-142">The description of the app.</span></span> <span data-ttu-id="7923a-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-144">publisher</span><span class="sxs-lookup"><span data-stu-id="7923a-144">publisher</span></span>|<span data-ttu-id="7923a-145">String</span><span class="sxs-lookup"><span data-stu-id="7923a-145">String</span></span>|<span data-ttu-id="7923a-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-146">The publisher of the app.</span></span> <span data-ttu-id="7923a-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7923a-148">largeIcon</span></span>|[<span data-ttu-id="7923a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7923a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7923a-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="7923a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7923a-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7923a-152">createdDateTime</span></span>|<span data-ttu-id="7923a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7923a-153">DateTimeOffset</span></span>|<span data-ttu-id="7923a-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-154">The date and time the app was created.</span></span> <span data-ttu-id="7923a-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7923a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7923a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7923a-157">DateTimeOffset</span></span>|<span data-ttu-id="7923a-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7923a-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7923a-160">isFeatured</span></span>|<span data-ttu-id="7923a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7923a-161">Boolean</span></span>|<span data-ttu-id="7923a-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7923a-163">privacyInformationUrl</span></span>|<span data-ttu-id="7923a-164">String</span><span class="sxs-lookup"><span data-stu-id="7923a-164">String</span></span>|<span data-ttu-id="7923a-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="7923a-165">The privacy statement Url.</span></span> <span data-ttu-id="7923a-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7923a-167">informationUrl</span></span>|<span data-ttu-id="7923a-168">String</span><span class="sxs-lookup"><span data-stu-id="7923a-168">String</span></span>|<span data-ttu-id="7923a-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="7923a-169">The more information Url.</span></span> <span data-ttu-id="7923a-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-171">owner</span><span class="sxs-lookup"><span data-stu-id="7923a-171">owner</span></span>|<span data-ttu-id="7923a-172">String</span><span class="sxs-lookup"><span data-stu-id="7923a-172">String</span></span>|<span data-ttu-id="7923a-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-173">The owner of the app.</span></span> <span data-ttu-id="7923a-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-175">developer</span><span class="sxs-lookup"><span data-stu-id="7923a-175">developer</span></span>|<span data-ttu-id="7923a-176">String</span><span class="sxs-lookup"><span data-stu-id="7923a-176">String</span></span>|<span data-ttu-id="7923a-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-177">The developer of the app.</span></span> <span data-ttu-id="7923a-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-179">notes</span><span class="sxs-lookup"><span data-stu-id="7923a-179">notes</span></span>|<span data-ttu-id="7923a-180">String</span><span class="sxs-lookup"><span data-stu-id="7923a-180">String</span></span>|<span data-ttu-id="7923a-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-181">Notes for the app.</span></span> <span data-ttu-id="7923a-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="7923a-183">uploadState</span></span>|<span data-ttu-id="7923a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="7923a-184">Int32</span></span>|<span data-ttu-id="7923a-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="7923a-185">The upload state.</span></span> <span data-ttu-id="7923a-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="7923a-187">publishingState</span></span>|[<span data-ttu-id="7923a-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="7923a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7923a-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-189">The publishing state for the app.</span></span> <span data-ttu-id="7923a-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="7923a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7923a-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="7923a-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7923a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7923a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7923a-193">isAssigned</span></span>|<span data-ttu-id="7923a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7923a-194">Boolean</span></span>|<span data-ttu-id="7923a-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="7923a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7923a-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7923a-197">roleScopeTagIds</span></span>|<span data-ttu-id="7923a-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7923a-198">String collection</span></span>|<span data-ttu-id="7923a-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7923a-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="7923a-201">dependentAppCount</span></span>|<span data-ttu-id="7923a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="7923a-202">Int32</span></span>|<span data-ttu-id="7923a-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7923a-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7923a-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7923a-205">committedContentVersion</span></span>|<span data-ttu-id="7923a-206">String</span><span class="sxs-lookup"><span data-stu-id="7923a-206">String</span></span>|<span data-ttu-id="7923a-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="7923a-207">The internal committed content version.</span></span> <span data-ttu-id="7923a-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7923a-209">fileName</span><span class="sxs-lookup"><span data-stu-id="7923a-209">fileName</span></span>|<span data-ttu-id="7923a-210">String</span><span class="sxs-lookup"><span data-stu-id="7923a-210">String</span></span>|<span data-ttu-id="7923a-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-211">The name of the main Lob application file.</span></span> <span data-ttu-id="7923a-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7923a-213">size</span><span class="sxs-lookup"><span data-stu-id="7923a-213">size</span></span>|<span data-ttu-id="7923a-214">Int64</span><span class="sxs-lookup"><span data-stu-id="7923a-214">Int64</span></span>|<span data-ttu-id="7923a-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="7923a-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="7923a-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="7923a-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7923a-217">инсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="7923a-217">installCommandLine</span></span>|<span data-ttu-id="7923a-218">String</span><span class="sxs-lookup"><span data-stu-id="7923a-218">String</span></span>|<span data-ttu-id="7923a-219">Командная строка для установки приложения</span><span class="sxs-lookup"><span data-stu-id="7923a-219">The command line to install this app</span></span>|
|<span data-ttu-id="7923a-220">унинсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="7923a-220">uninstallCommandLine</span></span>|<span data-ttu-id="7923a-221">String</span><span class="sxs-lookup"><span data-stu-id="7923a-221">String</span></span>|<span data-ttu-id="7923a-222">Командная строка для удаления приложения</span><span class="sxs-lookup"><span data-stu-id="7923a-222">The command line to uninstall this app</span></span>|
|<span data-ttu-id="7923a-223">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="7923a-223">applicableArchitectures</span></span>|[<span data-ttu-id="7923a-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="7923a-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="7923a-225">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="7923a-225">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="7923a-226">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="7923a-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="7923a-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7923a-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7923a-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7923a-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="7923a-229">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="7923a-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="7923a-230">минимумфридискспацеинмб</span><span class="sxs-lookup"><span data-stu-id="7923a-230">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="7923a-231">Int32</span><span class="sxs-lookup"><span data-stu-id="7923a-231">Int32</span></span>|<span data-ttu-id="7923a-232">Минимальное свободное место на диске, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-232">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="7923a-233">минимуммеморинмб</span><span class="sxs-lookup"><span data-stu-id="7923a-233">minimumMemoryInMB</span></span>|<span data-ttu-id="7923a-234">Int32</span><span class="sxs-lookup"><span data-stu-id="7923a-234">Int32</span></span>|<span data-ttu-id="7923a-235">Значение минимальной физической памяти, необходимой для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-235">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="7923a-236">минимумнумберофпроцессорс</span><span class="sxs-lookup"><span data-stu-id="7923a-236">minimumNumberOfProcessors</span></span>|<span data-ttu-id="7923a-237">Int32</span><span class="sxs-lookup"><span data-stu-id="7923a-237">Int32</span></span>|<span data-ttu-id="7923a-238">Значение минимального числа процессоров, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-238">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="7923a-239">минимумкпуспидинмхз</span><span class="sxs-lookup"><span data-stu-id="7923a-239">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="7923a-240">Int32</span><span class="sxs-lookup"><span data-stu-id="7923a-240">Int32</span></span>|<span data-ttu-id="7923a-241">Значение минимальной скорости ЦП, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-241">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="7923a-242">детектионрулес</span><span class="sxs-lookup"><span data-stu-id="7923a-242">detectionRules</span></span>|<span data-ttu-id="7923a-243">Коллекция [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="7923a-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="7923a-244">Правила обнаружения для определения бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="7923a-244">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7923a-245">рекуирементрулес</span><span class="sxs-lookup"><span data-stu-id="7923a-245">requirementRules</span></span>|<span data-ttu-id="7923a-246">Коллекция [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="7923a-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="7923a-247">Правила требований для обнаружения бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="7923a-247">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7923a-248">инсталлекспериенце</span><span class="sxs-lookup"><span data-stu-id="7923a-248">installExperience</span></span>|[<span data-ttu-id="7923a-249">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="7923a-249">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="7923a-250">Установка приложения.</span><span class="sxs-lookup"><span data-stu-id="7923a-250">The install experience for this app.</span></span>|
|<span data-ttu-id="7923a-251">ретурнкодес</span><span class="sxs-lookup"><span data-stu-id="7923a-251">returnCodes</span></span>|<span data-ttu-id="7923a-252">Коллекция [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="7923a-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="7923a-253">Коды возврата для поведения после установки.</span><span class="sxs-lookup"><span data-stu-id="7923a-253">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="7923a-254">мсиинформатион</span><span class="sxs-lookup"><span data-stu-id="7923a-254">msiInformation</span></span>|[<span data-ttu-id="7923a-255">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="7923a-255">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="7923a-256">Сведения о MSI, если это приложение Win32 является приложением MSI.</span><span class="sxs-lookup"><span data-stu-id="7923a-256">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="7923a-257">сетупфилепас</span><span class="sxs-lookup"><span data-stu-id="7923a-257">setupFilePath</span></span>|<span data-ttu-id="7923a-258">String</span><span class="sxs-lookup"><span data-stu-id="7923a-258">String</span></span>|<span data-ttu-id="7923a-259">Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="7923a-259">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="7923a-260">installLanguage</span><span class="sxs-lookup"><span data-stu-id="7923a-260">installLanguage</span></span>|<span data-ttu-id="7923a-261">String</span><span class="sxs-lookup"><span data-stu-id="7923a-261">String</span></span>|<span data-ttu-id="7923a-262">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7923a-262">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7923a-263">Ответ</span><span class="sxs-lookup"><span data-stu-id="7923a-263">Response</span></span>
<span data-ttu-id="7923a-264">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7923a-264">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7923a-265">Пример</span><span class="sxs-lookup"><span data-stu-id="7923a-265">Example</span></span>

### <a name="request"></a><span data-ttu-id="7923a-266">Запрос</span><span class="sxs-lookup"><span data-stu-id="7923a-266">Request</span></span>
<span data-ttu-id="7923a-267">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7923a-267">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2865

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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
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
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
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
  "setupFilePath": "Setup File Path value",
  "installLanguage": "Install Language value"
}
```

### <a name="response"></a><span data-ttu-id="7923a-268">Отклик</span><span class="sxs-lookup"><span data-stu-id="7923a-268">Response</span></span>
<span data-ttu-id="7923a-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7923a-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3037

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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
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
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
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
  "setupFilePath": "Setup File Path value",
  "installLanguage": "Install Language value"
}
```




