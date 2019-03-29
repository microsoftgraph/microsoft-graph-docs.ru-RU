---
title: Обновление win32LobApp
description: Обновление свойств объекта win32LobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2f528f854195af119a4a3c7404d017943bd1701
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970921"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="eaff5-103">Обновление win32LobApp</span><span class="sxs-lookup"><span data-stu-id="eaff5-103">Update win32LobApp</span></span>

> <span data-ttu-id="eaff5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaff5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaff5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eaff5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaff5-106">Обновление свойств объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="eaff5-106">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eaff5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eaff5-107">Prerequisites</span></span>
<span data-ttu-id="eaff5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaff5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaff5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eaff5-110">Permission type</span></span>|<span data-ttu-id="eaff5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eaff5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaff5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaff5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eaff5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaff5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eaff5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaff5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaff5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaff5-115">Not supported.</span></span>|
|<span data-ttu-id="eaff5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eaff5-116">Application</span></span>|<span data-ttu-id="eaff5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaff5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaff5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaff5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="eaff5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eaff5-119">Request headers</span></span>
|<span data-ttu-id="eaff5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eaff5-120">Header</span></span>|<span data-ttu-id="eaff5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eaff5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaff5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eaff5-122">Authorization</span></span>|<span data-ttu-id="eaff5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaff5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaff5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eaff5-124">Accept</span></span>|<span data-ttu-id="eaff5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eaff5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaff5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eaff5-126">Request body</span></span>
<span data-ttu-id="eaff5-127">В тексте запроса добавьте представление объекта [Win32LobApp](../resources/intune-apps-win32lobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eaff5-127">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="eaff5-128">В следующей таблице приведены свойства, необходимые при создании [win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-128">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="eaff5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="eaff5-129">Property</span></span>|<span data-ttu-id="eaff5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="eaff5-130">Type</span></span>|<span data-ttu-id="eaff5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="eaff5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaff5-132">id</span><span class="sxs-lookup"><span data-stu-id="eaff5-132">id</span></span>|<span data-ttu-id="eaff5-133">Строка</span><span class="sxs-lookup"><span data-stu-id="eaff5-133">String</span></span>|<span data-ttu-id="eaff5-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eaff5-134">Key of the entity.</span></span> <span data-ttu-id="eaff5-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="eaff5-136">displayName</span></span>|<span data-ttu-id="eaff5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="eaff5-137">String</span></span>|<span data-ttu-id="eaff5-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="eaff5-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="eaff5-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-140">description</span><span class="sxs-lookup"><span data-stu-id="eaff5-140">description</span></span>|<span data-ttu-id="eaff5-141">String</span><span class="sxs-lookup"><span data-stu-id="eaff5-141">String</span></span>|<span data-ttu-id="eaff5-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-142">The description of the app.</span></span> <span data-ttu-id="eaff5-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-144">publisher</span><span class="sxs-lookup"><span data-stu-id="eaff5-144">publisher</span></span>|<span data-ttu-id="eaff5-145">String</span><span class="sxs-lookup"><span data-stu-id="eaff5-145">String</span></span>|<span data-ttu-id="eaff5-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-146">The publisher of the app.</span></span> <span data-ttu-id="eaff5-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="eaff5-148">largeIcon</span></span>|[<span data-ttu-id="eaff5-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eaff5-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eaff5-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="eaff5-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="eaff5-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eaff5-152">createdDateTime</span></span>|<span data-ttu-id="eaff5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaff5-153">DateTimeOffset</span></span>|<span data-ttu-id="eaff5-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-154">The date and time the app was created.</span></span> <span data-ttu-id="eaff5-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eaff5-156">lastModifiedDateTime</span></span>|<span data-ttu-id="eaff5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaff5-157">DateTimeOffset</span></span>|<span data-ttu-id="eaff5-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-158">The date and time the app was last modified.</span></span> <span data-ttu-id="eaff5-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="eaff5-160">isFeatured</span></span>|<span data-ttu-id="eaff5-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaff5-161">Boolean</span></span>|<span data-ttu-id="eaff5-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eaff5-163">privacyInformationUrl</span></span>|<span data-ttu-id="eaff5-164">String</span><span class="sxs-lookup"><span data-stu-id="eaff5-164">String</span></span>|<span data-ttu-id="eaff5-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="eaff5-165">The privacy statement Url.</span></span> <span data-ttu-id="eaff5-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eaff5-167">informationUrl</span></span>|<span data-ttu-id="eaff5-168">String</span><span class="sxs-lookup"><span data-stu-id="eaff5-168">String</span></span>|<span data-ttu-id="eaff5-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="eaff5-169">The more information Url.</span></span> <span data-ttu-id="eaff5-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-171">owner</span><span class="sxs-lookup"><span data-stu-id="eaff5-171">owner</span></span>|<span data-ttu-id="eaff5-172">String</span><span class="sxs-lookup"><span data-stu-id="eaff5-172">String</span></span>|<span data-ttu-id="eaff5-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-173">The owner of the app.</span></span> <span data-ttu-id="eaff5-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-175">developer</span><span class="sxs-lookup"><span data-stu-id="eaff5-175">developer</span></span>|<span data-ttu-id="eaff5-176">String</span><span class="sxs-lookup"><span data-stu-id="eaff5-176">String</span></span>|<span data-ttu-id="eaff5-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-177">The developer of the app.</span></span> <span data-ttu-id="eaff5-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-179">notes</span><span class="sxs-lookup"><span data-stu-id="eaff5-179">notes</span></span>|<span data-ttu-id="eaff5-180">String</span><span class="sxs-lookup"><span data-stu-id="eaff5-180">String</span></span>|<span data-ttu-id="eaff5-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-181">Notes for the app.</span></span> <span data-ttu-id="eaff5-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="eaff5-183">uploadState</span></span>|<span data-ttu-id="eaff5-184">Int32</span><span class="sxs-lookup"><span data-stu-id="eaff5-184">Int32</span></span>|<span data-ttu-id="eaff5-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="eaff5-185">The upload state.</span></span> <span data-ttu-id="eaff5-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="eaff5-187">publishingState</span></span>|[<span data-ttu-id="eaff5-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="eaff5-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="eaff5-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-189">The publishing state for the app.</span></span> <span data-ttu-id="eaff5-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="eaff5-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="eaff5-191">НаСледуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="eaff5-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="eaff5-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="eaff5-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="eaff5-193">isAssigned</span></span>|<span data-ttu-id="eaff5-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaff5-194">Boolean</span></span>|<span data-ttu-id="eaff5-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="eaff5-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="eaff5-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eaff5-197">roleScopeTagIds</span></span>|<span data-ttu-id="eaff5-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="eaff5-198">String collection</span></span>|<span data-ttu-id="eaff5-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="eaff5-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaff5-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="eaff5-201">committedContentVersion</span></span>|<span data-ttu-id="eaff5-202">String</span><span class="sxs-lookup"><span data-stu-id="eaff5-202">String</span></span>|<span data-ttu-id="eaff5-203">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="eaff5-203">The internal committed content version.</span></span> <span data-ttu-id="eaff5-204">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="eaff5-205">fileName</span><span class="sxs-lookup"><span data-stu-id="eaff5-205">fileName</span></span>|<span data-ttu-id="eaff5-206">String</span><span class="sxs-lookup"><span data-stu-id="eaff5-206">String</span></span>|<span data-ttu-id="eaff5-207">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-207">The name of the main Lob application file.</span></span> <span data-ttu-id="eaff5-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="eaff5-209">size</span><span class="sxs-lookup"><span data-stu-id="eaff5-209">size</span></span>|<span data-ttu-id="eaff5-210">Int64</span><span class="sxs-lookup"><span data-stu-id="eaff5-210">Int64</span></span>|<span data-ttu-id="eaff5-211">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="eaff5-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="eaff5-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaff5-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="eaff5-213">Инсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="eaff5-213">installCommandLine</span></span>|<span data-ttu-id="eaff5-214">String</span><span class="sxs-lookup"><span data-stu-id="eaff5-214">String</span></span>|<span data-ttu-id="eaff5-215">Командная строка для установки приложения</span><span class="sxs-lookup"><span data-stu-id="eaff5-215">The command line to install this app</span></span>|
|<span data-ttu-id="eaff5-216">Унинсталлкоммандлине</span><span class="sxs-lookup"><span data-stu-id="eaff5-216">uninstallCommandLine</span></span>|<span data-ttu-id="eaff5-217">String</span><span class="sxs-lookup"><span data-stu-id="eaff5-217">String</span></span>|<span data-ttu-id="eaff5-218">Командная строка для удаления приложения</span><span class="sxs-lookup"><span data-stu-id="eaff5-218">The command line to uninstall this app</span></span>|
|<span data-ttu-id="eaff5-219">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="eaff5-219">applicableArchitectures</span></span>|[<span data-ttu-id="eaff5-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="eaff5-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="eaff5-221">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="eaff5-221">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="eaff5-222">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="eaff5-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="eaff5-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eaff5-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="eaff5-224">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eaff5-224">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="eaff5-225">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="eaff5-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="eaff5-226">Минимумфридискспацеинмб</span><span class="sxs-lookup"><span data-stu-id="eaff5-226">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="eaff5-227">Int32</span><span class="sxs-lookup"><span data-stu-id="eaff5-227">Int32</span></span>|<span data-ttu-id="eaff5-228">Минимальное свободное место на диске, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-228">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="eaff5-229">Минимуммеморинмб</span><span class="sxs-lookup"><span data-stu-id="eaff5-229">minimumMemoryInMB</span></span>|<span data-ttu-id="eaff5-230">Int32</span><span class="sxs-lookup"><span data-stu-id="eaff5-230">Int32</span></span>|<span data-ttu-id="eaff5-231">Значение минимальной физической памяти, необходимой для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-231">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="eaff5-232">Минимумнумберофпроцессорс</span><span class="sxs-lookup"><span data-stu-id="eaff5-232">minimumNumberOfProcessors</span></span>|<span data-ttu-id="eaff5-233">Int32</span><span class="sxs-lookup"><span data-stu-id="eaff5-233">Int32</span></span>|<span data-ttu-id="eaff5-234">Значение минимального числа процессоров, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-234">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="eaff5-235">Минимумкпуспидинмхз</span><span class="sxs-lookup"><span data-stu-id="eaff5-235">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="eaff5-236">Int32</span><span class="sxs-lookup"><span data-stu-id="eaff5-236">Int32</span></span>|<span data-ttu-id="eaff5-237">Значение минимальной скорости ЦП, необходимое для установки этого приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-237">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="eaff5-238">Детектионрулес</span><span class="sxs-lookup"><span data-stu-id="eaff5-238">detectionRules</span></span>|<span data-ttu-id="eaff5-239">Коллекция [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="eaff5-239">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="eaff5-240">Правила обнаружения для определения бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="eaff5-240">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="eaff5-241">Инсталлекспериенце</span><span class="sxs-lookup"><span data-stu-id="eaff5-241">installExperience</span></span>|[<span data-ttu-id="eaff5-242">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="eaff5-242">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="eaff5-243">Установка приложения.</span><span class="sxs-lookup"><span data-stu-id="eaff5-243">The install experience for this app.</span></span>|
|<span data-ttu-id="eaff5-244">Ретурнкодес</span><span class="sxs-lookup"><span data-stu-id="eaff5-244">returnCodes</span></span>|<span data-ttu-id="eaff5-245">Коллекция [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="eaff5-245">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="eaff5-246">Коды возврата для поведения после установки.</span><span class="sxs-lookup"><span data-stu-id="eaff5-246">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="eaff5-247">Мсиинформатион</span><span class="sxs-lookup"><span data-stu-id="eaff5-247">msiInformation</span></span>|[<span data-ttu-id="eaff5-248">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="eaff5-248">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="eaff5-249">Сведения о MSI, если это приложение Win32 является приложением MSI.</span><span class="sxs-lookup"><span data-stu-id="eaff5-249">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="eaff5-250">Сетупфилепас</span><span class="sxs-lookup"><span data-stu-id="eaff5-250">setupFilePath</span></span>|<span data-ttu-id="eaff5-251">String</span><span class="sxs-lookup"><span data-stu-id="eaff5-251">String</span></span>|<span data-ttu-id="eaff5-252">Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.</span><span class="sxs-lookup"><span data-stu-id="eaff5-252">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="eaff5-253">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaff5-253">Response</span></span>
<span data-ttu-id="eaff5-254">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eaff5-254">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaff5-255">Пример</span><span class="sxs-lookup"><span data-stu-id="eaff5-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="eaff5-256">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaff5-256">Request</span></span>
<span data-ttu-id="eaff5-257">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eaff5-257">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2364

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

### <a name="response"></a><span data-ttu-id="eaff5-258">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaff5-258">Response</span></span>
<span data-ttu-id="eaff5-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eaff5-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2536

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




