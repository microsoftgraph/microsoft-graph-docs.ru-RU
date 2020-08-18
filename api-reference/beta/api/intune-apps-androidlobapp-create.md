---
title: Create androidLobApp
description: Создание нового объекта androidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9c328752364b90167e4be9f446499023943ff447
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790128"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="f18cd-103">Create androidLobApp</span><span class="sxs-lookup"><span data-stu-id="f18cd-103">Create androidLobApp</span></span>

<span data-ttu-id="f18cd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f18cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f18cd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f18cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f18cd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f18cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f18cd-107">Создание нового объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-107">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f18cd-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f18cd-108">Prerequisites</span></span>
<span data-ttu-id="f18cd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f18cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f18cd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f18cd-111">Permission type</span></span>|<span data-ttu-id="f18cd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f18cd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f18cd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f18cd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f18cd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f18cd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f18cd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f18cd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f18cd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f18cd-116">Not supported.</span></span>|
|<span data-ttu-id="f18cd-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f18cd-117">Application</span></span>|<span data-ttu-id="f18cd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f18cd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f18cd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f18cd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f18cd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f18cd-120">Request headers</span></span>
|<span data-ttu-id="f18cd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f18cd-121">Header</span></span>|<span data-ttu-id="f18cd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f18cd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f18cd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f18cd-123">Authorization</span></span>|<span data-ttu-id="f18cd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f18cd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f18cd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f18cd-125">Accept</span></span>|<span data-ttu-id="f18cd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f18cd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f18cd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f18cd-127">Request body</span></span>
<span data-ttu-id="f18cd-128">В теле запроса добавьте представление объекта androidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f18cd-128">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="f18cd-129">Ниже показаны свойства, которые необходимо указывать при создании объекта androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="f18cd-129">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="f18cd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f18cd-130">Property</span></span>|<span data-ttu-id="f18cd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f18cd-131">Type</span></span>|<span data-ttu-id="f18cd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f18cd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f18cd-133">id</span><span class="sxs-lookup"><span data-stu-id="f18cd-133">id</span></span>|<span data-ttu-id="f18cd-134">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-134">String</span></span>|<span data-ttu-id="f18cd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f18cd-135">Key of the entity.</span></span> <span data-ttu-id="f18cd-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f18cd-137">displayName</span></span>|<span data-ttu-id="f18cd-138">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-138">String</span></span>|<span data-ttu-id="f18cd-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="f18cd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f18cd-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-141">description</span><span class="sxs-lookup"><span data-stu-id="f18cd-141">description</span></span>|<span data-ttu-id="f18cd-142">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-142">String</span></span>|<span data-ttu-id="f18cd-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-143">The description of the app.</span></span> <span data-ttu-id="f18cd-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f18cd-145">publisher</span></span>|<span data-ttu-id="f18cd-146">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-146">String</span></span>|<span data-ttu-id="f18cd-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-147">The publisher of the app.</span></span> <span data-ttu-id="f18cd-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f18cd-149">largeIcon</span></span>|[<span data-ttu-id="f18cd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f18cd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f18cd-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f18cd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f18cd-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f18cd-153">createdDateTime</span></span>|<span data-ttu-id="f18cd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f18cd-154">DateTimeOffset</span></span>|<span data-ttu-id="f18cd-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-155">The date and time the app was created.</span></span> <span data-ttu-id="f18cd-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f18cd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f18cd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f18cd-158">DateTimeOffset</span></span>|<span data-ttu-id="f18cd-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f18cd-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f18cd-161">isFeatured</span></span>|<span data-ttu-id="f18cd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f18cd-162">Boolean</span></span>|<span data-ttu-id="f18cd-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f18cd-164">privacyInformationUrl</span></span>|<span data-ttu-id="f18cd-165">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-165">String</span></span>|<span data-ttu-id="f18cd-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f18cd-166">The privacy statement Url.</span></span> <span data-ttu-id="f18cd-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f18cd-168">informationUrl</span></span>|<span data-ttu-id="f18cd-169">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-169">String</span></span>|<span data-ttu-id="f18cd-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f18cd-170">The more information Url.</span></span> <span data-ttu-id="f18cd-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-172">owner</span><span class="sxs-lookup"><span data-stu-id="f18cd-172">owner</span></span>|<span data-ttu-id="f18cd-173">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-173">String</span></span>|<span data-ttu-id="f18cd-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-174">The owner of the app.</span></span> <span data-ttu-id="f18cd-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-176">developer</span><span class="sxs-lookup"><span data-stu-id="f18cd-176">developer</span></span>|<span data-ttu-id="f18cd-177">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-177">String</span></span>|<span data-ttu-id="f18cd-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-178">The developer of the app.</span></span> <span data-ttu-id="f18cd-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-180">notes</span><span class="sxs-lookup"><span data-stu-id="f18cd-180">notes</span></span>|<span data-ttu-id="f18cd-181">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-181">String</span></span>|<span data-ttu-id="f18cd-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-182">Notes for the app.</span></span> <span data-ttu-id="f18cd-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f18cd-184">uploadState</span></span>|<span data-ttu-id="f18cd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f18cd-185">Int32</span></span>|<span data-ttu-id="f18cd-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="f18cd-186">The upload state.</span></span> <span data-ttu-id="f18cd-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="f18cd-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="f18cd-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="f18cd-189">publishingState</span></span>|[<span data-ttu-id="f18cd-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="f18cd-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f18cd-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-191">The publishing state for the app.</span></span> <span data-ttu-id="f18cd-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f18cd-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f18cd-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f18cd-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f18cd-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f18cd-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f18cd-195">isAssigned</span></span>|<span data-ttu-id="f18cd-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f18cd-196">Boolean</span></span>|<span data-ttu-id="f18cd-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="f18cd-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f18cd-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f18cd-199">roleScopeTagIds</span></span>|<span data-ttu-id="f18cd-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f18cd-200">String collection</span></span>|<span data-ttu-id="f18cd-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f18cd-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="f18cd-203">dependentAppCount</span></span>|<span data-ttu-id="f18cd-204">Int32</span><span class="sxs-lookup"><span data-stu-id="f18cd-204">Int32</span></span>|<span data-ttu-id="f18cd-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f18cd-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f18cd-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f18cd-207">committedContentVersion</span></span>|<span data-ttu-id="f18cd-208">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-208">String</span></span>|<span data-ttu-id="f18cd-209">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="f18cd-209">The internal committed content version.</span></span> <span data-ttu-id="f18cd-210">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f18cd-211">fileName</span><span class="sxs-lookup"><span data-stu-id="f18cd-211">fileName</span></span>|<span data-ttu-id="f18cd-212">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-212">String</span></span>|<span data-ttu-id="f18cd-213">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-213">The name of the main Lob application file.</span></span> <span data-ttu-id="f18cd-214">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f18cd-215">size</span><span class="sxs-lookup"><span data-stu-id="f18cd-215">size</span></span>|<span data-ttu-id="f18cd-216">Int64</span><span class="sxs-lookup"><span data-stu-id="f18cd-216">Int64</span></span>|<span data-ttu-id="f18cd-217">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="f18cd-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="f18cd-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f18cd-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f18cd-219">packageId</span><span class="sxs-lookup"><span data-stu-id="f18cd-219">packageId</span></span>|<span data-ttu-id="f18cd-220">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-220">String</span></span>|<span data-ttu-id="f18cd-221">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="f18cd-221">The package identifier.</span></span>|
|<span data-ttu-id="f18cd-222">identityName</span><span class="sxs-lookup"><span data-stu-id="f18cd-222">identityName</span></span>|<span data-ttu-id="f18cd-223">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-223">String</span></span>|<span data-ttu-id="f18cd-224">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-224">The Identity Name.</span></span>|
|<span data-ttu-id="f18cd-225">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f18cd-225">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f18cd-226">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f18cd-226">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="f18cd-227">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="f18cd-227">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f18cd-228">versionName</span><span class="sxs-lookup"><span data-stu-id="f18cd-228">versionName</span></span>|<span data-ttu-id="f18cd-229">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-229">String</span></span>|<span data-ttu-id="f18cd-230">Имя версии бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="f18cd-230">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f18cd-231">versionCode</span><span class="sxs-lookup"><span data-stu-id="f18cd-231">versionCode</span></span>|<span data-ttu-id="f18cd-232">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-232">String</span></span>|<span data-ttu-id="f18cd-233">Код версии бизнес-приложения Android.</span><span class="sxs-lookup"><span data-stu-id="f18cd-233">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f18cd-234">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f18cd-234">identityVersion</span></span>|<span data-ttu-id="f18cd-235">String</span><span class="sxs-lookup"><span data-stu-id="f18cd-235">String</span></span>|<span data-ttu-id="f18cd-236">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f18cd-236">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f18cd-237">Ответ</span><span class="sxs-lookup"><span data-stu-id="f18cd-237">Response</span></span>
<span data-ttu-id="f18cd-238">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidLobApp](../resources/intune-apps-androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f18cd-238">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f18cd-239">Пример</span><span class="sxs-lookup"><span data-stu-id="f18cd-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="f18cd-240">Запрос</span><span class="sxs-lookup"><span data-stu-id="f18cd-240">Request</span></span>
<span data-ttu-id="f18cd-241">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f18cd-241">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1413

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="f18cd-242">Отклик</span><span class="sxs-lookup"><span data-stu-id="f18cd-242">Response</span></span>
<span data-ttu-id="f18cd-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f18cd-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1585

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```



