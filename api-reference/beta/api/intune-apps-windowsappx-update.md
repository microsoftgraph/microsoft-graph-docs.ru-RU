---
title: Обновление windowsAppX
description: Обновление свойств объекта windowsAppX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9e70fd7a35d60ef2a210bd8c1ed6158ecc294553
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37171990"
---
# <a name="update-windowsappx"></a><span data-ttu-id="20780-103">Обновление windowsAppX</span><span class="sxs-lookup"><span data-stu-id="20780-103">Update windowsAppX</span></span>

> <span data-ttu-id="20780-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20780-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20780-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20780-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20780-106">Обновление свойств объекта [windowsAppX](../resources/intune-apps-windowsappx.md) .</span><span class="sxs-lookup"><span data-stu-id="20780-106">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20780-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="20780-107">Prerequisites</span></span>
<span data-ttu-id="20780-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20780-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20780-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20780-110">Permission type</span></span>|<span data-ttu-id="20780-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20780-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20780-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20780-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20780-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20780-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="20780-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20780-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20780-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20780-115">Not supported.</span></span>|
|<span data-ttu-id="20780-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20780-116">Application</span></span>|<span data-ttu-id="20780-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20780-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20780-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20780-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="20780-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20780-119">Request headers</span></span>
|<span data-ttu-id="20780-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20780-120">Header</span></span>|<span data-ttu-id="20780-121">Значение</span><span class="sxs-lookup"><span data-stu-id="20780-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20780-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20780-122">Authorization</span></span>|<span data-ttu-id="20780-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20780-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20780-124">Accept</span><span class="sxs-lookup"><span data-stu-id="20780-124">Accept</span></span>|<span data-ttu-id="20780-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20780-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20780-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="20780-126">Request body</span></span>
<span data-ttu-id="20780-127">В тексте запроса добавьте представление объекта [windowsAppX](../resources/intune-apps-windowsappx.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20780-127">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="20780-128">В следующей таблице приведены свойства, необходимые при создании [windowsAppX](../resources/intune-apps-windowsappx.md).</span><span class="sxs-lookup"><span data-stu-id="20780-128">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="20780-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="20780-129">Property</span></span>|<span data-ttu-id="20780-130">Тип</span><span class="sxs-lookup"><span data-stu-id="20780-130">Type</span></span>|<span data-ttu-id="20780-131">Описание</span><span class="sxs-lookup"><span data-stu-id="20780-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20780-132">id</span><span class="sxs-lookup"><span data-stu-id="20780-132">id</span></span>|<span data-ttu-id="20780-133">Строка</span><span class="sxs-lookup"><span data-stu-id="20780-133">String</span></span>|<span data-ttu-id="20780-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="20780-134">Key of the entity.</span></span> <span data-ttu-id="20780-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-136">displayName</span><span class="sxs-lookup"><span data-stu-id="20780-136">displayName</span></span>|<span data-ttu-id="20780-137">Строка</span><span class="sxs-lookup"><span data-stu-id="20780-137">String</span></span>|<span data-ttu-id="20780-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="20780-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="20780-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-140">description</span><span class="sxs-lookup"><span data-stu-id="20780-140">description</span></span>|<span data-ttu-id="20780-141">Строка</span><span class="sxs-lookup"><span data-stu-id="20780-141">String</span></span>|<span data-ttu-id="20780-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="20780-142">The description of the app.</span></span> <span data-ttu-id="20780-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-144">publisher</span><span class="sxs-lookup"><span data-stu-id="20780-144">publisher</span></span>|<span data-ttu-id="20780-145">String.</span><span class="sxs-lookup"><span data-stu-id="20780-145">String</span></span>|<span data-ttu-id="20780-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="20780-146">The publisher of the app.</span></span> <span data-ttu-id="20780-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="20780-148">largeIcon</span></span>|[<span data-ttu-id="20780-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="20780-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="20780-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="20780-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="20780-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20780-152">createdDateTime</span></span>|<span data-ttu-id="20780-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20780-153">DateTimeOffset</span></span>|<span data-ttu-id="20780-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="20780-154">The date and time the app was created.</span></span> <span data-ttu-id="20780-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20780-156">lastModifiedDateTime</span></span>|<span data-ttu-id="20780-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20780-157">DateTimeOffset</span></span>|<span data-ttu-id="20780-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="20780-158">The date and time the app was last modified.</span></span> <span data-ttu-id="20780-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="20780-160">isFeatured</span></span>|<span data-ttu-id="20780-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="20780-161">Boolean</span></span>|<span data-ttu-id="20780-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="20780-163">privacyInformationUrl</span></span>|<span data-ttu-id="20780-164">String.</span><span class="sxs-lookup"><span data-stu-id="20780-164">String</span></span>|<span data-ttu-id="20780-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="20780-165">The privacy statement Url.</span></span> <span data-ttu-id="20780-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="20780-167">informationUrl</span></span>|<span data-ttu-id="20780-168">String.</span><span class="sxs-lookup"><span data-stu-id="20780-168">String</span></span>|<span data-ttu-id="20780-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="20780-169">The more information Url.</span></span> <span data-ttu-id="20780-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-171">owner</span><span class="sxs-lookup"><span data-stu-id="20780-171">owner</span></span>|<span data-ttu-id="20780-172">String</span><span class="sxs-lookup"><span data-stu-id="20780-172">String</span></span>|<span data-ttu-id="20780-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="20780-173">The owner of the app.</span></span> <span data-ttu-id="20780-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-175">developer</span><span class="sxs-lookup"><span data-stu-id="20780-175">developer</span></span>|<span data-ttu-id="20780-176">String.</span><span class="sxs-lookup"><span data-stu-id="20780-176">String</span></span>|<span data-ttu-id="20780-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="20780-177">The developer of the app.</span></span> <span data-ttu-id="20780-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-179">notes</span><span class="sxs-lookup"><span data-stu-id="20780-179">notes</span></span>|<span data-ttu-id="20780-180">String.</span><span class="sxs-lookup"><span data-stu-id="20780-180">String</span></span>|<span data-ttu-id="20780-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="20780-181">Notes for the app.</span></span> <span data-ttu-id="20780-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="20780-183">uploadState</span></span>|<span data-ttu-id="20780-184">Int32</span><span class="sxs-lookup"><span data-stu-id="20780-184">Int32</span></span>|<span data-ttu-id="20780-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="20780-185">The upload state.</span></span> <span data-ttu-id="20780-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="20780-187">publishingState</span></span>|[<span data-ttu-id="20780-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="20780-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="20780-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="20780-189">The publishing state for the app.</span></span> <span data-ttu-id="20780-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="20780-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="20780-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="20780-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="20780-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="20780-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="20780-193">isAssigned</span></span>|<span data-ttu-id="20780-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="20780-194">Boolean</span></span>|<span data-ttu-id="20780-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="20780-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="20780-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20780-197">roleScopeTagIds</span></span>|<span data-ttu-id="20780-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="20780-198">String collection</span></span>|<span data-ttu-id="20780-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="20780-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="20780-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="20780-201">dependentAppCount</span></span>|<span data-ttu-id="20780-202">Int32</span><span class="sxs-lookup"><span data-stu-id="20780-202">Int32</span></span>|<span data-ttu-id="20780-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="20780-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="20780-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="20780-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="20780-205">committedContentVersion</span></span>|<span data-ttu-id="20780-206">String.</span><span class="sxs-lookup"><span data-stu-id="20780-206">String</span></span>|<span data-ttu-id="20780-207">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="20780-207">The internal committed content version.</span></span> <span data-ttu-id="20780-208">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="20780-209">fileName</span><span class="sxs-lookup"><span data-stu-id="20780-209">fileName</span></span>|<span data-ttu-id="20780-210">String.</span><span class="sxs-lookup"><span data-stu-id="20780-210">String</span></span>|<span data-ttu-id="20780-211">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="20780-211">The name of the main Lob application file.</span></span> <span data-ttu-id="20780-212">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="20780-213">size</span><span class="sxs-lookup"><span data-stu-id="20780-213">size</span></span>|<span data-ttu-id="20780-214">Int64</span><span class="sxs-lookup"><span data-stu-id="20780-214">Int64</span></span>|<span data-ttu-id="20780-215">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="20780-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="20780-216">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="20780-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="20780-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="20780-217">applicableArchitectures</span></span>|[<span data-ttu-id="20780-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="20780-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="20780-219">Архитектура Windows, которая поддерживается этим приложением.</span><span class="sxs-lookup"><span data-stu-id="20780-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="20780-220">Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="20780-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="20780-221">identityName</span><span class="sxs-lookup"><span data-stu-id="20780-221">identityName</span></span>|<span data-ttu-id="20780-222">String.</span><span class="sxs-lookup"><span data-stu-id="20780-222">String</span></span>|<span data-ttu-id="20780-223">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="20780-223">The Identity Name.</span></span>|
|<span data-ttu-id="20780-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="20780-224">identityPublisherHash</span></span>|<span data-ttu-id="20780-225">String</span><span class="sxs-lookup"><span data-stu-id="20780-225">String</span></span>|<span data-ttu-id="20780-226">Хэш издателей удостоверений.</span><span class="sxs-lookup"><span data-stu-id="20780-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="20780-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="20780-227">identityResourceIdentifier</span></span>|<span data-ttu-id="20780-228">String.</span><span class="sxs-lookup"><span data-stu-id="20780-228">String</span></span>|<span data-ttu-id="20780-229">Идентификатор ресурса Identity.</span><span class="sxs-lookup"><span data-stu-id="20780-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="20780-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="20780-230">isBundle</span></span>|<span data-ttu-id="20780-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="20780-231">Boolean</span></span>|<span data-ttu-id="20780-232">Указывает, является ли приложение пакетом.</span><span class="sxs-lookup"><span data-stu-id="20780-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="20780-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="20780-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="20780-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="20780-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="20780-235">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="20780-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="20780-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="20780-236">identityVersion</span></span>|<span data-ttu-id="20780-237">String</span><span class="sxs-lookup"><span data-stu-id="20780-237">String</span></span>|<span data-ttu-id="20780-238">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="20780-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="20780-239">Ответ</span><span class="sxs-lookup"><span data-stu-id="20780-239">Response</span></span>
<span data-ttu-id="20780-240">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsAppX](../resources/intune-apps-windowsappx.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20780-240">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20780-241">Пример</span><span class="sxs-lookup"><span data-stu-id="20780-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="20780-242">Запрос</span><span class="sxs-lookup"><span data-stu-id="20780-242">Request</span></span>
<span data-ttu-id="20780-243">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20780-243">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="20780-244">Отклик</span><span class="sxs-lookup"><span data-stu-id="20780-244">Response</span></span>
<span data-ttu-id="20780-p123">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20780-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




