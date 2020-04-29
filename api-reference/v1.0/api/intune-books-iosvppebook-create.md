---
title: Create iosVppEBook
description: Создание объекта iosVppEBook.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a7b7fe4f5bb7e264be2b9e48db5372380833e7e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43356007"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="e9eeb-103">Create iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="e9eeb-103">Create iosVppEBook</span></span>

<span data-ttu-id="e9eeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9eeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9eeb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9eeb-106">Создание объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="e9eeb-106">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9eeb-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e9eeb-107">Prerequisites</span></span>
<span data-ttu-id="e9eeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e9eeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9eeb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e9eeb-110">Permission type</span></span>|<span data-ttu-id="e9eeb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e9eeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9eeb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e9eeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e9eeb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9eeb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e9eeb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e9eeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9eeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-115">Not supported.</span></span>|
|<span data-ttu-id="e9eeb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e9eeb-116">Application</span></span>|<span data-ttu-id="e9eeb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9eeb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e9eeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="e9eeb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e9eeb-119">Request headers</span></span>
|<span data-ttu-id="e9eeb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e9eeb-120">Header</span></span>|<span data-ttu-id="e9eeb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e9eeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9eeb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e9eeb-122">Authorization</span></span>|<span data-ttu-id="e9eeb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9eeb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e9eeb-124">Accept</span></span>|<span data-ttu-id="e9eeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e9eeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9eeb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e9eeb-126">Request body</span></span>
<span data-ttu-id="e9eeb-127">В теле запроса добавьте представление объекта iosVppEBook в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-127">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="e9eeb-128">Ниже показаны свойства, которые необходимо указать при создании объекта iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-128">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="e9eeb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9eeb-129">Property</span></span>|<span data-ttu-id="e9eeb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e9eeb-130">Type</span></span>|<span data-ttu-id="e9eeb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e9eeb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9eeb-132">id</span><span class="sxs-lookup"><span data-stu-id="e9eeb-132">id</span></span>|<span data-ttu-id="e9eeb-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e9eeb-133">String</span></span>|<span data-ttu-id="e9eeb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-134">Key of the entity.</span></span> <span data-ttu-id="e9eeb-135">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="e9eeb-135">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e9eeb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e9eeb-136">displayName</span></span>|<span data-ttu-id="e9eeb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="e9eeb-137">String</span></span>|<span data-ttu-id="e9eeb-138">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-138">Name of the eBook.</span></span> <span data-ttu-id="e9eeb-139">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="e9eeb-139">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e9eeb-140">description</span><span class="sxs-lookup"><span data-stu-id="e9eeb-140">description</span></span>|<span data-ttu-id="e9eeb-141">String</span><span class="sxs-lookup"><span data-stu-id="e9eeb-141">String</span></span>|<span data-ttu-id="e9eeb-142">Описание.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-142">Description.</span></span> <span data-ttu-id="e9eeb-143">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="e9eeb-143">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e9eeb-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e9eeb-144">publisher</span></span>|<span data-ttu-id="e9eeb-145">String</span><span class="sxs-lookup"><span data-stu-id="e9eeb-145">String</span></span>|<span data-ttu-id="e9eeb-146">Издатель.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-146">Publisher.</span></span> <span data-ttu-id="e9eeb-147">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="e9eeb-147">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e9eeb-148">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9eeb-148">publishedDateTime</span></span>|<span data-ttu-id="e9eeb-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9eeb-149">DateTimeOffset</span></span>|<span data-ttu-id="e9eeb-150">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-150">The date and time when the eBook was published.</span></span> <span data-ttu-id="e9eeb-151">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="e9eeb-151">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e9eeb-152">largeCover</span><span class="sxs-lookup"><span data-stu-id="e9eeb-152">largeCover</span></span>|[<span data-ttu-id="e9eeb-153">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e9eeb-153">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e9eeb-154">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-154">Book cover.</span></span> <span data-ttu-id="e9eeb-155">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="e9eeb-155">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e9eeb-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9eeb-156">createdDateTime</span></span>|<span data-ttu-id="e9eeb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9eeb-157">DateTimeOffset</span></span>|<span data-ttu-id="e9eeb-158">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-158">The date and time when the eBook file was created.</span></span> <span data-ttu-id="e9eeb-159">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="e9eeb-159">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e9eeb-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9eeb-160">lastModifiedDateTime</span></span>|<span data-ttu-id="e9eeb-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9eeb-161">DateTimeOffset</span></span>|<span data-ttu-id="e9eeb-162">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-162">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="e9eeb-163">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="e9eeb-163">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e9eeb-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e9eeb-164">informationUrl</span></span>|<span data-ttu-id="e9eeb-165">String</span><span class="sxs-lookup"><span data-stu-id="e9eeb-165">String</span></span>|<span data-ttu-id="e9eeb-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-166">The more information Url.</span></span> <span data-ttu-id="e9eeb-167">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="e9eeb-167">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e9eeb-168">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e9eeb-168">privacyInformationUrl</span></span>|<span data-ttu-id="e9eeb-169">String</span><span class="sxs-lookup"><span data-stu-id="e9eeb-169">String</span></span>|<span data-ttu-id="e9eeb-170">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-170">The privacy statement Url.</span></span> <span data-ttu-id="e9eeb-171">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="e9eeb-171">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="e9eeb-172">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="e9eeb-172">vppTokenId</span></span>|<span data-ttu-id="e9eeb-173">Guid</span><span class="sxs-lookup"><span data-stu-id="e9eeb-173">Guid</span></span>|<span data-ttu-id="e9eeb-174">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-174">The Vpp token ID.</span></span>|
|<span data-ttu-id="e9eeb-175">appleId</span><span class="sxs-lookup"><span data-stu-id="e9eeb-175">appleId</span></span>|<span data-ttu-id="e9eeb-176">Строка</span><span class="sxs-lookup"><span data-stu-id="e9eeb-176">String</span></span>|<span data-ttu-id="e9eeb-177">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-177">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="e9eeb-178">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="e9eeb-178">vppOrganizationName</span></span>|<span data-ttu-id="e9eeb-179">String</span><span class="sxs-lookup"><span data-stu-id="e9eeb-179">String</span></span>|<span data-ttu-id="e9eeb-180">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-180">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="e9eeb-181">genres</span><span class="sxs-lookup"><span data-stu-id="e9eeb-181">genres</span></span>|<span data-ttu-id="e9eeb-182">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e9eeb-182">String collection</span></span>|<span data-ttu-id="e9eeb-183">Жанры.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-183">Genres.</span></span>|
|<span data-ttu-id="e9eeb-184">language</span><span class="sxs-lookup"><span data-stu-id="e9eeb-184">language</span></span>|<span data-ttu-id="e9eeb-185">String</span><span class="sxs-lookup"><span data-stu-id="e9eeb-185">String</span></span>|<span data-ttu-id="e9eeb-186">Язык.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-186">Language.</span></span>|
|<span data-ttu-id="e9eeb-187">seller</span><span class="sxs-lookup"><span data-stu-id="e9eeb-187">seller</span></span>|<span data-ttu-id="e9eeb-188">String</span><span class="sxs-lookup"><span data-stu-id="e9eeb-188">String</span></span>|<span data-ttu-id="e9eeb-189">Продавец.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-189">Seller.</span></span>|
|<span data-ttu-id="e9eeb-190">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e9eeb-190">totalLicenseCount</span></span>|<span data-ttu-id="e9eeb-191">Int32</span><span class="sxs-lookup"><span data-stu-id="e9eeb-191">Int32</span></span>|<span data-ttu-id="e9eeb-192">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-192">Total license count.</span></span>|
|<span data-ttu-id="e9eeb-193">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e9eeb-193">usedLicenseCount</span></span>|<span data-ttu-id="e9eeb-194">Int32</span><span class="sxs-lookup"><span data-stu-id="e9eeb-194">Int32</span></span>|<span data-ttu-id="e9eeb-195">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-195">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="e9eeb-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="e9eeb-196">Response</span></span>
<span data-ttu-id="e9eeb-197">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-197">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9eeb-198">Пример</span><span class="sxs-lookup"><span data-stu-id="e9eeb-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9eeb-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="e9eeb-199">Request</span></span>
<span data-ttu-id="e9eeb-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```

### <a name="response"></a><span data-ttu-id="e9eeb-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="e9eeb-201">Response</span></span>
<span data-ttu-id="e9eeb-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e9eeb-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```






