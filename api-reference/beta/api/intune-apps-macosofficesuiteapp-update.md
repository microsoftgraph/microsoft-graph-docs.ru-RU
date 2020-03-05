---
title: Обновление объекта macOSOfficeSuiteApp
description: Обновление свойств объекта macOSOfficeSuiteApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d6ac2c54da14d204cadfa4ba77fa47ab7b67f867
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445262"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="5d83e-103">Обновление объекта macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="5d83e-103">Update macOSOfficeSuiteApp</span></span>

<span data-ttu-id="5d83e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5d83e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d83e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d83e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d83e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d83e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d83e-107">Обновление свойств объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-107">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5d83e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5d83e-108">Prerequisites</span></span>
<span data-ttu-id="5d83e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d83e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d83e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5d83e-111">Permission type</span></span>|<span data-ttu-id="5d83e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5d83e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d83e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5d83e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d83e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d83e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5d83e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5d83e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d83e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d83e-116">Not supported.</span></span>|
|<span data-ttu-id="5d83e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5d83e-117">Application</span></span>|<span data-ttu-id="5d83e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d83e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d83e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5d83e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="5d83e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5d83e-120">Request headers</span></span>
|<span data-ttu-id="5d83e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5d83e-121">Header</span></span>|<span data-ttu-id="5d83e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5d83e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d83e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d83e-123">Authorization</span></span>|<span data-ttu-id="5d83e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5d83e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d83e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5d83e-125">Accept</span></span>|<span data-ttu-id="5d83e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d83e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d83e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5d83e-127">Request body</span></span>
<span data-ttu-id="5d83e-128">В тексте запроса добавьте представление объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d83e-128">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="5d83e-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-129">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="5d83e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d83e-130">Property</span></span>|<span data-ttu-id="5d83e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5d83e-131">Type</span></span>|<span data-ttu-id="5d83e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5d83e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d83e-133">id</span><span class="sxs-lookup"><span data-stu-id="5d83e-133">id</span></span>|<span data-ttu-id="5d83e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5d83e-134">String</span></span>|<span data-ttu-id="5d83e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5d83e-135">Key of the entity.</span></span> <span data-ttu-id="5d83e-136">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5d83e-137">displayName</span></span>|<span data-ttu-id="5d83e-138">Строка</span><span class="sxs-lookup"><span data-stu-id="5d83e-138">String</span></span>|<span data-ttu-id="5d83e-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="5d83e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5d83e-140">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-141">description</span><span class="sxs-lookup"><span data-stu-id="5d83e-141">description</span></span>|<span data-ttu-id="5d83e-142">Строка</span><span class="sxs-lookup"><span data-stu-id="5d83e-142">String</span></span>|<span data-ttu-id="5d83e-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="5d83e-143">The description of the app.</span></span> <span data-ttu-id="5d83e-144">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="5d83e-145">publisher</span></span>|<span data-ttu-id="5d83e-146">String</span><span class="sxs-lookup"><span data-stu-id="5d83e-146">String</span></span>|<span data-ttu-id="5d83e-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="5d83e-147">The publisher of the app.</span></span> <span data-ttu-id="5d83e-148">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5d83e-149">largeIcon</span></span>|[<span data-ttu-id="5d83e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5d83e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5d83e-151">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="5d83e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5d83e-152">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5d83e-153">createdDateTime</span></span>|<span data-ttu-id="5d83e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d83e-154">DateTimeOffset</span></span>|<span data-ttu-id="5d83e-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="5d83e-155">The date and time the app was created.</span></span> <span data-ttu-id="5d83e-156">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5d83e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="5d83e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5d83e-158">DateTimeOffset</span></span>|<span data-ttu-id="5d83e-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="5d83e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="5d83e-160">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5d83e-161">isFeatured</span></span>|<span data-ttu-id="5d83e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d83e-162">Boolean</span></span>|<span data-ttu-id="5d83e-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5d83e-164">privacyInformationUrl</span></span>|<span data-ttu-id="5d83e-165">String</span><span class="sxs-lookup"><span data-stu-id="5d83e-165">String</span></span>|<span data-ttu-id="5d83e-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5d83e-166">The privacy statement Url.</span></span> <span data-ttu-id="5d83e-167">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5d83e-168">informationUrl</span></span>|<span data-ttu-id="5d83e-169">String</span><span class="sxs-lookup"><span data-stu-id="5d83e-169">String</span></span>|<span data-ttu-id="5d83e-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5d83e-170">The more information Url.</span></span> <span data-ttu-id="5d83e-171">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-172">owner</span><span class="sxs-lookup"><span data-stu-id="5d83e-172">owner</span></span>|<span data-ttu-id="5d83e-173">String</span><span class="sxs-lookup"><span data-stu-id="5d83e-173">String</span></span>|<span data-ttu-id="5d83e-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="5d83e-174">The owner of the app.</span></span> <span data-ttu-id="5d83e-175">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-176">developer</span><span class="sxs-lookup"><span data-stu-id="5d83e-176">developer</span></span>|<span data-ttu-id="5d83e-177">String</span><span class="sxs-lookup"><span data-stu-id="5d83e-177">String</span></span>|<span data-ttu-id="5d83e-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="5d83e-178">The developer of the app.</span></span> <span data-ttu-id="5d83e-179">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-180">notes</span><span class="sxs-lookup"><span data-stu-id="5d83e-180">notes</span></span>|<span data-ttu-id="5d83e-181">String</span><span class="sxs-lookup"><span data-stu-id="5d83e-181">String</span></span>|<span data-ttu-id="5d83e-182">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="5d83e-182">Notes for the app.</span></span> <span data-ttu-id="5d83e-183">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="5d83e-184">uploadState</span></span>|<span data-ttu-id="5d83e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="5d83e-185">Int32</span></span>|<span data-ttu-id="5d83e-186">Состояние отправки.</span><span class="sxs-lookup"><span data-stu-id="5d83e-186">The upload state.</span></span> <span data-ttu-id="5d83e-187">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="5d83e-188">publishingState</span></span>|[<span data-ttu-id="5d83e-189">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="5d83e-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5d83e-190">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="5d83e-190">The publishing state for the app.</span></span> <span data-ttu-id="5d83e-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="5d83e-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5d83e-192">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="5d83e-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5d83e-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5d83e-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5d83e-194">isAssigned</span></span>|<span data-ttu-id="5d83e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d83e-195">Boolean</span></span>|<span data-ttu-id="5d83e-196">Значение, указывающее, назначено ли приложение по крайней мере одной группе.</span><span class="sxs-lookup"><span data-stu-id="5d83e-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5d83e-197">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5d83e-198">roleScopeTagIds</span></span>|<span data-ttu-id="5d83e-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5d83e-199">String collection</span></span>|<span data-ttu-id="5d83e-200">Список идентификаторов тегов области для этого мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="5d83e-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5d83e-201">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="5d83e-202">депендентаппкаунт</span><span class="sxs-lookup"><span data-stu-id="5d83e-202">dependentAppCount</span></span>|<span data-ttu-id="5d83e-203">Int32</span><span class="sxs-lookup"><span data-stu-id="5d83e-203">Int32</span></span>|<span data-ttu-id="5d83e-204">Общее количество зависимостей для дочернего приложения.</span><span class="sxs-lookup"><span data-stu-id="5d83e-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="5d83e-205">Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5d83e-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5d83e-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d83e-206">Response</span></span>
<span data-ttu-id="5d83e-207">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5d83e-207">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d83e-208">Пример</span><span class="sxs-lookup"><span data-stu-id="5d83e-208">Example</span></span>

### <a name="request"></a><span data-ttu-id="5d83e-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="5d83e-209">Request</span></span>
<span data-ttu-id="5d83e-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5d83e-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 718

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "dependentAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="5d83e-211">Отклик</span><span class="sxs-lookup"><span data-stu-id="5d83e-211">Response</span></span>
<span data-ttu-id="5d83e-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5d83e-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 890

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "dependentAppCount": 1
}
```





