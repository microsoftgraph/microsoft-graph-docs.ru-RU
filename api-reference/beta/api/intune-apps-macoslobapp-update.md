---
title: Обновление Макослобапп
description: Обновление свойств объекта Макослобапп.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 786c8df9a666b4728151b45ef3346fddd1b1297f
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792123"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="bfa13-103">Обновление Макослобапп</span><span class="sxs-lookup"><span data-stu-id="bfa13-103">Update macOSLobApp</span></span>

<span data-ttu-id="bfa13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfa13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bfa13-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfa13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfa13-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfa13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfa13-107">Обновление свойств объекта [макослобапп](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="bfa13-107">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfa13-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bfa13-108">Prerequisites</span></span>
<span data-ttu-id="bfa13-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfa13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfa13-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bfa13-111">Permission type</span></span>|<span data-ttu-id="bfa13-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bfa13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfa13-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bfa13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bfa13-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfa13-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bfa13-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bfa13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfa13-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfa13-116">Not supported.</span></span>|
|<span data-ttu-id="bfa13-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bfa13-117">Application</span></span>|<span data-ttu-id="bfa13-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfa13-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfa13-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bfa13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="bfa13-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bfa13-120">Request headers</span></span>
|<span data-ttu-id="bfa13-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bfa13-121">Header</span></span>|<span data-ttu-id="bfa13-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bfa13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfa13-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bfa13-123">Authorization</span></span>|<span data-ttu-id="bfa13-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bfa13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfa13-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bfa13-125">Accept</span></span>|<span data-ttu-id="bfa13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bfa13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfa13-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bfa13-127">Request body</span></span>
<span data-ttu-id="bfa13-128">В тексте запроса добавьте представление объекта [макослобапп](../resources/intune-apps-macoslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfa13-128">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="bfa13-129">В следующей таблице приведены свойства, необходимые при создании [макослобапп](../resources/intune-apps-macoslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-129">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="bfa13-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfa13-130">Property</span></span>|<span data-ttu-id="bfa13-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bfa13-131">Type</span></span>|<span data-ttu-id="bfa13-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bfa13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfa13-133">id</span><span class="sxs-lookup"><span data-stu-id="bfa13-133">id</span></span>|<span data-ttu-id="bfa13-134">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-134">String</span></span>|<span data-ttu-id="bfa13-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bfa13-135">Key of the entity.</span></span> <span data-ttu-id="bfa13-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-137">displayName</span><span class="sxs-lookup"><span data-stu-id="bfa13-137">displayName</span></span>|<span data-ttu-id="bfa13-138">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-138">String</span></span>|<span data-ttu-id="bfa13-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="bfa13-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bfa13-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-141">description</span><span class="sxs-lookup"><span data-stu-id="bfa13-141">description</span></span>|<span data-ttu-id="bfa13-142">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-142">String</span></span>|<span data-ttu-id="bfa13-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="bfa13-143">The description of the app.</span></span> <span data-ttu-id="bfa13-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-145">publisher</span><span class="sxs-lookup"><span data-stu-id="bfa13-145">publisher</span></span>|<span data-ttu-id="bfa13-146">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-146">String</span></span>|<span data-ttu-id="bfa13-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="bfa13-147">The publisher of the app.</span></span> <span data-ttu-id="bfa13-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bfa13-149">largeIcon</span></span>|[<span data-ttu-id="bfa13-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bfa13-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bfa13-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="bfa13-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bfa13-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bfa13-153">createdDateTime</span></span>|<span data-ttu-id="bfa13-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfa13-154">DateTimeOffset</span></span>|<span data-ttu-id="bfa13-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="bfa13-155">The date and time the app was created.</span></span> <span data-ttu-id="bfa13-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfa13-157">lastModifiedDateTime</span></span>|<span data-ttu-id="bfa13-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfa13-158">DateTimeOffset</span></span>|<span data-ttu-id="bfa13-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="bfa13-159">The date and time the app was last modified.</span></span> <span data-ttu-id="bfa13-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bfa13-161">isFeatured</span></span>|<span data-ttu-id="bfa13-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfa13-162">Boolean</span></span>|<span data-ttu-id="bfa13-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bfa13-164">privacyInformationUrl</span></span>|<span data-ttu-id="bfa13-165">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-165">String</span></span>|<span data-ttu-id="bfa13-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="bfa13-166">The privacy statement Url.</span></span> <span data-ttu-id="bfa13-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bfa13-168">informationUrl</span></span>|<span data-ttu-id="bfa13-169">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-169">String</span></span>|<span data-ttu-id="bfa13-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="bfa13-170">The more information Url.</span></span> <span data-ttu-id="bfa13-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-172">owner</span><span class="sxs-lookup"><span data-stu-id="bfa13-172">owner</span></span>|<span data-ttu-id="bfa13-173">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-173">String</span></span>|<span data-ttu-id="bfa13-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="bfa13-174">The owner of the app.</span></span> <span data-ttu-id="bfa13-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-176">developer</span><span class="sxs-lookup"><span data-stu-id="bfa13-176">developer</span></span>|<span data-ttu-id="bfa13-177">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-177">String</span></span>|<span data-ttu-id="bfa13-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="bfa13-178">The developer of the app.</span></span> <span data-ttu-id="bfa13-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-180">notes</span><span class="sxs-lookup"><span data-stu-id="bfa13-180">notes</span></span>|<span data-ttu-id="bfa13-181">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-181">String</span></span>|<span data-ttu-id="bfa13-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="bfa13-182">Notes for the app.</span></span> <span data-ttu-id="bfa13-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="bfa13-184">uploadState</span></span>|<span data-ttu-id="bfa13-185">Int32</span><span class="sxs-lookup"><span data-stu-id="bfa13-185">Int32</span></span>|<span data-ttu-id="bfa13-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="bfa13-186">The upload state.</span></span> <span data-ttu-id="bfa13-187">Возможные значения: 0 – `Not Ready` , 1 – `Ready` , 2 `Processing` .</span><span class="sxs-lookup"><span data-stu-id="bfa13-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="bfa13-188">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="bfa13-189">publishingState</span></span>|[<span data-ttu-id="bfa13-190">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="bfa13-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bfa13-191">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="bfa13-191">The publishing state for the app.</span></span> <span data-ttu-id="bfa13-192">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="bfa13-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bfa13-193">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="bfa13-194">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bfa13-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bfa13-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bfa13-195">isAssigned</span></span>|<span data-ttu-id="bfa13-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfa13-196">Boolean</span></span>|<span data-ttu-id="bfa13-197">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="bfa13-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="bfa13-198">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bfa13-199">roleScopeTagIds</span></span>|<span data-ttu-id="bfa13-200">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bfa13-200">String collection</span></span>|<span data-ttu-id="bfa13-201">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="bfa13-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="bfa13-202">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-203">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="bfa13-203">dependentAppCount</span></span>|<span data-ttu-id="bfa13-204">Int32</span><span class="sxs-lookup"><span data-stu-id="bfa13-204">Int32</span></span>|<span data-ttu-id="bfa13-205">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="bfa13-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="bfa13-206">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfa13-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="bfa13-207">committedContentVersion</span></span>|<span data-ttu-id="bfa13-208">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-208">String</span></span>|<span data-ttu-id="bfa13-209">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="bfa13-209">The internal committed content version.</span></span> <span data-ttu-id="bfa13-210">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bfa13-211">fileName</span><span class="sxs-lookup"><span data-stu-id="bfa13-211">fileName</span></span>|<span data-ttu-id="bfa13-212">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-212">String</span></span>|<span data-ttu-id="bfa13-213">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="bfa13-213">The name of the main Lob application file.</span></span> <span data-ttu-id="bfa13-214">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bfa13-215">size</span><span class="sxs-lookup"><span data-stu-id="bfa13-215">size</span></span>|<span data-ttu-id="bfa13-216">Int64</span><span class="sxs-lookup"><span data-stu-id="bfa13-216">Int64</span></span>|<span data-ttu-id="bfa13-217">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="bfa13-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="bfa13-218">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfa13-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bfa13-219">bundleId</span><span class="sxs-lookup"><span data-stu-id="bfa13-219">bundleId</span></span>|<span data-ttu-id="bfa13-220">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-220">String</span></span>|<span data-ttu-id="bfa13-221">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="bfa13-221">The bundle id.</span></span>|
|<span data-ttu-id="bfa13-222">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bfa13-222">minimumSupportedOperatingSystem</span></span>|<span data-ttu-id="bfa13-223">[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md);</span><span class="sxs-lookup"><span data-stu-id="bfa13-223">[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md)</span></span>|<span data-ttu-id="bfa13-224">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="bfa13-224">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="bfa13-225">buildNumber</span><span class="sxs-lookup"><span data-stu-id="bfa13-225">buildNumber</span></span>|<span data-ttu-id="bfa13-226">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-226">String</span></span>|<span data-ttu-id="bfa13-227">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="bfa13-227">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bfa13-228">versionNumber</span><span class="sxs-lookup"><span data-stu-id="bfa13-228">versionNumber</span></span>|<span data-ttu-id="bfa13-229">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-229">String</span></span>|<span data-ttu-id="bfa13-230">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="bfa13-230">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bfa13-231">чилдаппс</span><span class="sxs-lookup"><span data-stu-id="bfa13-231">childApps</span></span>|<span data-ttu-id="bfa13-232">Коллекция [макослобчилдапп](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfa13-232">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="bfa13-233">Список приложений в этом пакете набора</span><span class="sxs-lookup"><span data-stu-id="bfa13-233">The app list in this bundle package</span></span>|
|<span data-ttu-id="bfa13-234">identityVersion</span><span class="sxs-lookup"><span data-stu-id="bfa13-234">identityVersion</span></span>|<span data-ttu-id="bfa13-235">String</span><span class="sxs-lookup"><span data-stu-id="bfa13-235">String</span></span>|<span data-ttu-id="bfa13-236">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="bfa13-236">The identity version.</span></span>|
|<span data-ttu-id="bfa13-237">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="bfa13-237">md5HashChunkSize</span></span>|<span data-ttu-id="bfa13-238">Int32</span><span class="sxs-lookup"><span data-stu-id="bfa13-238">Int32</span></span>|<span data-ttu-id="bfa13-239">Размер фрагмента для хеша MD5</span><span class="sxs-lookup"><span data-stu-id="bfa13-239">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="bfa13-240">md5Hash</span><span class="sxs-lookup"><span data-stu-id="bfa13-240">md5Hash</span></span>|<span data-ttu-id="bfa13-241">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bfa13-241">String collection</span></span>|<span data-ttu-id="bfa13-242">Хэш-коды MD5</span><span class="sxs-lookup"><span data-stu-id="bfa13-242">The MD5 hash codes</span></span>|
|<span data-ttu-id="bfa13-243">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="bfa13-243">ignoreVersionDetection</span></span>|<span data-ttu-id="bfa13-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfa13-244">Boolean</span></span>|<span data-ttu-id="bfa13-245">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="bfa13-245">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="bfa13-246">Установите для этого параметра значение true для бизнес-приложений macOS (LoB), использующих функцию самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="bfa13-246">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="bfa13-247">Ответ</span><span class="sxs-lookup"><span data-stu-id="bfa13-247">Response</span></span>
<span data-ttu-id="bfa13-248">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макослобапп](../resources/intune-apps-macoslobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bfa13-248">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfa13-249">Пример</span><span class="sxs-lookup"><span data-stu-id="bfa13-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfa13-250">Запрос</span><span class="sxs-lookup"><span data-stu-id="bfa13-250">Request</span></span>
<span data-ttu-id="bfa13-251">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bfa13-251">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1616

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="bfa13-252">Отклик</span><span class="sxs-lookup"><span data-stu-id="bfa13-252">Response</span></span>
<span data-ttu-id="bfa13-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bfa13-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1788

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```



