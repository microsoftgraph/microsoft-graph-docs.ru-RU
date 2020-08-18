---
title: Create iosLobApp
description: Создание нового объекта iosLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ff80f7d187136b050809457da7798f364c8bda3
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791150"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="30546-103">Create iosLobApp</span><span class="sxs-lookup"><span data-stu-id="30546-103">Create iosLobApp</span></span>

<span data-ttu-id="30546-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30546-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30546-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30546-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30546-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30546-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30546-107">Создание нового объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-107">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30546-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="30546-108">Prerequisites</span></span>
<span data-ttu-id="30546-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30546-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30546-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30546-111">Permission type</span></span>|<span data-ttu-id="30546-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30546-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30546-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30546-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30546-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30546-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30546-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30546-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30546-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30546-116">Not supported.</span></span>|
|<span data-ttu-id="30546-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="30546-117">Application</span></span>|<span data-ttu-id="30546-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30546-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="30546-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30546-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="30546-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="30546-120">Request headers</span></span>
|<span data-ttu-id="30546-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30546-121">Header</span></span>|<span data-ttu-id="30546-122">Значение</span><span class="sxs-lookup"><span data-stu-id="30546-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30546-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30546-123">Authorization</span></span>|<span data-ttu-id="30546-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30546-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30546-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30546-125">Accept</span></span>|<span data-ttu-id="30546-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30546-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30546-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30546-127">Request body</span></span>
<span data-ttu-id="30546-128">В теле запроса добавьте представление объекта iosLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30546-128">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="30546-129">Ниже показаны свойства, которые необходимо указывать при создании объекта iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="30546-129">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="30546-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="30546-130">Property</span></span>|<span data-ttu-id="30546-131">Тип</span><span class="sxs-lookup"><span data-stu-id="30546-131">Type</span></span>|<span data-ttu-id="30546-132">Описание</span><span class="sxs-lookup"><span data-stu-id="30546-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30546-133">id</span><span class="sxs-lookup"><span data-stu-id="30546-133">id</span></span>|<span data-ttu-id="30546-134">String</span><span class="sxs-lookup"><span data-stu-id="30546-134">String</span></span>|<span data-ttu-id="30546-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="30546-135">Key of the entity.</span></span> <span data-ttu-id="30546-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-137">displayName</span><span class="sxs-lookup"><span data-stu-id="30546-137">displayName</span></span>|<span data-ttu-id="30546-138">String</span><span class="sxs-lookup"><span data-stu-id="30546-138">String</span></span>|<span data-ttu-id="30546-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="30546-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="30546-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-141">description</span><span class="sxs-lookup"><span data-stu-id="30546-141">description</span></span>|<span data-ttu-id="30546-142">String</span><span class="sxs-lookup"><span data-stu-id="30546-142">String</span></span>|<span data-ttu-id="30546-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="30546-143">The description of the app.</span></span> <span data-ttu-id="30546-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-145">publisher</span><span class="sxs-lookup"><span data-stu-id="30546-145">publisher</span></span>|<span data-ttu-id="30546-146">String</span><span class="sxs-lookup"><span data-stu-id="30546-146">String</span></span>|<span data-ttu-id="30546-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="30546-147">The publisher of the app.</span></span> <span data-ttu-id="30546-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="30546-149">largeIcon</span></span>|[<span data-ttu-id="30546-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="30546-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="30546-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="30546-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="30546-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30546-153">createdDateTime</span></span>|<span data-ttu-id="30546-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30546-154">DateTimeOffset</span></span>|<span data-ttu-id="30546-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="30546-155">The date and time the app was created.</span></span> <span data-ttu-id="30546-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30546-157">lastModifiedDateTime</span></span>|<span data-ttu-id="30546-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30546-158">DateTimeOffset</span></span>|<span data-ttu-id="30546-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="30546-159">The date and time the app was last modified.</span></span> <span data-ttu-id="30546-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="30546-161">isFeatured</span></span>|<span data-ttu-id="30546-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="30546-162">Boolean</span></span>|<span data-ttu-id="30546-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="30546-164">privacyInformationUrl</span></span>|<span data-ttu-id="30546-165">String</span><span class="sxs-lookup"><span data-stu-id="30546-165">String</span></span>|<span data-ttu-id="30546-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="30546-166">The privacy statement Url.</span></span> <span data-ttu-id="30546-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="30546-168">informationUrl</span></span>|<span data-ttu-id="30546-169">String</span><span class="sxs-lookup"><span data-stu-id="30546-169">String</span></span>|<span data-ttu-id="30546-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="30546-170">The more information Url.</span></span> <span data-ttu-id="30546-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-172">owner</span><span class="sxs-lookup"><span data-stu-id="30546-172">owner</span></span>|<span data-ttu-id="30546-173">String</span><span class="sxs-lookup"><span data-stu-id="30546-173">String</span></span>|<span data-ttu-id="30546-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="30546-174">The owner of the app.</span></span> <span data-ttu-id="30546-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-176">developer</span><span class="sxs-lookup"><span data-stu-id="30546-176">developer</span></span>|<span data-ttu-id="30546-177">String</span><span class="sxs-lookup"><span data-stu-id="30546-177">String</span></span>|<span data-ttu-id="30546-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="30546-178">The developer of the app.</span></span> <span data-ttu-id="30546-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-180">notes</span><span class="sxs-lookup"><span data-stu-id="30546-180">notes</span></span>|<span data-ttu-id="30546-181">String</span><span class="sxs-lookup"><span data-stu-id="30546-181">String</span></span>|<span data-ttu-id="30546-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="30546-182">Notes for the app.</span></span> <span data-ttu-id="30546-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="30546-184">uploadState</span></span>|<span data-ttu-id="30546-185">Int32</span><span class="sxs-lookup"><span data-stu-id="30546-185">Int32</span></span>|<span data-ttu-id="30546-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="30546-186">The upload state.</span></span> <span data-ttu-id="30546-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="30546-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="30546-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="30546-189">publishingState</span></span>|[<span data-ttu-id="30546-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="30546-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="30546-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="30546-191">The publishing state for the app.</span></span> <span data-ttu-id="30546-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="30546-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="30546-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="30546-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="30546-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="30546-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="30546-195">isAssigned</span></span>|<span data-ttu-id="30546-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="30546-196">Boolean</span></span>|<span data-ttu-id="30546-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="30546-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="30546-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="30546-199">roleScopeTagIds</span></span>|<span data-ttu-id="30546-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="30546-200">String collection</span></span>|<span data-ttu-id="30546-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="30546-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="30546-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="30546-203">dependentAppCount</span></span>|<span data-ttu-id="30546-204">Int32</span><span class="sxs-lookup"><span data-stu-id="30546-204">Int32</span></span>|<span data-ttu-id="30546-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="30546-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="30546-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="30546-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="30546-207">committedContentVersion</span></span>|<span data-ttu-id="30546-208">String</span><span class="sxs-lookup"><span data-stu-id="30546-208">String</span></span>|<span data-ttu-id="30546-209">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="30546-209">The internal committed content version.</span></span> <span data-ttu-id="30546-210">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="30546-211">fileName</span><span class="sxs-lookup"><span data-stu-id="30546-211">fileName</span></span>|<span data-ttu-id="30546-212">String</span><span class="sxs-lookup"><span data-stu-id="30546-212">String</span></span>|<span data-ttu-id="30546-213">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="30546-213">The name of the main Lob application file.</span></span> <span data-ttu-id="30546-214">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="30546-215">size</span><span class="sxs-lookup"><span data-stu-id="30546-215">size</span></span>|<span data-ttu-id="30546-216">Int64</span><span class="sxs-lookup"><span data-stu-id="30546-216">Int64</span></span>|<span data-ttu-id="30546-217">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="30546-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="30546-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="30546-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="30546-219">bundleId</span><span class="sxs-lookup"><span data-stu-id="30546-219">bundleId</span></span>|<span data-ttu-id="30546-220">String</span><span class="sxs-lookup"><span data-stu-id="30546-220">String</span></span>|<span data-ttu-id="30546-221">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="30546-221">The Identity Name.</span></span>|
|<span data-ttu-id="30546-222">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="30546-222">applicableDeviceType</span></span>|[<span data-ttu-id="30546-223">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="30546-223">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="30546-224">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="30546-224">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="30546-225">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="30546-225">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="30546-226">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="30546-226">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="30546-227">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="30546-227">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="30546-228">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="30546-228">expirationDateTime</span></span>|<span data-ttu-id="30546-229">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30546-229">DateTimeOffset</span></span>|<span data-ttu-id="30546-230">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="30546-230">The expiration time.</span></span>|
|<span data-ttu-id="30546-231">versionNumber</span><span class="sxs-lookup"><span data-stu-id="30546-231">versionNumber</span></span>|<span data-ttu-id="30546-232">String</span><span class="sxs-lookup"><span data-stu-id="30546-232">String</span></span>|<span data-ttu-id="30546-233">Номер версии бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="30546-233">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="30546-234">buildNumber</span><span class="sxs-lookup"><span data-stu-id="30546-234">buildNumber</span></span>|<span data-ttu-id="30546-235">String</span><span class="sxs-lookup"><span data-stu-id="30546-235">String</span></span>|<span data-ttu-id="30546-236">Номер сборки бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="30546-236">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="30546-237">identityVersion</span><span class="sxs-lookup"><span data-stu-id="30546-237">identityVersion</span></span>|<span data-ttu-id="30546-238">String</span><span class="sxs-lookup"><span data-stu-id="30546-238">String</span></span>|<span data-ttu-id="30546-239">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="30546-239">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="30546-240">Ответ</span><span class="sxs-lookup"><span data-stu-id="30546-240">Response</span></span>
<span data-ttu-id="30546-241">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosLobApp](../resources/intune-apps-ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="30546-241">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30546-242">Пример</span><span class="sxs-lookup"><span data-stu-id="30546-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="30546-243">Запрос</span><span class="sxs-lookup"><span data-stu-id="30546-243">Request</span></span>
<span data-ttu-id="30546-244">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30546-244">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1411

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
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="30546-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="30546-245">Response</span></span>
<span data-ttu-id="30546-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30546-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1583

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
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```



