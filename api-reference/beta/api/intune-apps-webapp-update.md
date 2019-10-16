---
title: Update webApp
description: Обновление свойств объекта webApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8292ab7c63ef64bfa94fa016e3198067bd037054
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37535137"
---
# <a name="update-webapp"></a><span data-ttu-id="75a7f-103">Update webApp</span><span class="sxs-lookup"><span data-stu-id="75a7f-103">Update webApp</span></span>

> <span data-ttu-id="75a7f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75a7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75a7f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="75a7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75a7f-106">Обновление свойств объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-106">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75a7f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="75a7f-107">Prerequisites</span></span>
<span data-ttu-id="75a7f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75a7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75a7f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="75a7f-110">Permission type</span></span>|<span data-ttu-id="75a7f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="75a7f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75a7f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="75a7f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75a7f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a7f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="75a7f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="75a7f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75a7f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="75a7f-115">Not supported.</span></span>|
|<span data-ttu-id="75a7f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="75a7f-116">Application</span></span>|<span data-ttu-id="75a7f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a7f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75a7f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="75a7f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="75a7f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="75a7f-119">Request headers</span></span>
|<span data-ttu-id="75a7f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="75a7f-120">Header</span></span>|<span data-ttu-id="75a7f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="75a7f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75a7f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="75a7f-122">Authorization</span></span>|<span data-ttu-id="75a7f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="75a7f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75a7f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="75a7f-124">Accept</span></span>|<span data-ttu-id="75a7f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75a7f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75a7f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="75a7f-126">Request body</span></span>
<span data-ttu-id="75a7f-127">В тексте запроса добавьте представление объекта [webApp](../resources/intune-apps-webapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75a7f-127">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="75a7f-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-128">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="75a7f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="75a7f-129">Property</span></span>|<span data-ttu-id="75a7f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="75a7f-130">Type</span></span>|<span data-ttu-id="75a7f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="75a7f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75a7f-132">id</span><span class="sxs-lookup"><span data-stu-id="75a7f-132">id</span></span>|<span data-ttu-id="75a7f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="75a7f-133">String</span></span>|<span data-ttu-id="75a7f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="75a7f-134">Key of the entity.</span></span> <span data-ttu-id="75a7f-135">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="75a7f-136">displayName</span></span>|<span data-ttu-id="75a7f-137">Строка</span><span class="sxs-lookup"><span data-stu-id="75a7f-137">String</span></span>|<span data-ttu-id="75a7f-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="75a7f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="75a7f-139">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-140">description</span><span class="sxs-lookup"><span data-stu-id="75a7f-140">description</span></span>|<span data-ttu-id="75a7f-141">Строка</span><span class="sxs-lookup"><span data-stu-id="75a7f-141">String</span></span>|<span data-ttu-id="75a7f-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="75a7f-142">The description of the app.</span></span> <span data-ttu-id="75a7f-143">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-144">publisher</span><span class="sxs-lookup"><span data-stu-id="75a7f-144">publisher</span></span>|<span data-ttu-id="75a7f-145">String</span><span class="sxs-lookup"><span data-stu-id="75a7f-145">String</span></span>|<span data-ttu-id="75a7f-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="75a7f-146">The publisher of the app.</span></span> <span data-ttu-id="75a7f-147">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="75a7f-148">largeIcon</span></span>|[<span data-ttu-id="75a7f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="75a7f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="75a7f-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="75a7f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="75a7f-151">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75a7f-152">createdDateTime</span></span>|<span data-ttu-id="75a7f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75a7f-153">DateTimeOffset</span></span>|<span data-ttu-id="75a7f-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="75a7f-154">The date and time the app was created.</span></span> <span data-ttu-id="75a7f-155">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75a7f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="75a7f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75a7f-157">DateTimeOffset</span></span>|<span data-ttu-id="75a7f-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="75a7f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="75a7f-159">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="75a7f-160">isFeatured</span></span>|<span data-ttu-id="75a7f-161">Логический</span><span class="sxs-lookup"><span data-stu-id="75a7f-161">Boolean</span></span>|<span data-ttu-id="75a7f-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="75a7f-163">privacyInformationUrl</span></span>|<span data-ttu-id="75a7f-164">String</span><span class="sxs-lookup"><span data-stu-id="75a7f-164">String</span></span>|<span data-ttu-id="75a7f-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="75a7f-165">The privacy statement Url.</span></span> <span data-ttu-id="75a7f-166">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="75a7f-167">informationUrl</span></span>|<span data-ttu-id="75a7f-168">String</span><span class="sxs-lookup"><span data-stu-id="75a7f-168">String</span></span>|<span data-ttu-id="75a7f-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="75a7f-169">The more information Url.</span></span> <span data-ttu-id="75a7f-170">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-171">owner</span><span class="sxs-lookup"><span data-stu-id="75a7f-171">owner</span></span>|<span data-ttu-id="75a7f-172">String</span><span class="sxs-lookup"><span data-stu-id="75a7f-172">String</span></span>|<span data-ttu-id="75a7f-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="75a7f-173">The owner of the app.</span></span> <span data-ttu-id="75a7f-174">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-175">developer</span><span class="sxs-lookup"><span data-stu-id="75a7f-175">developer</span></span>|<span data-ttu-id="75a7f-176">String</span><span class="sxs-lookup"><span data-stu-id="75a7f-176">String</span></span>|<span data-ttu-id="75a7f-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="75a7f-177">The developer of the app.</span></span> <span data-ttu-id="75a7f-178">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-179">notes</span><span class="sxs-lookup"><span data-stu-id="75a7f-179">notes</span></span>|<span data-ttu-id="75a7f-180">String</span><span class="sxs-lookup"><span data-stu-id="75a7f-180">String</span></span>|<span data-ttu-id="75a7f-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="75a7f-181">Notes for the app.</span></span> <span data-ttu-id="75a7f-182">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="75a7f-183">uploadState</span></span>|<span data-ttu-id="75a7f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="75a7f-184">Int32</span></span>|<span data-ttu-id="75a7f-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="75a7f-185">The upload state.</span></span> <span data-ttu-id="75a7f-186">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="75a7f-187">publishingState</span></span>|[<span data-ttu-id="75a7f-188">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="75a7f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="75a7f-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="75a7f-189">The publishing state for the app.</span></span> <span data-ttu-id="75a7f-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="75a7f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="75a7f-191">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="75a7f-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="75a7f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="75a7f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="75a7f-193">isAssigned</span></span>|<span data-ttu-id="75a7f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="75a7f-194">Boolean</span></span>|<span data-ttu-id="75a7f-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="75a7f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="75a7f-196">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="75a7f-197">roleScopeTagIds</span></span>|<span data-ttu-id="75a7f-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="75a7f-198">String collection</span></span>|<span data-ttu-id="75a7f-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="75a7f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="75a7f-200">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-201">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="75a7f-201">dependentAppCount</span></span>|<span data-ttu-id="75a7f-202">Int32</span><span class="sxs-lookup"><span data-stu-id="75a7f-202">Int32</span></span>|<span data-ttu-id="75a7f-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="75a7f-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="75a7f-204">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="75a7f-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="75a7f-205">appUrl</span><span class="sxs-lookup"><span data-stu-id="75a7f-205">appUrl</span></span>|<span data-ttu-id="75a7f-206">String</span><span class="sxs-lookup"><span data-stu-id="75a7f-206">String</span></span>|<span data-ttu-id="75a7f-207">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="75a7f-207">The web app URL.</span></span>|
|<span data-ttu-id="75a7f-208">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="75a7f-208">useManagedBrowser</span></span>|<span data-ttu-id="75a7f-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="75a7f-209">Boolean</span></span>|<span data-ttu-id="75a7f-210">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="75a7f-210">Whether or not to use managed browser.</span></span> <span data-ttu-id="75a7f-211">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="75a7f-211">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="75a7f-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="75a7f-212">Response</span></span>
<span data-ttu-id="75a7f-213">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [webApp](../resources/intune-apps-webapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="75a7f-213">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75a7f-214">Пример</span><span class="sxs-lookup"><span data-stu-id="75a7f-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="75a7f-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="75a7f-215">Request</span></span>
<span data-ttu-id="75a7f-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="75a7f-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="75a7f-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="75a7f-217">Response</span></span>
<span data-ttu-id="75a7f-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="75a7f-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






