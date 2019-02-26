---
title: Обновление объекта iosVppEBook
description: Обновление свойств объекта iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f4b307d54840549caf821defc736a68f90e7556
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253367"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="3282d-103">Обновление объекта iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="3282d-103">Update iosVppEBook</span></span>

> <span data-ttu-id="3282d-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3282d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3282d-105">Обновление свойств объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="3282d-105">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3282d-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3282d-106">Prerequisites</span></span>
<span data-ttu-id="3282d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3282d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3282d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3282d-109">Permission type</span></span>|<span data-ttu-id="3282d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3282d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3282d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3282d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3282d-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3282d-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3282d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3282d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3282d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3282d-114">Not supported.</span></span>|
|<span data-ttu-id="3282d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3282d-115">Application</span></span>|<span data-ttu-id="3282d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3282d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3282d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3282d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="3282d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3282d-118">Request headers</span></span>
|<span data-ttu-id="3282d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3282d-119">Header</span></span>|<span data-ttu-id="3282d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3282d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3282d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3282d-121">Authorization</span></span>|<span data-ttu-id="3282d-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3282d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3282d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3282d-123">Accept</span></span>|<span data-ttu-id="3282d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3282d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3282d-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3282d-125">Request body</span></span>
<span data-ttu-id="3282d-126">В теле запроса добавьте представление объекта [iosVppEBook](../resources/intune-books-iosvppebook.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3282d-126">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="3282d-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="3282d-127">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="3282d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3282d-128">Property</span></span>|<span data-ttu-id="3282d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3282d-129">Type</span></span>|<span data-ttu-id="3282d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3282d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3282d-131">id</span><span class="sxs-lookup"><span data-stu-id="3282d-131">id</span></span>|<span data-ttu-id="3282d-132">Строка</span><span class="sxs-lookup"><span data-stu-id="3282d-132">String</span></span>|<span data-ttu-id="3282d-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3282d-133">Key of the entity.</span></span> <span data-ttu-id="3282d-134">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3282d-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3282d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3282d-135">displayName</span></span>|<span data-ttu-id="3282d-136">String</span><span class="sxs-lookup"><span data-stu-id="3282d-136">String</span></span>|<span data-ttu-id="3282d-137">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3282d-137">Name of the eBook.</span></span> <span data-ttu-id="3282d-138">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3282d-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3282d-139">description</span><span class="sxs-lookup"><span data-stu-id="3282d-139">description</span></span>|<span data-ttu-id="3282d-140">Строка</span><span class="sxs-lookup"><span data-stu-id="3282d-140">String</span></span>|<span data-ttu-id="3282d-141">Описание.</span><span class="sxs-lookup"><span data-stu-id="3282d-141">Description.</span></span> <span data-ttu-id="3282d-142">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3282d-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3282d-143">publisher</span><span class="sxs-lookup"><span data-stu-id="3282d-143">publisher</span></span>|<span data-ttu-id="3282d-144">String</span><span class="sxs-lookup"><span data-stu-id="3282d-144">String</span></span>|<span data-ttu-id="3282d-145">Издатель.</span><span class="sxs-lookup"><span data-stu-id="3282d-145">Publisher.</span></span> <span data-ttu-id="3282d-146">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3282d-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3282d-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="3282d-147">publishedDateTime</span></span>|<span data-ttu-id="3282d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3282d-148">DateTimeOffset</span></span>|<span data-ttu-id="3282d-149">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3282d-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="3282d-150">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3282d-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3282d-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="3282d-151">largeCover</span></span>|[<span data-ttu-id="3282d-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3282d-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3282d-153">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="3282d-153">Book cover.</span></span> <span data-ttu-id="3282d-154">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3282d-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3282d-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3282d-155">createdDateTime</span></span>|<span data-ttu-id="3282d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3282d-156">DateTimeOffset</span></span>|<span data-ttu-id="3282d-157">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3282d-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="3282d-158">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3282d-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3282d-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3282d-159">lastModifiedDateTime</span></span>|<span data-ttu-id="3282d-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3282d-160">DateTimeOffset</span></span>|<span data-ttu-id="3282d-161">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3282d-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="3282d-162">Унаследован от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3282d-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3282d-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3282d-163">informationUrl</span></span>|<span data-ttu-id="3282d-164">String</span><span class="sxs-lookup"><span data-stu-id="3282d-164">String</span></span>|<span data-ttu-id="3282d-165">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3282d-165">The more information Url.</span></span> <span data-ttu-id="3282d-166">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3282d-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3282d-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3282d-167">privacyInformationUrl</span></span>|<span data-ttu-id="3282d-168">String</span><span class="sxs-lookup"><span data-stu-id="3282d-168">String</span></span>|<span data-ttu-id="3282d-169">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3282d-169">The privacy statement Url.</span></span> <span data-ttu-id="3282d-170">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3282d-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3282d-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="3282d-171">vppTokenId</span></span>|<span data-ttu-id="3282d-172">Guid</span><span class="sxs-lookup"><span data-stu-id="3282d-172">Guid</span></span>|<span data-ttu-id="3282d-173">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="3282d-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="3282d-174">appleId</span><span class="sxs-lookup"><span data-stu-id="3282d-174">appleId</span></span>|<span data-ttu-id="3282d-175">Строка</span><span class="sxs-lookup"><span data-stu-id="3282d-175">String</span></span>|<span data-ttu-id="3282d-176">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="3282d-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="3282d-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="3282d-177">vppOrganizationName</span></span>|<span data-ttu-id="3282d-178">String</span><span class="sxs-lookup"><span data-stu-id="3282d-178">String</span></span>|<span data-ttu-id="3282d-179">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="3282d-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="3282d-180">genres</span><span class="sxs-lookup"><span data-stu-id="3282d-180">genres</span></span>|<span data-ttu-id="3282d-181">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3282d-181">String collection</span></span>|<span data-ttu-id="3282d-182">Жанры.</span><span class="sxs-lookup"><span data-stu-id="3282d-182">Genres.</span></span>|
|<span data-ttu-id="3282d-183">language</span><span class="sxs-lookup"><span data-stu-id="3282d-183">language</span></span>|<span data-ttu-id="3282d-184">String</span><span class="sxs-lookup"><span data-stu-id="3282d-184">String</span></span>|<span data-ttu-id="3282d-185">Язык.</span><span class="sxs-lookup"><span data-stu-id="3282d-185">Language.</span></span>|
|<span data-ttu-id="3282d-186">seller</span><span class="sxs-lookup"><span data-stu-id="3282d-186">seller</span></span>|<span data-ttu-id="3282d-187">String</span><span class="sxs-lookup"><span data-stu-id="3282d-187">String</span></span>|<span data-ttu-id="3282d-188">Продавец.</span><span class="sxs-lookup"><span data-stu-id="3282d-188">Seller.</span></span>|
|<span data-ttu-id="3282d-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3282d-189">totalLicenseCount</span></span>|<span data-ttu-id="3282d-190">Int32</span><span class="sxs-lookup"><span data-stu-id="3282d-190">Int32</span></span>|<span data-ttu-id="3282d-191">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="3282d-191">Total license count.</span></span>|
|<span data-ttu-id="3282d-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3282d-192">usedLicenseCount</span></span>|<span data-ttu-id="3282d-193">Int32</span><span class="sxs-lookup"><span data-stu-id="3282d-193">Int32</span></span>|<span data-ttu-id="3282d-194">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="3282d-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="3282d-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="3282d-195">Response</span></span>
<span data-ttu-id="3282d-196">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3282d-196">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3282d-197">Пример</span><span class="sxs-lookup"><span data-stu-id="3282d-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="3282d-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="3282d-198">Request</span></span>
<span data-ttu-id="3282d-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3282d-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3282d-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="3282d-200">Response</span></span>
<span data-ttu-id="3282d-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3282d-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



