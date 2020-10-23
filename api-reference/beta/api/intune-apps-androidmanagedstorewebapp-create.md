---
title: Создание Андроидманажедсторевебапп
description: Создание нового объекта Андроидманажедсторевебапп.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 03980b4786eb953f94b40fa041093d21fbc33776
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700607"
---
# <a name="create-androidmanagedstorewebapp"></a><span data-ttu-id="7c3a2-103">Создание Андроидманажедсторевебапп</span><span class="sxs-lookup"><span data-stu-id="7c3a2-103">Create androidManagedStoreWebApp</span></span>

<span data-ttu-id="7c3a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c3a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c3a2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c3a2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c3a2-107">Создание нового объекта [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7c3a2-107">Create a new [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c3a2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7c3a2-108">Prerequisites</span></span>
<span data-ttu-id="7c3a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c3a2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c3a2-111">Permission type</span></span>|<span data-ttu-id="7c3a2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c3a2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c3a2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c3a2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7c3a2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c3a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-116">Not supported.</span></span>|
|<span data-ttu-id="7c3a2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c3a2-117">Application</span></span>|<span data-ttu-id="7c3a2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c3a2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c3a2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c3a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7c3a2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7c3a2-120">Request headers</span></span>
|<span data-ttu-id="7c3a2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7c3a2-121">Header</span></span>|<span data-ttu-id="7c3a2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7c3a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c3a2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7c3a2-123">Authorization</span></span>|<span data-ttu-id="7c3a2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c3a2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c3a2-125">Accept</span></span>|<span data-ttu-id="7c3a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c3a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c3a2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7c3a2-127">Request body</span></span>
<span data-ttu-id="7c3a2-128">В тексте запроса добавьте представление объекта Андроидманажедсторевебапп в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-128">In the request body, supply a JSON representation for the androidManagedStoreWebApp object.</span></span>

<span data-ttu-id="7c3a2-129">В следующей таблице приведены свойства, необходимые при создании Андроидманажедсторевебапп.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-129">The following table shows the properties that are required when you create the androidManagedStoreWebApp.</span></span>

|<span data-ttu-id="7c3a2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c3a2-130">Property</span></span>|<span data-ttu-id="7c3a2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7c3a2-131">Type</span></span>|<span data-ttu-id="7c3a2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7c3a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c3a2-133">id</span><span class="sxs-lookup"><span data-stu-id="7c3a2-133">id</span></span>|<span data-ttu-id="7c3a2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7c3a2-134">String</span></span>|<span data-ttu-id="7c3a2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-135">Key of the entity.</span></span> <span data-ttu-id="7c3a2-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7c3a2-137">displayName</span></span>|<span data-ttu-id="7c3a2-138">Строка</span><span class="sxs-lookup"><span data-stu-id="7c3a2-138">String</span></span>|<span data-ttu-id="7c3a2-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7c3a2-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-141">description</span><span class="sxs-lookup"><span data-stu-id="7c3a2-141">description</span></span>|<span data-ttu-id="7c3a2-142">Строка</span><span class="sxs-lookup"><span data-stu-id="7c3a2-142">String</span></span>|<span data-ttu-id="7c3a2-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-143">The description of the app.</span></span> <span data-ttu-id="7c3a2-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-145">publisher</span><span class="sxs-lookup"><span data-stu-id="7c3a2-145">publisher</span></span>|<span data-ttu-id="7c3a2-146">String</span><span class="sxs-lookup"><span data-stu-id="7c3a2-146">String</span></span>|<span data-ttu-id="7c3a2-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-147">The publisher of the app.</span></span> <span data-ttu-id="7c3a2-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7c3a2-149">largeIcon</span></span>|[<span data-ttu-id="7c3a2-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7c3a2-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7c3a2-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7c3a2-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c3a2-153">createdDateTime</span></span>|<span data-ttu-id="7c3a2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c3a2-154">DateTimeOffset</span></span>|<span data-ttu-id="7c3a2-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-155">The date and time the app was created.</span></span> <span data-ttu-id="7c3a2-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c3a2-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7c3a2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c3a2-158">DateTimeOffset</span></span>|<span data-ttu-id="7c3a2-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-159">The date and time the app was last modified.</span></span> <span data-ttu-id="7c3a2-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7c3a2-161">isFeatured</span></span>|<span data-ttu-id="7c3a2-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c3a2-162">Boolean</span></span>|<span data-ttu-id="7c3a2-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7c3a2-164">privacyInformationUrl</span></span>|<span data-ttu-id="7c3a2-165">String</span><span class="sxs-lookup"><span data-stu-id="7c3a2-165">String</span></span>|<span data-ttu-id="7c3a2-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-166">The privacy statement Url.</span></span> <span data-ttu-id="7c3a2-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7c3a2-168">informationUrl</span></span>|<span data-ttu-id="7c3a2-169">String</span><span class="sxs-lookup"><span data-stu-id="7c3a2-169">String</span></span>|<span data-ttu-id="7c3a2-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-170">The more information Url.</span></span> <span data-ttu-id="7c3a2-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-172">owner</span><span class="sxs-lookup"><span data-stu-id="7c3a2-172">owner</span></span>|<span data-ttu-id="7c3a2-173">String</span><span class="sxs-lookup"><span data-stu-id="7c3a2-173">String</span></span>|<span data-ttu-id="7c3a2-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-174">The owner of the app.</span></span> <span data-ttu-id="7c3a2-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-176">developer</span><span class="sxs-lookup"><span data-stu-id="7c3a2-176">developer</span></span>|<span data-ttu-id="7c3a2-177">String</span><span class="sxs-lookup"><span data-stu-id="7c3a2-177">String</span></span>|<span data-ttu-id="7c3a2-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-178">The developer of the app.</span></span> <span data-ttu-id="7c3a2-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-180">notes</span><span class="sxs-lookup"><span data-stu-id="7c3a2-180">notes</span></span>|<span data-ttu-id="7c3a2-181">String</span><span class="sxs-lookup"><span data-stu-id="7c3a2-181">String</span></span>|<span data-ttu-id="7c3a2-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-182">Notes for the app.</span></span> <span data-ttu-id="7c3a2-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="7c3a2-184">uploadState</span></span>|<span data-ttu-id="7c3a2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7c3a2-185">Int32</span></span>|<span data-ttu-id="7c3a2-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-186">The upload state.</span></span> <span data-ttu-id="7c3a2-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="7c3a2-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="7c3a2-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="7c3a2-189">publishingState</span></span>|[<span data-ttu-id="7c3a2-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="7c3a2-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7c3a2-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-191">The publishing state for the app.</span></span> <span data-ttu-id="7c3a2-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7c3a2-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="7c3a2-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7c3a2-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7c3a2-195">isAssigned</span></span>|<span data-ttu-id="7c3a2-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c3a2-196">Boolean</span></span>|<span data-ttu-id="7c3a2-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7c3a2-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7c3a2-199">roleScopeTagIds</span></span>|<span data-ttu-id="7c3a2-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7c3a2-200">String collection</span></span>|<span data-ttu-id="7c3a2-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7c3a2-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="7c3a2-203">dependentAppCount</span></span>|<span data-ttu-id="7c3a2-204">Int32</span><span class="sxs-lookup"><span data-stu-id="7c3a2-204">Int32</span></span>|<span data-ttu-id="7c3a2-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7c3a2-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="7c3a2-207">supersedingAppCount</span></span>|<span data-ttu-id="7c3a2-208">Int32</span><span class="sxs-lookup"><span data-stu-id="7c3a2-208">Int32</span></span>|<span data-ttu-id="7c3a2-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="7c3a2-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="7c3a2-211">supersededAppCount</span></span>|<span data-ttu-id="7c3a2-212">Int32</span><span class="sxs-lookup"><span data-stu-id="7c3a2-212">Int32</span></span>|<span data-ttu-id="7c3a2-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="7c3a2-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7c3a2-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="7c3a2-215">packageId</span><span class="sxs-lookup"><span data-stu-id="7c3a2-215">packageId</span></span>|<span data-ttu-id="7c3a2-216">String</span><span class="sxs-lookup"><span data-stu-id="7c3a2-216">String</span></span>|<span data-ttu-id="7c3a2-217">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-217">The package identifier.</span></span> <span data-ttu-id="7c3a2-218">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-218">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7c3a2-219">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="7c3a2-219">appIdentifier</span></span>|<span data-ttu-id="7c3a2-220">String</span><span class="sxs-lookup"><span data-stu-id="7c3a2-220">String</span></span>|<span data-ttu-id="7c3a2-221">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-221">The Identity Name.</span></span> <span data-ttu-id="7c3a2-222">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-222">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7c3a2-223">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7c3a2-223">usedLicenseCount</span></span>|<span data-ttu-id="7c3a2-224">Int32</span><span class="sxs-lookup"><span data-stu-id="7c3a2-224">Int32</span></span>|<span data-ttu-id="7c3a2-225">Количество используемых лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-225">The number of VPP licenses in use.</span></span> <span data-ttu-id="7c3a2-226">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-226">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7c3a2-227">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7c3a2-227">totalLicenseCount</span></span>|<span data-ttu-id="7c3a2-228">Int32</span><span class="sxs-lookup"><span data-stu-id="7c3a2-228">Int32</span></span>|<span data-ttu-id="7c3a2-229">Общее количество лицензий VPP.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-229">The total number of VPP licenses.</span></span> <span data-ttu-id="7c3a2-230">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-230">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7c3a2-231">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7c3a2-231">appStoreUrl</span></span>|<span data-ttu-id="7c3a2-232">String</span><span class="sxs-lookup"><span data-stu-id="7c3a2-232">String</span></span>|<span data-ttu-id="7c3a2-233">URL-адрес приложения для рабочего хранилища.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-233">The Play for Work Store app URL.</span></span> <span data-ttu-id="7c3a2-234">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-234">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7c3a2-235">Частный</span><span class="sxs-lookup"><span data-stu-id="7c3a2-235">isPrivate</span></span>|<span data-ttu-id="7c3a2-236">Логический</span><span class="sxs-lookup"><span data-stu-id="7c3a2-236">Boolean</span></span>|<span data-ttu-id="7c3a2-237">Указывает, доступно ли приложение только для указанных пользователей предприятия.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-237">Indicates whether the app is only available to a given enterprise's users.</span></span> <span data-ttu-id="7c3a2-238">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-238">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7c3a2-239">иссистемапп</span><span class="sxs-lookup"><span data-stu-id="7c3a2-239">isSystemApp</span></span>|<span data-ttu-id="7c3a2-240">Логический</span><span class="sxs-lookup"><span data-stu-id="7c3a2-240">Boolean</span></span>|<span data-ttu-id="7c3a2-241">Указывает, является ли приложение предустановленным системным приложением.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-241">Indicates whether the app is a preinstalled system app.</span></span> <span data-ttu-id="7c3a2-242">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-242">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7c3a2-243">апптраккс</span><span class="sxs-lookup"><span data-stu-id="7c3a2-243">appTracks</span></span>|<span data-ttu-id="7c3a2-244">Коллекция [андроидманажедстореапптракк](../resources/intune-apps-androidmanagedstoreapptrack.md)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-244">[androidManagedStoreAppTrack](../resources/intune-apps-androidmanagedstoreapptrack.md) collection</span></span>|<span data-ttu-id="7c3a2-245">Дорожки, которые видимы для этого предприятия.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-245">The tracks that are visible to this enterprise.</span></span> <span data-ttu-id="7c3a2-246">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-246">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|
|<span data-ttu-id="7c3a2-247">суппортсоемконфиг</span><span class="sxs-lookup"><span data-stu-id="7c3a2-247">supportsOemConfig</span></span>|<span data-ttu-id="7c3a2-248">Логический</span><span class="sxs-lookup"><span data-stu-id="7c3a2-248">Boolean</span></span>|<span data-ttu-id="7c3a2-249">Поддерживает ли это приложение политику Оемконфиг.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-249">Whether this app supports OEMConfig policy.</span></span> <span data-ttu-id="7c3a2-250">Наследуется от [андроидманажедстореапп](../resources/intune-apps-androidmanagedstoreapp.md)</span><span class="sxs-lookup"><span data-stu-id="7c3a2-250">Inherited from [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7c3a2-251">Ответ</span><span class="sxs-lookup"><span data-stu-id="7c3a2-251">Response</span></span>
<span data-ttu-id="7c3a2-252">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [андроидманажедсторевебапп](../resources/intune-apps-androidmanagedstorewebapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-252">If successful, this method returns a `201 Created` response code and a [androidManagedStoreWebApp](../resources/intune-apps-androidmanagedstorewebapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c3a2-253">Пример</span><span class="sxs-lookup"><span data-stu-id="7c3a2-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c3a2-254">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c3a2-254">Request</span></span>
<span data-ttu-id="7c3a2-255">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-255">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1228

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="7c3a2-256">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c3a2-256">Response</span></span>
<span data-ttu-id="7c3a2-p130">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7c3a2-p130">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1400

{
  "@odata.type": "#microsoft.graph.androidManagedStoreWebApp",
  "id": "e54aecbd-ecbd-e54a-bdec-4ae5bdec4ae5",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "isPrivate": true,
  "isSystemApp": true,
  "appTracks": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppTrack",
      "trackId": "Track Id value",
      "trackAlias": "Track Alias value"
    }
  ],
  "supportsOemConfig": true
}
```





