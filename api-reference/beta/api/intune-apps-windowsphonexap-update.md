---
title: Обновление Виндовсфонексап
description: Обновление свойств объекта Виндовсфонексап.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b0d4b9a101d67409d967999c5f4c956f906e5ca
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760720"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="797f8-103">Обновление Виндовсфонексап</span><span class="sxs-lookup"><span data-stu-id="797f8-103">Update windowsPhoneXAP</span></span>

> <span data-ttu-id="797f8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="797f8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="797f8-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="797f8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="797f8-106">Обновление свойств объекта [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="797f8-106">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="797f8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="797f8-107">Prerequisites</span></span>
<span data-ttu-id="797f8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="797f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="797f8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="797f8-110">Permission type</span></span>|<span data-ttu-id="797f8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="797f8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="797f8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="797f8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="797f8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="797f8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="797f8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="797f8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="797f8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="797f8-115">Not supported.</span></span>|
|<span data-ttu-id="797f8-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="797f8-116">Application</span></span>|<span data-ttu-id="797f8-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="797f8-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="797f8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="797f8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="797f8-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="797f8-119">Request headers</span></span>
|<span data-ttu-id="797f8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="797f8-120">Header</span></span>|<span data-ttu-id="797f8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="797f8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="797f8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="797f8-122">Authorization</span></span>|<span data-ttu-id="797f8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="797f8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="797f8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="797f8-124">Accept</span></span>|<span data-ttu-id="797f8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="797f8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="797f8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="797f8-126">Request body</span></span>
<span data-ttu-id="797f8-127">В тексте запроса добавьте представление объекта [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="797f8-127">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="797f8-128">В следующей таблице приведены свойства, необходимые при создании [виндовсфонексап](../resources/intune-apps-windowsphonexap.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-128">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="797f8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="797f8-129">Property</span></span>|<span data-ttu-id="797f8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="797f8-130">Type</span></span>|<span data-ttu-id="797f8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="797f8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="797f8-132">id</span><span class="sxs-lookup"><span data-stu-id="797f8-132">id</span></span>|<span data-ttu-id="797f8-133">Строка</span><span class="sxs-lookup"><span data-stu-id="797f8-133">String</span></span>|<span data-ttu-id="797f8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="797f8-134">Key of the entity.</span></span> <span data-ttu-id="797f8-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="797f8-136">displayName</span></span>|<span data-ttu-id="797f8-137">Строка</span><span class="sxs-lookup"><span data-stu-id="797f8-137">String</span></span>|<span data-ttu-id="797f8-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="797f8-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="797f8-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-140">description</span><span class="sxs-lookup"><span data-stu-id="797f8-140">description</span></span>|<span data-ttu-id="797f8-141">Строка</span><span class="sxs-lookup"><span data-stu-id="797f8-141">String</span></span>|<span data-ttu-id="797f8-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="797f8-142">The description of the app.</span></span> <span data-ttu-id="797f8-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-144">publisher</span><span class="sxs-lookup"><span data-stu-id="797f8-144">publisher</span></span>|<span data-ttu-id="797f8-145">String</span><span class="sxs-lookup"><span data-stu-id="797f8-145">String</span></span>|<span data-ttu-id="797f8-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="797f8-146">The publisher of the app.</span></span> <span data-ttu-id="797f8-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="797f8-148">largeIcon</span></span>|[<span data-ttu-id="797f8-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="797f8-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="797f8-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="797f8-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="797f8-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="797f8-152">createdDateTime</span></span>|<span data-ttu-id="797f8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="797f8-153">DateTimeOffset</span></span>|<span data-ttu-id="797f8-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="797f8-154">The date and time the app was created.</span></span> <span data-ttu-id="797f8-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="797f8-156">lastModifiedDateTime</span></span>|<span data-ttu-id="797f8-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="797f8-157">DateTimeOffset</span></span>|<span data-ttu-id="797f8-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="797f8-158">The date and time the app was last modified.</span></span> <span data-ttu-id="797f8-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="797f8-160">isFeatured</span></span>|<span data-ttu-id="797f8-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="797f8-161">Boolean</span></span>|<span data-ttu-id="797f8-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="797f8-163">privacyInformationUrl</span></span>|<span data-ttu-id="797f8-164">String</span><span class="sxs-lookup"><span data-stu-id="797f8-164">String</span></span>|<span data-ttu-id="797f8-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="797f8-165">The privacy statement Url.</span></span> <span data-ttu-id="797f8-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="797f8-167">informationUrl</span></span>|<span data-ttu-id="797f8-168">String</span><span class="sxs-lookup"><span data-stu-id="797f8-168">String</span></span>|<span data-ttu-id="797f8-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="797f8-169">The more information Url.</span></span> <span data-ttu-id="797f8-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-171">owner</span><span class="sxs-lookup"><span data-stu-id="797f8-171">owner</span></span>|<span data-ttu-id="797f8-172">String</span><span class="sxs-lookup"><span data-stu-id="797f8-172">String</span></span>|<span data-ttu-id="797f8-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="797f8-173">The owner of the app.</span></span> <span data-ttu-id="797f8-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-175">developer</span><span class="sxs-lookup"><span data-stu-id="797f8-175">developer</span></span>|<span data-ttu-id="797f8-176">String</span><span class="sxs-lookup"><span data-stu-id="797f8-176">String</span></span>|<span data-ttu-id="797f8-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="797f8-177">The developer of the app.</span></span> <span data-ttu-id="797f8-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-179">notes</span><span class="sxs-lookup"><span data-stu-id="797f8-179">notes</span></span>|<span data-ttu-id="797f8-180">String</span><span class="sxs-lookup"><span data-stu-id="797f8-180">String</span></span>|<span data-ttu-id="797f8-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="797f8-181">Notes for the app.</span></span> <span data-ttu-id="797f8-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="797f8-183">uploadState</span></span>|<span data-ttu-id="797f8-184">Int32</span><span class="sxs-lookup"><span data-stu-id="797f8-184">Int32</span></span>|<span data-ttu-id="797f8-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="797f8-185">The upload state.</span></span> <span data-ttu-id="797f8-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="797f8-187">publishingState</span></span>|[<span data-ttu-id="797f8-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="797f8-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="797f8-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="797f8-189">The publishing state for the app.</span></span> <span data-ttu-id="797f8-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="797f8-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="797f8-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="797f8-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="797f8-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="797f8-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="797f8-193">isAssigned</span></span>|<span data-ttu-id="797f8-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="797f8-194">Boolean</span></span>|<span data-ttu-id="797f8-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="797f8-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="797f8-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="797f8-197">roleScopeTagIds</span></span>|<span data-ttu-id="797f8-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="797f8-198">String collection</span></span>|<span data-ttu-id="797f8-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="797f8-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="797f8-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="797f8-201">dependentAppCount</span></span>|<span data-ttu-id="797f8-202">Int32</span><span class="sxs-lookup"><span data-stu-id="797f8-202">Int32</span></span>|<span data-ttu-id="797f8-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="797f8-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="797f8-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="797f8-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="797f8-205">committedContentVersion</span></span>|<span data-ttu-id="797f8-206">String</span><span class="sxs-lookup"><span data-stu-id="797f8-206">String</span></span>|<span data-ttu-id="797f8-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="797f8-207">The internal committed content version.</span></span> <span data-ttu-id="797f8-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="797f8-209">fileName</span><span class="sxs-lookup"><span data-stu-id="797f8-209">fileName</span></span>|<span data-ttu-id="797f8-210">String</span><span class="sxs-lookup"><span data-stu-id="797f8-210">String</span></span>|<span data-ttu-id="797f8-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="797f8-211">The name of the main Lob application file.</span></span> <span data-ttu-id="797f8-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="797f8-213">size</span><span class="sxs-lookup"><span data-stu-id="797f8-213">size</span></span>|<span data-ttu-id="797f8-214">Int64</span><span class="sxs-lookup"><span data-stu-id="797f8-214">Int64</span></span>|<span data-ttu-id="797f8-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="797f8-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="797f8-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="797f8-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="797f8-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="797f8-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="797f8-218">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="797f8-218">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="797f8-219">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="797f8-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="797f8-220">продуктидентифиер</span><span class="sxs-lookup"><span data-stu-id="797f8-220">productIdentifier</span></span>|<span data-ttu-id="797f8-221">String</span><span class="sxs-lookup"><span data-stu-id="797f8-221">String</span></span>|<span data-ttu-id="797f8-222">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="797f8-222">The Product Identifier.</span></span>|
|<span data-ttu-id="797f8-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="797f8-223">identityVersion</span></span>|<span data-ttu-id="797f8-224">String</span><span class="sxs-lookup"><span data-stu-id="797f8-224">String</span></span>|<span data-ttu-id="797f8-225">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="797f8-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="797f8-226">Ответ</span><span class="sxs-lookup"><span data-stu-id="797f8-226">Response</span></span>
<span data-ttu-id="797f8-227">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсфонексап](../resources/intune-apps-windowsphonexap.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="797f8-227">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="797f8-228">Пример</span><span class="sxs-lookup"><span data-stu-id="797f8-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="797f8-229">Запрос</span><span class="sxs-lookup"><span data-stu-id="797f8-229">Request</span></span>
<span data-ttu-id="797f8-230">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="797f8-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1237

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="797f8-231">Отклик</span><span class="sxs-lookup"><span data-stu-id="797f8-231">Response</span></span>
<span data-ttu-id="797f8-p122">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="797f8-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1409

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```




