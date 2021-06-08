---
title: Create microsoftStoreForBusinessApp
description: Создание объекта microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7dccd660fb741254d4b600e73f35a17864a9ba29
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759772"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="eac8a-103">Create microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="eac8a-103">Create microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="eac8a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eac8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eac8a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eac8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eac8a-106">Создание объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eac8a-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="eac8a-107">Prerequisites</span></span>
<span data-ttu-id="eac8a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eac8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eac8a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eac8a-110">Permission type</span></span>|<span data-ttu-id="eac8a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eac8a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eac8a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eac8a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eac8a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eac8a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eac8a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eac8a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eac8a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eac8a-115">Not supported.</span></span>|
|<span data-ttu-id="eac8a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="eac8a-116">Application</span></span>|<span data-ttu-id="eac8a-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eac8a-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eac8a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eac8a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="eac8a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eac8a-119">Request headers</span></span>
|<span data-ttu-id="eac8a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eac8a-120">Header</span></span>|<span data-ttu-id="eac8a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eac8a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eac8a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eac8a-122">Authorization</span></span>|<span data-ttu-id="eac8a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eac8a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eac8a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eac8a-124">Accept</span></span>|<span data-ttu-id="eac8a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eac8a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eac8a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eac8a-126">Request body</span></span>
<span data-ttu-id="eac8a-127">В тексте запроса добавьте представление объекта microsoftStoreForBusinessApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eac8a-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="eac8a-128">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="eac8a-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="eac8a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="eac8a-129">Property</span></span>|<span data-ttu-id="eac8a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="eac8a-130">Type</span></span>|<span data-ttu-id="eac8a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="eac8a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eac8a-132">id</span><span class="sxs-lookup"><span data-stu-id="eac8a-132">id</span></span>|<span data-ttu-id="eac8a-133">String</span><span class="sxs-lookup"><span data-stu-id="eac8a-133">String</span></span>|<span data-ttu-id="eac8a-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eac8a-134">Key of the entity.</span></span> <span data-ttu-id="eac8a-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="eac8a-136">displayName</span></span>|<span data-ttu-id="eac8a-137">String</span><span class="sxs-lookup"><span data-stu-id="eac8a-137">String</span></span>|<span data-ttu-id="eac8a-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="eac8a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="eac8a-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-140">description</span><span class="sxs-lookup"><span data-stu-id="eac8a-140">description</span></span>|<span data-ttu-id="eac8a-141">String</span><span class="sxs-lookup"><span data-stu-id="eac8a-141">String</span></span>|<span data-ttu-id="eac8a-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="eac8a-142">The description of the app.</span></span> <span data-ttu-id="eac8a-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-144">publisher</span><span class="sxs-lookup"><span data-stu-id="eac8a-144">publisher</span></span>|<span data-ttu-id="eac8a-145">String</span><span class="sxs-lookup"><span data-stu-id="eac8a-145">String</span></span>|<span data-ttu-id="eac8a-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="eac8a-146">The publisher of the app.</span></span> <span data-ttu-id="eac8a-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="eac8a-148">largeIcon</span></span>|[<span data-ttu-id="eac8a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eac8a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eac8a-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="eac8a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="eac8a-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eac8a-152">createdDateTime</span></span>|<span data-ttu-id="eac8a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eac8a-153">DateTimeOffset</span></span>|<span data-ttu-id="eac8a-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="eac8a-154">The date and time the app was created.</span></span> <span data-ttu-id="eac8a-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eac8a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="eac8a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eac8a-157">DateTimeOffset</span></span>|<span data-ttu-id="eac8a-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="eac8a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="eac8a-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="eac8a-160">isFeatured</span></span>|<span data-ttu-id="eac8a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="eac8a-161">Boolean</span></span>|<span data-ttu-id="eac8a-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eac8a-163">privacyInformationUrl</span></span>|<span data-ttu-id="eac8a-164">String</span><span class="sxs-lookup"><span data-stu-id="eac8a-164">String</span></span>|<span data-ttu-id="eac8a-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="eac8a-165">The privacy statement Url.</span></span> <span data-ttu-id="eac8a-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eac8a-167">informationUrl</span></span>|<span data-ttu-id="eac8a-168">String</span><span class="sxs-lookup"><span data-stu-id="eac8a-168">String</span></span>|<span data-ttu-id="eac8a-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="eac8a-169">The more information Url.</span></span> <span data-ttu-id="eac8a-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-171">owner</span><span class="sxs-lookup"><span data-stu-id="eac8a-171">owner</span></span>|<span data-ttu-id="eac8a-172">String</span><span class="sxs-lookup"><span data-stu-id="eac8a-172">String</span></span>|<span data-ttu-id="eac8a-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="eac8a-173">The owner of the app.</span></span> <span data-ttu-id="eac8a-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-175">developer</span><span class="sxs-lookup"><span data-stu-id="eac8a-175">developer</span></span>|<span data-ttu-id="eac8a-176">String</span><span class="sxs-lookup"><span data-stu-id="eac8a-176">String</span></span>|<span data-ttu-id="eac8a-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="eac8a-177">The developer of the app.</span></span> <span data-ttu-id="eac8a-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-179">notes</span><span class="sxs-lookup"><span data-stu-id="eac8a-179">notes</span></span>|<span data-ttu-id="eac8a-180">String</span><span class="sxs-lookup"><span data-stu-id="eac8a-180">String</span></span>|<span data-ttu-id="eac8a-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="eac8a-181">Notes for the app.</span></span> <span data-ttu-id="eac8a-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eac8a-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="eac8a-183">publishingState</span></span>|[<span data-ttu-id="eac8a-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="eac8a-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="eac8a-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="eac8a-185">The publishing state for the app.</span></span> <span data-ttu-id="eac8a-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="eac8a-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="eac8a-187">Унаследованный от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="eac8a-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="eac8a-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="eac8a-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="eac8a-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="eac8a-189">usedLicenseCount</span></span>|<span data-ttu-id="eac8a-190">Int32</span><span class="sxs-lookup"><span data-stu-id="eac8a-190">Int32</span></span>|<span data-ttu-id="eac8a-191">Количество используемых лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="eac8a-191">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="eac8a-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="eac8a-192">totalLicenseCount</span></span>|<span data-ttu-id="eac8a-193">Int32</span><span class="sxs-lookup"><span data-stu-id="eac8a-193">Int32</span></span>|<span data-ttu-id="eac8a-194">Общее количество лицензий на Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="eac8a-194">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="eac8a-195">productKey</span><span class="sxs-lookup"><span data-stu-id="eac8a-195">productKey</span></span>|<span data-ttu-id="eac8a-196">String</span><span class="sxs-lookup"><span data-stu-id="eac8a-196">String</span></span>|<span data-ttu-id="eac8a-197">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="eac8a-197">The app product key</span></span>|
|<span data-ttu-id="eac8a-198">licenseType</span><span class="sxs-lookup"><span data-stu-id="eac8a-198">licenseType</span></span>|[<span data-ttu-id="eac8a-199">MicrosoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="eac8a-199">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="eac8a-200">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="eac8a-200">The app license type.</span></span> <span data-ttu-id="eac8a-201">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="eac8a-201">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="eac8a-202">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="eac8a-202">packageIdentityName</span></span>|<span data-ttu-id="eac8a-203">String</span><span class="sxs-lookup"><span data-stu-id="eac8a-203">String</span></span>|<span data-ttu-id="eac8a-204">Идентификатор пакета приложения</span><span class="sxs-lookup"><span data-stu-id="eac8a-204">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="eac8a-205">Ответ</span><span class="sxs-lookup"><span data-stu-id="eac8a-205">Response</span></span>
<span data-ttu-id="eac8a-206">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="eac8a-206">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eac8a-207">Пример</span><span class="sxs-lookup"><span data-stu-id="eac8a-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="eac8a-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="eac8a-208">Request</span></span>
<span data-ttu-id="eac8a-209">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eac8a-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="eac8a-210">Отклик</span><span class="sxs-lookup"><span data-stu-id="eac8a-210">Response</span></span>
<span data-ttu-id="eac8a-p116">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eac8a-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




