---
title: Обновление win32LobApp
description: Обновление свойств объекта win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e3311aa409752353b3be63915a938a620e3aca2
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793250"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="52563-103">Обновление win32LobApp</span><span class="sxs-lookup"><span data-stu-id="52563-103">Update win32LobApp</span></span>

<span data-ttu-id="52563-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52563-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52563-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52563-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52563-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52563-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52563-107">Обновление свойств объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="52563-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52563-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="52563-108">Prerequisites</span></span>
<span data-ttu-id="52563-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="52563-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="52563-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52563-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52563-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="52563-111">Permission type</span></span>|<span data-ttu-id="52563-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="52563-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52563-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="52563-113">Delegated (work or school account)</span></span>|<span data-ttu-id="52563-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52563-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="52563-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="52563-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52563-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52563-116">Not supported.</span></span>|
|<span data-ttu-id="52563-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="52563-117">Application</span></span>|<span data-ttu-id="52563-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52563-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="52563-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="52563-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="52563-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="52563-120">Request headers</span></span>
|<span data-ttu-id="52563-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="52563-121">Header</span></span>|<span data-ttu-id="52563-122">Значение</span><span class="sxs-lookup"><span data-stu-id="52563-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52563-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="52563-123">Authorization</span></span>|<span data-ttu-id="52563-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="52563-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52563-125">Accept</span><span class="sxs-lookup"><span data-stu-id="52563-125">Accept</span></span>|<span data-ttu-id="52563-126">application/json</span><span class="sxs-lookup"><span data-stu-id="52563-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52563-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="52563-127">Request body</span></span>
<span data-ttu-id="52563-128">В тексте запроса добавьте представление объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52563-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="52563-129">В следующей таблице приведены свойства, необходимые при создании [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="52563-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="52563-130">Property</span></span>|<span data-ttu-id="52563-131">Тип</span><span class="sxs-lookup"><span data-stu-id="52563-131">Type</span></span>|<span data-ttu-id="52563-132">Описание</span><span class="sxs-lookup"><span data-stu-id="52563-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52563-133">id</span><span class="sxs-lookup"><span data-stu-id="52563-133">id</span></span>|<span data-ttu-id="52563-134">Строка</span><span class="sxs-lookup"><span data-stu-id="52563-134">String</span></span>|<span data-ttu-id="52563-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="52563-135">Key of the entity.</span></span> <span data-ttu-id="52563-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-137">displayName</span><span class="sxs-lookup"><span data-stu-id="52563-137">displayName</span></span>|<span data-ttu-id="52563-138">Строка</span><span class="sxs-lookup"><span data-stu-id="52563-138">String</span></span>|<span data-ttu-id="52563-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="52563-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="52563-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-141">description</span><span class="sxs-lookup"><span data-stu-id="52563-141">description</span></span>|<span data-ttu-id="52563-142">Строка</span><span class="sxs-lookup"><span data-stu-id="52563-142">String</span></span>|<span data-ttu-id="52563-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-143">The description of the app.</span></span> <span data-ttu-id="52563-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-145">publisher</span><span class="sxs-lookup"><span data-stu-id="52563-145">publisher</span></span>|<span data-ttu-id="52563-146">String</span><span class="sxs-lookup"><span data-stu-id="52563-146">String</span></span>|<span data-ttu-id="52563-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-147">The publisher of the app.</span></span> <span data-ttu-id="52563-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="52563-149">largeIcon</span></span>|[<span data-ttu-id="52563-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="52563-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="52563-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="52563-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="52563-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52563-153">createdDateTime</span></span>|<span data-ttu-id="52563-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52563-154">DateTimeOffset</span></span>|<span data-ttu-id="52563-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-155">The date and time the app was created.</span></span> <span data-ttu-id="52563-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52563-157">lastModifiedDateTime</span></span>|<span data-ttu-id="52563-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52563-158">DateTimeOffset</span></span>|<span data-ttu-id="52563-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-159">The date and time the app was last modified.</span></span> <span data-ttu-id="52563-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="52563-161">isFeatured</span></span>|<span data-ttu-id="52563-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="52563-162">Boolean</span></span>|<span data-ttu-id="52563-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="52563-164">privacyInformationUrl</span></span>|<span data-ttu-id="52563-165">String</span><span class="sxs-lookup"><span data-stu-id="52563-165">String</span></span>|<span data-ttu-id="52563-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="52563-166">The privacy statement Url.</span></span> <span data-ttu-id="52563-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="52563-168">informationUrl</span></span>|<span data-ttu-id="52563-169">String</span><span class="sxs-lookup"><span data-stu-id="52563-169">String</span></span>|<span data-ttu-id="52563-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="52563-170">The more information Url.</span></span> <span data-ttu-id="52563-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-172">owner</span><span class="sxs-lookup"><span data-stu-id="52563-172">owner</span></span>|<span data-ttu-id="52563-173">String</span><span class="sxs-lookup"><span data-stu-id="52563-173">String</span></span>|<span data-ttu-id="52563-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-174">The owner of the app.</span></span> <span data-ttu-id="52563-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-176">developer</span><span class="sxs-lookup"><span data-stu-id="52563-176">developer</span></span>|<span data-ttu-id="52563-177">String</span><span class="sxs-lookup"><span data-stu-id="52563-177">String</span></span>|<span data-ttu-id="52563-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-178">The developer of the app.</span></span> <span data-ttu-id="52563-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-180">notes</span><span class="sxs-lookup"><span data-stu-id="52563-180">notes</span></span>|<span data-ttu-id="52563-181">String</span><span class="sxs-lookup"><span data-stu-id="52563-181">String</span></span>|<span data-ttu-id="52563-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-182">Notes for the app.</span></span> <span data-ttu-id="52563-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="52563-184">uploadState</span></span>|<span data-ttu-id="52563-185">Int32</span><span class="sxs-lookup"><span data-stu-id="52563-185">Int32</span></span>|<span data-ttu-id="52563-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="52563-186">The upload state.</span></span> <span data-ttu-id="52563-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="52563-188">publishingState</span></span>|[<span data-ttu-id="52563-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="52563-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="52563-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-190">The publishing state for the app.</span></span> <span data-ttu-id="52563-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="52563-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="52563-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="52563-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="52563-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="52563-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="52563-194">isAssigned</span></span>|<span data-ttu-id="52563-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="52563-195">Boolean</span></span>|<span data-ttu-id="52563-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="52563-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="52563-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="52563-198">roleScopeTagIds</span></span>|<span data-ttu-id="52563-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="52563-199">String collection</span></span>|<span data-ttu-id="52563-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="52563-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="52563-202">dependentAppCount</span></span>|<span data-ttu-id="52563-203">Int32</span><span class="sxs-lookup"><span data-stu-id="52563-203">Int32</span></span>|<span data-ttu-id="52563-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="52563-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="52563-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="52563-206">committedContentVersion</span></span>|<span data-ttu-id="52563-207">String</span><span class="sxs-lookup"><span data-stu-id="52563-207">String</span></span>|<span data-ttu-id="52563-208">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="52563-208">The internal committed content version.</span></span> <span data-ttu-id="52563-209">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="52563-210">fileName</span><span class="sxs-lookup"><span data-stu-id="52563-210">fileName</span></span>|<span data-ttu-id="52563-211">String</span><span class="sxs-lookup"><span data-stu-id="52563-211">String</span></span>|<span data-ttu-id="52563-212">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-212">The name of the main Lob application file.</span></span> <span data-ttu-id="52563-213">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="52563-214">size</span><span class="sxs-lookup"><span data-stu-id="52563-214">size</span></span>|<span data-ttu-id="52563-215">Int64</span><span class="sxs-lookup"><span data-stu-id="52563-215">Int64</span></span>|<span data-ttu-id="52563-216">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="52563-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="52563-217">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="52563-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="52563-218">инсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="52563-218">installCommandLine</span></span>|<span data-ttu-id="52563-219">String</span><span class="sxs-lookup"><span data-stu-id="52563-219">String</span></span>|<span data-ttu-id="52563-220">Командная строка для установки приложения</span><span class="sxs-lookup"><span data-stu-id="52563-220">The command line to install this app</span></span>|
|<span data-ttu-id="52563-221">унинсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="52563-221">uninstallCommandLine</span></span>|<span data-ttu-id="52563-222">String</span><span class="sxs-lookup"><span data-stu-id="52563-222">String</span></span>|<span data-ttu-id="52563-223">Командная строка для удаления приложения</span><span class="sxs-lookup"><span data-stu-id="52563-223">The command line to uninstall this app</span></span>|
|<span data-ttu-id="52563-224">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="52563-224">applicableArchitectures</span></span>|[<span data-ttu-id="52563-225">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="52563-225">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="52563-226">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="52563-226">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="52563-227">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="52563-227">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="52563-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="52563-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="52563-229">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="52563-229">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="52563-230">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="52563-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="52563-231">минимумфридискспацеинмб</span><span class="sxs-lookup"><span data-stu-id="52563-231">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="52563-232">Int32</span><span class="sxs-lookup"><span data-stu-id="52563-232">Int32</span></span>|<span data-ttu-id="52563-233">Минимальное свободное место на диске, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-233">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="52563-234">минимуммеморинмб</span><span class="sxs-lookup"><span data-stu-id="52563-234">minimumMemoryInMB</span></span>|<span data-ttu-id="52563-235">Int32</span><span class="sxs-lookup"><span data-stu-id="52563-235">Int32</span></span>|<span data-ttu-id="52563-236">Значение минимальной физической памяти, необходимой для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-236">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="52563-237">минимумнумберофпроцессорс</span><span class="sxs-lookup"><span data-stu-id="52563-237">minimumNumberOfProcessors</span></span>|<span data-ttu-id="52563-238">Int32</span><span class="sxs-lookup"><span data-stu-id="52563-238">Int32</span></span>|<span data-ttu-id="52563-239">Значение минимального числа процессоров, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-239">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="52563-240">минимумкпуспидинмхз</span><span class="sxs-lookup"><span data-stu-id="52563-240">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="52563-241">Int32</span><span class="sxs-lookup"><span data-stu-id="52563-241">Int32</span></span>|<span data-ttu-id="52563-242">Значение минимальной скорости ЦП, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-242">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="52563-243">детектионрулес</span><span class="sxs-lookup"><span data-stu-id="52563-243">detectionRules</span></span>|<span data-ttu-id="52563-244">Коллекция [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="52563-244">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="52563-245">Правила обнаружения для определения бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="52563-245">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="52563-246">рекуирементрулес</span><span class="sxs-lookup"><span data-stu-id="52563-246">requirementRules</span></span>|<span data-ttu-id="52563-247">Коллекция [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="52563-247">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="52563-248">Правила требований для обнаружения бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="52563-248">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="52563-249">правила</span><span class="sxs-lookup"><span data-stu-id="52563-249">rules</span></span>|<span data-ttu-id="52563-250">Коллекция [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="52563-250">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="52563-251">Правила обнаружения и требований для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-251">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="52563-252">инсталлекспериенце</span><span class="sxs-lookup"><span data-stu-id="52563-252">installExperience</span></span>|[<span data-ttu-id="52563-253">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="52563-253">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="52563-254">Установка приложения.</span><span class="sxs-lookup"><span data-stu-id="52563-254">The install experience for this app.</span></span>|
|<span data-ttu-id="52563-255">ретурнкодес</span><span class="sxs-lookup"><span data-stu-id="52563-255">returnCodes</span></span>|<span data-ttu-id="52563-256">Коллекция [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="52563-256">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="52563-257">Коды возврата для поведения после установки.</span><span class="sxs-lookup"><span data-stu-id="52563-257">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="52563-258">мсиинформатион</span><span class="sxs-lookup"><span data-stu-id="52563-258">msiInformation</span></span>|[<span data-ttu-id="52563-259">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="52563-259">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="52563-260">Сведения о MSI, если это приложение Win32 является приложением MSI.</span><span class="sxs-lookup"><span data-stu-id="52563-260">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="52563-261">сетупфилепас</span><span class="sxs-lookup"><span data-stu-id="52563-261">setupFilePath</span></span>|<span data-ttu-id="52563-262">String</span><span class="sxs-lookup"><span data-stu-id="52563-262">String</span></span>|<span data-ttu-id="52563-263">Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="52563-263">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="52563-264">installLanguage</span><span class="sxs-lookup"><span data-stu-id="52563-264">installLanguage</span></span>|<span data-ttu-id="52563-265">String</span><span class="sxs-lookup"><span data-stu-id="52563-265">String</span></span>|<span data-ttu-id="52563-266">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="52563-266">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="52563-267">Ответ</span><span class="sxs-lookup"><span data-stu-id="52563-267">Response</span></span>
<span data-ttu-id="52563-268">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="52563-268">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52563-269">Пример</span><span class="sxs-lookup"><span data-stu-id="52563-269">Example</span></span>

### <a name="request"></a><span data-ttu-id="52563-270">Запрос</span><span class="sxs-lookup"><span data-stu-id="52563-270">Request</span></span>
<span data-ttu-id="52563-271">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="52563-271">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 3224

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
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
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

### <a name="response"></a><span data-ttu-id="52563-272">Отклик</span><span class="sxs-lookup"><span data-stu-id="52563-272">Response</span></span>
<span data-ttu-id="52563-273">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="52563-273">Here is an example of the response.</span></span> <span data-ttu-id="52563-274">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="52563-274">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="52563-275">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="52563-275">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3396

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
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
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



