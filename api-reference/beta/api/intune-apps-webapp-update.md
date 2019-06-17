---
title: Update webApp
description: Обновление свойств объекта webApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c685b595fe528a5fbc5cd5a10c007a0dea4564ca
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973412"
---
# <a name="update-webapp"></a><span data-ttu-id="eaf6e-103">Update webApp</span><span class="sxs-lookup"><span data-stu-id="eaf6e-103">Update webApp</span></span>

> <span data-ttu-id="eaf6e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaf6e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaf6e-106">Обновление свойств объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-106">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eaf6e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="eaf6e-107">Prerequisites</span></span>
<span data-ttu-id="eaf6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaf6e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eaf6e-110">Permission type</span></span>|<span data-ttu-id="eaf6e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eaf6e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaf6e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eaf6e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eaf6e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaf6e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eaf6e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eaf6e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaf6e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-115">Not supported.</span></span>|
|<span data-ttu-id="eaf6e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eaf6e-116">Application</span></span>|<span data-ttu-id="eaf6e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaf6e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eaf6e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="eaf6e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eaf6e-119">Request headers</span></span>
|<span data-ttu-id="eaf6e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eaf6e-120">Header</span></span>|<span data-ttu-id="eaf6e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eaf6e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaf6e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eaf6e-122">Authorization</span></span>|<span data-ttu-id="eaf6e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaf6e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eaf6e-124">Accept</span></span>|<span data-ttu-id="eaf6e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eaf6e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaf6e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eaf6e-126">Request body</span></span>
<span data-ttu-id="eaf6e-127">В тексте запроса добавьте представление объекта [webApp](../resources/intune-apps-webapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-127">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="eaf6e-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [webApp](../resources/intune-apps-webapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-128">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="eaf6e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="eaf6e-129">Property</span></span>|<span data-ttu-id="eaf6e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="eaf6e-130">Type</span></span>|<span data-ttu-id="eaf6e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="eaf6e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaf6e-132">id</span><span class="sxs-lookup"><span data-stu-id="eaf6e-132">id</span></span>|<span data-ttu-id="eaf6e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="eaf6e-133">String</span></span>|<span data-ttu-id="eaf6e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-134">Key of the entity.</span></span> <span data-ttu-id="eaf6e-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="eaf6e-136">displayName</span></span>|<span data-ttu-id="eaf6e-137">Строка</span><span class="sxs-lookup"><span data-stu-id="eaf6e-137">String</span></span>|<span data-ttu-id="eaf6e-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="eaf6e-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-140">description</span><span class="sxs-lookup"><span data-stu-id="eaf6e-140">description</span></span>|<span data-ttu-id="eaf6e-141">Строка</span><span class="sxs-lookup"><span data-stu-id="eaf6e-141">String</span></span>|<span data-ttu-id="eaf6e-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-142">The description of the app.</span></span> <span data-ttu-id="eaf6e-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-144">publisher</span><span class="sxs-lookup"><span data-stu-id="eaf6e-144">publisher</span></span>|<span data-ttu-id="eaf6e-145">String</span><span class="sxs-lookup"><span data-stu-id="eaf6e-145">String</span></span>|<span data-ttu-id="eaf6e-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-146">The publisher of the app.</span></span> <span data-ttu-id="eaf6e-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="eaf6e-148">largeIcon</span></span>|[<span data-ttu-id="eaf6e-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eaf6e-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eaf6e-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="eaf6e-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eaf6e-152">createdDateTime</span></span>|<span data-ttu-id="eaf6e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaf6e-153">DateTimeOffset</span></span>|<span data-ttu-id="eaf6e-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-154">The date and time the app was created.</span></span> <span data-ttu-id="eaf6e-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eaf6e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="eaf6e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaf6e-157">DateTimeOffset</span></span>|<span data-ttu-id="eaf6e-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-158">The date and time the app was last modified.</span></span> <span data-ttu-id="eaf6e-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="eaf6e-160">isFeatured</span></span>|<span data-ttu-id="eaf6e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaf6e-161">Boolean</span></span>|<span data-ttu-id="eaf6e-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eaf6e-163">privacyInformationUrl</span></span>|<span data-ttu-id="eaf6e-164">String</span><span class="sxs-lookup"><span data-stu-id="eaf6e-164">String</span></span>|<span data-ttu-id="eaf6e-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-165">The privacy statement Url.</span></span> <span data-ttu-id="eaf6e-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eaf6e-167">informationUrl</span></span>|<span data-ttu-id="eaf6e-168">String</span><span class="sxs-lookup"><span data-stu-id="eaf6e-168">String</span></span>|<span data-ttu-id="eaf6e-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-169">The more information Url.</span></span> <span data-ttu-id="eaf6e-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-171">owner</span><span class="sxs-lookup"><span data-stu-id="eaf6e-171">owner</span></span>|<span data-ttu-id="eaf6e-172">String</span><span class="sxs-lookup"><span data-stu-id="eaf6e-172">String</span></span>|<span data-ttu-id="eaf6e-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-173">The owner of the app.</span></span> <span data-ttu-id="eaf6e-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-175">developer</span><span class="sxs-lookup"><span data-stu-id="eaf6e-175">developer</span></span>|<span data-ttu-id="eaf6e-176">String</span><span class="sxs-lookup"><span data-stu-id="eaf6e-176">String</span></span>|<span data-ttu-id="eaf6e-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-177">The developer of the app.</span></span> <span data-ttu-id="eaf6e-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-179">notes</span><span class="sxs-lookup"><span data-stu-id="eaf6e-179">notes</span></span>|<span data-ttu-id="eaf6e-180">String</span><span class="sxs-lookup"><span data-stu-id="eaf6e-180">String</span></span>|<span data-ttu-id="eaf6e-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-181">Notes for the app.</span></span> <span data-ttu-id="eaf6e-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="eaf6e-183">uploadState</span></span>|<span data-ttu-id="eaf6e-184">Int32</span><span class="sxs-lookup"><span data-stu-id="eaf6e-184">Int32</span></span>|<span data-ttu-id="eaf6e-185">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-185">The upload state.</span></span> <span data-ttu-id="eaf6e-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="eaf6e-187">publishingState</span></span>|[<span data-ttu-id="eaf6e-188">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="eaf6e-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="eaf6e-189">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-189">The publishing state for the app.</span></span> <span data-ttu-id="eaf6e-190">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="eaf6e-191">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="eaf6e-192">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="eaf6e-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="eaf6e-193">isAssigned</span></span>|<span data-ttu-id="eaf6e-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaf6e-194">Boolean</span></span>|<span data-ttu-id="eaf6e-195">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="eaf6e-196">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eaf6e-197">roleScopeTagIds</span></span>|<span data-ttu-id="eaf6e-198">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="eaf6e-198">String collection</span></span>|<span data-ttu-id="eaf6e-199">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="eaf6e-200">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-201">Депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="eaf6e-201">dependentAppCount</span></span>|<span data-ttu-id="eaf6e-202">Int32</span><span class="sxs-lookup"><span data-stu-id="eaf6e-202">Int32</span></span>|<span data-ttu-id="eaf6e-203">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="eaf6e-204">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eaf6e-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaf6e-205">appUrl</span><span class="sxs-lookup"><span data-stu-id="eaf6e-205">appUrl</span></span>|<span data-ttu-id="eaf6e-206">String</span><span class="sxs-lookup"><span data-stu-id="eaf6e-206">String</span></span>|<span data-ttu-id="eaf6e-207">URL-адрес веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-207">The web app URL.</span></span>|
|<span data-ttu-id="eaf6e-208">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="eaf6e-208">useManagedBrowser</span></span>|<span data-ttu-id="eaf6e-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaf6e-209">Boolean</span></span>|<span data-ttu-id="eaf6e-210">Указывает, следует ли использовать управляемый браузер.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-210">Whether or not to use managed browser.</span></span> <span data-ttu-id="eaf6e-211">Это свойство применимо только к Android и iOS.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-211">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="eaf6e-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="eaf6e-212">Response</span></span>
<span data-ttu-id="eaf6e-213">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [webApp](../resources/intune-apps-webapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-213">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaf6e-214">Пример</span><span class="sxs-lookup"><span data-stu-id="eaf6e-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="eaf6e-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="eaf6e-215">Request</span></span>
<span data-ttu-id="eaf6e-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eaf6e-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="eaf6e-217">Response</span></span>
<span data-ttu-id="eaf6e-p120">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eaf6e-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





