---
title: Update androidStoreApp
description: Обновление свойств объекта androidStoreApp.
ms.openlocfilehash: 3db3566bee403d9fbafe502922f5739efd61000c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079321"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="c6a50-103">Update androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="c6a50-103">Update androidStoreApp</span></span>

> <span data-ttu-id="c6a50-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c6a50-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6a50-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6a50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6a50-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c6a50-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6a50-107">Обновление свойств объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-107">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6a50-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c6a50-108">Prerequisites</span></span>
<span data-ttu-id="c6a50-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6a50-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6a50-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6a50-111">Permission type</span></span>|<span data-ttu-id="c6a50-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6a50-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6a50-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6a50-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6a50-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6a50-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c6a50-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6a50-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6a50-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6a50-116">Not supported.</span></span>|
|<span data-ttu-id="c6a50-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6a50-117">Application</span></span>|<span data-ttu-id="c6a50-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6a50-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6a50-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6a50-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="c6a50-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6a50-120">Request headers</span></span>
|<span data-ttu-id="c6a50-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c6a50-121">Header</span></span>|<span data-ttu-id="c6a50-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c6a50-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6a50-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6a50-123">Authorization</span></span>|<span data-ttu-id="c6a50-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c6a50-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6a50-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c6a50-125">Accept</span></span>|<span data-ttu-id="c6a50-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6a50-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6a50-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c6a50-127">Request body</span></span>
<span data-ttu-id="c6a50-128">В теле запроса добавьте представление объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6a50-128">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="c6a50-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-129">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="c6a50-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6a50-130">Property</span></span>|<span data-ttu-id="c6a50-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c6a50-131">Type</span></span>|<span data-ttu-id="c6a50-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c6a50-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6a50-133">id</span><span class="sxs-lookup"><span data-stu-id="c6a50-133">id</span></span>|<span data-ttu-id="c6a50-134">String</span><span class="sxs-lookup"><span data-stu-id="c6a50-134">String</span></span>|<span data-ttu-id="c6a50-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c6a50-135">Key of the entity.</span></span> <span data-ttu-id="c6a50-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c6a50-137">displayName</span></span>|<span data-ttu-id="c6a50-138">String</span><span class="sxs-lookup"><span data-stu-id="c6a50-138">String</span></span>|<span data-ttu-id="c6a50-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c6a50-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c6a50-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-141">описание</span><span class="sxs-lookup"><span data-stu-id="c6a50-141">description</span></span>|<span data-ttu-id="c6a50-142">String</span><span class="sxs-lookup"><span data-stu-id="c6a50-142">String</span></span>|<span data-ttu-id="c6a50-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c6a50-143">The description of the app.</span></span> <span data-ttu-id="c6a50-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c6a50-145">publisher</span></span>|<span data-ttu-id="c6a50-146">String</span><span class="sxs-lookup"><span data-stu-id="c6a50-146">String</span></span>|<span data-ttu-id="c6a50-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c6a50-147">The publisher of the app.</span></span> <span data-ttu-id="c6a50-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c6a50-149">largeIcon</span></span>|[<span data-ttu-id="c6a50-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c6a50-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c6a50-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="c6a50-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c6a50-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6a50-153">createdDateTime</span></span>|<span data-ttu-id="c6a50-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6a50-154">DateTimeOffset</span></span>|<span data-ttu-id="c6a50-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="c6a50-155">The date and time the app was created.</span></span> <span data-ttu-id="c6a50-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6a50-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c6a50-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6a50-158">DateTimeOffset</span></span>|<span data-ttu-id="c6a50-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="c6a50-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c6a50-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c6a50-161">isFeatured</span></span>|<span data-ttu-id="c6a50-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c6a50-162">Boolean</span></span>|<span data-ttu-id="c6a50-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c6a50-164">privacyInformationUrl</span></span>|<span data-ttu-id="c6a50-165">String</span><span class="sxs-lookup"><span data-stu-id="c6a50-165">String</span></span>|<span data-ttu-id="c6a50-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c6a50-166">The privacy statement Url.</span></span> <span data-ttu-id="c6a50-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c6a50-168">informationUrl</span></span>|<span data-ttu-id="c6a50-169">String</span><span class="sxs-lookup"><span data-stu-id="c6a50-169">String</span></span>|<span data-ttu-id="c6a50-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="c6a50-170">The more information Url.</span></span> <span data-ttu-id="c6a50-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-172">owner</span><span class="sxs-lookup"><span data-stu-id="c6a50-172">owner</span></span>|<span data-ttu-id="c6a50-173">String</span><span class="sxs-lookup"><span data-stu-id="c6a50-173">String</span></span>|<span data-ttu-id="c6a50-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="c6a50-174">The owner of the app.</span></span> <span data-ttu-id="c6a50-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-176">developer</span><span class="sxs-lookup"><span data-stu-id="c6a50-176">developer</span></span>|<span data-ttu-id="c6a50-177">String</span><span class="sxs-lookup"><span data-stu-id="c6a50-177">String</span></span>|<span data-ttu-id="c6a50-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="c6a50-178">The developer of the app.</span></span> <span data-ttu-id="c6a50-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-180">notes</span><span class="sxs-lookup"><span data-stu-id="c6a50-180">notes</span></span>|<span data-ttu-id="c6a50-181">String</span><span class="sxs-lookup"><span data-stu-id="c6a50-181">String</span></span>|<span data-ttu-id="c6a50-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="c6a50-182">Notes for the app.</span></span> <span data-ttu-id="c6a50-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c6a50-184">uploadState</span></span>|<span data-ttu-id="c6a50-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c6a50-185">Int32</span></span>|<span data-ttu-id="c6a50-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="c6a50-186">The upload state.</span></span> <span data-ttu-id="c6a50-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c6a50-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c6a50-188">publishingState</span></span>|[<span data-ttu-id="c6a50-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c6a50-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c6a50-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="c6a50-190">The publishing state for the app.</span></span> <span data-ttu-id="c6a50-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="c6a50-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c6a50-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c6a50-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c6a50-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c6a50-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c6a50-194">packageId</span><span class="sxs-lookup"><span data-stu-id="c6a50-194">packageId</span></span>|<span data-ttu-id="c6a50-195">String</span><span class="sxs-lookup"><span data-stu-id="c6a50-195">String</span></span>|<span data-ttu-id="c6a50-196">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="c6a50-196">The package identifier.</span></span>|
|<span data-ttu-id="c6a50-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c6a50-197">appIdentifier</span></span>|<span data-ttu-id="c6a50-198">String</span><span class="sxs-lookup"><span data-stu-id="c6a50-198">String</span></span>|<span data-ttu-id="c6a50-199">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c6a50-199">The Identity Name.</span></span>|
|<span data-ttu-id="c6a50-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c6a50-200">appStoreUrl</span></span>|<span data-ttu-id="c6a50-201">String</span><span class="sxs-lookup"><span data-stu-id="c6a50-201">String</span></span>|<span data-ttu-id="c6a50-202">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="c6a50-202">The Android app store URL.</span></span>|
|<span data-ttu-id="c6a50-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c6a50-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c6a50-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c6a50-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="c6a50-205">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="c6a50-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="c6a50-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6a50-206">Response</span></span>
<span data-ttu-id="c6a50-207">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c6a50-207">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6a50-208">Пример</span><span class="sxs-lookup"><span data-stu-id="c6a50-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6a50-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6a50-209">Request</span></span>
<span data-ttu-id="c6a50-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6a50-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1128

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="c6a50-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="c6a50-211">Response</span></span>
<span data-ttu-id="c6a50-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c6a50-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1290

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```





