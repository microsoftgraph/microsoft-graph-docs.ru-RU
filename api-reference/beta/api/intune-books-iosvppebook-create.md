---
title: Create iosVppEBook
description: Создание объекта iosVppEBook.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4db5ede81c50e2161730995ec67087f7e3c28b5c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133677"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="0a708-103">Create iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="0a708-103">Create iosVppEBook</span></span>

<span data-ttu-id="0a708-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a708-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a708-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a708-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a708-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a708-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a708-107">Создание объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="0a708-107">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a708-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0a708-108">Prerequisites</span></span>
<span data-ttu-id="0a708-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a708-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a708-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a708-111">Permission type</span></span>|<span data-ttu-id="0a708-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a708-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a708-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a708-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a708-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a708-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0a708-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a708-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a708-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a708-116">Not supported.</span></span>|
|<span data-ttu-id="0a708-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0a708-117">Application</span></span>|<span data-ttu-id="0a708-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a708-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a708-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a708-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="0a708-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0a708-120">Request headers</span></span>
|<span data-ttu-id="0a708-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a708-121">Header</span></span>|<span data-ttu-id="0a708-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a708-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a708-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a708-123">Authorization</span></span>|<span data-ttu-id="0a708-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a708-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a708-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a708-125">Accept</span></span>|<span data-ttu-id="0a708-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a708-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a708-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a708-127">Request body</span></span>
<span data-ttu-id="0a708-128">В теле запроса добавьте представление объекта iosVppEBook в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a708-128">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="0a708-129">Ниже показаны свойства, которые необходимо указать при создании объекта iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="0a708-129">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="0a708-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a708-130">Property</span></span>|<span data-ttu-id="0a708-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0a708-131">Type</span></span>|<span data-ttu-id="0a708-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0a708-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a708-133">id</span><span class="sxs-lookup"><span data-stu-id="0a708-133">id</span></span>|<span data-ttu-id="0a708-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0a708-134">String</span></span>|<span data-ttu-id="0a708-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0a708-135">Key of the entity.</span></span> <span data-ttu-id="0a708-136">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="0a708-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="0a708-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0a708-137">displayName</span></span>|<span data-ttu-id="0a708-138">Строка</span><span class="sxs-lookup"><span data-stu-id="0a708-138">String</span></span>|<span data-ttu-id="0a708-139">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="0a708-139">Name of the eBook.</span></span> <span data-ttu-id="0a708-140">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="0a708-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="0a708-141">description</span><span class="sxs-lookup"><span data-stu-id="0a708-141">description</span></span>|<span data-ttu-id="0a708-142">Строка</span><span class="sxs-lookup"><span data-stu-id="0a708-142">String</span></span>|<span data-ttu-id="0a708-143">Описание.</span><span class="sxs-lookup"><span data-stu-id="0a708-143">Description.</span></span> <span data-ttu-id="0a708-144">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="0a708-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="0a708-145">publisher</span><span class="sxs-lookup"><span data-stu-id="0a708-145">publisher</span></span>|<span data-ttu-id="0a708-146">String</span><span class="sxs-lookup"><span data-stu-id="0a708-146">String</span></span>|<span data-ttu-id="0a708-147">Издатель.</span><span class="sxs-lookup"><span data-stu-id="0a708-147">Publisher.</span></span> <span data-ttu-id="0a708-148">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="0a708-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="0a708-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a708-149">publishedDateTime</span></span>|<span data-ttu-id="0a708-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a708-150">DateTimeOffset</span></span>|<span data-ttu-id="0a708-151">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="0a708-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="0a708-152">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="0a708-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="0a708-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="0a708-153">largeCover</span></span>|[<span data-ttu-id="0a708-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0a708-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0a708-155">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="0a708-155">Book cover.</span></span> <span data-ttu-id="0a708-156">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="0a708-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="0a708-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a708-157">createdDateTime</span></span>|<span data-ttu-id="0a708-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a708-158">DateTimeOffset</span></span>|<span data-ttu-id="0a708-159">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="0a708-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="0a708-160">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="0a708-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="0a708-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a708-161">lastModifiedDateTime</span></span>|<span data-ttu-id="0a708-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a708-162">DateTimeOffset</span></span>|<span data-ttu-id="0a708-163">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="0a708-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="0a708-164">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="0a708-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="0a708-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0a708-165">informationUrl</span></span>|<span data-ttu-id="0a708-166">String</span><span class="sxs-lookup"><span data-stu-id="0a708-166">String</span></span>|<span data-ttu-id="0a708-167">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="0a708-167">The more information Url.</span></span> <span data-ttu-id="0a708-168">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="0a708-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="0a708-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0a708-169">privacyInformationUrl</span></span>|<span data-ttu-id="0a708-170">String</span><span class="sxs-lookup"><span data-stu-id="0a708-170">String</span></span>|<span data-ttu-id="0a708-171">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="0a708-171">The privacy statement Url.</span></span> <span data-ttu-id="0a708-172">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="0a708-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="0a708-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="0a708-173">vppTokenId</span></span>|<span data-ttu-id="0a708-174">Guid</span><span class="sxs-lookup"><span data-stu-id="0a708-174">Guid</span></span>|<span data-ttu-id="0a708-175">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="0a708-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="0a708-176">appleId</span><span class="sxs-lookup"><span data-stu-id="0a708-176">appleId</span></span>|<span data-ttu-id="0a708-177">String</span><span class="sxs-lookup"><span data-stu-id="0a708-177">String</span></span>|<span data-ttu-id="0a708-178">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="0a708-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="0a708-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="0a708-179">vppOrganizationName</span></span>|<span data-ttu-id="0a708-180">String</span><span class="sxs-lookup"><span data-stu-id="0a708-180">String</span></span>|<span data-ttu-id="0a708-181">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="0a708-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="0a708-182">genres</span><span class="sxs-lookup"><span data-stu-id="0a708-182">genres</span></span>|<span data-ttu-id="0a708-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0a708-183">String collection</span></span>|<span data-ttu-id="0a708-184">Жанры.</span><span class="sxs-lookup"><span data-stu-id="0a708-184">Genres.</span></span>|
|<span data-ttu-id="0a708-185">language</span><span class="sxs-lookup"><span data-stu-id="0a708-185">language</span></span>|<span data-ttu-id="0a708-186">String</span><span class="sxs-lookup"><span data-stu-id="0a708-186">String</span></span>|<span data-ttu-id="0a708-187">Язык.</span><span class="sxs-lookup"><span data-stu-id="0a708-187">Language.</span></span>|
|<span data-ttu-id="0a708-188">seller</span><span class="sxs-lookup"><span data-stu-id="0a708-188">seller</span></span>|<span data-ttu-id="0a708-189">String</span><span class="sxs-lookup"><span data-stu-id="0a708-189">String</span></span>|<span data-ttu-id="0a708-190">Продавец.</span><span class="sxs-lookup"><span data-stu-id="0a708-190">Seller.</span></span>|
|<span data-ttu-id="0a708-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="0a708-191">totalLicenseCount</span></span>|<span data-ttu-id="0a708-192">Int32</span><span class="sxs-lookup"><span data-stu-id="0a708-192">Int32</span></span>|<span data-ttu-id="0a708-193">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="0a708-193">Total license count.</span></span>|
|<span data-ttu-id="0a708-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="0a708-194">usedLicenseCount</span></span>|<span data-ttu-id="0a708-195">Int32</span><span class="sxs-lookup"><span data-stu-id="0a708-195">Int32</span></span>|<span data-ttu-id="0a708-196">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="0a708-196">Used license count.</span></span>|
|<span data-ttu-id="0a708-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0a708-197">roleScopeTagIds</span></span>|<span data-ttu-id="0a708-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0a708-198">String collection</span></span>|<span data-ttu-id="0a708-199">Список тегов области для этого экземпляра Entity.</span><span class="sxs-lookup"><span data-stu-id="0a708-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="0a708-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="0a708-200">Response</span></span>
<span data-ttu-id="0a708-201">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0a708-201">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a708-202">Пример</span><span class="sxs-lookup"><span data-stu-id="0a708-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a708-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a708-203">Request</span></span>
<span data-ttu-id="0a708-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a708-204">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 854

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
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="0a708-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a708-205">Response</span></span>
<span data-ttu-id="0a708-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a708-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1026

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
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




