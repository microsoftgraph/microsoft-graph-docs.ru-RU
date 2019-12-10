---
title: Update iosStoreApp
description: Обновление свойств объекта iosStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed6bf2776a42d2e11d87946fcf3cfc71899f9b6f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39920880"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="f2bb3-103">Update iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="f2bb3-103">Update iosStoreApp</span></span>

> <span data-ttu-id="f2bb3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2bb3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2bb3-106">Обновление свойств объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-106">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2bb3-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f2bb3-107">Prerequisites</span></span>
<span data-ttu-id="f2bb3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2bb3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2bb3-110">Permission type</span></span>|<span data-ttu-id="f2bb3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2bb3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2bb3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2bb3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f2bb3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2bb3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2bb3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2bb3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2bb3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-115">Not supported.</span></span>|
|<span data-ttu-id="f2bb3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2bb3-116">Application</span></span>|<span data-ttu-id="f2bb3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2bb3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2bb3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2bb3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f2bb3-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f2bb3-119">Request headers</span></span>
|<span data-ttu-id="f2bb3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2bb3-120">Header</span></span>|<span data-ttu-id="f2bb3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="f2bb3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2bb3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2bb3-122">Authorization</span></span>|<span data-ttu-id="f2bb3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2bb3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="f2bb3-124">Accept</span></span>|<span data-ttu-id="f2bb3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f2bb3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2bb3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f2bb3-126">Request body</span></span>
<span data-ttu-id="f2bb3-127">В тексте запроса добавьте представление объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-127">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="f2bb3-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-128">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="f2bb3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2bb3-129">Property</span></span>|<span data-ttu-id="f2bb3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="f2bb3-130">Type</span></span>|<span data-ttu-id="f2bb3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f2bb3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2bb3-132">id</span><span class="sxs-lookup"><span data-stu-id="f2bb3-132">id</span></span>|<span data-ttu-id="f2bb3-133">Строка</span><span class="sxs-lookup"><span data-stu-id="f2bb3-133">String</span></span>|<span data-ttu-id="f2bb3-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-134">Key of the entity.</span></span> <span data-ttu-id="f2bb3-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f2bb3-136">displayName</span></span>|<span data-ttu-id="f2bb3-137">Строка</span><span class="sxs-lookup"><span data-stu-id="f2bb3-137">String</span></span>|<span data-ttu-id="f2bb3-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f2bb3-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-140">description</span><span class="sxs-lookup"><span data-stu-id="f2bb3-140">description</span></span>|<span data-ttu-id="f2bb3-141">Строка</span><span class="sxs-lookup"><span data-stu-id="f2bb3-141">String</span></span>|<span data-ttu-id="f2bb3-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-142">The description of the app.</span></span> <span data-ttu-id="f2bb3-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f2bb3-144">publisher</span></span>|<span data-ttu-id="f2bb3-145">Строка</span><span class="sxs-lookup"><span data-stu-id="f2bb3-145">String</span></span>|<span data-ttu-id="f2bb3-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-146">The publisher of the app.</span></span> <span data-ttu-id="f2bb3-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f2bb3-148">largeIcon</span></span>|[<span data-ttu-id="f2bb3-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f2bb3-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f2bb3-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f2bb3-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2bb3-152">createdDateTime</span></span>|<span data-ttu-id="f2bb3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2bb3-153">DateTimeOffset</span></span>|<span data-ttu-id="f2bb3-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-154">The date and time the app was created.</span></span> <span data-ttu-id="f2bb3-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2bb3-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f2bb3-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2bb3-157">DateTimeOffset</span></span>|<span data-ttu-id="f2bb3-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f2bb3-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f2bb3-160">isFeatured</span></span>|<span data-ttu-id="f2bb3-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2bb3-161">Boolean</span></span>|<span data-ttu-id="f2bb3-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f2bb3-163">privacyInformationUrl</span></span>|<span data-ttu-id="f2bb3-164">Строка</span><span class="sxs-lookup"><span data-stu-id="f2bb3-164">String</span></span>|<span data-ttu-id="f2bb3-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-165">The privacy statement Url.</span></span> <span data-ttu-id="f2bb3-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f2bb3-167">informationUrl</span></span>|<span data-ttu-id="f2bb3-168">Строка</span><span class="sxs-lookup"><span data-stu-id="f2bb3-168">String</span></span>|<span data-ttu-id="f2bb3-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-169">The more information Url.</span></span> <span data-ttu-id="f2bb3-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-171">owner</span><span class="sxs-lookup"><span data-stu-id="f2bb3-171">owner</span></span>|<span data-ttu-id="f2bb3-172">String</span><span class="sxs-lookup"><span data-stu-id="f2bb3-172">String</span></span>|<span data-ttu-id="f2bb3-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-173">The owner of the app.</span></span> <span data-ttu-id="f2bb3-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-175">developer</span><span class="sxs-lookup"><span data-stu-id="f2bb3-175">developer</span></span>|<span data-ttu-id="f2bb3-176">Строка</span><span class="sxs-lookup"><span data-stu-id="f2bb3-176">String</span></span>|<span data-ttu-id="f2bb3-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-177">The developer of the app.</span></span> <span data-ttu-id="f2bb3-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-179">notes</span><span class="sxs-lookup"><span data-stu-id="f2bb3-179">notes</span></span>|<span data-ttu-id="f2bb3-180">Строка</span><span class="sxs-lookup"><span data-stu-id="f2bb3-180">String</span></span>|<span data-ttu-id="f2bb3-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-181">Notes for the app.</span></span> <span data-ttu-id="f2bb3-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f2bb3-183">uploadState</span></span>|<span data-ttu-id="f2bb3-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f2bb3-184">Int32</span></span>|<span data-ttu-id="f2bb3-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-185">The upload state.</span></span> <span data-ttu-id="f2bb3-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f2bb3-187">publishingState</span></span>|[<span data-ttu-id="f2bb3-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="f2bb3-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f2bb3-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-189">The publishing state for the app.</span></span> <span data-ttu-id="f2bb3-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f2bb3-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f2bb3-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f2bb3-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f2bb3-193">isAssigned</span></span>|<span data-ttu-id="f2bb3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2bb3-194">Boolean</span></span>|<span data-ttu-id="f2bb3-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f2bb3-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2bb3-197">roleScopeTagIds</span></span>|<span data-ttu-id="f2bb3-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f2bb3-198">String collection</span></span>|<span data-ttu-id="f2bb3-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f2bb3-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="f2bb3-201">dependentAppCount</span></span>|<span data-ttu-id="f2bb3-202">Int32</span><span class="sxs-lookup"><span data-stu-id="f2bb3-202">Int32</span></span>|<span data-ttu-id="f2bb3-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f2bb3-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2bb3-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2bb3-205">bundleId</span><span class="sxs-lookup"><span data-stu-id="f2bb3-205">bundleId</span></span>|<span data-ttu-id="f2bb3-206">String</span><span class="sxs-lookup"><span data-stu-id="f2bb3-206">String</span></span>|<span data-ttu-id="f2bb3-207">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-207">The Identity Name.</span></span>|
|<span data-ttu-id="f2bb3-208">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f2bb3-208">appStoreUrl</span></span>|<span data-ttu-id="f2bb3-209">String</span><span class="sxs-lookup"><span data-stu-id="f2bb3-209">String</span></span>|<span data-ttu-id="f2bb3-210">URL-адрес в Apple App Store</span><span class="sxs-lookup"><span data-stu-id="f2bb3-210">The Apple App Store URL</span></span>|
|<span data-ttu-id="f2bb3-211">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f2bb3-211">applicableDeviceType</span></span>|[<span data-ttu-id="f2bb3-212">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f2bb3-212">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="f2bb3-213">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-213">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="f2bb3-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2bb3-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f2bb3-215">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2bb3-215">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="f2bb3-216">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="f2bb3-217">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2bb3-217">Response</span></span>
<span data-ttu-id="f2bb3-218">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-218">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2bb3-219">Пример</span><span class="sxs-lookup"><span data-stu-id="f2bb3-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2bb3-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2bb3-220">Request</span></span>
<span data-ttu-id="f2bb3-221">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1160

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

### <a name="response"></a><span data-ttu-id="f2bb3-222">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2bb3-222">Response</span></span>
<span data-ttu-id="f2bb3-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2bb3-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1332

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





