---
title: Create managedIOSStoreApp
description: Создание объекта managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20c14a37baabdb5bc0817fa81b4b5777c819570b
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791094"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="6a2c6-103">Create managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="6a2c6-103">Create managedIOSStoreApp</span></span>

<span data-ttu-id="6a2c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a2c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a2c6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a2c6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a2c6-107">Создание объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-107">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a2c6-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6a2c6-108">Prerequisites</span></span>
<span data-ttu-id="6a2c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a2c6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a2c6-111">Permission type</span></span>|<span data-ttu-id="6a2c6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a2c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a2c6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a2c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a2c6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a2c6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6a2c6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a2c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a2c6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-116">Not supported.</span></span>|
|<span data-ttu-id="6a2c6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="6a2c6-117">Application</span></span>|<span data-ttu-id="6a2c6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a2c6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a2c6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a2c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6a2c6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6a2c6-120">Request headers</span></span>
|<span data-ttu-id="6a2c6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6a2c6-121">Header</span></span>|<span data-ttu-id="6a2c6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6a2c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a2c6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a2c6-123">Authorization</span></span>|<span data-ttu-id="6a2c6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a2c6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6a2c6-125">Accept</span></span>|<span data-ttu-id="6a2c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a2c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a2c6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a2c6-127">Request body</span></span>
<span data-ttu-id="6a2c6-128">В теле запроса добавьте представление объекта managedIOSStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-128">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="6a2c6-129">Ниже показаны свойства, которые необходимо указывать при создании объекта managedIOSStoreApp.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-129">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="6a2c6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a2c6-130">Property</span></span>|<span data-ttu-id="6a2c6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6a2c6-131">Type</span></span>|<span data-ttu-id="6a2c6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6a2c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a2c6-133">id</span><span class="sxs-lookup"><span data-stu-id="6a2c6-133">id</span></span>|<span data-ttu-id="6a2c6-134">String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-134">String</span></span>|<span data-ttu-id="6a2c6-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-135">Key of the entity.</span></span> <span data-ttu-id="6a2c6-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6a2c6-137">displayName</span></span>|<span data-ttu-id="6a2c6-138">String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-138">String</span></span>|<span data-ttu-id="6a2c6-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6a2c6-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-141">description</span><span class="sxs-lookup"><span data-stu-id="6a2c6-141">description</span></span>|<span data-ttu-id="6a2c6-142">String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-142">String</span></span>|<span data-ttu-id="6a2c6-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-143">The description of the app.</span></span> <span data-ttu-id="6a2c6-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-145">publisher</span><span class="sxs-lookup"><span data-stu-id="6a2c6-145">publisher</span></span>|<span data-ttu-id="6a2c6-146">String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-146">String</span></span>|<span data-ttu-id="6a2c6-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-147">The publisher of the app.</span></span> <span data-ttu-id="6a2c6-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6a2c6-149">largeIcon</span></span>|[<span data-ttu-id="6a2c6-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6a2c6-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6a2c6-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6a2c6-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a2c6-153">createdDateTime</span></span>|<span data-ttu-id="6a2c6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a2c6-154">DateTimeOffset</span></span>|<span data-ttu-id="6a2c6-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-155">The date and time the app was created.</span></span> <span data-ttu-id="6a2c6-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a2c6-157">lastModifiedDateTime</span></span>|<span data-ttu-id="6a2c6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a2c6-158">DateTimeOffset</span></span>|<span data-ttu-id="6a2c6-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-159">The date and time the app was last modified.</span></span> <span data-ttu-id="6a2c6-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6a2c6-161">isFeatured</span></span>|<span data-ttu-id="6a2c6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a2c6-162">Boolean</span></span>|<span data-ttu-id="6a2c6-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6a2c6-164">privacyInformationUrl</span></span>|<span data-ttu-id="6a2c6-165">String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-165">String</span></span>|<span data-ttu-id="6a2c6-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-166">The privacy statement Url.</span></span> <span data-ttu-id="6a2c6-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6a2c6-168">informationUrl</span></span>|<span data-ttu-id="6a2c6-169">String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-169">String</span></span>|<span data-ttu-id="6a2c6-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-170">The more information Url.</span></span> <span data-ttu-id="6a2c6-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-172">owner</span><span class="sxs-lookup"><span data-stu-id="6a2c6-172">owner</span></span>|<span data-ttu-id="6a2c6-173">String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-173">String</span></span>|<span data-ttu-id="6a2c6-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-174">The owner of the app.</span></span> <span data-ttu-id="6a2c6-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-176">developer</span><span class="sxs-lookup"><span data-stu-id="6a2c6-176">developer</span></span>|<span data-ttu-id="6a2c6-177">String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-177">String</span></span>|<span data-ttu-id="6a2c6-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-178">The developer of the app.</span></span> <span data-ttu-id="6a2c6-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-180">notes</span><span class="sxs-lookup"><span data-stu-id="6a2c6-180">notes</span></span>|<span data-ttu-id="6a2c6-181">String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-181">String</span></span>|<span data-ttu-id="6a2c6-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-182">Notes for the app.</span></span> <span data-ttu-id="6a2c6-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="6a2c6-184">uploadState</span></span>|<span data-ttu-id="6a2c6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="6a2c6-185">Int32</span></span>|<span data-ttu-id="6a2c6-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-186">The upload state.</span></span> <span data-ttu-id="6a2c6-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="6a2c6-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="6a2c6-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="6a2c6-189">publishingState</span></span>|[<span data-ttu-id="6a2c6-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="6a2c6-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6a2c6-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-191">The publishing state for the app.</span></span> <span data-ttu-id="6a2c6-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6a2c6-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="6a2c6-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6a2c6-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6a2c6-195">isAssigned</span></span>|<span data-ttu-id="6a2c6-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a2c6-196">Boolean</span></span>|<span data-ttu-id="6a2c6-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6a2c6-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6a2c6-199">roleScopeTagIds</span></span>|<span data-ttu-id="6a2c6-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-200">String collection</span></span>|<span data-ttu-id="6a2c6-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6a2c6-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="6a2c6-203">dependentAppCount</span></span>|<span data-ttu-id="6a2c6-204">Int32</span><span class="sxs-lookup"><span data-stu-id="6a2c6-204">Int32</span></span>|<span data-ttu-id="6a2c6-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6a2c6-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6a2c6-207">appAvailability</span><span class="sxs-lookup"><span data-stu-id="6a2c6-207">appAvailability</span></span>|[<span data-ttu-id="6a2c6-208">манажедаппаваилабилити</span><span class="sxs-lookup"><span data-stu-id="6a2c6-208">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="6a2c6-209">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-209">The Application's availability.</span></span> <span data-ttu-id="6a2c6-210">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="6a2c6-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="6a2c6-211">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-211">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="6a2c6-212">version</span><span class="sxs-lookup"><span data-stu-id="6a2c6-212">version</span></span>|<span data-ttu-id="6a2c6-213">String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-213">String</span></span>|<span data-ttu-id="6a2c6-214">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-214">The Application's version.</span></span> <span data-ttu-id="6a2c6-215">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="6a2c6-215">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="6a2c6-216">bundleId</span><span class="sxs-lookup"><span data-stu-id="6a2c6-216">bundleId</span></span>|<span data-ttu-id="6a2c6-217">String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-217">String</span></span>|<span data-ttu-id="6a2c6-218">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-218">The app's Bundle ID.</span></span>|
|<span data-ttu-id="6a2c6-219">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6a2c6-219">appStoreUrl</span></span>|<span data-ttu-id="6a2c6-220">String</span><span class="sxs-lookup"><span data-stu-id="6a2c6-220">String</span></span>|<span data-ttu-id="6a2c6-221">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-221">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="6a2c6-222">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="6a2c6-222">applicableDeviceType</span></span>|[<span data-ttu-id="6a2c6-223">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="6a2c6-223">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="6a2c6-224">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-224">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="6a2c6-225">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6a2c6-225">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6a2c6-226">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6a2c6-226">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="6a2c6-227">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-227">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="6a2c6-228">Ответ</span><span class="sxs-lookup"><span data-stu-id="6a2c6-228">Response</span></span>
<span data-ttu-id="6a2c6-229">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-229">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a2c6-230">Пример</span><span class="sxs-lookup"><span data-stu-id="6a2c6-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a2c6-231">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a2c6-231">Request</span></span>
<span data-ttu-id="6a2c6-232">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-232">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1238

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
    "v12_0": true,
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="6a2c6-233">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a2c6-233">Response</span></span>
<span data-ttu-id="6a2c6-p121">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a2c6-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1410

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
    "v12_0": true,
    "v13_0": true
  }
}
```



