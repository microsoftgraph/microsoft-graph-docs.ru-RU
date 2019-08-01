---
title: Обновление объекта iosVppEBook
description: Обновление свойств объекта iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d68b8ba149b4b5f8b63029df98769d37a5fdd8c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001882"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="05b70-103">Обновление объекта iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="05b70-103">Update iosVppEBook</span></span>

> <span data-ttu-id="05b70-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05b70-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05b70-105">Обновление свойств объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="05b70-105">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05b70-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="05b70-106">Prerequisites</span></span>
<span data-ttu-id="05b70-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05b70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05b70-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05b70-109">Permission type</span></span>|<span data-ttu-id="05b70-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05b70-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05b70-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05b70-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05b70-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05b70-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05b70-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05b70-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05b70-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05b70-114">Not supported.</span></span>|
|<span data-ttu-id="05b70-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05b70-115">Application</span></span>|<span data-ttu-id="05b70-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05b70-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05b70-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05b70-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="05b70-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05b70-118">Request headers</span></span>
|<span data-ttu-id="05b70-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05b70-119">Header</span></span>|<span data-ttu-id="05b70-120">Значение</span><span class="sxs-lookup"><span data-stu-id="05b70-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05b70-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05b70-121">Authorization</span></span>|<span data-ttu-id="05b70-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05b70-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05b70-123">Accept</span><span class="sxs-lookup"><span data-stu-id="05b70-123">Accept</span></span>|<span data-ttu-id="05b70-124">application/json</span><span class="sxs-lookup"><span data-stu-id="05b70-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05b70-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05b70-125">Request body</span></span>
<span data-ttu-id="05b70-126">В теле запроса добавьте представление объекта [iosVppEBook](../resources/intune-books-iosvppebook.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05b70-126">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="05b70-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="05b70-127">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="05b70-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="05b70-128">Property</span></span>|<span data-ttu-id="05b70-129">Тип</span><span class="sxs-lookup"><span data-stu-id="05b70-129">Type</span></span>|<span data-ttu-id="05b70-130">Описание</span><span class="sxs-lookup"><span data-stu-id="05b70-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05b70-131">id</span><span class="sxs-lookup"><span data-stu-id="05b70-131">id</span></span>|<span data-ttu-id="05b70-132">Строка</span><span class="sxs-lookup"><span data-stu-id="05b70-132">String</span></span>|<span data-ttu-id="05b70-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="05b70-133">Key of the entity.</span></span> <span data-ttu-id="05b70-134">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="05b70-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="05b70-135">displayName</span><span class="sxs-lookup"><span data-stu-id="05b70-135">displayName</span></span>|<span data-ttu-id="05b70-136">Строка</span><span class="sxs-lookup"><span data-stu-id="05b70-136">String</span></span>|<span data-ttu-id="05b70-137">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="05b70-137">Name of the eBook.</span></span> <span data-ttu-id="05b70-138">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="05b70-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="05b70-139">description</span><span class="sxs-lookup"><span data-stu-id="05b70-139">description</span></span>|<span data-ttu-id="05b70-140">String</span><span class="sxs-lookup"><span data-stu-id="05b70-140">String</span></span>|<span data-ttu-id="05b70-141">Описание.</span><span class="sxs-lookup"><span data-stu-id="05b70-141">Description.</span></span> <span data-ttu-id="05b70-142">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="05b70-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="05b70-143">publisher</span><span class="sxs-lookup"><span data-stu-id="05b70-143">publisher</span></span>|<span data-ttu-id="05b70-144">String</span><span class="sxs-lookup"><span data-stu-id="05b70-144">String</span></span>|<span data-ttu-id="05b70-145">Издатель.</span><span class="sxs-lookup"><span data-stu-id="05b70-145">Publisher.</span></span> <span data-ttu-id="05b70-146">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="05b70-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="05b70-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="05b70-147">publishedDateTime</span></span>|<span data-ttu-id="05b70-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05b70-148">DateTimeOffset</span></span>|<span data-ttu-id="05b70-149">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="05b70-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="05b70-150">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="05b70-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="05b70-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="05b70-151">largeCover</span></span>|[<span data-ttu-id="05b70-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="05b70-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="05b70-153">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="05b70-153">Book cover.</span></span> <span data-ttu-id="05b70-154">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="05b70-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="05b70-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05b70-155">createdDateTime</span></span>|<span data-ttu-id="05b70-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05b70-156">DateTimeOffset</span></span>|<span data-ttu-id="05b70-157">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="05b70-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="05b70-158">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="05b70-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="05b70-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05b70-159">lastModifiedDateTime</span></span>|<span data-ttu-id="05b70-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05b70-160">DateTimeOffset</span></span>|<span data-ttu-id="05b70-161">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="05b70-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="05b70-162">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="05b70-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="05b70-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="05b70-163">informationUrl</span></span>|<span data-ttu-id="05b70-164">String</span><span class="sxs-lookup"><span data-stu-id="05b70-164">String</span></span>|<span data-ttu-id="05b70-165">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="05b70-165">The more information Url.</span></span> <span data-ttu-id="05b70-166">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="05b70-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="05b70-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="05b70-167">privacyInformationUrl</span></span>|<span data-ttu-id="05b70-168">String</span><span class="sxs-lookup"><span data-stu-id="05b70-168">String</span></span>|<span data-ttu-id="05b70-169">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="05b70-169">The privacy statement Url.</span></span> <span data-ttu-id="05b70-170">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="05b70-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="05b70-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="05b70-171">vppTokenId</span></span>|<span data-ttu-id="05b70-172">Guid</span><span class="sxs-lookup"><span data-stu-id="05b70-172">Guid</span></span>|<span data-ttu-id="05b70-173">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="05b70-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="05b70-174">appleId</span><span class="sxs-lookup"><span data-stu-id="05b70-174">appleId</span></span>|<span data-ttu-id="05b70-175">Строка</span><span class="sxs-lookup"><span data-stu-id="05b70-175">String</span></span>|<span data-ttu-id="05b70-176">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="05b70-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="05b70-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="05b70-177">vppOrganizationName</span></span>|<span data-ttu-id="05b70-178">String</span><span class="sxs-lookup"><span data-stu-id="05b70-178">String</span></span>|<span data-ttu-id="05b70-179">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="05b70-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="05b70-180">genres</span><span class="sxs-lookup"><span data-stu-id="05b70-180">genres</span></span>|<span data-ttu-id="05b70-181">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="05b70-181">String collection</span></span>|<span data-ttu-id="05b70-182">Жанры.</span><span class="sxs-lookup"><span data-stu-id="05b70-182">Genres.</span></span>|
|<span data-ttu-id="05b70-183">language</span><span class="sxs-lookup"><span data-stu-id="05b70-183">language</span></span>|<span data-ttu-id="05b70-184">String</span><span class="sxs-lookup"><span data-stu-id="05b70-184">String</span></span>|<span data-ttu-id="05b70-185">Язык.</span><span class="sxs-lookup"><span data-stu-id="05b70-185">Language.</span></span>|
|<span data-ttu-id="05b70-186">seller</span><span class="sxs-lookup"><span data-stu-id="05b70-186">seller</span></span>|<span data-ttu-id="05b70-187">String</span><span class="sxs-lookup"><span data-stu-id="05b70-187">String</span></span>|<span data-ttu-id="05b70-188">Продавец.</span><span class="sxs-lookup"><span data-stu-id="05b70-188">Seller.</span></span>|
|<span data-ttu-id="05b70-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="05b70-189">totalLicenseCount</span></span>|<span data-ttu-id="05b70-190">Int32</span><span class="sxs-lookup"><span data-stu-id="05b70-190">Int32</span></span>|<span data-ttu-id="05b70-191">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="05b70-191">Total license count.</span></span>|
|<span data-ttu-id="05b70-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="05b70-192">usedLicenseCount</span></span>|<span data-ttu-id="05b70-193">Int32</span><span class="sxs-lookup"><span data-stu-id="05b70-193">Int32</span></span>|<span data-ttu-id="05b70-194">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="05b70-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="05b70-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="05b70-195">Response</span></span>
<span data-ttu-id="05b70-196">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05b70-196">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05b70-197">Пример</span><span class="sxs-lookup"><span data-stu-id="05b70-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="05b70-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="05b70-198">Request</span></span>
<span data-ttu-id="05b70-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05b70-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
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

### <a name="response"></a><span data-ttu-id="05b70-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="05b70-200">Response</span></span>
<span data-ttu-id="05b70-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05b70-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



