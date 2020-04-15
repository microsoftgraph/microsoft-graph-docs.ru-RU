---
title: Update microsoftStoreForBusinessApp
description: Обновление свойств объекта microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5463470cc0fd9fb67fc693b2678cfa190fdefe91
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411649"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="0e3dd-103">Update microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="0e3dd-103">Update microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="0e3dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e3dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e3dd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e3dd-106">Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-106">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e3dd-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0e3dd-107">Prerequisites</span></span>
<span data-ttu-id="0e3dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e3dd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e3dd-110">Permission type</span></span>|<span data-ttu-id="0e3dd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e3dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e3dd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e3dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e3dd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e3dd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0e3dd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e3dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e3dd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-115">Not supported.</span></span>|
|<span data-ttu-id="0e3dd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e3dd-116">Application</span></span>|<span data-ttu-id="0e3dd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e3dd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e3dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="0e3dd-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0e3dd-119">Request headers</span></span>
|<span data-ttu-id="0e3dd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e3dd-120">Header</span></span>|<span data-ttu-id="0e3dd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0e3dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e3dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e3dd-122">Authorization</span></span>|<span data-ttu-id="0e3dd-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e3dd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0e3dd-124">Accept</span></span>|<span data-ttu-id="0e3dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e3dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e3dd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0e3dd-126">Request body</span></span>
<span data-ttu-id="0e3dd-127">В теле запроса добавьте представление объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="0e3dd-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="0e3dd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e3dd-129">Property</span></span>|<span data-ttu-id="0e3dd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0e3dd-130">Type</span></span>|<span data-ttu-id="0e3dd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0e3dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e3dd-132">id</span><span class="sxs-lookup"><span data-stu-id="0e3dd-132">id</span></span>|<span data-ttu-id="0e3dd-133">Строка</span><span class="sxs-lookup"><span data-stu-id="0e3dd-133">String</span></span>|<span data-ttu-id="0e3dd-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-134">Key of the entity.</span></span> <span data-ttu-id="0e3dd-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0e3dd-136">displayName</span></span>|<span data-ttu-id="0e3dd-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0e3dd-137">String</span></span>|<span data-ttu-id="0e3dd-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0e3dd-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-140">description</span><span class="sxs-lookup"><span data-stu-id="0e3dd-140">description</span></span>|<span data-ttu-id="0e3dd-141">String</span><span class="sxs-lookup"><span data-stu-id="0e3dd-141">String</span></span>|<span data-ttu-id="0e3dd-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-142">The description of the app.</span></span> <span data-ttu-id="0e3dd-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-144">publisher</span><span class="sxs-lookup"><span data-stu-id="0e3dd-144">publisher</span></span>|<span data-ttu-id="0e3dd-145">String</span><span class="sxs-lookup"><span data-stu-id="0e3dd-145">String</span></span>|<span data-ttu-id="0e3dd-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-146">The publisher of the app.</span></span> <span data-ttu-id="0e3dd-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0e3dd-148">largeIcon</span></span>|[<span data-ttu-id="0e3dd-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0e3dd-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0e3dd-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0e3dd-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e3dd-152">createdDateTime</span></span>|<span data-ttu-id="0e3dd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3dd-153">DateTimeOffset</span></span>|<span data-ttu-id="0e3dd-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-154">The date and time the app was created.</span></span> <span data-ttu-id="0e3dd-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e3dd-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0e3dd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3dd-157">DateTimeOffset</span></span>|<span data-ttu-id="0e3dd-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0e3dd-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0e3dd-160">isFeatured</span></span>|<span data-ttu-id="0e3dd-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e3dd-161">Boolean</span></span>|<span data-ttu-id="0e3dd-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0e3dd-163">privacyInformationUrl</span></span>|<span data-ttu-id="0e3dd-164">String</span><span class="sxs-lookup"><span data-stu-id="0e3dd-164">String</span></span>|<span data-ttu-id="0e3dd-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-165">The privacy statement Url.</span></span> <span data-ttu-id="0e3dd-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0e3dd-167">informationUrl</span></span>|<span data-ttu-id="0e3dd-168">String</span><span class="sxs-lookup"><span data-stu-id="0e3dd-168">String</span></span>|<span data-ttu-id="0e3dd-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-169">The more information Url.</span></span> <span data-ttu-id="0e3dd-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-171">owner</span><span class="sxs-lookup"><span data-stu-id="0e3dd-171">owner</span></span>|<span data-ttu-id="0e3dd-172">String</span><span class="sxs-lookup"><span data-stu-id="0e3dd-172">String</span></span>|<span data-ttu-id="0e3dd-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-173">The owner of the app.</span></span> <span data-ttu-id="0e3dd-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-175">developer</span><span class="sxs-lookup"><span data-stu-id="0e3dd-175">developer</span></span>|<span data-ttu-id="0e3dd-176">String</span><span class="sxs-lookup"><span data-stu-id="0e3dd-176">String</span></span>|<span data-ttu-id="0e3dd-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-177">The developer of the app.</span></span> <span data-ttu-id="0e3dd-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-179">notes</span><span class="sxs-lookup"><span data-stu-id="0e3dd-179">notes</span></span>|<span data-ttu-id="0e3dd-180">String</span><span class="sxs-lookup"><span data-stu-id="0e3dd-180">String</span></span>|<span data-ttu-id="0e3dd-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-181">Notes for the app.</span></span> <span data-ttu-id="0e3dd-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0e3dd-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="0e3dd-183">publishingState</span></span>|[<span data-ttu-id="0e3dd-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="0e3dd-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0e3dd-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-185">The publishing state for the app.</span></span> <span data-ttu-id="0e3dd-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0e3dd-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0e3dd-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0e3dd-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0e3dd-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="0e3dd-189">usedLicenseCount</span></span>|<span data-ttu-id="0e3dd-190">Int32</span><span class="sxs-lookup"><span data-stu-id="0e3dd-190">Int32</span></span>|<span data-ttu-id="0e3dd-191">Количество используемых лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-191">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="0e3dd-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="0e3dd-192">totalLicenseCount</span></span>|<span data-ttu-id="0e3dd-193">Int32</span><span class="sxs-lookup"><span data-stu-id="0e3dd-193">Int32</span></span>|<span data-ttu-id="0e3dd-194">Общее количество лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-194">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="0e3dd-195">productKey</span><span class="sxs-lookup"><span data-stu-id="0e3dd-195">productKey</span></span>|<span data-ttu-id="0e3dd-196">Строка</span><span class="sxs-lookup"><span data-stu-id="0e3dd-196">String</span></span>|<span data-ttu-id="0e3dd-197">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-197">The app product key</span></span>|
|<span data-ttu-id="0e3dd-198">licenseType</span><span class="sxs-lookup"><span data-stu-id="0e3dd-198">licenseType</span></span>|[<span data-ttu-id="0e3dd-199">микрософтсторефорбусинесслиценсетипе</span><span class="sxs-lookup"><span data-stu-id="0e3dd-199">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="0e3dd-200">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-200">The app license type.</span></span> <span data-ttu-id="0e3dd-201">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-201">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="0e3dd-202">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="0e3dd-202">packageIdentityName</span></span>|<span data-ttu-id="0e3dd-203">String</span><span class="sxs-lookup"><span data-stu-id="0e3dd-203">String</span></span>|<span data-ttu-id="0e3dd-204">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="0e3dd-204">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="0e3dd-205">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e3dd-205">Response</span></span>
<span data-ttu-id="0e3dd-206">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-206">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e3dd-207">Пример</span><span class="sxs-lookup"><span data-stu-id="0e3dd-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e3dd-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e3dd-208">Request</span></span>
<span data-ttu-id="0e3dd-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 769

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="0e3dd-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e3dd-210">Response</span></span>
<span data-ttu-id="0e3dd-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0e3dd-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```






