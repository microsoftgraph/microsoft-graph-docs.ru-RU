---
title: Update windowsUniversalAppX
description: Обновление свойств объекта windowsUniversalAppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a49b42e050b2dbc9229b71a13dede3a82f8a529
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959651"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="95e5e-103">Update windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="95e5e-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="95e5e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95e5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95e5e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95e5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95e5e-106">Обновление свойств объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95e5e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="95e5e-107">Prerequisites</span></span>
<span data-ttu-id="95e5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95e5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95e5e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95e5e-110">Permission type</span></span>|<span data-ttu-id="95e5e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="95e5e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95e5e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95e5e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95e5e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95e5e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="95e5e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95e5e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95e5e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95e5e-115">Not supported.</span></span>|
|<span data-ttu-id="95e5e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95e5e-116">Application</span></span>|<span data-ttu-id="95e5e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95e5e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95e5e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95e5e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="95e5e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95e5e-119">Request headers</span></span>
|<span data-ttu-id="95e5e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="95e5e-120">Header</span></span>|<span data-ttu-id="95e5e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="95e5e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95e5e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95e5e-122">Authorization</span></span>|<span data-ttu-id="95e5e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95e5e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95e5e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="95e5e-124">Accept</span></span>|<span data-ttu-id="95e5e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95e5e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95e5e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="95e5e-126">Request body</span></span>
<span data-ttu-id="95e5e-127">В теле запроса добавьте представление объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95e5e-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="95e5e-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="95e5e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="95e5e-129">Property</span></span>|<span data-ttu-id="95e5e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="95e5e-130">Type</span></span>|<span data-ttu-id="95e5e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="95e5e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95e5e-132">id</span><span class="sxs-lookup"><span data-stu-id="95e5e-132">id</span></span>|<span data-ttu-id="95e5e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="95e5e-133">String</span></span>|<span data-ttu-id="95e5e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="95e5e-134">Key of the entity.</span></span> <span data-ttu-id="95e5e-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="95e5e-136">displayName</span></span>|<span data-ttu-id="95e5e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="95e5e-137">String</span></span>|<span data-ttu-id="95e5e-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="95e5e-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="95e5e-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-140">description</span><span class="sxs-lookup"><span data-stu-id="95e5e-140">description</span></span>|<span data-ttu-id="95e5e-141">Строка</span><span class="sxs-lookup"><span data-stu-id="95e5e-141">String</span></span>|<span data-ttu-id="95e5e-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-142">The description of the app.</span></span> <span data-ttu-id="95e5e-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-144">publisher</span><span class="sxs-lookup"><span data-stu-id="95e5e-144">publisher</span></span>|<span data-ttu-id="95e5e-145">String</span><span class="sxs-lookup"><span data-stu-id="95e5e-145">String</span></span>|<span data-ttu-id="95e5e-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-146">The publisher of the app.</span></span> <span data-ttu-id="95e5e-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="95e5e-148">largeIcon</span></span>|[<span data-ttu-id="95e5e-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="95e5e-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="95e5e-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="95e5e-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="95e5e-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95e5e-152">createdDateTime</span></span>|<span data-ttu-id="95e5e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95e5e-153">DateTimeOffset</span></span>|<span data-ttu-id="95e5e-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-154">The date and time the app was created.</span></span> <span data-ttu-id="95e5e-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95e5e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="95e5e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95e5e-157">DateTimeOffset</span></span>|<span data-ttu-id="95e5e-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-158">The date and time the app was last modified.</span></span> <span data-ttu-id="95e5e-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="95e5e-160">isFeatured</span></span>|<span data-ttu-id="95e5e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="95e5e-161">Boolean</span></span>|<span data-ttu-id="95e5e-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="95e5e-163">privacyInformationUrl</span></span>|<span data-ttu-id="95e5e-164">String</span><span class="sxs-lookup"><span data-stu-id="95e5e-164">String</span></span>|<span data-ttu-id="95e5e-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="95e5e-165">The privacy statement Url.</span></span> <span data-ttu-id="95e5e-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="95e5e-167">informationUrl</span></span>|<span data-ttu-id="95e5e-168">String</span><span class="sxs-lookup"><span data-stu-id="95e5e-168">String</span></span>|<span data-ttu-id="95e5e-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="95e5e-169">The more information Url.</span></span> <span data-ttu-id="95e5e-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-171">owner</span><span class="sxs-lookup"><span data-stu-id="95e5e-171">owner</span></span>|<span data-ttu-id="95e5e-172">String</span><span class="sxs-lookup"><span data-stu-id="95e5e-172">String</span></span>|<span data-ttu-id="95e5e-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-173">The owner of the app.</span></span> <span data-ttu-id="95e5e-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-175">developer</span><span class="sxs-lookup"><span data-stu-id="95e5e-175">developer</span></span>|<span data-ttu-id="95e5e-176">String</span><span class="sxs-lookup"><span data-stu-id="95e5e-176">String</span></span>|<span data-ttu-id="95e5e-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-177">The developer of the app.</span></span> <span data-ttu-id="95e5e-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-179">notes</span><span class="sxs-lookup"><span data-stu-id="95e5e-179">notes</span></span>|<span data-ttu-id="95e5e-180">String</span><span class="sxs-lookup"><span data-stu-id="95e5e-180">String</span></span>|<span data-ttu-id="95e5e-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-181">Notes for the app.</span></span> <span data-ttu-id="95e5e-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="95e5e-183">uploadState</span></span>|<span data-ttu-id="95e5e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="95e5e-184">Int32</span></span>|<span data-ttu-id="95e5e-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="95e5e-185">The upload state.</span></span> <span data-ttu-id="95e5e-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="95e5e-187">publishingState</span></span>|[<span data-ttu-id="95e5e-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="95e5e-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="95e5e-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-189">The publishing state for the app.</span></span> <span data-ttu-id="95e5e-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="95e5e-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="95e5e-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="95e5e-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="95e5e-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="95e5e-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="95e5e-193">isAssigned</span></span>|<span data-ttu-id="95e5e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="95e5e-194">Boolean</span></span>|<span data-ttu-id="95e5e-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="95e5e-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="95e5e-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95e5e-197">roleScopeTagIds</span></span>|<span data-ttu-id="95e5e-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="95e5e-198">String collection</span></span>|<span data-ttu-id="95e5e-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="95e5e-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="95e5e-201">dependentAppCount</span></span>|<span data-ttu-id="95e5e-202">Int32</span><span class="sxs-lookup"><span data-stu-id="95e5e-202">Int32</span></span>|<span data-ttu-id="95e5e-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="95e5e-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="95e5e-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="95e5e-205">committedContentVersion</span></span>|<span data-ttu-id="95e5e-206">String</span><span class="sxs-lookup"><span data-stu-id="95e5e-206">String</span></span>|<span data-ttu-id="95e5e-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="95e5e-207">The internal committed content version.</span></span> <span data-ttu-id="95e5e-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="95e5e-209">fileName</span><span class="sxs-lookup"><span data-stu-id="95e5e-209">fileName</span></span>|<span data-ttu-id="95e5e-210">String</span><span class="sxs-lookup"><span data-stu-id="95e5e-210">String</span></span>|<span data-ttu-id="95e5e-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-211">The name of the main Lob application file.</span></span> <span data-ttu-id="95e5e-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="95e5e-213">size</span><span class="sxs-lookup"><span data-stu-id="95e5e-213">size</span></span>|<span data-ttu-id="95e5e-214">Int64</span><span class="sxs-lookup"><span data-stu-id="95e5e-214">Int64</span></span>|<span data-ttu-id="95e5e-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="95e5e-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="95e5e-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="95e5e-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="95e5e-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="95e5e-217">applicableArchitectures</span></span>|[<span data-ttu-id="95e5e-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="95e5e-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="95e5e-219">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="95e5e-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="95e5e-220">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="95e5e-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="95e5e-221">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="95e5e-221">applicableDeviceTypes</span></span>|[<span data-ttu-id="95e5e-222">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="95e5e-222">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="95e5e-223">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="95e5e-223">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="95e5e-224">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="95e5e-224">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="95e5e-225">identityName</span><span class="sxs-lookup"><span data-stu-id="95e5e-225">identityName</span></span>|<span data-ttu-id="95e5e-226">String</span><span class="sxs-lookup"><span data-stu-id="95e5e-226">String</span></span>|<span data-ttu-id="95e5e-227">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-227">The Identity Name.</span></span>|
|<span data-ttu-id="95e5e-228">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="95e5e-228">identityPublisherHash</span></span>|<span data-ttu-id="95e5e-229">String</span><span class="sxs-lookup"><span data-stu-id="95e5e-229">String</span></span>|<span data-ttu-id="95e5e-230">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="95e5e-230">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="95e5e-231">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="95e5e-231">identityResourceIdentifier</span></span>|<span data-ttu-id="95e5e-232">String</span><span class="sxs-lookup"><span data-stu-id="95e5e-232">String</span></span>|<span data-ttu-id="95e5e-233">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="95e5e-233">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="95e5e-234">isBundle</span><span class="sxs-lookup"><span data-stu-id="95e5e-234">isBundle</span></span>|<span data-ttu-id="95e5e-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="95e5e-235">Boolean</span></span>|<span data-ttu-id="95e5e-236">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="95e5e-236">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="95e5e-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="95e5e-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="95e5e-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="95e5e-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="95e5e-239">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="95e5e-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="95e5e-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="95e5e-240">identityVersion</span></span>|<span data-ttu-id="95e5e-241">String</span><span class="sxs-lookup"><span data-stu-id="95e5e-241">String</span></span>|<span data-ttu-id="95e5e-242">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="95e5e-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="95e5e-243">Ответ</span><span class="sxs-lookup"><span data-stu-id="95e5e-243">Response</span></span>
<span data-ttu-id="95e5e-244">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="95e5e-244">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95e5e-245">Пример</span><span class="sxs-lookup"><span data-stu-id="95e5e-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="95e5e-246">Запрос</span><span class="sxs-lookup"><span data-stu-id="95e5e-246">Request</span></span>
<span data-ttu-id="95e5e-247">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95e5e-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="95e5e-248">Отклик</span><span class="sxs-lookup"><span data-stu-id="95e5e-248">Response</span></span>
<span data-ttu-id="95e5e-p124">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="95e5e-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```





