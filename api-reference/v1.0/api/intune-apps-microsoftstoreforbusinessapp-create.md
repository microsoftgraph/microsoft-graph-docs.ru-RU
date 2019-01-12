---
title: Create microsoftStoreForBusinessApp
description: Создание объекта microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1f3a7147158ba0eb2e5df5c4199491225457ab8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972238"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="39a6d-103">Create microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="39a6d-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="39a6d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="39a6d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39a6d-105">Создание объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-105">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39a6d-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="39a6d-106">Prerequisites</span></span>
<span data-ttu-id="39a6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39a6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39a6d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39a6d-109">Permission type</span></span>|<span data-ttu-id="39a6d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39a6d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39a6d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39a6d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="39a6d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39a6d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="39a6d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39a6d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39a6d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39a6d-114">Not supported.</span></span>|
|<span data-ttu-id="39a6d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39a6d-115">Application</span></span>|<span data-ttu-id="39a6d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39a6d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39a6d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39a6d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="39a6d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39a6d-118">Request headers</span></span>
|<span data-ttu-id="39a6d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39a6d-119">Header</span></span>|<span data-ttu-id="39a6d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="39a6d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39a6d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="39a6d-121">Authorization</span></span>|<span data-ttu-id="39a6d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="39a6d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39a6d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="39a6d-123">Accept</span></span>|<span data-ttu-id="39a6d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="39a6d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39a6d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="39a6d-125">Request body</span></span>
<span data-ttu-id="39a6d-126">В тексте запроса добавьте представление объекта microsoftStoreForBusinessApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39a6d-126">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="39a6d-127">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="39a6d-127">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="39a6d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="39a6d-128">Property</span></span>|<span data-ttu-id="39a6d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="39a6d-129">Type</span></span>|<span data-ttu-id="39a6d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="39a6d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39a6d-131">id</span><span class="sxs-lookup"><span data-stu-id="39a6d-131">id</span></span>|<span data-ttu-id="39a6d-132">Строка</span><span class="sxs-lookup"><span data-stu-id="39a6d-132">String</span></span>|<span data-ttu-id="39a6d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="39a6d-133">Key of the entity.</span></span> <span data-ttu-id="39a6d-134">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="39a6d-135">displayName</span></span>|<span data-ttu-id="39a6d-136">String</span><span class="sxs-lookup"><span data-stu-id="39a6d-136">String</span></span>|<span data-ttu-id="39a6d-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="39a6d-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="39a6d-138">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-139">описание</span><span class="sxs-lookup"><span data-stu-id="39a6d-139">description</span></span>|<span data-ttu-id="39a6d-140">String</span><span class="sxs-lookup"><span data-stu-id="39a6d-140">String</span></span>|<span data-ttu-id="39a6d-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="39a6d-141">The description of the app.</span></span> <span data-ttu-id="39a6d-142">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-143">publisher</span><span class="sxs-lookup"><span data-stu-id="39a6d-143">publisher</span></span>|<span data-ttu-id="39a6d-144">String</span><span class="sxs-lookup"><span data-stu-id="39a6d-144">String</span></span>|<span data-ttu-id="39a6d-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="39a6d-145">The publisher of the app.</span></span> <span data-ttu-id="39a6d-146">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="39a6d-147">largeIcon</span></span>|[<span data-ttu-id="39a6d-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="39a6d-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="39a6d-149">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="39a6d-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="39a6d-150">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39a6d-151">createdDateTime</span></span>|<span data-ttu-id="39a6d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39a6d-152">DateTimeOffset</span></span>|<span data-ttu-id="39a6d-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="39a6d-153">The date and time the app was created.</span></span> <span data-ttu-id="39a6d-154">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39a6d-155">lastModifiedDateTime</span></span>|<span data-ttu-id="39a6d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39a6d-156">DateTimeOffset</span></span>|<span data-ttu-id="39a6d-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="39a6d-157">The date and time the app was last modified.</span></span> <span data-ttu-id="39a6d-158">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="39a6d-159">isFeatured</span></span>|<span data-ttu-id="39a6d-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="39a6d-160">Boolean</span></span>|<span data-ttu-id="39a6d-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="39a6d-162">privacyInformationUrl</span></span>|<span data-ttu-id="39a6d-163">String</span><span class="sxs-lookup"><span data-stu-id="39a6d-163">String</span></span>|<span data-ttu-id="39a6d-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="39a6d-164">The privacy statement Url.</span></span> <span data-ttu-id="39a6d-165">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="39a6d-166">informationUrl</span></span>|<span data-ttu-id="39a6d-167">String</span><span class="sxs-lookup"><span data-stu-id="39a6d-167">String</span></span>|<span data-ttu-id="39a6d-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="39a6d-168">The more information Url.</span></span> <span data-ttu-id="39a6d-169">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-170">owner</span><span class="sxs-lookup"><span data-stu-id="39a6d-170">owner</span></span>|<span data-ttu-id="39a6d-171">String</span><span class="sxs-lookup"><span data-stu-id="39a6d-171">String</span></span>|<span data-ttu-id="39a6d-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="39a6d-172">The owner of the app.</span></span> <span data-ttu-id="39a6d-173">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-174">developer</span><span class="sxs-lookup"><span data-stu-id="39a6d-174">developer</span></span>|<span data-ttu-id="39a6d-175">String</span><span class="sxs-lookup"><span data-stu-id="39a6d-175">String</span></span>|<span data-ttu-id="39a6d-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="39a6d-176">The developer of the app.</span></span> <span data-ttu-id="39a6d-177">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-178">notes</span><span class="sxs-lookup"><span data-stu-id="39a6d-178">notes</span></span>|<span data-ttu-id="39a6d-179">String</span><span class="sxs-lookup"><span data-stu-id="39a6d-179">String</span></span>|<span data-ttu-id="39a6d-180">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="39a6d-180">Notes for the app.</span></span> <span data-ttu-id="39a6d-181">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="39a6d-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="39a6d-182">publishingState</span></span>|[<span data-ttu-id="39a6d-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="39a6d-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="39a6d-184">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="39a6d-184">The publishing state for the app.</span></span> <span data-ttu-id="39a6d-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="39a6d-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="39a6d-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39a6d-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="39a6d-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="39a6d-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="39a6d-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="39a6d-188">usedLicenseCount</span></span>|<span data-ttu-id="39a6d-189">Int32</span><span class="sxs-lookup"><span data-stu-id="39a6d-189">Int32</span></span>|<span data-ttu-id="39a6d-190">Количество используемых лицензий Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="39a6d-190">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="39a6d-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="39a6d-191">totalLicenseCount</span></span>|<span data-ttu-id="39a6d-192">Int32</span><span class="sxs-lookup"><span data-stu-id="39a6d-192">Int32</span></span>|<span data-ttu-id="39a6d-193">Общее количество лицензий Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="39a6d-193">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="39a6d-194">productKey</span><span class="sxs-lookup"><span data-stu-id="39a6d-194">productKey</span></span>|<span data-ttu-id="39a6d-195">String</span><span class="sxs-lookup"><span data-stu-id="39a6d-195">String</span></span>|<span data-ttu-id="39a6d-196">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="39a6d-196">The app product key</span></span>|
|<span data-ttu-id="39a6d-197">licenseType</span><span class="sxs-lookup"><span data-stu-id="39a6d-197">licenseType</span></span>|[<span data-ttu-id="39a6d-198">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="39a6d-198">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="39a6d-199">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="39a6d-199">The app license type.</span></span> <span data-ttu-id="39a6d-200">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="39a6d-200">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="39a6d-201">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="39a6d-201">packageIdentityName</span></span>|<span data-ttu-id="39a6d-202">String</span><span class="sxs-lookup"><span data-stu-id="39a6d-202">String</span></span>|<span data-ttu-id="39a6d-203">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="39a6d-203">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="39a6d-204">Ответ</span><span class="sxs-lookup"><span data-stu-id="39a6d-204">Response</span></span>
<span data-ttu-id="39a6d-205">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="39a6d-205">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39a6d-206">Пример</span><span class="sxs-lookup"><span data-stu-id="39a6d-206">Example</span></span>
### <a name="request"></a><span data-ttu-id="39a6d-207">Запрос</span><span class="sxs-lookup"><span data-stu-id="39a6d-207">Request</span></span>
<span data-ttu-id="39a6d-208">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39a6d-208">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="39a6d-209">Ответ</span><span class="sxs-lookup"><span data-stu-id="39a6d-209">Response</span></span>
<span data-ttu-id="39a6d-p116">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="39a6d-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



