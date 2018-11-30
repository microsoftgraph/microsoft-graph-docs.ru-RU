---
title: Create managedAndroidStoreApp
description: Создание нового объекта managedAndroidStoreApp.
ms.openlocfilehash: 10f343b694f7e852eff28be1182f335e1a723a34
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081261"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="0479f-103">Create managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="0479f-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="0479f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0479f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0479f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0479f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0479f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0479f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0479f-107">Создание нового объекта [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-107">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0479f-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0479f-108">Prerequisites</span></span>
<span data-ttu-id="0479f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0479f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0479f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0479f-111">Permission type</span></span>|<span data-ttu-id="0479f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0479f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0479f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0479f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0479f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0479f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0479f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0479f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0479f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0479f-116">Not supported.</span></span>|
|<span data-ttu-id="0479f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0479f-117">Application</span></span>|<span data-ttu-id="0479f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0479f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0479f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0479f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0479f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0479f-120">Request headers</span></span>
|<span data-ttu-id="0479f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0479f-121">Header</span></span>|<span data-ttu-id="0479f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0479f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0479f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0479f-123">Authorization</span></span>|<span data-ttu-id="0479f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0479f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0479f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0479f-125">Accept</span></span>|<span data-ttu-id="0479f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0479f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0479f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0479f-127">Request body</span></span>
<span data-ttu-id="0479f-128">В теле запроса добавьте представление объекта managedAndroidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0479f-128">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="0479f-129">Ниже показаны свойства, которые необходимо указывать при создании объекта managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="0479f-129">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="0479f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0479f-130">Property</span></span>|<span data-ttu-id="0479f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0479f-131">Type</span></span>|<span data-ttu-id="0479f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0479f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0479f-133">id</span><span class="sxs-lookup"><span data-stu-id="0479f-133">id</span></span>|<span data-ttu-id="0479f-134">String</span><span class="sxs-lookup"><span data-stu-id="0479f-134">String</span></span>|<span data-ttu-id="0479f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0479f-135">Key of the entity.</span></span> <span data-ttu-id="0479f-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0479f-137">displayName</span></span>|<span data-ttu-id="0479f-138">String</span><span class="sxs-lookup"><span data-stu-id="0479f-138">String</span></span>|<span data-ttu-id="0479f-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="0479f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0479f-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-141">описание</span><span class="sxs-lookup"><span data-stu-id="0479f-141">description</span></span>|<span data-ttu-id="0479f-142">String</span><span class="sxs-lookup"><span data-stu-id="0479f-142">String</span></span>|<span data-ttu-id="0479f-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="0479f-143">The description of the app.</span></span> <span data-ttu-id="0479f-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="0479f-145">publisher</span></span>|<span data-ttu-id="0479f-146">String</span><span class="sxs-lookup"><span data-stu-id="0479f-146">String</span></span>|<span data-ttu-id="0479f-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="0479f-147">The publisher of the app.</span></span> <span data-ttu-id="0479f-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0479f-149">largeIcon</span></span>|[<span data-ttu-id="0479f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0479f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0479f-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="0479f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0479f-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0479f-153">createdDateTime</span></span>|<span data-ttu-id="0479f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0479f-154">DateTimeOffset</span></span>|<span data-ttu-id="0479f-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="0479f-155">The date and time the app was created.</span></span> <span data-ttu-id="0479f-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0479f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="0479f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0479f-158">DateTimeOffset</span></span>|<span data-ttu-id="0479f-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="0479f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="0479f-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0479f-161">isFeatured</span></span>|<span data-ttu-id="0479f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0479f-162">Boolean</span></span>|<span data-ttu-id="0479f-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0479f-164">privacyInformationUrl</span></span>|<span data-ttu-id="0479f-165">String</span><span class="sxs-lookup"><span data-stu-id="0479f-165">String</span></span>|<span data-ttu-id="0479f-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="0479f-166">The privacy statement Url.</span></span> <span data-ttu-id="0479f-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0479f-168">informationUrl</span></span>|<span data-ttu-id="0479f-169">String</span><span class="sxs-lookup"><span data-stu-id="0479f-169">String</span></span>|<span data-ttu-id="0479f-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="0479f-170">The more information Url.</span></span> <span data-ttu-id="0479f-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-172">owner</span><span class="sxs-lookup"><span data-stu-id="0479f-172">owner</span></span>|<span data-ttu-id="0479f-173">String</span><span class="sxs-lookup"><span data-stu-id="0479f-173">String</span></span>|<span data-ttu-id="0479f-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="0479f-174">The owner of the app.</span></span> <span data-ttu-id="0479f-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-176">developer</span><span class="sxs-lookup"><span data-stu-id="0479f-176">developer</span></span>|<span data-ttu-id="0479f-177">String</span><span class="sxs-lookup"><span data-stu-id="0479f-177">String</span></span>|<span data-ttu-id="0479f-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="0479f-178">The developer of the app.</span></span> <span data-ttu-id="0479f-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-180">notes</span><span class="sxs-lookup"><span data-stu-id="0479f-180">notes</span></span>|<span data-ttu-id="0479f-181">String</span><span class="sxs-lookup"><span data-stu-id="0479f-181">String</span></span>|<span data-ttu-id="0479f-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="0479f-182">Notes for the app.</span></span> <span data-ttu-id="0479f-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="0479f-184">uploadState</span></span>|<span data-ttu-id="0479f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0479f-185">Int32</span></span>|<span data-ttu-id="0479f-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="0479f-186">The upload state.</span></span> <span data-ttu-id="0479f-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0479f-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="0479f-188">publishingState</span></span>|[<span data-ttu-id="0479f-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0479f-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0479f-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="0479f-190">The publishing state for the app.</span></span> <span data-ttu-id="0479f-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="0479f-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0479f-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0479f-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0479f-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0479f-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="0479f-194">appAvailability</span></span>|[<span data-ttu-id="0479f-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="0479f-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="0479f-196">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="0479f-196">The Application's availability.</span></span> <span data-ttu-id="0479f-197">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="0479f-198">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="0479f-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="0479f-199">version</span><span class="sxs-lookup"><span data-stu-id="0479f-199">version</span></span>|<span data-ttu-id="0479f-200">String</span><span class="sxs-lookup"><span data-stu-id="0479f-200">String</span></span>|<span data-ttu-id="0479f-201">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="0479f-201">The Application's version.</span></span> <span data-ttu-id="0479f-202">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="0479f-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="0479f-203">packageId</span><span class="sxs-lookup"><span data-stu-id="0479f-203">packageId</span></span>|<span data-ttu-id="0479f-204">String</span><span class="sxs-lookup"><span data-stu-id="0479f-204">String</span></span>|<span data-ttu-id="0479f-205">ИД пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="0479f-205">The app's package ID.</span></span>|
|<span data-ttu-id="0479f-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0479f-206">appStoreUrl</span></span>|<span data-ttu-id="0479f-207">String</span><span class="sxs-lookup"><span data-stu-id="0479f-207">String</span></span>|<span data-ttu-id="0479f-208">AppStoreUrl для Android.</span><span class="sxs-lookup"><span data-stu-id="0479f-208">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="0479f-209">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0479f-209">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0479f-210">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0479f-210">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="0479f-211">Значение, которое представляет минимальную поддерживаемую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="0479f-211">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="0479f-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="0479f-212">Response</span></span>
<span data-ttu-id="0479f-213">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0479f-213">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0479f-214">Пример</span><span class="sxs-lookup"><span data-stu-id="0479f-214">Example</span></span>
### <a name="request"></a><span data-ttu-id="0479f-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="0479f-215">Request</span></span>
<span data-ttu-id="0479f-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0479f-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1216

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
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

### <a name="response"></a><span data-ttu-id="0479f-217">Ответ</span><span class="sxs-lookup"><span data-stu-id="0479f-217">Response</span></span>
<span data-ttu-id="0479f-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="0479f-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1324

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "packageId": "Package Id value",
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





