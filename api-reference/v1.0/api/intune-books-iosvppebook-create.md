---
title: Create iosVppEBook
description: Создание объекта iosVppEBook.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2baa0da642f5335ed804d9b0b3861aa8fd4ebe51
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515674"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="87bc4-103">Create iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="87bc4-103">Create iosVppEBook</span></span>

<span data-ttu-id="87bc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87bc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87bc4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87bc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87bc4-106">Создание объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="87bc4-106">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87bc4-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="87bc4-107">Prerequisites</span></span>
<span data-ttu-id="87bc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87bc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87bc4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87bc4-110">Permission type</span></span>|<span data-ttu-id="87bc4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="87bc4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87bc4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87bc4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="87bc4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87bc4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="87bc4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87bc4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87bc4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87bc4-115">Not supported.</span></span>|
|<span data-ttu-id="87bc4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87bc4-116">Application</span></span>|<span data-ttu-id="87bc4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87bc4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87bc4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87bc4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="87bc4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="87bc4-119">Request headers</span></span>
|<span data-ttu-id="87bc4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87bc4-120">Header</span></span>|<span data-ttu-id="87bc4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="87bc4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87bc4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="87bc4-122">Authorization</span></span>|<span data-ttu-id="87bc4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87bc4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87bc4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="87bc4-124">Accept</span></span>|<span data-ttu-id="87bc4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="87bc4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87bc4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87bc4-126">Request body</span></span>
<span data-ttu-id="87bc4-127">В теле запроса добавьте представление объекта iosVppEBook в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87bc4-127">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="87bc4-128">Ниже показаны свойства, которые необходимо указать при создании объекта iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="87bc4-128">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="87bc4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="87bc4-129">Property</span></span>|<span data-ttu-id="87bc4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="87bc4-130">Type</span></span>|<span data-ttu-id="87bc4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="87bc4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87bc4-132">id</span><span class="sxs-lookup"><span data-stu-id="87bc4-132">id</span></span>|<span data-ttu-id="87bc4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="87bc4-133">String</span></span>|<span data-ttu-id="87bc4-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="87bc4-134">Key of the entity.</span></span> <span data-ttu-id="87bc4-135">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="87bc4-135">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="87bc4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="87bc4-136">displayName</span></span>|<span data-ttu-id="87bc4-137">Строка</span><span class="sxs-lookup"><span data-stu-id="87bc4-137">String</span></span>|<span data-ttu-id="87bc4-138">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="87bc4-138">Name of the eBook.</span></span> <span data-ttu-id="87bc4-139">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="87bc4-139">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="87bc4-140">description</span><span class="sxs-lookup"><span data-stu-id="87bc4-140">description</span></span>|<span data-ttu-id="87bc4-141">String</span><span class="sxs-lookup"><span data-stu-id="87bc4-141">String</span></span>|<span data-ttu-id="87bc4-142">Описание.</span><span class="sxs-lookup"><span data-stu-id="87bc4-142">Description.</span></span> <span data-ttu-id="87bc4-143">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="87bc4-143">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="87bc4-144">publisher</span><span class="sxs-lookup"><span data-stu-id="87bc4-144">publisher</span></span>|<span data-ttu-id="87bc4-145">Строка</span><span class="sxs-lookup"><span data-stu-id="87bc4-145">String</span></span>|<span data-ttu-id="87bc4-146">Издатель.</span><span class="sxs-lookup"><span data-stu-id="87bc4-146">Publisher.</span></span> <span data-ttu-id="87bc4-147">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="87bc4-147">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="87bc4-148">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="87bc4-148">publishedDateTime</span></span>|<span data-ttu-id="87bc4-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87bc4-149">DateTimeOffset</span></span>|<span data-ttu-id="87bc4-150">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="87bc4-150">The date and time when the eBook was published.</span></span> <span data-ttu-id="87bc4-151">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="87bc4-151">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="87bc4-152">largeCover</span><span class="sxs-lookup"><span data-stu-id="87bc4-152">largeCover</span></span>|[<span data-ttu-id="87bc4-153">mimeContent</span><span class="sxs-lookup"><span data-stu-id="87bc4-153">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="87bc4-154">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="87bc4-154">Book cover.</span></span> <span data-ttu-id="87bc4-155">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="87bc4-155">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="87bc4-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87bc4-156">createdDateTime</span></span>|<span data-ttu-id="87bc4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87bc4-157">DateTimeOffset</span></span>|<span data-ttu-id="87bc4-158">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="87bc4-158">The date and time when the eBook file was created.</span></span> <span data-ttu-id="87bc4-159">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="87bc4-159">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="87bc4-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87bc4-160">lastModifiedDateTime</span></span>|<span data-ttu-id="87bc4-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87bc4-161">DateTimeOffset</span></span>|<span data-ttu-id="87bc4-162">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="87bc4-162">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="87bc4-163">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="87bc4-163">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="87bc4-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="87bc4-164">informationUrl</span></span>|<span data-ttu-id="87bc4-165">Строка</span><span class="sxs-lookup"><span data-stu-id="87bc4-165">String</span></span>|<span data-ttu-id="87bc4-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="87bc4-166">The more information Url.</span></span> <span data-ttu-id="87bc4-167">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="87bc4-167">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="87bc4-168">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="87bc4-168">privacyInformationUrl</span></span>|<span data-ttu-id="87bc4-169">Строка</span><span class="sxs-lookup"><span data-stu-id="87bc4-169">String</span></span>|<span data-ttu-id="87bc4-170">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="87bc4-170">The privacy statement Url.</span></span> <span data-ttu-id="87bc4-171">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="87bc4-171">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="87bc4-172">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="87bc4-172">vppTokenId</span></span>|<span data-ttu-id="87bc4-173">Guid</span><span class="sxs-lookup"><span data-stu-id="87bc4-173">Guid</span></span>|<span data-ttu-id="87bc4-174">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="87bc4-174">The Vpp token ID.</span></span>|
|<span data-ttu-id="87bc4-175">appleId</span><span class="sxs-lookup"><span data-stu-id="87bc4-175">appleId</span></span>|<span data-ttu-id="87bc4-176">Строка</span><span class="sxs-lookup"><span data-stu-id="87bc4-176">String</span></span>|<span data-ttu-id="87bc4-177">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="87bc4-177">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="87bc4-178">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="87bc4-178">vppOrganizationName</span></span>|<span data-ttu-id="87bc4-179">Строка</span><span class="sxs-lookup"><span data-stu-id="87bc4-179">String</span></span>|<span data-ttu-id="87bc4-180">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="87bc4-180">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="87bc4-181">genres</span><span class="sxs-lookup"><span data-stu-id="87bc4-181">genres</span></span>|<span data-ttu-id="87bc4-182">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="87bc4-182">String collection</span></span>|<span data-ttu-id="87bc4-183">Жанры.</span><span class="sxs-lookup"><span data-stu-id="87bc4-183">Genres.</span></span>|
|<span data-ttu-id="87bc4-184">language</span><span class="sxs-lookup"><span data-stu-id="87bc4-184">language</span></span>|<span data-ttu-id="87bc4-185">Строка</span><span class="sxs-lookup"><span data-stu-id="87bc4-185">String</span></span>|<span data-ttu-id="87bc4-186">Язык.</span><span class="sxs-lookup"><span data-stu-id="87bc4-186">Language.</span></span>|
|<span data-ttu-id="87bc4-187">seller</span><span class="sxs-lookup"><span data-stu-id="87bc4-187">seller</span></span>|<span data-ttu-id="87bc4-188">String</span><span class="sxs-lookup"><span data-stu-id="87bc4-188">String</span></span>|<span data-ttu-id="87bc4-189">Продавец.</span><span class="sxs-lookup"><span data-stu-id="87bc4-189">Seller.</span></span>|
|<span data-ttu-id="87bc4-190">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="87bc4-190">totalLicenseCount</span></span>|<span data-ttu-id="87bc4-191">Int32</span><span class="sxs-lookup"><span data-stu-id="87bc4-191">Int32</span></span>|<span data-ttu-id="87bc4-192">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="87bc4-192">Total license count.</span></span>|
|<span data-ttu-id="87bc4-193">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="87bc4-193">usedLicenseCount</span></span>|<span data-ttu-id="87bc4-194">Int32</span><span class="sxs-lookup"><span data-stu-id="87bc4-194">Int32</span></span>|<span data-ttu-id="87bc4-195">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="87bc4-195">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="87bc4-196">Ответ</span><span class="sxs-lookup"><span data-stu-id="87bc4-196">Response</span></span>
<span data-ttu-id="87bc4-197">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="87bc4-197">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87bc4-198">Пример</span><span class="sxs-lookup"><span data-stu-id="87bc4-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="87bc4-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="87bc4-199">Request</span></span>
<span data-ttu-id="87bc4-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87bc4-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="87bc4-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="87bc4-201">Response</span></span>
<span data-ttu-id="87bc4-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="87bc4-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




