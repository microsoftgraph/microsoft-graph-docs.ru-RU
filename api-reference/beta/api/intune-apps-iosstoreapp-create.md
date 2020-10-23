---
title: Create iosStoreApp
description: Создание объекта iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b081c5214c05d599184b6ea08c5cb77b1460d48e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700271"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="64c33-103">Create iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="64c33-103">Create iosStoreApp</span></span>

<span data-ttu-id="64c33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64c33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64c33-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c33-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64c33-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64c33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64c33-107">Создание объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-107">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64c33-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="64c33-108">Prerequisites</span></span>
<span data-ttu-id="64c33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64c33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64c33-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64c33-111">Permission type</span></span>|<span data-ttu-id="64c33-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64c33-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64c33-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64c33-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64c33-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c33-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="64c33-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64c33-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64c33-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64c33-116">Not supported.</span></span>|
|<span data-ttu-id="64c33-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64c33-117">Application</span></span>|<span data-ttu-id="64c33-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64c33-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="64c33-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64c33-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="64c33-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="64c33-120">Request headers</span></span>
|<span data-ttu-id="64c33-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64c33-121">Header</span></span>|<span data-ttu-id="64c33-122">Значение</span><span class="sxs-lookup"><span data-stu-id="64c33-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64c33-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64c33-123">Authorization</span></span>|<span data-ttu-id="64c33-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64c33-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64c33-125">Accept</span><span class="sxs-lookup"><span data-stu-id="64c33-125">Accept</span></span>|<span data-ttu-id="64c33-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64c33-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64c33-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64c33-127">Request body</span></span>
<span data-ttu-id="64c33-128">В теле запроса добавьте представление объекта iosStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64c33-128">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="64c33-129">Ниже показаны свойства, которые необходимо указывать при создании объекта iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="64c33-129">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="64c33-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="64c33-130">Property</span></span>|<span data-ttu-id="64c33-131">Тип</span><span class="sxs-lookup"><span data-stu-id="64c33-131">Type</span></span>|<span data-ttu-id="64c33-132">Описание</span><span class="sxs-lookup"><span data-stu-id="64c33-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64c33-133">id</span><span class="sxs-lookup"><span data-stu-id="64c33-133">id</span></span>|<span data-ttu-id="64c33-134">Строка</span><span class="sxs-lookup"><span data-stu-id="64c33-134">String</span></span>|<span data-ttu-id="64c33-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="64c33-135">Key of the entity.</span></span> <span data-ttu-id="64c33-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-137">displayName</span><span class="sxs-lookup"><span data-stu-id="64c33-137">displayName</span></span>|<span data-ttu-id="64c33-138">Строка</span><span class="sxs-lookup"><span data-stu-id="64c33-138">String</span></span>|<span data-ttu-id="64c33-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="64c33-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="64c33-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-141">description</span><span class="sxs-lookup"><span data-stu-id="64c33-141">description</span></span>|<span data-ttu-id="64c33-142">Строка</span><span class="sxs-lookup"><span data-stu-id="64c33-142">String</span></span>|<span data-ttu-id="64c33-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="64c33-143">The description of the app.</span></span> <span data-ttu-id="64c33-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-145">publisher</span><span class="sxs-lookup"><span data-stu-id="64c33-145">publisher</span></span>|<span data-ttu-id="64c33-146">String</span><span class="sxs-lookup"><span data-stu-id="64c33-146">String</span></span>|<span data-ttu-id="64c33-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="64c33-147">The publisher of the app.</span></span> <span data-ttu-id="64c33-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="64c33-149">largeIcon</span></span>|[<span data-ttu-id="64c33-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="64c33-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="64c33-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="64c33-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="64c33-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64c33-153">createdDateTime</span></span>|<span data-ttu-id="64c33-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64c33-154">DateTimeOffset</span></span>|<span data-ttu-id="64c33-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="64c33-155">The date and time the app was created.</span></span> <span data-ttu-id="64c33-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64c33-157">lastModifiedDateTime</span></span>|<span data-ttu-id="64c33-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64c33-158">DateTimeOffset</span></span>|<span data-ttu-id="64c33-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="64c33-159">The date and time the app was last modified.</span></span> <span data-ttu-id="64c33-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="64c33-161">isFeatured</span></span>|<span data-ttu-id="64c33-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="64c33-162">Boolean</span></span>|<span data-ttu-id="64c33-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="64c33-164">privacyInformationUrl</span></span>|<span data-ttu-id="64c33-165">String</span><span class="sxs-lookup"><span data-stu-id="64c33-165">String</span></span>|<span data-ttu-id="64c33-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="64c33-166">The privacy statement Url.</span></span> <span data-ttu-id="64c33-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="64c33-168">informationUrl</span></span>|<span data-ttu-id="64c33-169">String</span><span class="sxs-lookup"><span data-stu-id="64c33-169">String</span></span>|<span data-ttu-id="64c33-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="64c33-170">The more information Url.</span></span> <span data-ttu-id="64c33-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-172">owner</span><span class="sxs-lookup"><span data-stu-id="64c33-172">owner</span></span>|<span data-ttu-id="64c33-173">String</span><span class="sxs-lookup"><span data-stu-id="64c33-173">String</span></span>|<span data-ttu-id="64c33-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="64c33-174">The owner of the app.</span></span> <span data-ttu-id="64c33-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-176">developer</span><span class="sxs-lookup"><span data-stu-id="64c33-176">developer</span></span>|<span data-ttu-id="64c33-177">String</span><span class="sxs-lookup"><span data-stu-id="64c33-177">String</span></span>|<span data-ttu-id="64c33-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="64c33-178">The developer of the app.</span></span> <span data-ttu-id="64c33-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-180">notes</span><span class="sxs-lookup"><span data-stu-id="64c33-180">notes</span></span>|<span data-ttu-id="64c33-181">String</span><span class="sxs-lookup"><span data-stu-id="64c33-181">String</span></span>|<span data-ttu-id="64c33-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="64c33-182">Notes for the app.</span></span> <span data-ttu-id="64c33-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="64c33-184">uploadState</span></span>|<span data-ttu-id="64c33-185">Int32</span><span class="sxs-lookup"><span data-stu-id="64c33-185">Int32</span></span>|<span data-ttu-id="64c33-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="64c33-186">The upload state.</span></span> <span data-ttu-id="64c33-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="64c33-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="64c33-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="64c33-189">publishingState</span></span>|[<span data-ttu-id="64c33-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="64c33-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="64c33-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="64c33-191">The publishing state for the app.</span></span> <span data-ttu-id="64c33-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="64c33-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="64c33-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="64c33-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="64c33-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="64c33-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="64c33-195">isAssigned</span></span>|<span data-ttu-id="64c33-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="64c33-196">Boolean</span></span>|<span data-ttu-id="64c33-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="64c33-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="64c33-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64c33-199">roleScopeTagIds</span></span>|<span data-ttu-id="64c33-200">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="64c33-200">String collection</span></span>|<span data-ttu-id="64c33-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="64c33-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="64c33-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="64c33-203">dependentAppCount</span></span>|<span data-ttu-id="64c33-204">Int32</span><span class="sxs-lookup"><span data-stu-id="64c33-204">Int32</span></span>|<span data-ttu-id="64c33-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="64c33-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="64c33-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-207">суперседингаппкаунт</span><span class="sxs-lookup"><span data-stu-id="64c33-207">supersedingAppCount</span></span>|<span data-ttu-id="64c33-208">Int32</span><span class="sxs-lookup"><span data-stu-id="64c33-208">Int32</span></span>|<span data-ttu-id="64c33-209">Общее количество приложений, которые напрямую или косвенно заменяют данное приложение.</span><span class="sxs-lookup"><span data-stu-id="64c33-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="64c33-210">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-211">суперседедаппкаунт</span><span class="sxs-lookup"><span data-stu-id="64c33-211">supersededAppCount</span></span>|<span data-ttu-id="64c33-212">Int32</span><span class="sxs-lookup"><span data-stu-id="64c33-212">Int32</span></span>|<span data-ttu-id="64c33-213">Общее число приложений, для которых это приложение напрямую или косвенно заменяется.</span><span class="sxs-lookup"><span data-stu-id="64c33-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="64c33-214">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="64c33-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="64c33-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="64c33-215">bundleId</span></span>|<span data-ttu-id="64c33-216">String</span><span class="sxs-lookup"><span data-stu-id="64c33-216">String</span></span>|<span data-ttu-id="64c33-217">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="64c33-217">The Identity Name.</span></span>|
|<span data-ttu-id="64c33-218">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="64c33-218">appStoreUrl</span></span>|<span data-ttu-id="64c33-219">String</span><span class="sxs-lookup"><span data-stu-id="64c33-219">String</span></span>|<span data-ttu-id="64c33-220">URL-адрес в Apple App Store</span><span class="sxs-lookup"><span data-stu-id="64c33-220">The Apple App Store URL</span></span>|
|<span data-ttu-id="64c33-221">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="64c33-221">applicableDeviceType</span></span>|[<span data-ttu-id="64c33-222">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="64c33-222">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="64c33-223">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="64c33-223">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="64c33-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="64c33-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="64c33-225">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="64c33-225">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="64c33-226">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="64c33-226">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="64c33-227">Ответ</span><span class="sxs-lookup"><span data-stu-id="64c33-227">Response</span></span>
<span data-ttu-id="64c33-228">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="64c33-228">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64c33-229">Пример</span><span class="sxs-lookup"><span data-stu-id="64c33-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="64c33-230">Запрос</span><span class="sxs-lookup"><span data-stu-id="64c33-230">Request</span></span>
<span data-ttu-id="64c33-231">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64c33-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="64c33-232">Отклик</span><span class="sxs-lookup"><span data-stu-id="64c33-232">Response</span></span>
<span data-ttu-id="64c33-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64c33-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





