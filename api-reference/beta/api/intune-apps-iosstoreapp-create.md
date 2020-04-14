---
title: Create iosStoreApp
description: Создание объекта iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e56c542d8be5bc23b0dd85b57431f2bf69ae5eb0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394705"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="ce4dc-103">Create iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="ce4dc-103">Create iosStoreApp</span></span>

<span data-ttu-id="ce4dc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce4dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce4dc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce4dc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce4dc-107">Создание объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-107">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce4dc-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ce4dc-108">Prerequisites</span></span>
<span data-ttu-id="ce4dc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce4dc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce4dc-111">Permission type</span></span>|<span data-ttu-id="ce4dc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce4dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce4dc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce4dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce4dc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce4dc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce4dc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce4dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce4dc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-116">Not supported.</span></span>|
|<span data-ttu-id="ce4dc-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ce4dc-117">Application</span></span>|<span data-ttu-id="ce4dc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce4dc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce4dc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce4dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ce4dc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ce4dc-120">Request headers</span></span>
|<span data-ttu-id="ce4dc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce4dc-121">Header</span></span>|<span data-ttu-id="ce4dc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ce4dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce4dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce4dc-123">Authorization</span></span>|<span data-ttu-id="ce4dc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce4dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce4dc-125">Accept</span></span>|<span data-ttu-id="ce4dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce4dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce4dc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce4dc-127">Request body</span></span>
<span data-ttu-id="ce4dc-128">В теле запроса добавьте представление объекта iosStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-128">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="ce4dc-129">Ниже показаны свойства, которые необходимо указывать при создании объекта iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-129">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="ce4dc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce4dc-130">Property</span></span>|<span data-ttu-id="ce4dc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ce4dc-131">Type</span></span>|<span data-ttu-id="ce4dc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ce4dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce4dc-133">id</span><span class="sxs-lookup"><span data-stu-id="ce4dc-133">id</span></span>|<span data-ttu-id="ce4dc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4dc-134">String</span></span>|<span data-ttu-id="ce4dc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-135">Key of the entity.</span></span> <span data-ttu-id="ce4dc-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ce4dc-137">displayName</span></span>|<span data-ttu-id="ce4dc-138">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4dc-138">String</span></span>|<span data-ttu-id="ce4dc-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ce4dc-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-141">description</span><span class="sxs-lookup"><span data-stu-id="ce4dc-141">description</span></span>|<span data-ttu-id="ce4dc-142">Строка</span><span class="sxs-lookup"><span data-stu-id="ce4dc-142">String</span></span>|<span data-ttu-id="ce4dc-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-143">The description of the app.</span></span> <span data-ttu-id="ce4dc-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ce4dc-145">publisher</span></span>|<span data-ttu-id="ce4dc-146">String</span><span class="sxs-lookup"><span data-stu-id="ce4dc-146">String</span></span>|<span data-ttu-id="ce4dc-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-147">The publisher of the app.</span></span> <span data-ttu-id="ce4dc-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ce4dc-149">largeIcon</span></span>|[<span data-ttu-id="ce4dc-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ce4dc-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ce4dc-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ce4dc-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce4dc-153">createdDateTime</span></span>|<span data-ttu-id="ce4dc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce4dc-154">DateTimeOffset</span></span>|<span data-ttu-id="ce4dc-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-155">The date and time the app was created.</span></span> <span data-ttu-id="ce4dc-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce4dc-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ce4dc-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce4dc-158">DateTimeOffset</span></span>|<span data-ttu-id="ce4dc-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ce4dc-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ce4dc-161">isFeatured</span></span>|<span data-ttu-id="ce4dc-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce4dc-162">Boolean</span></span>|<span data-ttu-id="ce4dc-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ce4dc-164">privacyInformationUrl</span></span>|<span data-ttu-id="ce4dc-165">String</span><span class="sxs-lookup"><span data-stu-id="ce4dc-165">String</span></span>|<span data-ttu-id="ce4dc-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-166">The privacy statement Url.</span></span> <span data-ttu-id="ce4dc-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ce4dc-168">informationUrl</span></span>|<span data-ttu-id="ce4dc-169">String</span><span class="sxs-lookup"><span data-stu-id="ce4dc-169">String</span></span>|<span data-ttu-id="ce4dc-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-170">The more information Url.</span></span> <span data-ttu-id="ce4dc-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-172">owner</span><span class="sxs-lookup"><span data-stu-id="ce4dc-172">owner</span></span>|<span data-ttu-id="ce4dc-173">String</span><span class="sxs-lookup"><span data-stu-id="ce4dc-173">String</span></span>|<span data-ttu-id="ce4dc-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-174">The owner of the app.</span></span> <span data-ttu-id="ce4dc-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-176">developer</span><span class="sxs-lookup"><span data-stu-id="ce4dc-176">developer</span></span>|<span data-ttu-id="ce4dc-177">String</span><span class="sxs-lookup"><span data-stu-id="ce4dc-177">String</span></span>|<span data-ttu-id="ce4dc-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-178">The developer of the app.</span></span> <span data-ttu-id="ce4dc-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-180">notes</span><span class="sxs-lookup"><span data-stu-id="ce4dc-180">notes</span></span>|<span data-ttu-id="ce4dc-181">String</span><span class="sxs-lookup"><span data-stu-id="ce4dc-181">String</span></span>|<span data-ttu-id="ce4dc-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-182">Notes for the app.</span></span> <span data-ttu-id="ce4dc-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ce4dc-184">uploadState</span></span>|<span data-ttu-id="ce4dc-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ce4dc-185">Int32</span></span>|<span data-ttu-id="ce4dc-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-186">The upload state.</span></span> <span data-ttu-id="ce4dc-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ce4dc-188">publishingState</span></span>|[<span data-ttu-id="ce4dc-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="ce4dc-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ce4dc-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-190">The publishing state for the app.</span></span> <span data-ttu-id="ce4dc-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ce4dc-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ce4dc-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ce4dc-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ce4dc-194">isAssigned</span></span>|<span data-ttu-id="ce4dc-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce4dc-195">Boolean</span></span>|<span data-ttu-id="ce4dc-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ce4dc-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ce4dc-198">roleScopeTagIds</span></span>|<span data-ttu-id="ce4dc-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ce4dc-199">String collection</span></span>|<span data-ttu-id="ce4dc-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ce4dc-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="ce4dc-202">dependentAppCount</span></span>|<span data-ttu-id="ce4dc-203">Int32</span><span class="sxs-lookup"><span data-stu-id="ce4dc-203">Int32</span></span>|<span data-ttu-id="ce4dc-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ce4dc-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ce4dc-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ce4dc-206">bundleId</span><span class="sxs-lookup"><span data-stu-id="ce4dc-206">bundleId</span></span>|<span data-ttu-id="ce4dc-207">String</span><span class="sxs-lookup"><span data-stu-id="ce4dc-207">String</span></span>|<span data-ttu-id="ce4dc-208">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-208">The Identity Name.</span></span>|
|<span data-ttu-id="ce4dc-209">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ce4dc-209">appStoreUrl</span></span>|<span data-ttu-id="ce4dc-210">String</span><span class="sxs-lookup"><span data-stu-id="ce4dc-210">String</span></span>|<span data-ttu-id="ce4dc-211">URL-адрес в Apple App Store</span><span class="sxs-lookup"><span data-stu-id="ce4dc-211">The Apple App Store URL</span></span>|
|<span data-ttu-id="ce4dc-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ce4dc-212">applicableDeviceType</span></span>|[<span data-ttu-id="ce4dc-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ce4dc-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="ce4dc-214">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="ce4dc-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ce4dc-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ce4dc-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ce4dc-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="ce4dc-217">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-217">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="ce4dc-218">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce4dc-218">Response</span></span>
<span data-ttu-id="ce4dc-219">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-219">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce4dc-220">Пример</span><span class="sxs-lookup"><span data-stu-id="ce4dc-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce4dc-221">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce4dc-221">Request</span></span>
<span data-ttu-id="ce4dc-222">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="ce4dc-223">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce4dc-223">Response</span></span>
<span data-ttu-id="ce4dc-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce4dc-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



