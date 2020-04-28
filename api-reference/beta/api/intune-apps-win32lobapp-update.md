---
title: Обновление win32LobApp
description: Обновление свойств объекта win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60d20ea301f3553f041b55b5bce31856d81e5cdc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43393874"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="af752-103">Обновление win32LobApp</span><span class="sxs-lookup"><span data-stu-id="af752-103">Update win32LobApp</span></span>

<span data-ttu-id="af752-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af752-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af752-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af752-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af752-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af752-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af752-107">Обновление свойств объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="af752-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af752-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="af752-108">Prerequisites</span></span>
<span data-ttu-id="af752-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af752-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af752-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af752-111">Permission type</span></span>|<span data-ttu-id="af752-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af752-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af752-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af752-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af752-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af752-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="af752-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af752-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af752-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af752-116">Not supported.</span></span>|
|<span data-ttu-id="af752-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af752-117">Application</span></span>|<span data-ttu-id="af752-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af752-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af752-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af752-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="af752-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="af752-120">Request headers</span></span>
|<span data-ttu-id="af752-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af752-121">Header</span></span>|<span data-ttu-id="af752-122">Значение</span><span class="sxs-lookup"><span data-stu-id="af752-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af752-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af752-123">Authorization</span></span>|<span data-ttu-id="af752-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af752-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af752-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af752-125">Accept</span></span>|<span data-ttu-id="af752-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af752-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af752-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af752-127">Request body</span></span>
<span data-ttu-id="af752-128">В тексте запроса добавьте представление объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af752-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="af752-129">В следующей таблице приведены свойства, необходимые при создании [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="af752-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="af752-130">Property</span></span>|<span data-ttu-id="af752-131">Тип</span><span class="sxs-lookup"><span data-stu-id="af752-131">Type</span></span>|<span data-ttu-id="af752-132">Описание</span><span class="sxs-lookup"><span data-stu-id="af752-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af752-133">id</span><span class="sxs-lookup"><span data-stu-id="af752-133">id</span></span>|<span data-ttu-id="af752-134">Строка</span><span class="sxs-lookup"><span data-stu-id="af752-134">String</span></span>|<span data-ttu-id="af752-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="af752-135">Key of the entity.</span></span> <span data-ttu-id="af752-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-137">displayName</span><span class="sxs-lookup"><span data-stu-id="af752-137">displayName</span></span>|<span data-ttu-id="af752-138">Строка</span><span class="sxs-lookup"><span data-stu-id="af752-138">String</span></span>|<span data-ttu-id="af752-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="af752-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="af752-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-141">description</span><span class="sxs-lookup"><span data-stu-id="af752-141">description</span></span>|<span data-ttu-id="af752-142">Строка</span><span class="sxs-lookup"><span data-stu-id="af752-142">String</span></span>|<span data-ttu-id="af752-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-143">The description of the app.</span></span> <span data-ttu-id="af752-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-145">publisher</span><span class="sxs-lookup"><span data-stu-id="af752-145">publisher</span></span>|<span data-ttu-id="af752-146">String</span><span class="sxs-lookup"><span data-stu-id="af752-146">String</span></span>|<span data-ttu-id="af752-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-147">The publisher of the app.</span></span> <span data-ttu-id="af752-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="af752-149">largeIcon</span></span>|[<span data-ttu-id="af752-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="af752-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="af752-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="af752-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="af752-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af752-153">createdDateTime</span></span>|<span data-ttu-id="af752-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af752-154">DateTimeOffset</span></span>|<span data-ttu-id="af752-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-155">The date and time the app was created.</span></span> <span data-ttu-id="af752-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af752-157">lastModifiedDateTime</span></span>|<span data-ttu-id="af752-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af752-158">DateTimeOffset</span></span>|<span data-ttu-id="af752-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-159">The date and time the app was last modified.</span></span> <span data-ttu-id="af752-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="af752-161">isFeatured</span></span>|<span data-ttu-id="af752-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="af752-162">Boolean</span></span>|<span data-ttu-id="af752-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="af752-164">privacyInformationUrl</span></span>|<span data-ttu-id="af752-165">String</span><span class="sxs-lookup"><span data-stu-id="af752-165">String</span></span>|<span data-ttu-id="af752-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="af752-166">The privacy statement Url.</span></span> <span data-ttu-id="af752-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="af752-168">informationUrl</span></span>|<span data-ttu-id="af752-169">String</span><span class="sxs-lookup"><span data-stu-id="af752-169">String</span></span>|<span data-ttu-id="af752-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="af752-170">The more information Url.</span></span> <span data-ttu-id="af752-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-172">owner</span><span class="sxs-lookup"><span data-stu-id="af752-172">owner</span></span>|<span data-ttu-id="af752-173">String</span><span class="sxs-lookup"><span data-stu-id="af752-173">String</span></span>|<span data-ttu-id="af752-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-174">The owner of the app.</span></span> <span data-ttu-id="af752-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-176">developer</span><span class="sxs-lookup"><span data-stu-id="af752-176">developer</span></span>|<span data-ttu-id="af752-177">String</span><span class="sxs-lookup"><span data-stu-id="af752-177">String</span></span>|<span data-ttu-id="af752-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-178">The developer of the app.</span></span> <span data-ttu-id="af752-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-180">notes</span><span class="sxs-lookup"><span data-stu-id="af752-180">notes</span></span>|<span data-ttu-id="af752-181">String</span><span class="sxs-lookup"><span data-stu-id="af752-181">String</span></span>|<span data-ttu-id="af752-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-182">Notes for the app.</span></span> <span data-ttu-id="af752-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="af752-184">uploadState</span></span>|<span data-ttu-id="af752-185">Int32</span><span class="sxs-lookup"><span data-stu-id="af752-185">Int32</span></span>|<span data-ttu-id="af752-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="af752-186">The upload state.</span></span> <span data-ttu-id="af752-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="af752-188">publishingState</span></span>|[<span data-ttu-id="af752-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="af752-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="af752-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-190">The publishing state for the app.</span></span> <span data-ttu-id="af752-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="af752-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="af752-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="af752-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="af752-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="af752-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="af752-194">isAssigned</span></span>|<span data-ttu-id="af752-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="af752-195">Boolean</span></span>|<span data-ttu-id="af752-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="af752-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="af752-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="af752-198">roleScopeTagIds</span></span>|<span data-ttu-id="af752-199">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="af752-199">String collection</span></span>|<span data-ttu-id="af752-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="af752-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="af752-202">dependentAppCount</span></span>|<span data-ttu-id="af752-203">Int32</span><span class="sxs-lookup"><span data-stu-id="af752-203">Int32</span></span>|<span data-ttu-id="af752-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="af752-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="af752-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="af752-206">committedContentVersion</span></span>|<span data-ttu-id="af752-207">String</span><span class="sxs-lookup"><span data-stu-id="af752-207">String</span></span>|<span data-ttu-id="af752-208">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="af752-208">The internal committed content version.</span></span> <span data-ttu-id="af752-209">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="af752-210">fileName</span><span class="sxs-lookup"><span data-stu-id="af752-210">fileName</span></span>|<span data-ttu-id="af752-211">String</span><span class="sxs-lookup"><span data-stu-id="af752-211">String</span></span>|<span data-ttu-id="af752-212">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-212">The name of the main Lob application file.</span></span> <span data-ttu-id="af752-213">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="af752-214">size</span><span class="sxs-lookup"><span data-stu-id="af752-214">size</span></span>|<span data-ttu-id="af752-215">Int64</span><span class="sxs-lookup"><span data-stu-id="af752-215">Int64</span></span>|<span data-ttu-id="af752-216">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="af752-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="af752-217">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="af752-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="af752-218">инсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="af752-218">installCommandLine</span></span>|<span data-ttu-id="af752-219">String</span><span class="sxs-lookup"><span data-stu-id="af752-219">String</span></span>|<span data-ttu-id="af752-220">Командная строка для установки приложения</span><span class="sxs-lookup"><span data-stu-id="af752-220">The command line to install this app</span></span>|
|<span data-ttu-id="af752-221">унинсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="af752-221">uninstallCommandLine</span></span>|<span data-ttu-id="af752-222">String</span><span class="sxs-lookup"><span data-stu-id="af752-222">String</span></span>|<span data-ttu-id="af752-223">Командная строка для удаления приложения</span><span class="sxs-lookup"><span data-stu-id="af752-223">The command line to uninstall this app</span></span>|
|<span data-ttu-id="af752-224">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="af752-224">applicableArchitectures</span></span>|[<span data-ttu-id="af752-225">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="af752-225">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="af752-226">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="af752-226">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="af752-227">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="af752-227">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="af752-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="af752-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="af752-229">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="af752-229">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="af752-230">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="af752-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="af752-231">минимумфридискспацеинмб</span><span class="sxs-lookup"><span data-stu-id="af752-231">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="af752-232">Int32</span><span class="sxs-lookup"><span data-stu-id="af752-232">Int32</span></span>|<span data-ttu-id="af752-233">Минимальное свободное место на диске, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-233">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="af752-234">минимуммеморинмб</span><span class="sxs-lookup"><span data-stu-id="af752-234">minimumMemoryInMB</span></span>|<span data-ttu-id="af752-235">Int32</span><span class="sxs-lookup"><span data-stu-id="af752-235">Int32</span></span>|<span data-ttu-id="af752-236">Значение минимальной физической памяти, необходимой для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-236">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="af752-237">минимумнумберофпроцессорс</span><span class="sxs-lookup"><span data-stu-id="af752-237">minimumNumberOfProcessors</span></span>|<span data-ttu-id="af752-238">Int32</span><span class="sxs-lookup"><span data-stu-id="af752-238">Int32</span></span>|<span data-ttu-id="af752-239">Значение минимального числа процессоров, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-239">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="af752-240">минимумкпуспидинмхз</span><span class="sxs-lookup"><span data-stu-id="af752-240">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="af752-241">Int32</span><span class="sxs-lookup"><span data-stu-id="af752-241">Int32</span></span>|<span data-ttu-id="af752-242">Значение минимальной скорости ЦП, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-242">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="af752-243">детектионрулес</span><span class="sxs-lookup"><span data-stu-id="af752-243">detectionRules</span></span>|<span data-ttu-id="af752-244">Коллекция [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="af752-244">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="af752-245">Правила обнаружения для определения бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="af752-245">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="af752-246">рекуирементрулес</span><span class="sxs-lookup"><span data-stu-id="af752-246">requirementRules</span></span>|<span data-ttu-id="af752-247">Коллекция [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="af752-247">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="af752-248">Правила требований для обнаружения бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="af752-248">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="af752-249">инсталлекспериенце</span><span class="sxs-lookup"><span data-stu-id="af752-249">installExperience</span></span>|[<span data-ttu-id="af752-250">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="af752-250">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="af752-251">Установка приложения.</span><span class="sxs-lookup"><span data-stu-id="af752-251">The install experience for this app.</span></span>|
|<span data-ttu-id="af752-252">ретурнкодес</span><span class="sxs-lookup"><span data-stu-id="af752-252">returnCodes</span></span>|<span data-ttu-id="af752-253">Коллекция [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="af752-253">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="af752-254">Коды возврата для поведения после установки.</span><span class="sxs-lookup"><span data-stu-id="af752-254">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="af752-255">мсиинформатион</span><span class="sxs-lookup"><span data-stu-id="af752-255">msiInformation</span></span>|[<span data-ttu-id="af752-256">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="af752-256">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="af752-257">Сведения о MSI, если это приложение Win32 является приложением MSI.</span><span class="sxs-lookup"><span data-stu-id="af752-257">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="af752-258">сетупфилепас</span><span class="sxs-lookup"><span data-stu-id="af752-258">setupFilePath</span></span>|<span data-ttu-id="af752-259">String</span><span class="sxs-lookup"><span data-stu-id="af752-259">String</span></span>|<span data-ttu-id="af752-260">Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="af752-260">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="af752-261">installLanguage</span><span class="sxs-lookup"><span data-stu-id="af752-261">installLanguage</span></span>|<span data-ttu-id="af752-262">String</span><span class="sxs-lookup"><span data-stu-id="af752-262">String</span></span>|<span data-ttu-id="af752-263">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="af752-263">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="af752-264">Ответ</span><span class="sxs-lookup"><span data-stu-id="af752-264">Response</span></span>
<span data-ttu-id="af752-265">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="af752-265">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af752-266">Пример</span><span class="sxs-lookup"><span data-stu-id="af752-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="af752-267">Запрос</span><span class="sxs-lookup"><span data-stu-id="af752-267">Request</span></span>
<span data-ttu-id="af752-268">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af752-268">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="af752-269">Отклик</span><span class="sxs-lookup"><span data-stu-id="af752-269">Response</span></span>
<span data-ttu-id="af752-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af752-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



