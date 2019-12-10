---
title: Обновление windowsAppX
description: Обновление свойств объекта windowsAppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7200699852f912951e52bebba8b8269e3e43978b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39933743"
---
# <a name="update-windowsappx"></a><span data-ttu-id="d8e49-103">Обновление windowsAppX</span><span class="sxs-lookup"><span data-stu-id="d8e49-103">Update windowsAppX</span></span>

> <span data-ttu-id="d8e49-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8e49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8e49-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8e49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8e49-106">Обновление свойств объекта [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="d8e49-106">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8e49-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d8e49-107">Prerequisites</span></span>
<span data-ttu-id="d8e49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8e49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8e49-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8e49-110">Permission type</span></span>|<span data-ttu-id="d8e49-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8e49-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8e49-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8e49-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8e49-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8e49-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8e49-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8e49-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8e49-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8e49-115">Not supported.</span></span>|
|<span data-ttu-id="d8e49-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8e49-116">Application</span></span>|<span data-ttu-id="d8e49-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8e49-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8e49-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8e49-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="d8e49-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d8e49-119">Request headers</span></span>
|<span data-ttu-id="d8e49-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8e49-120">Header</span></span>|<span data-ttu-id="d8e49-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d8e49-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8e49-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8e49-122">Authorization</span></span>|<span data-ttu-id="d8e49-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8e49-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8e49-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d8e49-124">Accept</span></span>|<span data-ttu-id="d8e49-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8e49-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8e49-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8e49-126">Request body</span></span>
<span data-ttu-id="d8e49-127">В тексте запроса добавьте представление объекта [windowsAppX](../resources/intune-apps-windowsappx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8e49-127">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="d8e49-128">В следующей таблице приведены свойства, необходимые при создании [windowsAppX](../resources/intune-apps-windowsappx.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-128">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="d8e49-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8e49-129">Property</span></span>|<span data-ttu-id="d8e49-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d8e49-130">Type</span></span>|<span data-ttu-id="d8e49-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d8e49-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8e49-132">id</span><span class="sxs-lookup"><span data-stu-id="d8e49-132">id</span></span>|<span data-ttu-id="d8e49-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d8e49-133">String</span></span>|<span data-ttu-id="d8e49-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d8e49-134">Key of the entity.</span></span> <span data-ttu-id="d8e49-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d8e49-136">displayName</span></span>|<span data-ttu-id="d8e49-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d8e49-137">String</span></span>|<span data-ttu-id="d8e49-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d8e49-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d8e49-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-140">description</span><span class="sxs-lookup"><span data-stu-id="d8e49-140">description</span></span>|<span data-ttu-id="d8e49-141">Строка</span><span class="sxs-lookup"><span data-stu-id="d8e49-141">String</span></span>|<span data-ttu-id="d8e49-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-142">The description of the app.</span></span> <span data-ttu-id="d8e49-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-144">publisher</span><span class="sxs-lookup"><span data-stu-id="d8e49-144">publisher</span></span>|<span data-ttu-id="d8e49-145">Строка</span><span class="sxs-lookup"><span data-stu-id="d8e49-145">String</span></span>|<span data-ttu-id="d8e49-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-146">The publisher of the app.</span></span> <span data-ttu-id="d8e49-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d8e49-148">largeIcon</span></span>|[<span data-ttu-id="d8e49-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d8e49-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d8e49-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d8e49-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d8e49-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8e49-152">createdDateTime</span></span>|<span data-ttu-id="d8e49-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8e49-153">DateTimeOffset</span></span>|<span data-ttu-id="d8e49-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-154">The date and time the app was created.</span></span> <span data-ttu-id="d8e49-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8e49-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d8e49-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8e49-157">DateTimeOffset</span></span>|<span data-ttu-id="d8e49-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d8e49-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d8e49-160">isFeatured</span></span>|<span data-ttu-id="d8e49-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8e49-161">Boolean</span></span>|<span data-ttu-id="d8e49-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d8e49-163">privacyInformationUrl</span></span>|<span data-ttu-id="d8e49-164">Строка</span><span class="sxs-lookup"><span data-stu-id="d8e49-164">String</span></span>|<span data-ttu-id="d8e49-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d8e49-165">The privacy statement Url.</span></span> <span data-ttu-id="d8e49-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d8e49-167">informationUrl</span></span>|<span data-ttu-id="d8e49-168">Строка</span><span class="sxs-lookup"><span data-stu-id="d8e49-168">String</span></span>|<span data-ttu-id="d8e49-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d8e49-169">The more information Url.</span></span> <span data-ttu-id="d8e49-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-171">owner</span><span class="sxs-lookup"><span data-stu-id="d8e49-171">owner</span></span>|<span data-ttu-id="d8e49-172">String</span><span class="sxs-lookup"><span data-stu-id="d8e49-172">String</span></span>|<span data-ttu-id="d8e49-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-173">The owner of the app.</span></span> <span data-ttu-id="d8e49-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-175">developer</span><span class="sxs-lookup"><span data-stu-id="d8e49-175">developer</span></span>|<span data-ttu-id="d8e49-176">Строка</span><span class="sxs-lookup"><span data-stu-id="d8e49-176">String</span></span>|<span data-ttu-id="d8e49-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-177">The developer of the app.</span></span> <span data-ttu-id="d8e49-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-179">notes</span><span class="sxs-lookup"><span data-stu-id="d8e49-179">notes</span></span>|<span data-ttu-id="d8e49-180">Строка</span><span class="sxs-lookup"><span data-stu-id="d8e49-180">String</span></span>|<span data-ttu-id="d8e49-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-181">Notes for the app.</span></span> <span data-ttu-id="d8e49-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="d8e49-183">uploadState</span></span>|<span data-ttu-id="d8e49-184">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e49-184">Int32</span></span>|<span data-ttu-id="d8e49-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="d8e49-185">The upload state.</span></span> <span data-ttu-id="d8e49-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="d8e49-187">publishingState</span></span>|[<span data-ttu-id="d8e49-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="d8e49-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d8e49-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-189">The publishing state for the app.</span></span> <span data-ttu-id="d8e49-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d8e49-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d8e49-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="d8e49-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d8e49-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d8e49-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d8e49-193">isAssigned</span></span>|<span data-ttu-id="d8e49-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8e49-194">Boolean</span></span>|<span data-ttu-id="d8e49-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="d8e49-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d8e49-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d8e49-197">roleScopeTagIds</span></span>|<span data-ttu-id="d8e49-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d8e49-198">String collection</span></span>|<span data-ttu-id="d8e49-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d8e49-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="d8e49-201">dependentAppCount</span></span>|<span data-ttu-id="d8e49-202">Int32</span><span class="sxs-lookup"><span data-stu-id="d8e49-202">Int32</span></span>|<span data-ttu-id="d8e49-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d8e49-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="d8e49-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d8e49-205">committedContentVersion</span></span>|<span data-ttu-id="d8e49-206">Строка</span><span class="sxs-lookup"><span data-stu-id="d8e49-206">String</span></span>|<span data-ttu-id="d8e49-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="d8e49-207">The internal committed content version.</span></span> <span data-ttu-id="d8e49-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d8e49-209">fileName</span><span class="sxs-lookup"><span data-stu-id="d8e49-209">fileName</span></span>|<span data-ttu-id="d8e49-210">Строка</span><span class="sxs-lookup"><span data-stu-id="d8e49-210">String</span></span>|<span data-ttu-id="d8e49-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-211">The name of the main Lob application file.</span></span> <span data-ttu-id="d8e49-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d8e49-213">size</span><span class="sxs-lookup"><span data-stu-id="d8e49-213">size</span></span>|<span data-ttu-id="d8e49-214">Int64</span><span class="sxs-lookup"><span data-stu-id="d8e49-214">Int64</span></span>|<span data-ttu-id="d8e49-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="d8e49-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="d8e49-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d8e49-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d8e49-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="d8e49-217">applicableArchitectures</span></span>|[<span data-ttu-id="d8e49-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="d8e49-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="d8e49-219">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="d8e49-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="d8e49-220">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="d8e49-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="d8e49-221">identityName</span><span class="sxs-lookup"><span data-stu-id="d8e49-221">identityName</span></span>|<span data-ttu-id="d8e49-222">Строка</span><span class="sxs-lookup"><span data-stu-id="d8e49-222">String</span></span>|<span data-ttu-id="d8e49-223">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-223">The Identity Name.</span></span>|
|<span data-ttu-id="d8e49-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="d8e49-224">identityPublisherHash</span></span>|<span data-ttu-id="d8e49-225">Строка</span><span class="sxs-lookup"><span data-stu-id="d8e49-225">String</span></span>|<span data-ttu-id="d8e49-226">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="d8e49-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="d8e49-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="d8e49-227">identityResourceIdentifier</span></span>|<span data-ttu-id="d8e49-228">String</span><span class="sxs-lookup"><span data-stu-id="d8e49-228">String</span></span>|<span data-ttu-id="d8e49-229">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="d8e49-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="d8e49-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="d8e49-230">isBundle</span></span>|<span data-ttu-id="d8e49-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8e49-231">Boolean</span></span>|<span data-ttu-id="d8e49-232">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="d8e49-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="d8e49-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d8e49-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d8e49-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d8e49-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="d8e49-235">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="d8e49-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d8e49-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="d8e49-236">identityVersion</span></span>|<span data-ttu-id="d8e49-237">String</span><span class="sxs-lookup"><span data-stu-id="d8e49-237">String</span></span>|<span data-ttu-id="d8e49-238">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="d8e49-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="d8e49-239">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8e49-239">Response</span></span>
<span data-ttu-id="d8e49-240">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsAppX](../resources/intune-apps-windowsappx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8e49-240">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8e49-241">Пример</span><span class="sxs-lookup"><span data-stu-id="d8e49-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8e49-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8e49-242">Request</span></span>
<span data-ttu-id="d8e49-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8e49-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="d8e49-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8e49-244">Response</span></span>
<span data-ttu-id="d8e49-p123">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8e49-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1585

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```





