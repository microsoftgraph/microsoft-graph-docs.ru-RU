---
title: Создание объекта androidStoreApp
description: Создание объекта androidStoreApp.
author: tfitzmac
ms.openlocfilehash: 3a28a00433d6a5cda83892efcc12284f7c10480a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358669"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="c5ec8-103">Создание объекта androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="c5ec8-103">Create androidStoreApp</span></span>

> <span data-ttu-id="c5ec8-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5ec8-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5ec8-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5ec8-107">Создание объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-107">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5ec8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c5ec8-108">Prerequisites</span></span>
<span data-ttu-id="c5ec8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5ec8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5ec8-111">Permission type</span></span>|<span data-ttu-id="c5ec8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5ec8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5ec8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5ec8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5ec8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5ec8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5ec8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5ec8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5ec8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-116">Not supported.</span></span>|
|<span data-ttu-id="c5ec8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5ec8-117">Application</span></span>|<span data-ttu-id="c5ec8-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5ec8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5ec8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c5ec8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5ec8-120">Request headers</span></span>
|<span data-ttu-id="c5ec8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5ec8-121">Header</span></span>|<span data-ttu-id="c5ec8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5ec8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5ec8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c5ec8-123">Authorization</span></span>|<span data-ttu-id="c5ec8-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c5ec8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5ec8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5ec8-125">Accept</span></span>|<span data-ttu-id="c5ec8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5ec8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5ec8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5ec8-127">Request body</span></span>
<span data-ttu-id="c5ec8-128">В тексте запроса добавьте представление объекта androidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-128">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="c5ec8-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-129">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="c5ec8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5ec8-130">Property</span></span>|<span data-ttu-id="c5ec8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5ec8-131">Type</span></span>|<span data-ttu-id="c5ec8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5ec8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5ec8-133">id</span><span class="sxs-lookup"><span data-stu-id="c5ec8-133">id</span></span>|<span data-ttu-id="c5ec8-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c5ec8-134">String</span></span>|<span data-ttu-id="c5ec8-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-135">Key of the entity.</span></span> <span data-ttu-id="c5ec8-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c5ec8-137">displayName</span></span>|<span data-ttu-id="c5ec8-138">String</span><span class="sxs-lookup"><span data-stu-id="c5ec8-138">String</span></span>|<span data-ttu-id="c5ec8-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c5ec8-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-141">описание</span><span class="sxs-lookup"><span data-stu-id="c5ec8-141">description</span></span>|<span data-ttu-id="c5ec8-142">String</span><span class="sxs-lookup"><span data-stu-id="c5ec8-142">String</span></span>|<span data-ttu-id="c5ec8-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-143">The description of the app.</span></span> <span data-ttu-id="c5ec8-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c5ec8-145">publisher</span></span>|<span data-ttu-id="c5ec8-146">String</span><span class="sxs-lookup"><span data-stu-id="c5ec8-146">String</span></span>|<span data-ttu-id="c5ec8-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-147">The publisher of the app.</span></span> <span data-ttu-id="c5ec8-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c5ec8-149">largeIcon</span></span>|[<span data-ttu-id="c5ec8-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c5ec8-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c5ec8-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c5ec8-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5ec8-153">createdDateTime</span></span>|<span data-ttu-id="c5ec8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5ec8-154">DateTimeOffset</span></span>|<span data-ttu-id="c5ec8-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-155">The date and time the app was created.</span></span> <span data-ttu-id="c5ec8-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5ec8-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c5ec8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5ec8-158">DateTimeOffset</span></span>|<span data-ttu-id="c5ec8-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c5ec8-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c5ec8-161">isFeatured</span></span>|<span data-ttu-id="c5ec8-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5ec8-162">Boolean</span></span>|<span data-ttu-id="c5ec8-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c5ec8-164">privacyInformationUrl</span></span>|<span data-ttu-id="c5ec8-165">String</span><span class="sxs-lookup"><span data-stu-id="c5ec8-165">String</span></span>|<span data-ttu-id="c5ec8-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-166">The privacy statement Url.</span></span> <span data-ttu-id="c5ec8-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c5ec8-168">informationUrl</span></span>|<span data-ttu-id="c5ec8-169">String</span><span class="sxs-lookup"><span data-stu-id="c5ec8-169">String</span></span>|<span data-ttu-id="c5ec8-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-170">The more information Url.</span></span> <span data-ttu-id="c5ec8-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-172">owner</span><span class="sxs-lookup"><span data-stu-id="c5ec8-172">owner</span></span>|<span data-ttu-id="c5ec8-173">String</span><span class="sxs-lookup"><span data-stu-id="c5ec8-173">String</span></span>|<span data-ttu-id="c5ec8-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-174">The owner of the app.</span></span> <span data-ttu-id="c5ec8-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-176">developer</span><span class="sxs-lookup"><span data-stu-id="c5ec8-176">developer</span></span>|<span data-ttu-id="c5ec8-177">String</span><span class="sxs-lookup"><span data-stu-id="c5ec8-177">String</span></span>|<span data-ttu-id="c5ec8-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-178">The developer of the app.</span></span> <span data-ttu-id="c5ec8-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-180">notes</span><span class="sxs-lookup"><span data-stu-id="c5ec8-180">notes</span></span>|<span data-ttu-id="c5ec8-181">String</span><span class="sxs-lookup"><span data-stu-id="c5ec8-181">String</span></span>|<span data-ttu-id="c5ec8-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-182">Notes for the app.</span></span> <span data-ttu-id="c5ec8-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c5ec8-184">uploadState</span></span>|<span data-ttu-id="c5ec8-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c5ec8-185">Int32</span></span>|<span data-ttu-id="c5ec8-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-186">The upload state.</span></span> <span data-ttu-id="c5ec8-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5ec8-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c5ec8-188">publishingState</span></span>|[<span data-ttu-id="c5ec8-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c5ec8-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c5ec8-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-190">The publishing state for the app.</span></span> <span data-ttu-id="c5ec8-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c5ec8-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c5ec8-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c5ec8-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c5ec8-194">packageId</span><span class="sxs-lookup"><span data-stu-id="c5ec8-194">packageId</span></span>|<span data-ttu-id="c5ec8-195">String</span><span class="sxs-lookup"><span data-stu-id="c5ec8-195">String</span></span>|<span data-ttu-id="c5ec8-196">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-196">The package identifier.</span></span>|
|<span data-ttu-id="c5ec8-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c5ec8-197">appIdentifier</span></span>|<span data-ttu-id="c5ec8-198">String</span><span class="sxs-lookup"><span data-stu-id="c5ec8-198">String</span></span>|<span data-ttu-id="c5ec8-199">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-199">The Identity Name.</span></span>|
|<span data-ttu-id="c5ec8-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c5ec8-200">appStoreUrl</span></span>|<span data-ttu-id="c5ec8-201">String</span><span class="sxs-lookup"><span data-stu-id="c5ec8-201">String</span></span>|<span data-ttu-id="c5ec8-202">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-202">The Android app store URL.</span></span>|
|<span data-ttu-id="c5ec8-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c5ec8-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c5ec8-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c5ec8-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="c5ec8-205">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-205">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="c5ec8-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="c5ec8-206">Response</span></span>
<span data-ttu-id="c5ec8-207">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-207">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5ec8-208">Пример</span><span class="sxs-lookup"><span data-stu-id="c5ec8-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5ec8-209">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5ec8-209">Request</span></span>
<span data-ttu-id="c5ec8-210">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-210">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1182

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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

### <a name="response"></a><span data-ttu-id="c5ec8-211">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5ec8-211">Response</span></span>
<span data-ttu-id="c5ec8-p117">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c5ec8-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





