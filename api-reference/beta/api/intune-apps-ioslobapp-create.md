---
title: Create iosLobApp
description: Создание нового объекта iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 29866456703ab0c6a95b0b393b6a961baaf4b413
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140842"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="303b5-103">Create iosLobApp</span><span class="sxs-lookup"><span data-stu-id="303b5-103">Create iosLobApp</span></span>

<span data-ttu-id="303b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="303b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="303b5-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="303b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="303b5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="303b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="303b5-107">Создание нового объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-107">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="303b5-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="303b5-108">Prerequisites</span></span>
<span data-ttu-id="303b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="303b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="303b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="303b5-111">Permission type</span></span>|<span data-ttu-id="303b5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="303b5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="303b5-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="303b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="303b5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="303b5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="303b5-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="303b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="303b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="303b5-116">Not supported.</span></span>|
|<span data-ttu-id="303b5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="303b5-117">Application</span></span>|<span data-ttu-id="303b5-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="303b5-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="303b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="303b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="303b5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="303b5-120">Request headers</span></span>
|<span data-ttu-id="303b5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="303b5-121">Header</span></span>|<span data-ttu-id="303b5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="303b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="303b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="303b5-123">Authorization</span></span>|<span data-ttu-id="303b5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="303b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="303b5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="303b5-125">Accept</span></span>|<span data-ttu-id="303b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="303b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="303b5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="303b5-127">Request body</span></span>
<span data-ttu-id="303b5-128">В теле запроса добавьте представление объекта iosLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="303b5-128">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="303b5-129">Ниже показаны свойства, которые необходимо указывать при создании объекта iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="303b5-129">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="303b5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="303b5-130">Property</span></span>|<span data-ttu-id="303b5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="303b5-131">Type</span></span>|<span data-ttu-id="303b5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="303b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="303b5-133">id</span><span class="sxs-lookup"><span data-stu-id="303b5-133">id</span></span>|<span data-ttu-id="303b5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="303b5-134">String</span></span>|<span data-ttu-id="303b5-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="303b5-135">Key of the entity.</span></span> <span data-ttu-id="303b5-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="303b5-137">displayName</span></span>|<span data-ttu-id="303b5-138">Строка</span><span class="sxs-lookup"><span data-stu-id="303b5-138">String</span></span>|<span data-ttu-id="303b5-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="303b5-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="303b5-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-141">description</span><span class="sxs-lookup"><span data-stu-id="303b5-141">description</span></span>|<span data-ttu-id="303b5-142">Строка</span><span class="sxs-lookup"><span data-stu-id="303b5-142">String</span></span>|<span data-ttu-id="303b5-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="303b5-143">The description of the app.</span></span> <span data-ttu-id="303b5-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-145">publisher</span><span class="sxs-lookup"><span data-stu-id="303b5-145">publisher</span></span>|<span data-ttu-id="303b5-146">String</span><span class="sxs-lookup"><span data-stu-id="303b5-146">String</span></span>|<span data-ttu-id="303b5-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="303b5-147">The publisher of the app.</span></span> <span data-ttu-id="303b5-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="303b5-149">largeIcon</span></span>|[<span data-ttu-id="303b5-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="303b5-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="303b5-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="303b5-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="303b5-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="303b5-153">createdDateTime</span></span>|<span data-ttu-id="303b5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="303b5-154">DateTimeOffset</span></span>|<span data-ttu-id="303b5-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="303b5-155">The date and time the app was created.</span></span> <span data-ttu-id="303b5-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="303b5-157">lastModifiedDateTime</span></span>|<span data-ttu-id="303b5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="303b5-158">DateTimeOffset</span></span>|<span data-ttu-id="303b5-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="303b5-159">The date and time the app was last modified.</span></span> <span data-ttu-id="303b5-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="303b5-161">isFeatured</span></span>|<span data-ttu-id="303b5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="303b5-162">Boolean</span></span>|<span data-ttu-id="303b5-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="303b5-164">privacyInformationUrl</span></span>|<span data-ttu-id="303b5-165">String</span><span class="sxs-lookup"><span data-stu-id="303b5-165">String</span></span>|<span data-ttu-id="303b5-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="303b5-166">The privacy statement Url.</span></span> <span data-ttu-id="303b5-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="303b5-168">informationUrl</span></span>|<span data-ttu-id="303b5-169">String</span><span class="sxs-lookup"><span data-stu-id="303b5-169">String</span></span>|<span data-ttu-id="303b5-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="303b5-170">The more information Url.</span></span> <span data-ttu-id="303b5-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-172">owner</span><span class="sxs-lookup"><span data-stu-id="303b5-172">owner</span></span>|<span data-ttu-id="303b5-173">String</span><span class="sxs-lookup"><span data-stu-id="303b5-173">String</span></span>|<span data-ttu-id="303b5-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="303b5-174">The owner of the app.</span></span> <span data-ttu-id="303b5-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-176">developer</span><span class="sxs-lookup"><span data-stu-id="303b5-176">developer</span></span>|<span data-ttu-id="303b5-177">String</span><span class="sxs-lookup"><span data-stu-id="303b5-177">String</span></span>|<span data-ttu-id="303b5-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="303b5-178">The developer of the app.</span></span> <span data-ttu-id="303b5-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-180">notes</span><span class="sxs-lookup"><span data-stu-id="303b5-180">notes</span></span>|<span data-ttu-id="303b5-181">String</span><span class="sxs-lookup"><span data-stu-id="303b5-181">String</span></span>|<span data-ttu-id="303b5-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="303b5-182">Notes for the app.</span></span> <span data-ttu-id="303b5-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="303b5-184">uploadState</span></span>|<span data-ttu-id="303b5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="303b5-185">Int32</span></span>|<span data-ttu-id="303b5-186">Состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="303b5-186">The upload state.</span></span> <span data-ttu-id="303b5-187">Возможные значения: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="303b5-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="303b5-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="303b5-189">publishingState</span></span>|[<span data-ttu-id="303b5-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="303b5-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="303b5-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="303b5-191">The publishing state for the app.</span></span> <span data-ttu-id="303b5-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="303b5-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="303b5-193">Унаследованный от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="303b5-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="303b5-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="303b5-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="303b5-195">isAssigned</span></span>|<span data-ttu-id="303b5-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="303b5-196">Boolean</span></span>|<span data-ttu-id="303b5-197">Значение, указывающее, назначено ли приложению по крайней мере одна группа.</span><span class="sxs-lookup"><span data-stu-id="303b5-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="303b5-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="303b5-199">roleScopeTagIds</span></span>|<span data-ttu-id="303b5-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="303b5-200">String collection</span></span>|<span data-ttu-id="303b5-201">Список ids тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="303b5-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="303b5-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="303b5-203">dependentAppCount</span></span>|<span data-ttu-id="303b5-204">Int32</span><span class="sxs-lookup"><span data-stu-id="303b5-204">Int32</span></span>|<span data-ttu-id="303b5-205">Общее число зависимостей, которые имеет детское приложение.</span><span class="sxs-lookup"><span data-stu-id="303b5-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="303b5-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="303b5-207">supersedingAppCount</span></span>|<span data-ttu-id="303b5-208">Int32</span><span class="sxs-lookup"><span data-stu-id="303b5-208">Int32</span></span>|<span data-ttu-id="303b5-209">Общее число приложений, которые это приложение прямо или косвенно перемежает.</span><span class="sxs-lookup"><span data-stu-id="303b5-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="303b5-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="303b5-211">supersededAppCount</span></span>|<span data-ttu-id="303b5-212">Int32</span><span class="sxs-lookup"><span data-stu-id="303b5-212">Int32</span></span>|<span data-ttu-id="303b5-213">Общее число приложений, которые это приложение прямо или косвенно вымежает.</span><span class="sxs-lookup"><span data-stu-id="303b5-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="303b5-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="303b5-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="303b5-215">committedContentVersion</span></span>|<span data-ttu-id="303b5-216">String</span><span class="sxs-lookup"><span data-stu-id="303b5-216">String</span></span>|<span data-ttu-id="303b5-217">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="303b5-217">The internal committed content version.</span></span> <span data-ttu-id="303b5-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="303b5-219">fileName</span><span class="sxs-lookup"><span data-stu-id="303b5-219">fileName</span></span>|<span data-ttu-id="303b5-220">String</span><span class="sxs-lookup"><span data-stu-id="303b5-220">String</span></span>|<span data-ttu-id="303b5-221">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="303b5-221">The name of the main Lob application file.</span></span> <span data-ttu-id="303b5-222">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="303b5-223">size</span><span class="sxs-lookup"><span data-stu-id="303b5-223">size</span></span>|<span data-ttu-id="303b5-224">Int64</span><span class="sxs-lookup"><span data-stu-id="303b5-224">Int64</span></span>|<span data-ttu-id="303b5-225">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="303b5-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="303b5-226">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="303b5-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="303b5-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="303b5-227">bundleId</span></span>|<span data-ttu-id="303b5-228">String</span><span class="sxs-lookup"><span data-stu-id="303b5-228">String</span></span>|<span data-ttu-id="303b5-229">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="303b5-229">The Identity Name.</span></span>|
|<span data-ttu-id="303b5-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="303b5-230">applicableDeviceType</span></span>|[<span data-ttu-id="303b5-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="303b5-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="303b5-232">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="303b5-232">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="303b5-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="303b5-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="303b5-234">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="303b5-234">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="303b5-235">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="303b5-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="303b5-236">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="303b5-236">expirationDateTime</span></span>|<span data-ttu-id="303b5-237">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="303b5-237">DateTimeOffset</span></span>|<span data-ttu-id="303b5-238">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="303b5-238">The expiration time.</span></span>|
|<span data-ttu-id="303b5-239">versionNumber</span><span class="sxs-lookup"><span data-stu-id="303b5-239">versionNumber</span></span>|<span data-ttu-id="303b5-240">String</span><span class="sxs-lookup"><span data-stu-id="303b5-240">String</span></span>|<span data-ttu-id="303b5-241">Номер версии бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="303b5-241">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="303b5-242">buildNumber</span><span class="sxs-lookup"><span data-stu-id="303b5-242">buildNumber</span></span>|<span data-ttu-id="303b5-243">String</span><span class="sxs-lookup"><span data-stu-id="303b5-243">String</span></span>|<span data-ttu-id="303b5-244">Номер сборки бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="303b5-244">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="303b5-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="303b5-245">identityVersion</span></span>|<span data-ttu-id="303b5-246">String</span><span class="sxs-lookup"><span data-stu-id="303b5-246">String</span></span>|<span data-ttu-id="303b5-247">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="303b5-247">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="303b5-248">Ответ</span><span class="sxs-lookup"><span data-stu-id="303b5-248">Response</span></span>
<span data-ttu-id="303b5-249">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosLobApp](../resources/intune-apps-ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="303b5-249">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="303b5-250">Пример</span><span class="sxs-lookup"><span data-stu-id="303b5-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="303b5-251">Запрос</span><span class="sxs-lookup"><span data-stu-id="303b5-251">Request</span></span>
<span data-ttu-id="303b5-252">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="303b5-252">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="303b5-253">Отклик</span><span class="sxs-lookup"><span data-stu-id="303b5-253">Response</span></span>
<span data-ttu-id="303b5-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="303b5-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




