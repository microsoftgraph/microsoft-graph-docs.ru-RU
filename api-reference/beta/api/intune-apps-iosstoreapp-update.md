---
title: Update iosStoreApp
description: Обновление свойств объекта iosStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2939708cc49e056e584f419b16efc8c7d7129ab8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935915"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="f256e-103">Update iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="f256e-103">Update iosStoreApp</span></span>

> <span data-ttu-id="f256e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f256e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f256e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f256e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f256e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f256e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f256e-107">Обновление свойств объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-107">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f256e-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f256e-108">Prerequisites</span></span>
<span data-ttu-id="f256e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f256e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f256e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f256e-111">Permission type</span></span>|<span data-ttu-id="f256e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f256e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f256e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f256e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f256e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f256e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f256e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f256e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f256e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f256e-116">Not supported.</span></span>|
|<span data-ttu-id="f256e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f256e-117">Application</span></span>|<span data-ttu-id="f256e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f256e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f256e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f256e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f256e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f256e-120">Request headers</span></span>
|<span data-ttu-id="f256e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f256e-121">Header</span></span>|<span data-ttu-id="f256e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f256e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f256e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f256e-123">Authorization</span></span>|<span data-ttu-id="f256e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f256e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f256e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f256e-125">Accept</span></span>|<span data-ttu-id="f256e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f256e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f256e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f256e-127">Request body</span></span>
<span data-ttu-id="f256e-128">В тексте запроса добавьте представление объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f256e-128">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="f256e-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-129">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="f256e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f256e-130">Property</span></span>|<span data-ttu-id="f256e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f256e-131">Type</span></span>|<span data-ttu-id="f256e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f256e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f256e-133">id</span><span class="sxs-lookup"><span data-stu-id="f256e-133">id</span></span>|<span data-ttu-id="f256e-134">String</span><span class="sxs-lookup"><span data-stu-id="f256e-134">String</span></span>|<span data-ttu-id="f256e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f256e-135">Key of the entity.</span></span> <span data-ttu-id="f256e-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f256e-137">displayName</span></span>|<span data-ttu-id="f256e-138">String</span><span class="sxs-lookup"><span data-stu-id="f256e-138">String</span></span>|<span data-ttu-id="f256e-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="f256e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f256e-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-141">описание</span><span class="sxs-lookup"><span data-stu-id="f256e-141">description</span></span>|<span data-ttu-id="f256e-142">String</span><span class="sxs-lookup"><span data-stu-id="f256e-142">String</span></span>|<span data-ttu-id="f256e-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f256e-143">The description of the app.</span></span> <span data-ttu-id="f256e-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f256e-145">publisher</span></span>|<span data-ttu-id="f256e-146">String</span><span class="sxs-lookup"><span data-stu-id="f256e-146">String</span></span>|<span data-ttu-id="f256e-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f256e-147">The publisher of the app.</span></span> <span data-ttu-id="f256e-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f256e-149">largeIcon</span></span>|[<span data-ttu-id="f256e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f256e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f256e-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f256e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f256e-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f256e-153">createdDateTime</span></span>|<span data-ttu-id="f256e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f256e-154">DateTimeOffset</span></span>|<span data-ttu-id="f256e-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f256e-155">The date and time the app was created.</span></span> <span data-ttu-id="f256e-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f256e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f256e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f256e-158">DateTimeOffset</span></span>|<span data-ttu-id="f256e-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f256e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f256e-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f256e-161">isFeatured</span></span>|<span data-ttu-id="f256e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f256e-162">Boolean</span></span>|<span data-ttu-id="f256e-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f256e-164">privacyInformationUrl</span></span>|<span data-ttu-id="f256e-165">String</span><span class="sxs-lookup"><span data-stu-id="f256e-165">String</span></span>|<span data-ttu-id="f256e-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f256e-166">The privacy statement Url.</span></span> <span data-ttu-id="f256e-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f256e-168">informationUrl</span></span>|<span data-ttu-id="f256e-169">String</span><span class="sxs-lookup"><span data-stu-id="f256e-169">String</span></span>|<span data-ttu-id="f256e-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f256e-170">The more information Url.</span></span> <span data-ttu-id="f256e-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-172">owner</span><span class="sxs-lookup"><span data-stu-id="f256e-172">owner</span></span>|<span data-ttu-id="f256e-173">String</span><span class="sxs-lookup"><span data-stu-id="f256e-173">String</span></span>|<span data-ttu-id="f256e-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f256e-174">The owner of the app.</span></span> <span data-ttu-id="f256e-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-176">developer</span><span class="sxs-lookup"><span data-stu-id="f256e-176">developer</span></span>|<span data-ttu-id="f256e-177">String</span><span class="sxs-lookup"><span data-stu-id="f256e-177">String</span></span>|<span data-ttu-id="f256e-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f256e-178">The developer of the app.</span></span> <span data-ttu-id="f256e-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-180">notes</span><span class="sxs-lookup"><span data-stu-id="f256e-180">notes</span></span>|<span data-ttu-id="f256e-181">String</span><span class="sxs-lookup"><span data-stu-id="f256e-181">String</span></span>|<span data-ttu-id="f256e-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="f256e-182">Notes for the app.</span></span> <span data-ttu-id="f256e-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f256e-184">uploadState</span></span>|<span data-ttu-id="f256e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f256e-185">Int32</span></span>|<span data-ttu-id="f256e-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="f256e-186">The upload state.</span></span> <span data-ttu-id="f256e-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f256e-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f256e-188">publishingState</span></span>|[<span data-ttu-id="f256e-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f256e-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f256e-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="f256e-190">The publishing state for the app.</span></span> <span data-ttu-id="f256e-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f256e-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f256e-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f256e-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f256e-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f256e-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f256e-194">bundleId</span><span class="sxs-lookup"><span data-stu-id="f256e-194">bundleId</span></span>|<span data-ttu-id="f256e-195">String</span><span class="sxs-lookup"><span data-stu-id="f256e-195">String</span></span>|<span data-ttu-id="f256e-196">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f256e-196">The Identity Name.</span></span>|
|<span data-ttu-id="f256e-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f256e-197">appStoreUrl</span></span>|<span data-ttu-id="f256e-198">String</span><span class="sxs-lookup"><span data-stu-id="f256e-198">String</span></span>|<span data-ttu-id="f256e-199">URL-адрес в Apple App Store</span><span class="sxs-lookup"><span data-stu-id="f256e-199">The Apple App Store URL</span></span>|
|<span data-ttu-id="f256e-200">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f256e-200">applicableDeviceType</span></span>|[<span data-ttu-id="f256e-201">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f256e-201">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="f256e-202">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="f256e-202">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="f256e-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f256e-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f256e-204">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f256e-204">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="f256e-205">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="f256e-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="f256e-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="f256e-206">Response</span></span>
<span data-ttu-id="f256e-207">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosStoreApp](../resources/intune-apps-iosstoreapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f256e-207">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f256e-208">Пример</span><span class="sxs-lookup"><span data-stu-id="f256e-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="f256e-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="f256e-209">Request</span></span>
<span data-ttu-id="f256e-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f256e-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1042

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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="f256e-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="f256e-211">Response</span></span>
<span data-ttu-id="f256e-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f256e-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1200

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```





