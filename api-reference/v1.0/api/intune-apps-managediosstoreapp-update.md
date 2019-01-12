---
title: Обновление managedIOSStoreApp
description: Обновляет свойства объекта managedIOSStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75ee18a47c693c9099ccd18fb0b5434353c85397
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923371"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="030e8-103">Обновление managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="030e8-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="030e8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="030e8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="030e8-105">Обновляет свойства объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-105">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="030e8-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="030e8-106">Prerequisites</span></span>
<span data-ttu-id="030e8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="030e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="030e8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="030e8-109">Permission type</span></span>|<span data-ttu-id="030e8-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="030e8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="030e8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="030e8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="030e8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="030e8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="030e8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="030e8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="030e8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="030e8-114">Not supported.</span></span>|
|<span data-ttu-id="030e8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="030e8-115">Application</span></span>|<span data-ttu-id="030e8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="030e8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="030e8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="030e8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="030e8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="030e8-118">Request headers</span></span>
|<span data-ttu-id="030e8-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="030e8-119">Header</span></span>|<span data-ttu-id="030e8-120">Значение</span><span class="sxs-lookup"><span data-stu-id="030e8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="030e8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="030e8-121">Authorization</span></span>|<span data-ttu-id="030e8-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="030e8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="030e8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="030e8-123">Accept</span></span>|<span data-ttu-id="030e8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="030e8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="030e8-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="030e8-125">Request body</span></span>
<span data-ttu-id="030e8-126">В теле запроса добавьте представление объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="030e8-126">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="030e8-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-127">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="030e8-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="030e8-128">Property</span></span>|<span data-ttu-id="030e8-129">Тип</span><span class="sxs-lookup"><span data-stu-id="030e8-129">Type</span></span>|<span data-ttu-id="030e8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="030e8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="030e8-131">id</span><span class="sxs-lookup"><span data-stu-id="030e8-131">id</span></span>|<span data-ttu-id="030e8-132">Строка</span><span class="sxs-lookup"><span data-stu-id="030e8-132">String</span></span>|<span data-ttu-id="030e8-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="030e8-133">Key of the entity.</span></span> <span data-ttu-id="030e8-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-135">displayName</span><span class="sxs-lookup"><span data-stu-id="030e8-135">displayName</span></span>|<span data-ttu-id="030e8-136">String</span><span class="sxs-lookup"><span data-stu-id="030e8-136">String</span></span>|<span data-ttu-id="030e8-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="030e8-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="030e8-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-139">описание</span><span class="sxs-lookup"><span data-stu-id="030e8-139">description</span></span>|<span data-ttu-id="030e8-140">String</span><span class="sxs-lookup"><span data-stu-id="030e8-140">String</span></span>|<span data-ttu-id="030e8-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="030e8-141">The description of the app.</span></span> <span data-ttu-id="030e8-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-143">publisher</span><span class="sxs-lookup"><span data-stu-id="030e8-143">publisher</span></span>|<span data-ttu-id="030e8-144">String</span><span class="sxs-lookup"><span data-stu-id="030e8-144">String</span></span>|<span data-ttu-id="030e8-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="030e8-145">The publisher of the app.</span></span> <span data-ttu-id="030e8-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="030e8-147">largeIcon</span></span>|[<span data-ttu-id="030e8-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="030e8-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="030e8-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="030e8-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="030e8-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="030e8-151">createdDateTime</span></span>|<span data-ttu-id="030e8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="030e8-152">DateTimeOffset</span></span>|<span data-ttu-id="030e8-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="030e8-153">The date and time the app was created.</span></span> <span data-ttu-id="030e8-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="030e8-155">lastModifiedDateTime</span></span>|<span data-ttu-id="030e8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="030e8-156">DateTimeOffset</span></span>|<span data-ttu-id="030e8-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="030e8-157">The date and time the app was last modified.</span></span> <span data-ttu-id="030e8-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="030e8-159">isFeatured</span></span>|<span data-ttu-id="030e8-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="030e8-160">Boolean</span></span>|<span data-ttu-id="030e8-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="030e8-162">privacyInformationUrl</span></span>|<span data-ttu-id="030e8-163">String</span><span class="sxs-lookup"><span data-stu-id="030e8-163">String</span></span>|<span data-ttu-id="030e8-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="030e8-164">The privacy statement Url.</span></span> <span data-ttu-id="030e8-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="030e8-166">informationUrl</span></span>|<span data-ttu-id="030e8-167">String</span><span class="sxs-lookup"><span data-stu-id="030e8-167">String</span></span>|<span data-ttu-id="030e8-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="030e8-168">The more information Url.</span></span> <span data-ttu-id="030e8-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-170">owner</span><span class="sxs-lookup"><span data-stu-id="030e8-170">owner</span></span>|<span data-ttu-id="030e8-171">String</span><span class="sxs-lookup"><span data-stu-id="030e8-171">String</span></span>|<span data-ttu-id="030e8-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="030e8-172">The owner of the app.</span></span> <span data-ttu-id="030e8-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-174">developer</span><span class="sxs-lookup"><span data-stu-id="030e8-174">developer</span></span>|<span data-ttu-id="030e8-175">String</span><span class="sxs-lookup"><span data-stu-id="030e8-175">String</span></span>|<span data-ttu-id="030e8-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="030e8-176">The developer of the app.</span></span> <span data-ttu-id="030e8-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-178">notes</span><span class="sxs-lookup"><span data-stu-id="030e8-178">notes</span></span>|<span data-ttu-id="030e8-179">String</span><span class="sxs-lookup"><span data-stu-id="030e8-179">String</span></span>|<span data-ttu-id="030e8-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="030e8-180">Notes for the app.</span></span> <span data-ttu-id="030e8-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="030e8-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="030e8-182">publishingState</span></span>|[<span data-ttu-id="030e8-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="030e8-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="030e8-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="030e8-184">The publishing state for the app.</span></span> <span data-ttu-id="030e8-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="030e8-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="030e8-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="030e8-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="030e8-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="030e8-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="030e8-188">appAvailability</span></span>|[<span data-ttu-id="030e8-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="030e8-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="030e8-190">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="030e8-190">The Application's availability.</span></span> <span data-ttu-id="030e8-191">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="030e8-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="030e8-192">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="030e8-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="030e8-193">version</span><span class="sxs-lookup"><span data-stu-id="030e8-193">version</span></span>|<span data-ttu-id="030e8-194">String</span><span class="sxs-lookup"><span data-stu-id="030e8-194">String</span></span>|<span data-ttu-id="030e8-195">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="030e8-195">The Application's version.</span></span> <span data-ttu-id="030e8-196">Наследуется от [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="030e8-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="030e8-197">bundleId</span><span class="sxs-lookup"><span data-stu-id="030e8-197">bundleId</span></span>|<span data-ttu-id="030e8-198">String</span><span class="sxs-lookup"><span data-stu-id="030e8-198">String</span></span>|<span data-ttu-id="030e8-199">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="030e8-199">The app's Bundle ID.</span></span>|
|<span data-ttu-id="030e8-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="030e8-200">appStoreUrl</span></span>|<span data-ttu-id="030e8-201">String</span><span class="sxs-lookup"><span data-stu-id="030e8-201">String</span></span>|<span data-ttu-id="030e8-202">AppStoreUrl для Apple.</span><span class="sxs-lookup"><span data-stu-id="030e8-202">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="030e8-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="030e8-203">applicableDeviceType</span></span>|[<span data-ttu-id="030e8-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="030e8-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="030e8-205">Архитектура iOS, поддерживаемая этим приложением.</span><span class="sxs-lookup"><span data-stu-id="030e8-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="030e8-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="030e8-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="030e8-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="030e8-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="030e8-208">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="030e8-208">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="030e8-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="030e8-209">Response</span></span>
<span data-ttu-id="030e8-210">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="030e8-210">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="030e8-211">Пример</span><span class="sxs-lookup"><span data-stu-id="030e8-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="030e8-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="030e8-212">Request</span></span>
<span data-ttu-id="030e8-213">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="030e8-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1084

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="030e8-214">Ответ</span><span class="sxs-lookup"><span data-stu-id="030e8-214">Response</span></span>
<span data-ttu-id="030e8-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="030e8-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1256

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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



