---
title: Update androidLobApp
description: Обновление свойств объекта androidLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c60056f7e7bfb5b5be6ece2327031ae15b03bbfb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355703"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="40222-103">Update androidLobApp</span><span class="sxs-lookup"><span data-stu-id="40222-103">Update androidLobApp</span></span>

> <span data-ttu-id="40222-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40222-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40222-105">Обновление свойств объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-105">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40222-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="40222-106">Prerequisites</span></span>
<span data-ttu-id="40222-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40222-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40222-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40222-109">Permission type</span></span>|<span data-ttu-id="40222-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40222-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40222-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40222-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40222-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40222-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40222-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40222-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40222-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40222-114">Not supported.</span></span>|
|<span data-ttu-id="40222-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40222-115">Application</span></span>|<span data-ttu-id="40222-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40222-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40222-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40222-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="40222-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40222-118">Request headers</span></span>
|<span data-ttu-id="40222-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40222-119">Header</span></span>|<span data-ttu-id="40222-120">Значение</span><span class="sxs-lookup"><span data-stu-id="40222-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40222-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40222-121">Authorization</span></span>|<span data-ttu-id="40222-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40222-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40222-123">Accept</span><span class="sxs-lookup"><span data-stu-id="40222-123">Accept</span></span>|<span data-ttu-id="40222-124">application/json</span><span class="sxs-lookup"><span data-stu-id="40222-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40222-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40222-125">Request body</span></span>
<span data-ttu-id="40222-126">В теле запроса добавьте представление объекта [androidLobApp](../resources/intune-apps-androidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40222-126">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="40222-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-127">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="40222-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="40222-128">Property</span></span>|<span data-ttu-id="40222-129">Тип</span><span class="sxs-lookup"><span data-stu-id="40222-129">Type</span></span>|<span data-ttu-id="40222-130">Описание</span><span class="sxs-lookup"><span data-stu-id="40222-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40222-131">id</span><span class="sxs-lookup"><span data-stu-id="40222-131">id</span></span>|<span data-ttu-id="40222-132">Строка</span><span class="sxs-lookup"><span data-stu-id="40222-132">String</span></span>|<span data-ttu-id="40222-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="40222-133">Key of the entity.</span></span> <span data-ttu-id="40222-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-135">displayName</span><span class="sxs-lookup"><span data-stu-id="40222-135">displayName</span></span>|<span data-ttu-id="40222-136">Строка</span><span class="sxs-lookup"><span data-stu-id="40222-136">String</span></span>|<span data-ttu-id="40222-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="40222-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="40222-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-139">description</span><span class="sxs-lookup"><span data-stu-id="40222-139">description</span></span>|<span data-ttu-id="40222-140">Строка</span><span class="sxs-lookup"><span data-stu-id="40222-140">String</span></span>|<span data-ttu-id="40222-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="40222-141">The description of the app.</span></span> <span data-ttu-id="40222-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-143">publisher</span><span class="sxs-lookup"><span data-stu-id="40222-143">publisher</span></span>|<span data-ttu-id="40222-144">String</span><span class="sxs-lookup"><span data-stu-id="40222-144">String</span></span>|<span data-ttu-id="40222-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="40222-145">The publisher of the app.</span></span> <span data-ttu-id="40222-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="40222-147">largeIcon</span></span>|[<span data-ttu-id="40222-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="40222-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="40222-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="40222-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="40222-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40222-151">createdDateTime</span></span>|<span data-ttu-id="40222-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40222-152">DateTimeOffset</span></span>|<span data-ttu-id="40222-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="40222-153">The date and time the app was created.</span></span> <span data-ttu-id="40222-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40222-155">lastModifiedDateTime</span></span>|<span data-ttu-id="40222-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40222-156">DateTimeOffset</span></span>|<span data-ttu-id="40222-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="40222-157">The date and time the app was last modified.</span></span> <span data-ttu-id="40222-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="40222-159">isFeatured</span></span>|<span data-ttu-id="40222-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="40222-160">Boolean</span></span>|<span data-ttu-id="40222-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="40222-162">privacyInformationUrl</span></span>|<span data-ttu-id="40222-163">String</span><span class="sxs-lookup"><span data-stu-id="40222-163">String</span></span>|<span data-ttu-id="40222-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="40222-164">The privacy statement Url.</span></span> <span data-ttu-id="40222-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="40222-166">informationUrl</span></span>|<span data-ttu-id="40222-167">String</span><span class="sxs-lookup"><span data-stu-id="40222-167">String</span></span>|<span data-ttu-id="40222-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="40222-168">The more information Url.</span></span> <span data-ttu-id="40222-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-170">owner</span><span class="sxs-lookup"><span data-stu-id="40222-170">owner</span></span>|<span data-ttu-id="40222-171">String</span><span class="sxs-lookup"><span data-stu-id="40222-171">String</span></span>|<span data-ttu-id="40222-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="40222-172">The owner of the app.</span></span> <span data-ttu-id="40222-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-174">developer</span><span class="sxs-lookup"><span data-stu-id="40222-174">developer</span></span>|<span data-ttu-id="40222-175">String</span><span class="sxs-lookup"><span data-stu-id="40222-175">String</span></span>|<span data-ttu-id="40222-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="40222-176">The developer of the app.</span></span> <span data-ttu-id="40222-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-178">notes</span><span class="sxs-lookup"><span data-stu-id="40222-178">notes</span></span>|<span data-ttu-id="40222-179">String</span><span class="sxs-lookup"><span data-stu-id="40222-179">String</span></span>|<span data-ttu-id="40222-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="40222-180">Notes for the app.</span></span> <span data-ttu-id="40222-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="40222-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="40222-182">publishingState</span></span>|[<span data-ttu-id="40222-183">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="40222-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="40222-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="40222-184">The publishing state for the app.</span></span> <span data-ttu-id="40222-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="40222-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="40222-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="40222-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="40222-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="40222-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="40222-188">committedContentVersion</span></span>|<span data-ttu-id="40222-189">String</span><span class="sxs-lookup"><span data-stu-id="40222-189">String</span></span>|<span data-ttu-id="40222-190">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="40222-190">The internal committed content version.</span></span> <span data-ttu-id="40222-191">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="40222-192">fileName</span><span class="sxs-lookup"><span data-stu-id="40222-192">fileName</span></span>|<span data-ttu-id="40222-193">String</span><span class="sxs-lookup"><span data-stu-id="40222-193">String</span></span>|<span data-ttu-id="40222-194">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="40222-194">The name of the main Lob application file.</span></span> <span data-ttu-id="40222-195">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="40222-196">size</span><span class="sxs-lookup"><span data-stu-id="40222-196">size</span></span>|<span data-ttu-id="40222-197">Int64</span><span class="sxs-lookup"><span data-stu-id="40222-197">Int64</span></span>|<span data-ttu-id="40222-198">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="40222-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="40222-199">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="40222-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="40222-200">packageId</span><span class="sxs-lookup"><span data-stu-id="40222-200">packageId</span></span>|<span data-ttu-id="40222-201">String</span><span class="sxs-lookup"><span data-stu-id="40222-201">String</span></span>|<span data-ttu-id="40222-202">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="40222-202">The package identifier.</span></span>|
|<span data-ttu-id="40222-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="40222-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="40222-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="40222-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="40222-205">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="40222-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="40222-206">versionName</span><span class="sxs-lookup"><span data-stu-id="40222-206">versionName</span></span>|<span data-ttu-id="40222-207">String</span><span class="sxs-lookup"><span data-stu-id="40222-207">String</span></span>|<span data-ttu-id="40222-208">Имя версии бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="40222-208">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="40222-209">versionCode</span><span class="sxs-lookup"><span data-stu-id="40222-209">versionCode</span></span>|<span data-ttu-id="40222-210">String</span><span class="sxs-lookup"><span data-stu-id="40222-210">String</span></span>|<span data-ttu-id="40222-211">Код версии бизнес-приложения Android.</span><span class="sxs-lookup"><span data-stu-id="40222-211">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="40222-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="40222-212">Response</span></span>
<span data-ttu-id="40222-213">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidLobApp](../resources/intune-apps-androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="40222-213">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40222-214">Пример</span><span class="sxs-lookup"><span data-stu-id="40222-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="40222-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="40222-215">Request</span></span>
<span data-ttu-id="40222-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40222-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1075

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="40222-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="40222-217">Response</span></span>
<span data-ttu-id="40222-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40222-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```




