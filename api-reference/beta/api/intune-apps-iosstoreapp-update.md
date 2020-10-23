---
title: Update iosStoreApp
description: Обновление свойств объекта iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d2dca0d19827b84cf99cef86fd9f3bf2c73027e7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700208"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="a88c9-103">Update iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="a88c9-103">Update iosStoreApp</span></span>

<span data-ttu-id="a88c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a88c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a88c9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a88c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a88c9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a88c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a88c9-107">Обновление свойств объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-107">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a88c9-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a88c9-108">Prerequisites</span></span>
<span data-ttu-id="a88c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a88c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a88c9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a88c9-111">Permission type</span></span>|<span data-ttu-id="a88c9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a88c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a88c9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a88c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a88c9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a88c9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a88c9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a88c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a88c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a88c9-116">Not supported.</span></span>|
|<span data-ttu-id="a88c9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a88c9-117">Application</span></span>|<span data-ttu-id="a88c9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a88c9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a88c9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a88c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a88c9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a88c9-120">Request headers</span></span>
|<span data-ttu-id="a88c9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a88c9-121">Header</span></span>|<span data-ttu-id="a88c9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a88c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a88c9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a88c9-123">Authorization</span></span>|<span data-ttu-id="a88c9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a88c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a88c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a88c9-125">Accept</span></span>|<span data-ttu-id="a88c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a88c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a88c9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a88c9-127">Request body</span></span>
<span data-ttu-id="a88c9-128">В тексте запроса добавьте представление объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a88c9-128">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="a88c9-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-129">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="a88c9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a88c9-130">Property</span></span>|<span data-ttu-id="a88c9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a88c9-131">Type</span></span>|<span data-ttu-id="a88c9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a88c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a88c9-133">id</span><span class="sxs-lookup"><span data-stu-id="a88c9-133">id</span></span>|<span data-ttu-id="a88c9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a88c9-134">String</span></span>|<span data-ttu-id="a88c9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a88c9-135">Key of the entity.</span></span> <span data-ttu-id="a88c9-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a88c9-137">displayName</span></span>|<span data-ttu-id="a88c9-138">Строка</span><span class="sxs-lookup"><span data-stu-id="a88c9-138">String</span></span>|<span data-ttu-id="a88c9-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="a88c9-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a88c9-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-141">description</span><span class="sxs-lookup"><span data-stu-id="a88c9-141">description</span></span>|<span data-ttu-id="a88c9-142">Строка</span><span class="sxs-lookup"><span data-stu-id="a88c9-142">String</span></span>|<span data-ttu-id="a88c9-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="a88c9-143">The description of the app.</span></span> <span data-ttu-id="a88c9-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a88c9-145">publisher</span></span>|<span data-ttu-id="a88c9-146">String</span><span class="sxs-lookup"><span data-stu-id="a88c9-146">String</span></span>|<span data-ttu-id="a88c9-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="a88c9-147">The publisher of the app.</span></span> <span data-ttu-id="a88c9-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a88c9-149">largeIcon</span></span>|[<span data-ttu-id="a88c9-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a88c9-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a88c9-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="a88c9-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a88c9-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a88c9-153">createdDateTime</span></span>|<span data-ttu-id="a88c9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a88c9-154">DateTimeOffset</span></span>|<span data-ttu-id="a88c9-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="a88c9-155">The date and time the app was created.</span></span> <span data-ttu-id="a88c9-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a88c9-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a88c9-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a88c9-158">DateTimeOffset</span></span>|<span data-ttu-id="a88c9-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="a88c9-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a88c9-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a88c9-161">isFeatured</span></span>|<span data-ttu-id="a88c9-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a88c9-162">Boolean</span></span>|<span data-ttu-id="a88c9-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a88c9-164">privacyInformationUrl</span></span>|<span data-ttu-id="a88c9-165">String</span><span class="sxs-lookup"><span data-stu-id="a88c9-165">String</span></span>|<span data-ttu-id="a88c9-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="a88c9-166">The privacy statement Url.</span></span> <span data-ttu-id="a88c9-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a88c9-168">informationUrl</span></span>|<span data-ttu-id="a88c9-169">String</span><span class="sxs-lookup"><span data-stu-id="a88c9-169">String</span></span>|<span data-ttu-id="a88c9-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="a88c9-170">The more information Url.</span></span> <span data-ttu-id="a88c9-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-172">owner</span><span class="sxs-lookup"><span data-stu-id="a88c9-172">owner</span></span>|<span data-ttu-id="a88c9-173">String</span><span class="sxs-lookup"><span data-stu-id="a88c9-173">String</span></span>|<span data-ttu-id="a88c9-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="a88c9-174">The owner of the app.</span></span> <span data-ttu-id="a88c9-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-176">developer</span><span class="sxs-lookup"><span data-stu-id="a88c9-176">developer</span></span>|<span data-ttu-id="a88c9-177">String</span><span class="sxs-lookup"><span data-stu-id="a88c9-177">String</span></span>|<span data-ttu-id="a88c9-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="a88c9-178">The developer of the app.</span></span> <span data-ttu-id="a88c9-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-180">notes</span><span class="sxs-lookup"><span data-stu-id="a88c9-180">notes</span></span>|<span data-ttu-id="a88c9-181">String</span><span class="sxs-lookup"><span data-stu-id="a88c9-181">String</span></span>|<span data-ttu-id="a88c9-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="a88c9-182">Notes for the app.</span></span> <span data-ttu-id="a88c9-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a88c9-184">uploadState</span></span>|<span data-ttu-id="a88c9-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a88c9-185">Int32</span></span>|<span data-ttu-id="a88c9-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="a88c9-186">The upload state.</span></span> <span data-ttu-id="a88c9-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="a88c9-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="a88c9-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="a88c9-189">publishingState</span></span>|[<span data-ttu-id="a88c9-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="a88c9-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a88c9-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="a88c9-191">The publishing state for the app.</span></span> <span data-ttu-id="a88c9-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="a88c9-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a88c9-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="a88c9-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a88c9-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a88c9-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a88c9-195">isAssigned</span></span>|<span data-ttu-id="a88c9-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a88c9-196">Boolean</span></span>|<span data-ttu-id="a88c9-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="a88c9-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a88c9-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a88c9-199">roleScopeTagIds</span></span>|<span data-ttu-id="a88c9-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a88c9-200">String collection</span></span>|<span data-ttu-id="a88c9-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="a88c9-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a88c9-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a88c9-203">dependentAppCount</span></span>|<span data-ttu-id="a88c9-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a88c9-204">Int32</span></span>|<span data-ttu-id="a88c9-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="a88c9-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a88c9-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a88c9-207">supersedingAppCount</span></span>|<span data-ttu-id="a88c9-208">Int32</span><span class="sxs-lookup"><span data-stu-id="a88c9-208">Int32</span></span>|<span data-ttu-id="a88c9-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="a88c9-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="a88c9-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="a88c9-211">supersededAppCount</span></span>|<span data-ttu-id="a88c9-212">Int32</span><span class="sxs-lookup"><span data-stu-id="a88c9-212">Int32</span></span>|<span data-ttu-id="a88c9-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="a88c9-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="a88c9-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a88c9-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="a88c9-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="a88c9-215">bundleId</span></span>|<span data-ttu-id="a88c9-216">String</span><span class="sxs-lookup"><span data-stu-id="a88c9-216">String</span></span>|<span data-ttu-id="a88c9-217">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="a88c9-217">The Identity Name.</span></span>|
|<span data-ttu-id="a88c9-218">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a88c9-218">appStoreUrl</span></span>|<span data-ttu-id="a88c9-219">String</span><span class="sxs-lookup"><span data-stu-id="a88c9-219">String</span></span>|<span data-ttu-id="a88c9-220">URL-адрес в Apple App Store</span><span class="sxs-lookup"><span data-stu-id="a88c9-220">The Apple App Store URL</span></span>|
|<span data-ttu-id="a88c9-221">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="a88c9-221">applicableDeviceType</span></span>|[<span data-ttu-id="a88c9-222">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="a88c9-222">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="a88c9-223">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="a88c9-223">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="a88c9-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a88c9-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a88c9-225">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a88c9-225">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="a88c9-226">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="a88c9-226">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="a88c9-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="a88c9-227">Response</span></span>
<span data-ttu-id="a88c9-228">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a88c9-228">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a88c9-229">Пример</span><span class="sxs-lookup"><span data-stu-id="a88c9-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="a88c9-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="a88c9-230">Request</span></span>
<span data-ttu-id="a88c9-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a88c9-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1217

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```

### <a name="response"></a><span data-ttu-id="a88c9-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="a88c9-232">Response</span></span>
<span data-ttu-id="a88c9-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a88c9-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1389

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
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
  }
}
```





