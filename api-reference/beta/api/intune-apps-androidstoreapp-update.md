---
title: Update androidStoreApp
description: Обновление свойств объекта androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4ff090e0ebee3da71b44060d7d20c6b27d213668
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984425"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="8df3f-103">Update androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="8df3f-103">Update androidStoreApp</span></span>

> <span data-ttu-id="8df3f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8df3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8df3f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8df3f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8df3f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8df3f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8df3f-107">Обновление свойств объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-107">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8df3f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8df3f-108">Prerequisites</span></span>
<span data-ttu-id="8df3f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8df3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8df3f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8df3f-111">Permission type</span></span>|<span data-ttu-id="8df3f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8df3f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8df3f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8df3f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8df3f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8df3f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8df3f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8df3f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8df3f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8df3f-116">Not supported.</span></span>|
|<span data-ttu-id="8df3f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8df3f-117">Application</span></span>|<span data-ttu-id="8df3f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8df3f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8df3f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8df3f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8df3f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8df3f-120">Request headers</span></span>
|<span data-ttu-id="8df3f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8df3f-121">Header</span></span>|<span data-ttu-id="8df3f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8df3f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8df3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8df3f-123">Authorization</span></span>|<span data-ttu-id="8df3f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="8df3f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8df3f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8df3f-125">Accept</span></span>|<span data-ttu-id="8df3f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8df3f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8df3f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8df3f-127">Request body</span></span>
<span data-ttu-id="8df3f-128">В теле запроса добавьте представление объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8df3f-128">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="8df3f-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-129">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="8df3f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8df3f-130">Property</span></span>|<span data-ttu-id="8df3f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8df3f-131">Type</span></span>|<span data-ttu-id="8df3f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8df3f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8df3f-133">id</span><span class="sxs-lookup"><span data-stu-id="8df3f-133">id</span></span>|<span data-ttu-id="8df3f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8df3f-134">String</span></span>|<span data-ttu-id="8df3f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8df3f-135">Key of the entity.</span></span> <span data-ttu-id="8df3f-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8df3f-137">displayName</span></span>|<span data-ttu-id="8df3f-138">String</span><span class="sxs-lookup"><span data-stu-id="8df3f-138">String</span></span>|<span data-ttu-id="8df3f-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="8df3f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8df3f-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-141">описание</span><span class="sxs-lookup"><span data-stu-id="8df3f-141">description</span></span>|<span data-ttu-id="8df3f-142">String</span><span class="sxs-lookup"><span data-stu-id="8df3f-142">String</span></span>|<span data-ttu-id="8df3f-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="8df3f-143">The description of the app.</span></span> <span data-ttu-id="8df3f-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8df3f-145">publisher</span></span>|<span data-ttu-id="8df3f-146">String</span><span class="sxs-lookup"><span data-stu-id="8df3f-146">String</span></span>|<span data-ttu-id="8df3f-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="8df3f-147">The publisher of the app.</span></span> <span data-ttu-id="8df3f-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8df3f-149">largeIcon</span></span>|[<span data-ttu-id="8df3f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8df3f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8df3f-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="8df3f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8df3f-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8df3f-153">createdDateTime</span></span>|<span data-ttu-id="8df3f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8df3f-154">DateTimeOffset</span></span>|<span data-ttu-id="8df3f-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="8df3f-155">The date and time the app was created.</span></span> <span data-ttu-id="8df3f-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8df3f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8df3f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8df3f-158">DateTimeOffset</span></span>|<span data-ttu-id="8df3f-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="8df3f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8df3f-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8df3f-161">isFeatured</span></span>|<span data-ttu-id="8df3f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8df3f-162">Boolean</span></span>|<span data-ttu-id="8df3f-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8df3f-164">privacyInformationUrl</span></span>|<span data-ttu-id="8df3f-165">String</span><span class="sxs-lookup"><span data-stu-id="8df3f-165">String</span></span>|<span data-ttu-id="8df3f-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8df3f-166">The privacy statement Url.</span></span> <span data-ttu-id="8df3f-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8df3f-168">informationUrl</span></span>|<span data-ttu-id="8df3f-169">String</span><span class="sxs-lookup"><span data-stu-id="8df3f-169">String</span></span>|<span data-ttu-id="8df3f-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="8df3f-170">The more information Url.</span></span> <span data-ttu-id="8df3f-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-172">owner</span><span class="sxs-lookup"><span data-stu-id="8df3f-172">owner</span></span>|<span data-ttu-id="8df3f-173">String</span><span class="sxs-lookup"><span data-stu-id="8df3f-173">String</span></span>|<span data-ttu-id="8df3f-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="8df3f-174">The owner of the app.</span></span> <span data-ttu-id="8df3f-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-176">developer</span><span class="sxs-lookup"><span data-stu-id="8df3f-176">developer</span></span>|<span data-ttu-id="8df3f-177">String</span><span class="sxs-lookup"><span data-stu-id="8df3f-177">String</span></span>|<span data-ttu-id="8df3f-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="8df3f-178">The developer of the app.</span></span> <span data-ttu-id="8df3f-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-180">notes</span><span class="sxs-lookup"><span data-stu-id="8df3f-180">notes</span></span>|<span data-ttu-id="8df3f-181">String</span><span class="sxs-lookup"><span data-stu-id="8df3f-181">String</span></span>|<span data-ttu-id="8df3f-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="8df3f-182">Notes for the app.</span></span> <span data-ttu-id="8df3f-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8df3f-184">uploadState</span></span>|<span data-ttu-id="8df3f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8df3f-185">Int32</span></span>|<span data-ttu-id="8df3f-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="8df3f-186">The upload state.</span></span> <span data-ttu-id="8df3f-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8df3f-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8df3f-188">publishingState</span></span>|[<span data-ttu-id="8df3f-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8df3f-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8df3f-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="8df3f-190">The publishing state for the app.</span></span> <span data-ttu-id="8df3f-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="8df3f-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8df3f-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8df3f-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8df3f-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8df3f-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8df3f-194">packageId</span><span class="sxs-lookup"><span data-stu-id="8df3f-194">packageId</span></span>|<span data-ttu-id="8df3f-195">String</span><span class="sxs-lookup"><span data-stu-id="8df3f-195">String</span></span>|<span data-ttu-id="8df3f-196">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="8df3f-196">The package identifier.</span></span>|
|<span data-ttu-id="8df3f-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="8df3f-197">appIdentifier</span></span>|<span data-ttu-id="8df3f-198">String</span><span class="sxs-lookup"><span data-stu-id="8df3f-198">String</span></span>|<span data-ttu-id="8df3f-199">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="8df3f-199">The Identity Name.</span></span>|
|<span data-ttu-id="8df3f-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8df3f-200">appStoreUrl</span></span>|<span data-ttu-id="8df3f-201">String</span><span class="sxs-lookup"><span data-stu-id="8df3f-201">String</span></span>|<span data-ttu-id="8df3f-202">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="8df3f-202">The Android app store URL.</span></span>|
|<span data-ttu-id="8df3f-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8df3f-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8df3f-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8df3f-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="8df3f-205">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="8df3f-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="8df3f-206">Ответ</span><span class="sxs-lookup"><span data-stu-id="8df3f-206">Response</span></span>
<span data-ttu-id="8df3f-207">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8df3f-207">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8df3f-208">Пример</span><span class="sxs-lookup"><span data-stu-id="8df3f-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="8df3f-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="8df3f-209">Request</span></span>
<span data-ttu-id="8df3f-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8df3f-210">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8df3f-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="8df3f-211">Response</span></span>
<span data-ttu-id="8df3f-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8df3f-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





