---
title: Update webApp
description: Обновление свойств объекта webApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c1fb65ad13c1019ad33f87b125b4797ebc4730f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39934093"
---
# <a name="update-webapp"></a><span data-ttu-id="b1a39-103">Update webApp</span><span class="sxs-lookup"><span data-stu-id="b1a39-103">Update webApp</span></span>

> <span data-ttu-id="b1a39-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1a39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1a39-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1a39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1a39-106">Обновление свойств объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-106">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1a39-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b1a39-107">Prerequisites</span></span>
<span data-ttu-id="b1a39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1a39-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1a39-110">Permission type</span></span>|<span data-ttu-id="b1a39-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1a39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1a39-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1a39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1a39-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1a39-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b1a39-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1a39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1a39-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1a39-115">Not supported.</span></span>|
|<span data-ttu-id="b1a39-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1a39-116">Application</span></span>|<span data-ttu-id="b1a39-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1a39-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1a39-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1a39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b1a39-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b1a39-119">Request headers</span></span>
|<span data-ttu-id="b1a39-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1a39-120">Header</span></span>|<span data-ttu-id="b1a39-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b1a39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1a39-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1a39-122">Authorization</span></span>|<span data-ttu-id="b1a39-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1a39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1a39-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b1a39-124">Accept</span></span>|<span data-ttu-id="b1a39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1a39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1a39-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b1a39-126">Request body</span></span>
<span data-ttu-id="b1a39-127">В тексте запроса добавьте представление объекта [webApp](../resources/intune-apps-webapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1a39-127">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="b1a39-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-128">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="b1a39-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1a39-129">Property</span></span>|<span data-ttu-id="b1a39-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b1a39-130">Type</span></span>|<span data-ttu-id="b1a39-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b1a39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1a39-132">id</span><span class="sxs-lookup"><span data-stu-id="b1a39-132">id</span></span>|<span data-ttu-id="b1a39-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b1a39-133">String</span></span>|<span data-ttu-id="b1a39-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b1a39-134">Key of the entity.</span></span> <span data-ttu-id="b1a39-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b1a39-136">displayName</span></span>|<span data-ttu-id="b1a39-137">Строка</span><span class="sxs-lookup"><span data-stu-id="b1a39-137">String</span></span>|<span data-ttu-id="b1a39-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="b1a39-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b1a39-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-140">description</span><span class="sxs-lookup"><span data-stu-id="b1a39-140">description</span></span>|<span data-ttu-id="b1a39-141">Строка</span><span class="sxs-lookup"><span data-stu-id="b1a39-141">String</span></span>|<span data-ttu-id="b1a39-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="b1a39-142">The description of the app.</span></span> <span data-ttu-id="b1a39-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b1a39-144">publisher</span></span>|<span data-ttu-id="b1a39-145">Строка</span><span class="sxs-lookup"><span data-stu-id="b1a39-145">String</span></span>|<span data-ttu-id="b1a39-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="b1a39-146">The publisher of the app.</span></span> <span data-ttu-id="b1a39-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b1a39-148">largeIcon</span></span>|[<span data-ttu-id="b1a39-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b1a39-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b1a39-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="b1a39-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b1a39-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1a39-152">createdDateTime</span></span>|<span data-ttu-id="b1a39-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1a39-153">DateTimeOffset</span></span>|<span data-ttu-id="b1a39-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="b1a39-154">The date and time the app was created.</span></span> <span data-ttu-id="b1a39-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1a39-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b1a39-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1a39-157">DateTimeOffset</span></span>|<span data-ttu-id="b1a39-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="b1a39-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b1a39-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b1a39-160">isFeatured</span></span>|<span data-ttu-id="b1a39-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1a39-161">Boolean</span></span>|<span data-ttu-id="b1a39-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b1a39-163">privacyInformationUrl</span></span>|<span data-ttu-id="b1a39-164">Строка</span><span class="sxs-lookup"><span data-stu-id="b1a39-164">String</span></span>|<span data-ttu-id="b1a39-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b1a39-165">The privacy statement Url.</span></span> <span data-ttu-id="b1a39-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b1a39-167">informationUrl</span></span>|<span data-ttu-id="b1a39-168">Строка</span><span class="sxs-lookup"><span data-stu-id="b1a39-168">String</span></span>|<span data-ttu-id="b1a39-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b1a39-169">The more information Url.</span></span> <span data-ttu-id="b1a39-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-171">owner</span><span class="sxs-lookup"><span data-stu-id="b1a39-171">owner</span></span>|<span data-ttu-id="b1a39-172">String</span><span class="sxs-lookup"><span data-stu-id="b1a39-172">String</span></span>|<span data-ttu-id="b1a39-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="b1a39-173">The owner of the app.</span></span> <span data-ttu-id="b1a39-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-175">developer</span><span class="sxs-lookup"><span data-stu-id="b1a39-175">developer</span></span>|<span data-ttu-id="b1a39-176">Строка</span><span class="sxs-lookup"><span data-stu-id="b1a39-176">String</span></span>|<span data-ttu-id="b1a39-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="b1a39-177">The developer of the app.</span></span> <span data-ttu-id="b1a39-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-179">notes</span><span class="sxs-lookup"><span data-stu-id="b1a39-179">notes</span></span>|<span data-ttu-id="b1a39-180">Строка</span><span class="sxs-lookup"><span data-stu-id="b1a39-180">String</span></span>|<span data-ttu-id="b1a39-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="b1a39-181">Notes for the app.</span></span> <span data-ttu-id="b1a39-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b1a39-183">uploadState</span></span>|<span data-ttu-id="b1a39-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b1a39-184">Int32</span></span>|<span data-ttu-id="b1a39-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="b1a39-185">The upload state.</span></span> <span data-ttu-id="b1a39-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b1a39-187">publishingState</span></span>|[<span data-ttu-id="b1a39-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="b1a39-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b1a39-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="b1a39-189">The publishing state for the app.</span></span> <span data-ttu-id="b1a39-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="b1a39-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b1a39-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="b1a39-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b1a39-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b1a39-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b1a39-193">isAssigned</span></span>|<span data-ttu-id="b1a39-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1a39-194">Boolean</span></span>|<span data-ttu-id="b1a39-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="b1a39-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b1a39-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1a39-197">roleScopeTagIds</span></span>|<span data-ttu-id="b1a39-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b1a39-198">String collection</span></span>|<span data-ttu-id="b1a39-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="b1a39-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b1a39-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="b1a39-201">dependentAppCount</span></span>|<span data-ttu-id="b1a39-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b1a39-202">Int32</span></span>|<span data-ttu-id="b1a39-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="b1a39-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b1a39-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b1a39-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b1a39-205">appUrl</span><span class="sxs-lookup"><span data-stu-id="b1a39-205">appUrl</span></span>|<span data-ttu-id="b1a39-206">String</span><span class="sxs-lookup"><span data-stu-id="b1a39-206">String</span></span>|<span data-ttu-id="b1a39-207">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="b1a39-207">The web app URL.</span></span>|
|<span data-ttu-id="b1a39-208">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="b1a39-208">useManagedBrowser</span></span>|<span data-ttu-id="b1a39-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1a39-209">Boolean</span></span>|<span data-ttu-id="b1a39-210">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="b1a39-210">Whether or not to use managed browser.</span></span> <span data-ttu-id="b1a39-211">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="b1a39-211">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="b1a39-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1a39-212">Response</span></span>
<span data-ttu-id="b1a39-213">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [webApp](../resources/intune-apps-webapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b1a39-213">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1a39-214">Пример</span><span class="sxs-lookup"><span data-stu-id="b1a39-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1a39-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1a39-215">Request</span></span>
<span data-ttu-id="b1a39-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1a39-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 779

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="b1a39-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1a39-217">Response</span></span>
<span data-ttu-id="b1a39-p120">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1a39-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 951

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```





