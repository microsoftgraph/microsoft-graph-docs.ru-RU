---
title: Создание объекта androidStoreApp
description: Создание объекта androidStoreApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fa67da6ecbf1a2d0b508c228265998b69b86c4f3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401938"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="99460-103">Создание объекта androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="99460-103">Create androidStoreApp</span></span>

> <span data-ttu-id="99460-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="99460-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="99460-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99460-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99460-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99460-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99460-107">Создание объекта [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-107">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99460-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="99460-108">Prerequisites</span></span>
<span data-ttu-id="99460-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="99460-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="99460-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99460-111">Permission type</span></span>|<span data-ttu-id="99460-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="99460-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99460-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99460-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99460-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99460-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="99460-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99460-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99460-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99460-116">Not supported.</span></span>|
|<span data-ttu-id="99460-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99460-117">Application</span></span>|<span data-ttu-id="99460-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99460-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99460-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99460-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="99460-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99460-120">Request headers</span></span>
|<span data-ttu-id="99460-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99460-121">Header</span></span>|<span data-ttu-id="99460-122">Значение</span><span class="sxs-lookup"><span data-stu-id="99460-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99460-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99460-123">Authorization</span></span>|<span data-ttu-id="99460-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="99460-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99460-125">Accept</span><span class="sxs-lookup"><span data-stu-id="99460-125">Accept</span></span>|<span data-ttu-id="99460-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99460-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99460-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="99460-127">Request body</span></span>
<span data-ttu-id="99460-128">В тексте запроса добавьте представление объекта androidStoreApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99460-128">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="99460-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="99460-129">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="99460-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="99460-130">Property</span></span>|<span data-ttu-id="99460-131">Тип</span><span class="sxs-lookup"><span data-stu-id="99460-131">Type</span></span>|<span data-ttu-id="99460-132">Описание</span><span class="sxs-lookup"><span data-stu-id="99460-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99460-133">id</span><span class="sxs-lookup"><span data-stu-id="99460-133">id</span></span>|<span data-ttu-id="99460-134">String</span><span class="sxs-lookup"><span data-stu-id="99460-134">String</span></span>|<span data-ttu-id="99460-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="99460-135">Key of the entity.</span></span> <span data-ttu-id="99460-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-137">displayName</span><span class="sxs-lookup"><span data-stu-id="99460-137">displayName</span></span>|<span data-ttu-id="99460-138">String</span><span class="sxs-lookup"><span data-stu-id="99460-138">String</span></span>|<span data-ttu-id="99460-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="99460-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="99460-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-141">description</span><span class="sxs-lookup"><span data-stu-id="99460-141">description</span></span>|<span data-ttu-id="99460-142">String</span><span class="sxs-lookup"><span data-stu-id="99460-142">String</span></span>|<span data-ttu-id="99460-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="99460-143">The description of the app.</span></span> <span data-ttu-id="99460-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-145">publisher</span><span class="sxs-lookup"><span data-stu-id="99460-145">publisher</span></span>|<span data-ttu-id="99460-146">String</span><span class="sxs-lookup"><span data-stu-id="99460-146">String</span></span>|<span data-ttu-id="99460-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="99460-147">The publisher of the app.</span></span> <span data-ttu-id="99460-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="99460-149">largeIcon</span></span>|[<span data-ttu-id="99460-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="99460-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="99460-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="99460-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="99460-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99460-153">createdDateTime</span></span>|<span data-ttu-id="99460-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99460-154">DateTimeOffset</span></span>|<span data-ttu-id="99460-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="99460-155">The date and time the app was created.</span></span> <span data-ttu-id="99460-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99460-157">lastModifiedDateTime</span></span>|<span data-ttu-id="99460-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99460-158">DateTimeOffset</span></span>|<span data-ttu-id="99460-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="99460-159">The date and time the app was last modified.</span></span> <span data-ttu-id="99460-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="99460-161">isFeatured</span></span>|<span data-ttu-id="99460-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="99460-162">Boolean</span></span>|<span data-ttu-id="99460-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="99460-164">privacyInformationUrl</span></span>|<span data-ttu-id="99460-165">String</span><span class="sxs-lookup"><span data-stu-id="99460-165">String</span></span>|<span data-ttu-id="99460-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="99460-166">The privacy statement Url.</span></span> <span data-ttu-id="99460-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="99460-168">informationUrl</span></span>|<span data-ttu-id="99460-169">String</span><span class="sxs-lookup"><span data-stu-id="99460-169">String</span></span>|<span data-ttu-id="99460-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="99460-170">The more information Url.</span></span> <span data-ttu-id="99460-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-172">owner</span><span class="sxs-lookup"><span data-stu-id="99460-172">owner</span></span>|<span data-ttu-id="99460-173">String</span><span class="sxs-lookup"><span data-stu-id="99460-173">String</span></span>|<span data-ttu-id="99460-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="99460-174">The owner of the app.</span></span> <span data-ttu-id="99460-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-176">developer</span><span class="sxs-lookup"><span data-stu-id="99460-176">developer</span></span>|<span data-ttu-id="99460-177">String</span><span class="sxs-lookup"><span data-stu-id="99460-177">String</span></span>|<span data-ttu-id="99460-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="99460-178">The developer of the app.</span></span> <span data-ttu-id="99460-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-180">notes</span><span class="sxs-lookup"><span data-stu-id="99460-180">notes</span></span>|<span data-ttu-id="99460-181">String</span><span class="sxs-lookup"><span data-stu-id="99460-181">String</span></span>|<span data-ttu-id="99460-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="99460-182">Notes for the app.</span></span> <span data-ttu-id="99460-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="99460-184">uploadState</span></span>|<span data-ttu-id="99460-185">Int32</span><span class="sxs-lookup"><span data-stu-id="99460-185">Int32</span></span>|<span data-ttu-id="99460-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="99460-186">The upload state.</span></span> <span data-ttu-id="99460-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="99460-188">publishingState</span></span>|[<span data-ttu-id="99460-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="99460-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="99460-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="99460-190">The publishing state for the app.</span></span> <span data-ttu-id="99460-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="99460-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="99460-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="99460-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="99460-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="99460-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="99460-194">isAssigned</span></span>|<span data-ttu-id="99460-195">Логический</span><span class="sxs-lookup"><span data-stu-id="99460-195">Boolean</span></span>|<span data-ttu-id="99460-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="99460-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="99460-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="99460-198">roleScopeTagIds</span></span>|<span data-ttu-id="99460-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="99460-199">String collection</span></span>|<span data-ttu-id="99460-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="99460-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="99460-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="99460-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="99460-202">packageId</span><span class="sxs-lookup"><span data-stu-id="99460-202">packageId</span></span>|<span data-ttu-id="99460-203">String</span><span class="sxs-lookup"><span data-stu-id="99460-203">String</span></span>|<span data-ttu-id="99460-204">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="99460-204">The package identifier.</span></span>|
|<span data-ttu-id="99460-205">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="99460-205">appIdentifier</span></span>|<span data-ttu-id="99460-206">String</span><span class="sxs-lookup"><span data-stu-id="99460-206">String</span></span>|<span data-ttu-id="99460-207">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="99460-207">The Identity Name.</span></span>|
|<span data-ttu-id="99460-208">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="99460-208">appStoreUrl</span></span>|<span data-ttu-id="99460-209">String</span><span class="sxs-lookup"><span data-stu-id="99460-209">String</span></span>|<span data-ttu-id="99460-210">URL-адрес магазина приложений для Android.</span><span class="sxs-lookup"><span data-stu-id="99460-210">The Android app store URL.</span></span>|
|<span data-ttu-id="99460-211">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="99460-211">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="99460-212">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="99460-212">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="99460-213">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="99460-213">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="99460-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="99460-214">Response</span></span>
<span data-ttu-id="99460-215">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidStoreApp](../resources/intune-apps-androidstoreapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="99460-215">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99460-216">Пример</span><span class="sxs-lookup"><span data-stu-id="99460-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="99460-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="99460-217">Request</span></span>
<span data-ttu-id="99460-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99460-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1203

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

### <a name="response"></a><span data-ttu-id="99460-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="99460-219">Response</span></span>
<span data-ttu-id="99460-p119">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="99460-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1375

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




