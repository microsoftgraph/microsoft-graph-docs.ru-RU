---
title: Update windowsUniversalAppX
description: Обновление свойств объекта windowsUniversalAppX.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c666beca7d59d3ffab25464fde3b15b2de3b9416
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43393127"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="b20e2-103">Update windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="b20e2-103">Update windowsUniversalAppX</span></span>

<span data-ttu-id="b20e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b20e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b20e2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b20e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b20e2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b20e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b20e2-107">Обновление свойств объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-107">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b20e2-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b20e2-108">Prerequisites</span></span>
<span data-ttu-id="b20e2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b20e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b20e2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b20e2-111">Permission type</span></span>|<span data-ttu-id="b20e2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b20e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b20e2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b20e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b20e2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b20e2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b20e2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b20e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b20e2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b20e2-116">Not supported.</span></span>|
|<span data-ttu-id="b20e2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b20e2-117">Application</span></span>|<span data-ttu-id="b20e2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b20e2-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b20e2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b20e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b20e2-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b20e2-120">Request headers</span></span>
|<span data-ttu-id="b20e2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b20e2-121">Header</span></span>|<span data-ttu-id="b20e2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b20e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b20e2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b20e2-123">Authorization</span></span>|<span data-ttu-id="b20e2-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b20e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b20e2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b20e2-125">Accept</span></span>|<span data-ttu-id="b20e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b20e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b20e2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b20e2-127">Request body</span></span>
<span data-ttu-id="b20e2-128">В теле запроса добавьте представление объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b20e2-128">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="b20e2-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-129">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="b20e2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b20e2-130">Property</span></span>|<span data-ttu-id="b20e2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b20e2-131">Type</span></span>|<span data-ttu-id="b20e2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b20e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b20e2-133">id</span><span class="sxs-lookup"><span data-stu-id="b20e2-133">id</span></span>|<span data-ttu-id="b20e2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b20e2-134">String</span></span>|<span data-ttu-id="b20e2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b20e2-135">Key of the entity.</span></span> <span data-ttu-id="b20e2-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b20e2-137">displayName</span></span>|<span data-ttu-id="b20e2-138">Строка</span><span class="sxs-lookup"><span data-stu-id="b20e2-138">String</span></span>|<span data-ttu-id="b20e2-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b20e2-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b20e2-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-141">description</span><span class="sxs-lookup"><span data-stu-id="b20e2-141">description</span></span>|<span data-ttu-id="b20e2-142">Строка</span><span class="sxs-lookup"><span data-stu-id="b20e2-142">String</span></span>|<span data-ttu-id="b20e2-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-143">The description of the app.</span></span> <span data-ttu-id="b20e2-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-145">publisher</span><span class="sxs-lookup"><span data-stu-id="b20e2-145">publisher</span></span>|<span data-ttu-id="b20e2-146">String</span><span class="sxs-lookup"><span data-stu-id="b20e2-146">String</span></span>|<span data-ttu-id="b20e2-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-147">The publisher of the app.</span></span> <span data-ttu-id="b20e2-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b20e2-149">largeIcon</span></span>|[<span data-ttu-id="b20e2-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b20e2-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b20e2-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b20e2-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b20e2-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b20e2-153">createdDateTime</span></span>|<span data-ttu-id="b20e2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b20e2-154">DateTimeOffset</span></span>|<span data-ttu-id="b20e2-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-155">The date and time the app was created.</span></span> <span data-ttu-id="b20e2-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b20e2-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b20e2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b20e2-158">DateTimeOffset</span></span>|<span data-ttu-id="b20e2-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b20e2-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b20e2-161">isFeatured</span></span>|<span data-ttu-id="b20e2-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b20e2-162">Boolean</span></span>|<span data-ttu-id="b20e2-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b20e2-164">privacyInformationUrl</span></span>|<span data-ttu-id="b20e2-165">String</span><span class="sxs-lookup"><span data-stu-id="b20e2-165">String</span></span>|<span data-ttu-id="b20e2-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b20e2-166">The privacy statement Url.</span></span> <span data-ttu-id="b20e2-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b20e2-168">informationUrl</span></span>|<span data-ttu-id="b20e2-169">String</span><span class="sxs-lookup"><span data-stu-id="b20e2-169">String</span></span>|<span data-ttu-id="b20e2-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b20e2-170">The more information Url.</span></span> <span data-ttu-id="b20e2-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-172">owner</span><span class="sxs-lookup"><span data-stu-id="b20e2-172">owner</span></span>|<span data-ttu-id="b20e2-173">String</span><span class="sxs-lookup"><span data-stu-id="b20e2-173">String</span></span>|<span data-ttu-id="b20e2-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-174">The owner of the app.</span></span> <span data-ttu-id="b20e2-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-176">developer</span><span class="sxs-lookup"><span data-stu-id="b20e2-176">developer</span></span>|<span data-ttu-id="b20e2-177">String</span><span class="sxs-lookup"><span data-stu-id="b20e2-177">String</span></span>|<span data-ttu-id="b20e2-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-178">The developer of the app.</span></span> <span data-ttu-id="b20e2-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-180">notes</span><span class="sxs-lookup"><span data-stu-id="b20e2-180">notes</span></span>|<span data-ttu-id="b20e2-181">String</span><span class="sxs-lookup"><span data-stu-id="b20e2-181">String</span></span>|<span data-ttu-id="b20e2-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-182">Notes for the app.</span></span> <span data-ttu-id="b20e2-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b20e2-184">uploadState</span></span>|<span data-ttu-id="b20e2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b20e2-185">Int32</span></span>|<span data-ttu-id="b20e2-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="b20e2-186">The upload state.</span></span> <span data-ttu-id="b20e2-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="b20e2-188">publishingState</span></span>|[<span data-ttu-id="b20e2-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="b20e2-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b20e2-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-190">The publishing state for the app.</span></span> <span data-ttu-id="b20e2-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b20e2-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b20e2-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="b20e2-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b20e2-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b20e2-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b20e2-194">isAssigned</span></span>|<span data-ttu-id="b20e2-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b20e2-195">Boolean</span></span>|<span data-ttu-id="b20e2-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="b20e2-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b20e2-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b20e2-198">roleScopeTagIds</span></span>|<span data-ttu-id="b20e2-199">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="b20e2-199">String collection</span></span>|<span data-ttu-id="b20e2-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b20e2-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="b20e2-202">dependentAppCount</span></span>|<span data-ttu-id="b20e2-203">Int32</span><span class="sxs-lookup"><span data-stu-id="b20e2-203">Int32</span></span>|<span data-ttu-id="b20e2-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b20e2-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b20e2-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b20e2-206">committedContentVersion</span></span>|<span data-ttu-id="b20e2-207">String</span><span class="sxs-lookup"><span data-stu-id="b20e2-207">String</span></span>|<span data-ttu-id="b20e2-208">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="b20e2-208">The internal committed content version.</span></span> <span data-ttu-id="b20e2-209">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b20e2-210">fileName</span><span class="sxs-lookup"><span data-stu-id="b20e2-210">fileName</span></span>|<span data-ttu-id="b20e2-211">String</span><span class="sxs-lookup"><span data-stu-id="b20e2-211">String</span></span>|<span data-ttu-id="b20e2-212">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-212">The name of the main Lob application file.</span></span> <span data-ttu-id="b20e2-213">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b20e2-214">size</span><span class="sxs-lookup"><span data-stu-id="b20e2-214">size</span></span>|<span data-ttu-id="b20e2-215">Int64</span><span class="sxs-lookup"><span data-stu-id="b20e2-215">Int64</span></span>|<span data-ttu-id="b20e2-216">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="b20e2-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="b20e2-217">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="b20e2-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b20e2-218">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="b20e2-218">applicableArchitectures</span></span>|[<span data-ttu-id="b20e2-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b20e2-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b20e2-220">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="b20e2-220">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="b20e2-221">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="b20e2-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b20e2-222">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="b20e2-222">applicableDeviceTypes</span></span>|[<span data-ttu-id="b20e2-223">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="b20e2-223">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="b20e2-224">Типы устройств с Windows, которые поддерживаются этим приложением.</span><span class="sxs-lookup"><span data-stu-id="b20e2-224">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="b20e2-225">Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="b20e2-225">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="b20e2-226">identityName</span><span class="sxs-lookup"><span data-stu-id="b20e2-226">identityName</span></span>|<span data-ttu-id="b20e2-227">String</span><span class="sxs-lookup"><span data-stu-id="b20e2-227">String</span></span>|<span data-ttu-id="b20e2-228">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-228">The Identity Name.</span></span>|
|<span data-ttu-id="b20e2-229">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="b20e2-229">identityPublisherHash</span></span>|<span data-ttu-id="b20e2-230">String</span><span class="sxs-lookup"><span data-stu-id="b20e2-230">String</span></span>|<span data-ttu-id="b20e2-231">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="b20e2-231">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="b20e2-232">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b20e2-232">identityResourceIdentifier</span></span>|<span data-ttu-id="b20e2-233">String</span><span class="sxs-lookup"><span data-stu-id="b20e2-233">String</span></span>|<span data-ttu-id="b20e2-234">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="b20e2-234">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="b20e2-235">isBundle</span><span class="sxs-lookup"><span data-stu-id="b20e2-235">isBundle</span></span>|<span data-ttu-id="b20e2-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="b20e2-236">Boolean</span></span>|<span data-ttu-id="b20e2-237">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="b20e2-237">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="b20e2-238">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b20e2-238">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b20e2-239">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b20e2-239">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="b20e2-240">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="b20e2-240">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b20e2-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b20e2-241">identityVersion</span></span>|<span data-ttu-id="b20e2-242">String</span><span class="sxs-lookup"><span data-stu-id="b20e2-242">String</span></span>|<span data-ttu-id="b20e2-243">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="b20e2-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="b20e2-244">Ответ</span><span class="sxs-lookup"><span data-stu-id="b20e2-244">Response</span></span>
<span data-ttu-id="b20e2-245">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b20e2-245">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b20e2-246">Пример</span><span class="sxs-lookup"><span data-stu-id="b20e2-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="b20e2-247">Запрос</span><span class="sxs-lookup"><span data-stu-id="b20e2-247">Request</span></span>
<span data-ttu-id="b20e2-248">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b20e2-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableDeviceTypes": "desktop",
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

### <a name="response"></a><span data-ttu-id="b20e2-249">Отклик</span><span class="sxs-lookup"><span data-stu-id="b20e2-249">Response</span></span>
<span data-ttu-id="b20e2-p124">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b20e2-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableDeviceTypes": "desktop",
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



