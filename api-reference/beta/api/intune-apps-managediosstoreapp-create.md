---
title: Create managedIOSStoreApp
description: Создание объекта managedIOSStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 749200c1c9d6e87eb65d34f264d862baab35ef34
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329566"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="b4991-103">Create managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="b4991-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="b4991-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4991-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4991-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4991-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4991-106">Создание объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-106">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4991-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b4991-107">Prerequisites</span></span>
<span data-ttu-id="b4991-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4991-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4991-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4991-110">Permission type</span></span>|<span data-ttu-id="b4991-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4991-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4991-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4991-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4991-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4991-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4991-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4991-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4991-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4991-115">Not supported.</span></span>|
|<span data-ttu-id="b4991-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4991-116">Application</span></span>|<span data-ttu-id="b4991-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4991-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4991-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4991-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b4991-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4991-119">Request headers</span></span>
|<span data-ttu-id="b4991-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4991-120">Header</span></span>|<span data-ttu-id="b4991-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b4991-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4991-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4991-122">Authorization</span></span>|<span data-ttu-id="b4991-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4991-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4991-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b4991-124">Accept</span></span>|<span data-ttu-id="b4991-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4991-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4991-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b4991-126">Request body</span></span>
<span data-ttu-id="b4991-127">В теле запроса добавьте представление объекта managedIOSStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4991-127">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="b4991-128">Ниже показаны свойства, которые необходимо указывать при создании объекта managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="b4991-128">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="b4991-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4991-129">Property</span></span>|<span data-ttu-id="b4991-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b4991-130">Type</span></span>|<span data-ttu-id="b4991-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b4991-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4991-132">id</span><span class="sxs-lookup"><span data-stu-id="b4991-132">id</span></span>|<span data-ttu-id="b4991-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b4991-133">String</span></span>|<span data-ttu-id="b4991-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b4991-134">Key of the entity.</span></span> <span data-ttu-id="b4991-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b4991-136">displayName</span></span>|<span data-ttu-id="b4991-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b4991-137">String</span></span>|<span data-ttu-id="b4991-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b4991-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b4991-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-140">description</span><span class="sxs-lookup"><span data-stu-id="b4991-140">description</span></span>|<span data-ttu-id="b4991-141">String</span><span class="sxs-lookup"><span data-stu-id="b4991-141">String</span></span>|<span data-ttu-id="b4991-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-142">The description of the app.</span></span> <span data-ttu-id="b4991-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b4991-144">publisher</span></span>|<span data-ttu-id="b4991-145">String</span><span class="sxs-lookup"><span data-stu-id="b4991-145">String</span></span>|<span data-ttu-id="b4991-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-146">The publisher of the app.</span></span> <span data-ttu-id="b4991-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b4991-148">largeIcon</span></span>|[<span data-ttu-id="b4991-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b4991-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b4991-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b4991-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b4991-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4991-152">createdDateTime</span></span>|<span data-ttu-id="b4991-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4991-153">DateTimeOffset</span></span>|<span data-ttu-id="b4991-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-154">The date and time the app was created.</span></span> <span data-ttu-id="b4991-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4991-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b4991-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4991-157">DateTimeOffset</span></span>|<span data-ttu-id="b4991-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b4991-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b4991-160">isFeatured</span></span>|<span data-ttu-id="b4991-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4991-161">Boolean</span></span>|<span data-ttu-id="b4991-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b4991-163">privacyInformationUrl</span></span>|<span data-ttu-id="b4991-164">String</span><span class="sxs-lookup"><span data-stu-id="b4991-164">String</span></span>|<span data-ttu-id="b4991-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b4991-165">The privacy statement Url.</span></span> <span data-ttu-id="b4991-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b4991-167">informationUrl</span></span>|<span data-ttu-id="b4991-168">String</span><span class="sxs-lookup"><span data-stu-id="b4991-168">String</span></span>|<span data-ttu-id="b4991-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b4991-169">The more information Url.</span></span> <span data-ttu-id="b4991-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-171">owner</span><span class="sxs-lookup"><span data-stu-id="b4991-171">owner</span></span>|<span data-ttu-id="b4991-172">String</span><span class="sxs-lookup"><span data-stu-id="b4991-172">String</span></span>|<span data-ttu-id="b4991-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-173">The owner of the app.</span></span> <span data-ttu-id="b4991-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-175">developer</span><span class="sxs-lookup"><span data-stu-id="b4991-175">developer</span></span>|<span data-ttu-id="b4991-176">String</span><span class="sxs-lookup"><span data-stu-id="b4991-176">String</span></span>|<span data-ttu-id="b4991-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-177">The developer of the app.</span></span> <span data-ttu-id="b4991-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-179">notes</span><span class="sxs-lookup"><span data-stu-id="b4991-179">notes</span></span>|<span data-ttu-id="b4991-180">String</span><span class="sxs-lookup"><span data-stu-id="b4991-180">String</span></span>|<span data-ttu-id="b4991-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-181">Notes for the app.</span></span> <span data-ttu-id="b4991-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b4991-183">uploadState</span></span>|<span data-ttu-id="b4991-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b4991-184">Int32</span></span>|<span data-ttu-id="b4991-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="b4991-185">The upload state.</span></span> <span data-ttu-id="b4991-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b4991-187">publishingState</span></span>|[<span data-ttu-id="b4991-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="b4991-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b4991-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-189">The publishing state for the app.</span></span> <span data-ttu-id="b4991-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b4991-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b4991-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b4991-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b4991-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b4991-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b4991-193">isAssigned</span></span>|<span data-ttu-id="b4991-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4991-194">Boolean</span></span>|<span data-ttu-id="b4991-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="b4991-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b4991-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b4991-197">roleScopeTagIds</span></span>|<span data-ttu-id="b4991-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b4991-198">String collection</span></span>|<span data-ttu-id="b4991-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b4991-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="b4991-201">dependentAppCount</span></span>|<span data-ttu-id="b4991-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b4991-202">Int32</span></span>|<span data-ttu-id="b4991-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b4991-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b4991-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="b4991-205">appAvailability</span></span>|[<span data-ttu-id="b4991-206">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="b4991-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="b4991-207">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-207">The Application's availability.</span></span> <span data-ttu-id="b4991-208">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b4991-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="b4991-209">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="b4991-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="b4991-210">version</span><span class="sxs-lookup"><span data-stu-id="b4991-210">version</span></span>|<span data-ttu-id="b4991-211">String</span><span class="sxs-lookup"><span data-stu-id="b4991-211">String</span></span>|<span data-ttu-id="b4991-212">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-212">The Application's version.</span></span> <span data-ttu-id="b4991-213">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4991-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="b4991-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="b4991-214">bundleId</span></span>|<span data-ttu-id="b4991-215">String</span><span class="sxs-lookup"><span data-stu-id="b4991-215">String</span></span>|<span data-ttu-id="b4991-216">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="b4991-216">The app's Bundle ID.</span></span>|
|<span data-ttu-id="b4991-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b4991-217">appStoreUrl</span></span>|<span data-ttu-id="b4991-218">String</span><span class="sxs-lookup"><span data-stu-id="b4991-218">String</span></span>|<span data-ttu-id="b4991-219">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="b4991-219">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="b4991-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="b4991-220">applicableDeviceType</span></span>|[<span data-ttu-id="b4991-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="b4991-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="b4991-222">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="b4991-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="b4991-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b4991-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b4991-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b4991-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="b4991-225">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="b4991-225">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="b4991-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4991-226">Response</span></span>
<span data-ttu-id="b4991-227">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b4991-227">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4991-228">Пример</span><span class="sxs-lookup"><span data-stu-id="b4991-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4991-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4991-229">Request</span></span>
<span data-ttu-id="b4991-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4991-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1218

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="b4991-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4991-231">Response</span></span>
<span data-ttu-id="b4991-p121">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4991-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1390

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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
    "v12_0": true
  }
}
```






