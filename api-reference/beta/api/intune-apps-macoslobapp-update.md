---
title: Обновление Макослобапп
description: Обновление свойств объекта Макослобапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f246f2b743154a9a74c6289670a73124ba23c572
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975296"
---
# <a name="update-macoslobapp"></a><span data-ttu-id="9fedd-103">Обновление Макослобапп</span><span class="sxs-lookup"><span data-stu-id="9fedd-103">Update macOSLobApp</span></span>

> <span data-ttu-id="9fedd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fedd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9fedd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fedd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fedd-106">Обновление свойств объекта [макослобапп](../resources/intune-apps-macoslobapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9fedd-106">Update the properties of a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9fedd-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9fedd-107">Prerequisites</span></span>
<span data-ttu-id="9fedd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fedd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fedd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9fedd-110">Permission type</span></span>|<span data-ttu-id="9fedd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9fedd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fedd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9fedd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9fedd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fedd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9fedd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9fedd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fedd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fedd-115">Not supported.</span></span>|
|<span data-ttu-id="9fedd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9fedd-116">Application</span></span>|<span data-ttu-id="9fedd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9fedd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fedd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9fedd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9fedd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9fedd-119">Request headers</span></span>
|<span data-ttu-id="9fedd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9fedd-120">Header</span></span>|<span data-ttu-id="9fedd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9fedd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fedd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9fedd-122">Authorization</span></span>|<span data-ttu-id="9fedd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9fedd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fedd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9fedd-124">Accept</span></span>|<span data-ttu-id="9fedd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9fedd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fedd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9fedd-126">Request body</span></span>
<span data-ttu-id="9fedd-127">В тексте запроса добавьте представление объекта [макослобапп](../resources/intune-apps-macoslobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fedd-127">In the request body, supply a JSON representation for the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

<span data-ttu-id="9fedd-128">В следующей таблице приведены свойства, необходимые при создании [макослобапп](../resources/intune-apps-macoslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-128">The following table shows the properties that are required when you create the [macOSLobApp](../resources/intune-apps-macoslobapp.md).</span></span>

|<span data-ttu-id="9fedd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fedd-129">Property</span></span>|<span data-ttu-id="9fedd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9fedd-130">Type</span></span>|<span data-ttu-id="9fedd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9fedd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fedd-132">id</span><span class="sxs-lookup"><span data-stu-id="9fedd-132">id</span></span>|<span data-ttu-id="9fedd-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9fedd-133">String</span></span>|<span data-ttu-id="9fedd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9fedd-134">Key of the entity.</span></span> <span data-ttu-id="9fedd-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9fedd-136">displayName</span></span>|<span data-ttu-id="9fedd-137">Строка</span><span class="sxs-lookup"><span data-stu-id="9fedd-137">String</span></span>|<span data-ttu-id="9fedd-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="9fedd-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9fedd-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-140">description</span><span class="sxs-lookup"><span data-stu-id="9fedd-140">description</span></span>|<span data-ttu-id="9fedd-141">Строка</span><span class="sxs-lookup"><span data-stu-id="9fedd-141">String</span></span>|<span data-ttu-id="9fedd-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="9fedd-142">The description of the app.</span></span> <span data-ttu-id="9fedd-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9fedd-144">publisher</span></span>|<span data-ttu-id="9fedd-145">String</span><span class="sxs-lookup"><span data-stu-id="9fedd-145">String</span></span>|<span data-ttu-id="9fedd-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="9fedd-146">The publisher of the app.</span></span> <span data-ttu-id="9fedd-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9fedd-148">largeIcon</span></span>|[<span data-ttu-id="9fedd-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9fedd-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9fedd-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="9fedd-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9fedd-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9fedd-152">createdDateTime</span></span>|<span data-ttu-id="9fedd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fedd-153">DateTimeOffset</span></span>|<span data-ttu-id="9fedd-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="9fedd-154">The date and time the app was created.</span></span> <span data-ttu-id="9fedd-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fedd-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9fedd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fedd-157">DateTimeOffset</span></span>|<span data-ttu-id="9fedd-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="9fedd-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9fedd-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9fedd-160">isFeatured</span></span>|<span data-ttu-id="9fedd-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fedd-161">Boolean</span></span>|<span data-ttu-id="9fedd-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9fedd-163">privacyInformationUrl</span></span>|<span data-ttu-id="9fedd-164">String</span><span class="sxs-lookup"><span data-stu-id="9fedd-164">String</span></span>|<span data-ttu-id="9fedd-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="9fedd-165">The privacy statement Url.</span></span> <span data-ttu-id="9fedd-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9fedd-167">informationUrl</span></span>|<span data-ttu-id="9fedd-168">String</span><span class="sxs-lookup"><span data-stu-id="9fedd-168">String</span></span>|<span data-ttu-id="9fedd-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="9fedd-169">The more information Url.</span></span> <span data-ttu-id="9fedd-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-171">owner</span><span class="sxs-lookup"><span data-stu-id="9fedd-171">owner</span></span>|<span data-ttu-id="9fedd-172">String</span><span class="sxs-lookup"><span data-stu-id="9fedd-172">String</span></span>|<span data-ttu-id="9fedd-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="9fedd-173">The owner of the app.</span></span> <span data-ttu-id="9fedd-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-175">developer</span><span class="sxs-lookup"><span data-stu-id="9fedd-175">developer</span></span>|<span data-ttu-id="9fedd-176">String</span><span class="sxs-lookup"><span data-stu-id="9fedd-176">String</span></span>|<span data-ttu-id="9fedd-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="9fedd-177">The developer of the app.</span></span> <span data-ttu-id="9fedd-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-179">notes</span><span class="sxs-lookup"><span data-stu-id="9fedd-179">notes</span></span>|<span data-ttu-id="9fedd-180">String</span><span class="sxs-lookup"><span data-stu-id="9fedd-180">String</span></span>|<span data-ttu-id="9fedd-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="9fedd-181">Notes for the app.</span></span> <span data-ttu-id="9fedd-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9fedd-183">uploadState</span></span>|<span data-ttu-id="9fedd-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9fedd-184">Int32</span></span>|<span data-ttu-id="9fedd-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="9fedd-185">The upload state.</span></span> <span data-ttu-id="9fedd-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9fedd-187">publishingState</span></span>|[<span data-ttu-id="9fedd-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="9fedd-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9fedd-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="9fedd-189">The publishing state for the app.</span></span> <span data-ttu-id="9fedd-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="9fedd-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9fedd-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9fedd-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9fedd-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9fedd-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9fedd-193">isAssigned</span></span>|<span data-ttu-id="9fedd-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fedd-194">Boolean</span></span>|<span data-ttu-id="9fedd-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="9fedd-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9fedd-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9fedd-197">roleScopeTagIds</span></span>|<span data-ttu-id="9fedd-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9fedd-198">String collection</span></span>|<span data-ttu-id="9fedd-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9fedd-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9fedd-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="9fedd-201">dependentAppCount</span></span>|<span data-ttu-id="9fedd-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9fedd-202">Int32</span></span>|<span data-ttu-id="9fedd-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="9fedd-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9fedd-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9fedd-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9fedd-205">committedContentVersion</span></span>|<span data-ttu-id="9fedd-206">String</span><span class="sxs-lookup"><span data-stu-id="9fedd-206">String</span></span>|<span data-ttu-id="9fedd-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="9fedd-207">The internal committed content version.</span></span> <span data-ttu-id="9fedd-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9fedd-209">fileName</span><span class="sxs-lookup"><span data-stu-id="9fedd-209">fileName</span></span>|<span data-ttu-id="9fedd-210">String</span><span class="sxs-lookup"><span data-stu-id="9fedd-210">String</span></span>|<span data-ttu-id="9fedd-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="9fedd-211">The name of the main Lob application file.</span></span> <span data-ttu-id="9fedd-212">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9fedd-213">size</span><span class="sxs-lookup"><span data-stu-id="9fedd-213">size</span></span>|<span data-ttu-id="9fedd-214">Int64</span><span class="sxs-lookup"><span data-stu-id="9fedd-214">Int64</span></span>|<span data-ttu-id="9fedd-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="9fedd-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="9fedd-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9fedd-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9fedd-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="9fedd-217">bundleId</span></span>|<span data-ttu-id="9fedd-218">String</span><span class="sxs-lookup"><span data-stu-id="9fedd-218">String</span></span>|<span data-ttu-id="9fedd-219">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="9fedd-219">The bundle id.</span></span>|
|<span data-ttu-id="9fedd-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9fedd-220">minimumSupportedOperatingSystem</span></span>|<span data-ttu-id="9fedd-221">[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md);</span><span class="sxs-lookup"><span data-stu-id="9fedd-221">[macOSMinimumOperatingSystem](../resources/intune-apps-macosminimumoperatingsystem.md)</span></span>|<span data-ttu-id="9fedd-222">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="9fedd-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9fedd-223">buildNumber</span><span class="sxs-lookup"><span data-stu-id="9fedd-223">buildNumber</span></span>|<span data-ttu-id="9fedd-224">String</span><span class="sxs-lookup"><span data-stu-id="9fedd-224">String</span></span>|<span data-ttu-id="9fedd-225">Номер сборки бизнес-приложения MacOS бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="9fedd-225">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9fedd-226">versionNumber</span><span class="sxs-lookup"><span data-stu-id="9fedd-226">versionNumber</span></span>|<span data-ttu-id="9fedd-227">String</span><span class="sxs-lookup"><span data-stu-id="9fedd-227">String</span></span>|<span data-ttu-id="9fedd-228">Номер версии приложения MacOS для бизнеса (LoB).</span><span class="sxs-lookup"><span data-stu-id="9fedd-228">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9fedd-229">Чилдаппс</span><span class="sxs-lookup"><span data-stu-id="9fedd-229">childApps</span></span>|<span data-ttu-id="9fedd-230">Коллекция [макослобчилдапп](../resources/intune-apps-macoslobchildapp.md)</span><span class="sxs-lookup"><span data-stu-id="9fedd-230">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="9fedd-231">Список приложений в этом пакете набора</span><span class="sxs-lookup"><span data-stu-id="9fedd-231">The app list in this bundle package</span></span>|
|<span data-ttu-id="9fedd-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9fedd-232">identityVersion</span></span>|<span data-ttu-id="9fedd-233">String</span><span class="sxs-lookup"><span data-stu-id="9fedd-233">String</span></span>|<span data-ttu-id="9fedd-234">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="9fedd-234">The identity version.</span></span>|
|<span data-ttu-id="9fedd-235">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="9fedd-235">md5HashChunkSize</span></span>|<span data-ttu-id="9fedd-236">Int32</span><span class="sxs-lookup"><span data-stu-id="9fedd-236">Int32</span></span>|<span data-ttu-id="9fedd-237">Размер фрагмента для хеша MD5</span><span class="sxs-lookup"><span data-stu-id="9fedd-237">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="9fedd-238">md5Hash</span><span class="sxs-lookup"><span data-stu-id="9fedd-238">md5Hash</span></span>|<span data-ttu-id="9fedd-239">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9fedd-239">String collection</span></span>|<span data-ttu-id="9fedd-240">Хэш-коды MD5</span><span class="sxs-lookup"><span data-stu-id="9fedd-240">The MD5 hash codes</span></span>|
|<span data-ttu-id="9fedd-241">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="9fedd-241">ignoreVersionDetection</span></span>|<span data-ttu-id="9fedd-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fedd-242">Boolean</span></span>|<span data-ttu-id="9fedd-243">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="9fedd-243">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="9fedd-244">Установите для этого параметра значение true для бизнес-приложений macOS (LoB), использующих функцию самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="9fedd-244">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="9fedd-245">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fedd-245">Response</span></span>
<span data-ttu-id="9fedd-246">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макослобапп](../resources/intune-apps-macoslobapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9fedd-246">If successful, this method returns a `200 OK` response code and an updated [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fedd-247">Пример</span><span class="sxs-lookup"><span data-stu-id="9fedd-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="9fedd-248">Запрос</span><span class="sxs-lookup"><span data-stu-id="9fedd-248">Request</span></span>
<span data-ttu-id="9fedd-249">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9fedd-249">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1574

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
    "v10_13": true
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

### <a name="response"></a><span data-ttu-id="9fedd-250">Отклик</span><span class="sxs-lookup"><span data-stu-id="9fedd-250">Response</span></span>
<span data-ttu-id="9fedd-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9fedd-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1746

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
    "v10_13": true
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





