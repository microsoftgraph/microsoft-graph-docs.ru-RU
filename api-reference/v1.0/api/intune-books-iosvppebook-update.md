---
title: Обновление объекта iosVppEBook
description: Обновление свойств объекта iosVppEBook.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cba3e1eb6fa3b6398006fb9db3c50f8c644b93da
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515639"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="acebb-103">Обновление объекта iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="acebb-103">Update iosVppEBook</span></span>

<span data-ttu-id="acebb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acebb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="acebb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="acebb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acebb-106">Обновление свойств объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="acebb-106">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acebb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="acebb-107">Prerequisites</span></span>
<span data-ttu-id="acebb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acebb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acebb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acebb-110">Permission type</span></span>|<span data-ttu-id="acebb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="acebb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acebb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acebb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="acebb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acebb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="acebb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acebb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acebb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acebb-115">Not supported.</span></span>|
|<span data-ttu-id="acebb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="acebb-116">Application</span></span>|<span data-ttu-id="acebb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acebb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acebb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acebb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="acebb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="acebb-119">Request headers</span></span>
|<span data-ttu-id="acebb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="acebb-120">Header</span></span>|<span data-ttu-id="acebb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="acebb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acebb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="acebb-122">Authorization</span></span>|<span data-ttu-id="acebb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="acebb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acebb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="acebb-124">Accept</span></span>|<span data-ttu-id="acebb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="acebb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acebb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="acebb-126">Request body</span></span>
<span data-ttu-id="acebb-127">В теле запроса добавьте представление объекта [iosVppEBook](../resources/intune-books-iosvppebook.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="acebb-127">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="acebb-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="acebb-128">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="acebb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="acebb-129">Property</span></span>|<span data-ttu-id="acebb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="acebb-130">Type</span></span>|<span data-ttu-id="acebb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="acebb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acebb-132">id</span><span class="sxs-lookup"><span data-stu-id="acebb-132">id</span></span>|<span data-ttu-id="acebb-133">Строка</span><span class="sxs-lookup"><span data-stu-id="acebb-133">String</span></span>|<span data-ttu-id="acebb-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="acebb-134">Key of the entity.</span></span> <span data-ttu-id="acebb-135">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="acebb-135">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="acebb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="acebb-136">displayName</span></span>|<span data-ttu-id="acebb-137">Строка</span><span class="sxs-lookup"><span data-stu-id="acebb-137">String</span></span>|<span data-ttu-id="acebb-138">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="acebb-138">Name of the eBook.</span></span> <span data-ttu-id="acebb-139">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="acebb-139">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="acebb-140">description</span><span class="sxs-lookup"><span data-stu-id="acebb-140">description</span></span>|<span data-ttu-id="acebb-141">String</span><span class="sxs-lookup"><span data-stu-id="acebb-141">String</span></span>|<span data-ttu-id="acebb-142">Описание.</span><span class="sxs-lookup"><span data-stu-id="acebb-142">Description.</span></span> <span data-ttu-id="acebb-143">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="acebb-143">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="acebb-144">publisher</span><span class="sxs-lookup"><span data-stu-id="acebb-144">publisher</span></span>|<span data-ttu-id="acebb-145">Строка</span><span class="sxs-lookup"><span data-stu-id="acebb-145">String</span></span>|<span data-ttu-id="acebb-146">Издатель.</span><span class="sxs-lookup"><span data-stu-id="acebb-146">Publisher.</span></span> <span data-ttu-id="acebb-147">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="acebb-147">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="acebb-148">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="acebb-148">publishedDateTime</span></span>|<span data-ttu-id="acebb-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acebb-149">DateTimeOffset</span></span>|<span data-ttu-id="acebb-150">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="acebb-150">The date and time when the eBook was published.</span></span> <span data-ttu-id="acebb-151">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="acebb-151">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="acebb-152">largeCover</span><span class="sxs-lookup"><span data-stu-id="acebb-152">largeCover</span></span>|[<span data-ttu-id="acebb-153">mimeContent</span><span class="sxs-lookup"><span data-stu-id="acebb-153">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="acebb-154">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="acebb-154">Book cover.</span></span> <span data-ttu-id="acebb-155">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="acebb-155">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="acebb-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="acebb-156">createdDateTime</span></span>|<span data-ttu-id="acebb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acebb-157">DateTimeOffset</span></span>|<span data-ttu-id="acebb-158">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="acebb-158">The date and time when the eBook file was created.</span></span> <span data-ttu-id="acebb-159">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="acebb-159">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="acebb-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="acebb-160">lastModifiedDateTime</span></span>|<span data-ttu-id="acebb-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acebb-161">DateTimeOffset</span></span>|<span data-ttu-id="acebb-162">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="acebb-162">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="acebb-163">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="acebb-163">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="acebb-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="acebb-164">informationUrl</span></span>|<span data-ttu-id="acebb-165">Строка</span><span class="sxs-lookup"><span data-stu-id="acebb-165">String</span></span>|<span data-ttu-id="acebb-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="acebb-166">The more information Url.</span></span> <span data-ttu-id="acebb-167">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="acebb-167">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="acebb-168">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="acebb-168">privacyInformationUrl</span></span>|<span data-ttu-id="acebb-169">Строка</span><span class="sxs-lookup"><span data-stu-id="acebb-169">String</span></span>|<span data-ttu-id="acebb-170">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="acebb-170">The privacy statement Url.</span></span> <span data-ttu-id="acebb-171">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="acebb-171">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="acebb-172">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="acebb-172">vppTokenId</span></span>|<span data-ttu-id="acebb-173">Guid</span><span class="sxs-lookup"><span data-stu-id="acebb-173">Guid</span></span>|<span data-ttu-id="acebb-174">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="acebb-174">The Vpp token ID.</span></span>|
|<span data-ttu-id="acebb-175">appleId</span><span class="sxs-lookup"><span data-stu-id="acebb-175">appleId</span></span>|<span data-ttu-id="acebb-176">Строка</span><span class="sxs-lookup"><span data-stu-id="acebb-176">String</span></span>|<span data-ttu-id="acebb-177">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="acebb-177">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="acebb-178">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="acebb-178">vppOrganizationName</span></span>|<span data-ttu-id="acebb-179">Строка</span><span class="sxs-lookup"><span data-stu-id="acebb-179">String</span></span>|<span data-ttu-id="acebb-180">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="acebb-180">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="acebb-181">genres</span><span class="sxs-lookup"><span data-stu-id="acebb-181">genres</span></span>|<span data-ttu-id="acebb-182">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="acebb-182">String collection</span></span>|<span data-ttu-id="acebb-183">Жанры.</span><span class="sxs-lookup"><span data-stu-id="acebb-183">Genres.</span></span>|
|<span data-ttu-id="acebb-184">language</span><span class="sxs-lookup"><span data-stu-id="acebb-184">language</span></span>|<span data-ttu-id="acebb-185">Строка</span><span class="sxs-lookup"><span data-stu-id="acebb-185">String</span></span>|<span data-ttu-id="acebb-186">Язык.</span><span class="sxs-lookup"><span data-stu-id="acebb-186">Language.</span></span>|
|<span data-ttu-id="acebb-187">seller</span><span class="sxs-lookup"><span data-stu-id="acebb-187">seller</span></span>|<span data-ttu-id="acebb-188">String</span><span class="sxs-lookup"><span data-stu-id="acebb-188">String</span></span>|<span data-ttu-id="acebb-189">Продавец.</span><span class="sxs-lookup"><span data-stu-id="acebb-189">Seller.</span></span>|
|<span data-ttu-id="acebb-190">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="acebb-190">totalLicenseCount</span></span>|<span data-ttu-id="acebb-191">Int32</span><span class="sxs-lookup"><span data-stu-id="acebb-191">Int32</span></span>|<span data-ttu-id="acebb-192">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="acebb-192">Total license count.</span></span>|
|<span data-ttu-id="acebb-193">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="acebb-193">usedLicenseCount</span></span>|<span data-ttu-id="acebb-194">Int32</span><span class="sxs-lookup"><span data-stu-id="acebb-194">Int32</span></span>|<span data-ttu-id="acebb-195">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="acebb-195">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="acebb-196">Отклик</span><span class="sxs-lookup"><span data-stu-id="acebb-196">Response</span></span>
<span data-ttu-id="acebb-197">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="acebb-197">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acebb-198">Пример</span><span class="sxs-lookup"><span data-stu-id="acebb-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="acebb-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="acebb-199">Request</span></span>
<span data-ttu-id="acebb-200">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="acebb-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="acebb-201">Отклик</span><span class="sxs-lookup"><span data-stu-id="acebb-201">Response</span></span>
<span data-ttu-id="acebb-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="acebb-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




