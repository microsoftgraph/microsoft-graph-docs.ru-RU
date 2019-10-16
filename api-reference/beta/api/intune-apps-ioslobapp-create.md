---
title: Create iosLobApp
description: Создание нового объекта iosLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad0df70f908c42084d8f9769c1b01bf8d65929aa
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535438"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="3725b-103">Create iosLobApp</span><span class="sxs-lookup"><span data-stu-id="3725b-103">Create iosLobApp</span></span>

> <span data-ttu-id="3725b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3725b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3725b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3725b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3725b-106">Создание нового объекта [iosLobApp](../resources/intune-apps-ioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-106">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3725b-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3725b-107">Prerequisites</span></span>
<span data-ttu-id="3725b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3725b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3725b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3725b-110">Permission type</span></span>|<span data-ttu-id="3725b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3725b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3725b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3725b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3725b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3725b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3725b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3725b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3725b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3725b-115">Not supported.</span></span>|
|<span data-ttu-id="3725b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3725b-116">Application</span></span>|<span data-ttu-id="3725b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3725b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3725b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3725b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3725b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3725b-119">Request headers</span></span>
|<span data-ttu-id="3725b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3725b-120">Header</span></span>|<span data-ttu-id="3725b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3725b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3725b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3725b-122">Authorization</span></span>|<span data-ttu-id="3725b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3725b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3725b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3725b-124">Accept</span></span>|<span data-ttu-id="3725b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3725b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3725b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3725b-126">Request body</span></span>
<span data-ttu-id="3725b-127">В теле запроса добавьте представление объекта iosLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3725b-127">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="3725b-128">Ниже показаны свойства, которые необходимо указывать при создании объекта iosLobApp.</span><span class="sxs-lookup"><span data-stu-id="3725b-128">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="3725b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3725b-129">Property</span></span>|<span data-ttu-id="3725b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3725b-130">Type</span></span>|<span data-ttu-id="3725b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3725b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3725b-132">id</span><span class="sxs-lookup"><span data-stu-id="3725b-132">id</span></span>|<span data-ttu-id="3725b-133">Строка</span><span class="sxs-lookup"><span data-stu-id="3725b-133">String</span></span>|<span data-ttu-id="3725b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3725b-134">Key of the entity.</span></span> <span data-ttu-id="3725b-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3725b-136">displayName</span></span>|<span data-ttu-id="3725b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3725b-137">String</span></span>|<span data-ttu-id="3725b-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="3725b-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3725b-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-140">description</span><span class="sxs-lookup"><span data-stu-id="3725b-140">description</span></span>|<span data-ttu-id="3725b-141">Строка</span><span class="sxs-lookup"><span data-stu-id="3725b-141">String</span></span>|<span data-ttu-id="3725b-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="3725b-142">The description of the app.</span></span> <span data-ttu-id="3725b-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-144">publisher</span><span class="sxs-lookup"><span data-stu-id="3725b-144">publisher</span></span>|<span data-ttu-id="3725b-145">String</span><span class="sxs-lookup"><span data-stu-id="3725b-145">String</span></span>|<span data-ttu-id="3725b-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="3725b-146">The publisher of the app.</span></span> <span data-ttu-id="3725b-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3725b-148">largeIcon</span></span>|[<span data-ttu-id="3725b-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3725b-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3725b-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="3725b-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3725b-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3725b-152">createdDateTime</span></span>|<span data-ttu-id="3725b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3725b-153">DateTimeOffset</span></span>|<span data-ttu-id="3725b-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="3725b-154">The date and time the app was created.</span></span> <span data-ttu-id="3725b-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3725b-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3725b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3725b-157">DateTimeOffset</span></span>|<span data-ttu-id="3725b-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="3725b-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3725b-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3725b-160">isFeatured</span></span>|<span data-ttu-id="3725b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="3725b-161">Boolean</span></span>|<span data-ttu-id="3725b-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3725b-163">privacyInformationUrl</span></span>|<span data-ttu-id="3725b-164">String</span><span class="sxs-lookup"><span data-stu-id="3725b-164">String</span></span>|<span data-ttu-id="3725b-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3725b-165">The privacy statement Url.</span></span> <span data-ttu-id="3725b-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3725b-167">informationUrl</span></span>|<span data-ttu-id="3725b-168">String</span><span class="sxs-lookup"><span data-stu-id="3725b-168">String</span></span>|<span data-ttu-id="3725b-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3725b-169">The more information Url.</span></span> <span data-ttu-id="3725b-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-171">owner</span><span class="sxs-lookup"><span data-stu-id="3725b-171">owner</span></span>|<span data-ttu-id="3725b-172">String</span><span class="sxs-lookup"><span data-stu-id="3725b-172">String</span></span>|<span data-ttu-id="3725b-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="3725b-173">The owner of the app.</span></span> <span data-ttu-id="3725b-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-175">developer</span><span class="sxs-lookup"><span data-stu-id="3725b-175">developer</span></span>|<span data-ttu-id="3725b-176">String</span><span class="sxs-lookup"><span data-stu-id="3725b-176">String</span></span>|<span data-ttu-id="3725b-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="3725b-177">The developer of the app.</span></span> <span data-ttu-id="3725b-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-179">notes</span><span class="sxs-lookup"><span data-stu-id="3725b-179">notes</span></span>|<span data-ttu-id="3725b-180">String</span><span class="sxs-lookup"><span data-stu-id="3725b-180">String</span></span>|<span data-ttu-id="3725b-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="3725b-181">Notes for the app.</span></span> <span data-ttu-id="3725b-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="3725b-183">uploadState</span></span>|<span data-ttu-id="3725b-184">Int32</span><span class="sxs-lookup"><span data-stu-id="3725b-184">Int32</span></span>|<span data-ttu-id="3725b-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="3725b-185">The upload state.</span></span> <span data-ttu-id="3725b-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="3725b-187">publishingState</span></span>|[<span data-ttu-id="3725b-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="3725b-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3725b-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="3725b-189">The publishing state for the app.</span></span> <span data-ttu-id="3725b-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="3725b-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3725b-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="3725b-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3725b-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3725b-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3725b-193">isAssigned</span></span>|<span data-ttu-id="3725b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="3725b-194">Boolean</span></span>|<span data-ttu-id="3725b-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="3725b-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3725b-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3725b-197">roleScopeTagIds</span></span>|<span data-ttu-id="3725b-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3725b-198">String collection</span></span>|<span data-ttu-id="3725b-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="3725b-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3725b-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="3725b-201">dependentAppCount</span></span>|<span data-ttu-id="3725b-202">Int32</span><span class="sxs-lookup"><span data-stu-id="3725b-202">Int32</span></span>|<span data-ttu-id="3725b-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="3725b-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="3725b-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="3725b-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3725b-205">committedContentVersion</span></span>|<span data-ttu-id="3725b-206">String</span><span class="sxs-lookup"><span data-stu-id="3725b-206">String</span></span>|<span data-ttu-id="3725b-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="3725b-207">The internal committed content version.</span></span> <span data-ttu-id="3725b-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3725b-209">fileName</span><span class="sxs-lookup"><span data-stu-id="3725b-209">fileName</span></span>|<span data-ttu-id="3725b-210">String</span><span class="sxs-lookup"><span data-stu-id="3725b-210">String</span></span>|<span data-ttu-id="3725b-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="3725b-211">The name of the main Lob application file.</span></span> <span data-ttu-id="3725b-212">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3725b-213">size</span><span class="sxs-lookup"><span data-stu-id="3725b-213">size</span></span>|<span data-ttu-id="3725b-214">Int64</span><span class="sxs-lookup"><span data-stu-id="3725b-214">Int64</span></span>|<span data-ttu-id="3725b-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="3725b-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="3725b-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3725b-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3725b-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="3725b-217">bundleId</span></span>|<span data-ttu-id="3725b-218">String</span><span class="sxs-lookup"><span data-stu-id="3725b-218">String</span></span>|<span data-ttu-id="3725b-219">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3725b-219">The Identity Name.</span></span>|
|<span data-ttu-id="3725b-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="3725b-220">applicableDeviceType</span></span>|[<span data-ttu-id="3725b-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3725b-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="3725b-222">Архитектура iOS, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="3725b-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="3725b-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3725b-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3725b-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3725b-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="3725b-225">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="3725b-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3725b-226">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3725b-226">expirationDateTime</span></span>|<span data-ttu-id="3725b-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3725b-227">DateTimeOffset</span></span>|<span data-ttu-id="3725b-228">Срок действия.</span><span class="sxs-lookup"><span data-stu-id="3725b-228">The expiration time.</span></span>|
|<span data-ttu-id="3725b-229">versionNumber</span><span class="sxs-lookup"><span data-stu-id="3725b-229">versionNumber</span></span>|<span data-ttu-id="3725b-230">String</span><span class="sxs-lookup"><span data-stu-id="3725b-230">String</span></span>|<span data-ttu-id="3725b-231">Номер версии бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="3725b-231">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3725b-232">buildNumber</span><span class="sxs-lookup"><span data-stu-id="3725b-232">buildNumber</span></span>|<span data-ttu-id="3725b-233">String</span><span class="sxs-lookup"><span data-stu-id="3725b-233">String</span></span>|<span data-ttu-id="3725b-234">Номер сборки бизнес-приложения для iOS.</span><span class="sxs-lookup"><span data-stu-id="3725b-234">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3725b-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="3725b-235">identityVersion</span></span>|<span data-ttu-id="3725b-236">String</span><span class="sxs-lookup"><span data-stu-id="3725b-236">String</span></span>|<span data-ttu-id="3725b-237">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3725b-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="3725b-238">Ответ</span><span class="sxs-lookup"><span data-stu-id="3725b-238">Response</span></span>
<span data-ttu-id="3725b-239">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosLobApp](../resources/intune-apps-ioslobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3725b-239">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3725b-240">Пример</span><span class="sxs-lookup"><span data-stu-id="3725b-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="3725b-241">Запрос</span><span class="sxs-lookup"><span data-stu-id="3725b-241">Request</span></span>
<span data-ttu-id="3725b-242">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3725b-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3725b-243">Отклик</span><span class="sxs-lookup"><span data-stu-id="3725b-243">Response</span></span>
<span data-ttu-id="3725b-p122">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3725b-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






