---
title: Create iosLobApp
description: Создание нового объекта iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bac65fd7fe3272b6cf52531781271ad22a2068a1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157416"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="ef84f-103">Create iosLobApp</span><span class="sxs-lookup"><span data-stu-id="ef84f-103">Create iosLobApp</span></span>

<span data-ttu-id="ef84f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef84f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef84f-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef84f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef84f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ef84f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef84f-107">Создание нового объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-107">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef84f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ef84f-108">Prerequisites</span></span>
<span data-ttu-id="ef84f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef84f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef84f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef84f-111">Permission type</span></span>|<span data-ttu-id="ef84f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef84f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef84f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef84f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef84f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef84f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef84f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef84f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef84f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef84f-116">Not supported.</span></span>|
|<span data-ttu-id="ef84f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef84f-117">Application</span></span>|<span data-ttu-id="ef84f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef84f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef84f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef84f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ef84f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ef84f-120">Request headers</span></span>
|<span data-ttu-id="ef84f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ef84f-121">Header</span></span>|<span data-ttu-id="ef84f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ef84f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef84f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef84f-123">Authorization</span></span>|<span data-ttu-id="ef84f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef84f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef84f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef84f-125">Accept</span></span>|<span data-ttu-id="ef84f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef84f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef84f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef84f-127">Request body</span></span>
<span data-ttu-id="ef84f-128">В теле запроса добавьте представление объекта iosLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef84f-128">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="ef84f-129">Ниже показаны свойства, которые необходимо указывать при создании объекта iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="ef84f-129">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="ef84f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef84f-130">Property</span></span>|<span data-ttu-id="ef84f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ef84f-131">Type</span></span>|<span data-ttu-id="ef84f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ef84f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef84f-133">id</span><span class="sxs-lookup"><span data-stu-id="ef84f-133">id</span></span>|<span data-ttu-id="ef84f-134">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-134">String</span></span>|<span data-ttu-id="ef84f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ef84f-135">Key of the entity.</span></span> <span data-ttu-id="ef84f-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ef84f-137">displayName</span></span>|<span data-ttu-id="ef84f-138">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-138">String</span></span>|<span data-ttu-id="ef84f-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ef84f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ef84f-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-141">description</span><span class="sxs-lookup"><span data-stu-id="ef84f-141">description</span></span>|<span data-ttu-id="ef84f-142">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-142">String</span></span>|<span data-ttu-id="ef84f-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-143">The description of the app.</span></span> <span data-ttu-id="ef84f-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ef84f-145">publisher</span></span>|<span data-ttu-id="ef84f-146">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-146">String</span></span>|<span data-ttu-id="ef84f-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-147">The publisher of the app.</span></span> <span data-ttu-id="ef84f-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ef84f-149">largeIcon</span></span>|[<span data-ttu-id="ef84f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ef84f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ef84f-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ef84f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ef84f-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef84f-153">createdDateTime</span></span>|<span data-ttu-id="ef84f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef84f-154">DateTimeOffset</span></span>|<span data-ttu-id="ef84f-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-155">The date and time the app was created.</span></span> <span data-ttu-id="ef84f-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef84f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ef84f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef84f-158">DateTimeOffset</span></span>|<span data-ttu-id="ef84f-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ef84f-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ef84f-161">isFeatured</span></span>|<span data-ttu-id="ef84f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef84f-162">Boolean</span></span>|<span data-ttu-id="ef84f-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ef84f-164">privacyInformationUrl</span></span>|<span data-ttu-id="ef84f-165">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-165">String</span></span>|<span data-ttu-id="ef84f-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ef84f-166">The privacy statement Url.</span></span> <span data-ttu-id="ef84f-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ef84f-168">informationUrl</span></span>|<span data-ttu-id="ef84f-169">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-169">String</span></span>|<span data-ttu-id="ef84f-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ef84f-170">The more information Url.</span></span> <span data-ttu-id="ef84f-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-172">owner</span><span class="sxs-lookup"><span data-stu-id="ef84f-172">owner</span></span>|<span data-ttu-id="ef84f-173">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-173">String</span></span>|<span data-ttu-id="ef84f-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-174">The owner of the app.</span></span> <span data-ttu-id="ef84f-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-176">developer</span><span class="sxs-lookup"><span data-stu-id="ef84f-176">developer</span></span>|<span data-ttu-id="ef84f-177">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-177">String</span></span>|<span data-ttu-id="ef84f-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-178">The developer of the app.</span></span> <span data-ttu-id="ef84f-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-180">notes</span><span class="sxs-lookup"><span data-stu-id="ef84f-180">notes</span></span>|<span data-ttu-id="ef84f-181">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-181">String</span></span>|<span data-ttu-id="ef84f-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-182">Notes for the app.</span></span> <span data-ttu-id="ef84f-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ef84f-184">uploadState</span></span>|<span data-ttu-id="ef84f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ef84f-185">Int32</span></span>|<span data-ttu-id="ef84f-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="ef84f-186">The upload state.</span></span> <span data-ttu-id="ef84f-187">Возможные значения: 0- `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="ef84f-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ef84f-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ef84f-189">publishingState</span></span>|[<span data-ttu-id="ef84f-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ef84f-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ef84f-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-191">The publishing state for the app.</span></span> <span data-ttu-id="ef84f-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ef84f-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ef84f-193">Наследуется от [mobileApp.](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ef84f-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ef84f-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ef84f-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ef84f-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ef84f-195">isAssigned</span></span>|<span data-ttu-id="ef84f-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef84f-196">Boolean</span></span>|<span data-ttu-id="ef84f-197">Значение, указывающее, назначено ли приложению хотя бы одна группа.</span><span class="sxs-lookup"><span data-stu-id="ef84f-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ef84f-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef84f-199">roleScopeTagIds</span></span>|<span data-ttu-id="ef84f-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ef84f-200">String collection</span></span>|<span data-ttu-id="ef84f-201">Список ид тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ef84f-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ef84f-203">dependentAppCount</span></span>|<span data-ttu-id="ef84f-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ef84f-204">Int32</span></span>|<span data-ttu-id="ef84f-205">Общее количество зависимостей, которые есть у этого приложения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ef84f-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="ef84f-207">supersedingAppCount</span></span>|<span data-ttu-id="ef84f-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ef84f-208">Int32</span></span>|<span data-ttu-id="ef84f-209">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="ef84f-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="ef84f-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="ef84f-211">supersededAppCount</span></span>|<span data-ttu-id="ef84f-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ef84f-212">Int32</span></span>|<span data-ttu-id="ef84f-213">Общее количество приложений, которые это приложение напрямую или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="ef84f-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="ef84f-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ef84f-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ef84f-215">committedContentVersion</span></span>|<span data-ttu-id="ef84f-216">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-216">String</span></span>|<span data-ttu-id="ef84f-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="ef84f-217">The internal committed content version.</span></span> <span data-ttu-id="ef84f-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ef84f-219">fileName</span><span class="sxs-lookup"><span data-stu-id="ef84f-219">fileName</span></span>|<span data-ttu-id="ef84f-220">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-220">String</span></span>|<span data-ttu-id="ef84f-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-221">The name of the main Lob application file.</span></span> <span data-ttu-id="ef84f-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ef84f-223">size</span><span class="sxs-lookup"><span data-stu-id="ef84f-223">size</span></span>|<span data-ttu-id="ef84f-224">Int64</span><span class="sxs-lookup"><span data-stu-id="ef84f-224">Int64</span></span>|<span data-ttu-id="ef84f-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="ef84f-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="ef84f-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ef84f-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ef84f-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="ef84f-227">bundleId</span></span>|<span data-ttu-id="ef84f-228">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-228">String</span></span>|<span data-ttu-id="ef84f-229">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-229">The Identity Name.</span></span>|
|<span data-ttu-id="ef84f-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ef84f-230">applicableDeviceType</span></span>|[<span data-ttu-id="ef84f-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ef84f-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="ef84f-232">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ef84f-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="ef84f-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ef84f-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ef84f-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ef84f-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="ef84f-235">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ef84f-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ef84f-236">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ef84f-236">expirationDateTime</span></span>|<span data-ttu-id="ef84f-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef84f-237">DateTimeOffset</span></span>|<span data-ttu-id="ef84f-238">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="ef84f-238">The expiration time.</span></span>|
|<span data-ttu-id="ef84f-239">versionNumber</span><span class="sxs-lookup"><span data-stu-id="ef84f-239">versionNumber</span></span>|<span data-ttu-id="ef84f-240">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-240">String</span></span>|<span data-ttu-id="ef84f-241">Номер версии бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="ef84f-241">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ef84f-242">buildNumber</span><span class="sxs-lookup"><span data-stu-id="ef84f-242">buildNumber</span></span>|<span data-ttu-id="ef84f-243">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-243">String</span></span>|<span data-ttu-id="ef84f-244">Номер сборки бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="ef84f-244">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ef84f-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ef84f-245">identityVersion</span></span>|<span data-ttu-id="ef84f-246">String</span><span class="sxs-lookup"><span data-stu-id="ef84f-246">String</span></span>|<span data-ttu-id="ef84f-247">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ef84f-247">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ef84f-248">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef84f-248">Response</span></span>
<span data-ttu-id="ef84f-249">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosLobApp](../resources/intune-apps-ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ef84f-249">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef84f-250">Пример</span><span class="sxs-lookup"><span data-stu-id="ef84f-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef84f-251">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef84f-251">Request</span></span>
<span data-ttu-id="ef84f-252">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef84f-252">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1488

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="ef84f-253">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef84f-253">Response</span></span>
<span data-ttu-id="ef84f-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ef84f-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1660

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




