---
title: Обновление объекта iosVppEBook
description: Обновление свойств объекта iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c3565a104c1f970293a9d6fc6b9ea5fcdd470228
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982346"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="11dd2-103">Обновление объекта iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="11dd2-103">Update iosVppEBook</span></span>

> <span data-ttu-id="11dd2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="11dd2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11dd2-105">Обновление свойств объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="11dd2-105">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="11dd2-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="11dd2-106">Prerequisites</span></span>
<span data-ttu-id="11dd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11dd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11dd2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11dd2-109">Permission type</span></span>|<span data-ttu-id="11dd2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="11dd2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11dd2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11dd2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="11dd2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11dd2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="11dd2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11dd2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11dd2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11dd2-114">Not supported.</span></span>|
|<span data-ttu-id="11dd2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11dd2-115">Application</span></span>|<span data-ttu-id="11dd2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11dd2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11dd2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11dd2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="11dd2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11dd2-118">Request headers</span></span>
|<span data-ttu-id="11dd2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11dd2-119">Header</span></span>|<span data-ttu-id="11dd2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="11dd2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11dd2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="11dd2-121">Authorization</span></span>|<span data-ttu-id="11dd2-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="11dd2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11dd2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="11dd2-123">Accept</span></span>|<span data-ttu-id="11dd2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="11dd2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11dd2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="11dd2-125">Request body</span></span>
<span data-ttu-id="11dd2-126">В теле запроса добавьте представление объекта [iosVppEBook](../resources/intune-books-iosvppebook.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11dd2-126">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="11dd2-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="11dd2-127">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="11dd2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="11dd2-128">Property</span></span>|<span data-ttu-id="11dd2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="11dd2-129">Type</span></span>|<span data-ttu-id="11dd2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="11dd2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11dd2-131">id</span><span class="sxs-lookup"><span data-stu-id="11dd2-131">id</span></span>|<span data-ttu-id="11dd2-132">String</span><span class="sxs-lookup"><span data-stu-id="11dd2-132">String</span></span>|<span data-ttu-id="11dd2-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="11dd2-133">Key of the entity.</span></span> <span data-ttu-id="11dd2-134">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="11dd2-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="11dd2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="11dd2-135">displayName</span></span>|<span data-ttu-id="11dd2-136">String</span><span class="sxs-lookup"><span data-stu-id="11dd2-136">String</span></span>|<span data-ttu-id="11dd2-137">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="11dd2-137">Name of the eBook.</span></span> <span data-ttu-id="11dd2-138">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="11dd2-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="11dd2-139">описание</span><span class="sxs-lookup"><span data-stu-id="11dd2-139">description</span></span>|<span data-ttu-id="11dd2-140">String</span><span class="sxs-lookup"><span data-stu-id="11dd2-140">String</span></span>|<span data-ttu-id="11dd2-141">Описание.</span><span class="sxs-lookup"><span data-stu-id="11dd2-141">Description.</span></span> <span data-ttu-id="11dd2-142">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="11dd2-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="11dd2-143">publisher</span><span class="sxs-lookup"><span data-stu-id="11dd2-143">publisher</span></span>|<span data-ttu-id="11dd2-144">String</span><span class="sxs-lookup"><span data-stu-id="11dd2-144">String</span></span>|<span data-ttu-id="11dd2-145">Издатель.</span><span class="sxs-lookup"><span data-stu-id="11dd2-145">Publisher.</span></span> <span data-ttu-id="11dd2-146">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="11dd2-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="11dd2-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="11dd2-147">publishedDateTime</span></span>|<span data-ttu-id="11dd2-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11dd2-148">DateTimeOffset</span></span>|<span data-ttu-id="11dd2-149">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="11dd2-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="11dd2-150">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="11dd2-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="11dd2-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="11dd2-151">largeCover</span></span>|[<span data-ttu-id="11dd2-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="11dd2-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="11dd2-153">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="11dd2-153">Book cover.</span></span> <span data-ttu-id="11dd2-154">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="11dd2-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="11dd2-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11dd2-155">createdDateTime</span></span>|<span data-ttu-id="11dd2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11dd2-156">DateTimeOffset</span></span>|<span data-ttu-id="11dd2-157">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="11dd2-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="11dd2-158">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="11dd2-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="11dd2-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11dd2-159">lastModifiedDateTime</span></span>|<span data-ttu-id="11dd2-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11dd2-160">DateTimeOffset</span></span>|<span data-ttu-id="11dd2-161">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="11dd2-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="11dd2-162">Унаследован от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="11dd2-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="11dd2-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="11dd2-163">informationUrl</span></span>|<span data-ttu-id="11dd2-164">String</span><span class="sxs-lookup"><span data-stu-id="11dd2-164">String</span></span>|<span data-ttu-id="11dd2-165">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="11dd2-165">The more information Url.</span></span> <span data-ttu-id="11dd2-166">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="11dd2-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="11dd2-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="11dd2-167">privacyInformationUrl</span></span>|<span data-ttu-id="11dd2-168">String</span><span class="sxs-lookup"><span data-stu-id="11dd2-168">String</span></span>|<span data-ttu-id="11dd2-169">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="11dd2-169">The privacy statement Url.</span></span> <span data-ttu-id="11dd2-170">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="11dd2-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="11dd2-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="11dd2-171">vppTokenId</span></span>|<span data-ttu-id="11dd2-172">Guid</span><span class="sxs-lookup"><span data-stu-id="11dd2-172">Guid</span></span>|<span data-ttu-id="11dd2-173">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="11dd2-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="11dd2-174">appleId</span><span class="sxs-lookup"><span data-stu-id="11dd2-174">appleId</span></span>|<span data-ttu-id="11dd2-175">String</span><span class="sxs-lookup"><span data-stu-id="11dd2-175">String</span></span>|<span data-ttu-id="11dd2-176">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="11dd2-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="11dd2-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="11dd2-177">vppOrganizationName</span></span>|<span data-ttu-id="11dd2-178">String</span><span class="sxs-lookup"><span data-stu-id="11dd2-178">String</span></span>|<span data-ttu-id="11dd2-179">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="11dd2-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="11dd2-180">genres</span><span class="sxs-lookup"><span data-stu-id="11dd2-180">genres</span></span>|<span data-ttu-id="11dd2-181">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="11dd2-181">String collection</span></span>|<span data-ttu-id="11dd2-182">Жанры.</span><span class="sxs-lookup"><span data-stu-id="11dd2-182">Genres.</span></span>|
|<span data-ttu-id="11dd2-183">language</span><span class="sxs-lookup"><span data-stu-id="11dd2-183">language</span></span>|<span data-ttu-id="11dd2-184">String</span><span class="sxs-lookup"><span data-stu-id="11dd2-184">String</span></span>|<span data-ttu-id="11dd2-185">Язык.</span><span class="sxs-lookup"><span data-stu-id="11dd2-185">Language.</span></span>|
|<span data-ttu-id="11dd2-186">seller</span><span class="sxs-lookup"><span data-stu-id="11dd2-186">seller</span></span>|<span data-ttu-id="11dd2-187">String</span><span class="sxs-lookup"><span data-stu-id="11dd2-187">String</span></span>|<span data-ttu-id="11dd2-188">Продавец.</span><span class="sxs-lookup"><span data-stu-id="11dd2-188">Seller.</span></span>|
|<span data-ttu-id="11dd2-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="11dd2-189">totalLicenseCount</span></span>|<span data-ttu-id="11dd2-190">Int32</span><span class="sxs-lookup"><span data-stu-id="11dd2-190">Int32</span></span>|<span data-ttu-id="11dd2-191">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="11dd2-191">Total license count.</span></span>|
|<span data-ttu-id="11dd2-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="11dd2-192">usedLicenseCount</span></span>|<span data-ttu-id="11dd2-193">Int32</span><span class="sxs-lookup"><span data-stu-id="11dd2-193">Int32</span></span>|<span data-ttu-id="11dd2-194">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="11dd2-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="11dd2-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="11dd2-195">Response</span></span>
<span data-ttu-id="11dd2-196">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="11dd2-196">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11dd2-197">Пример</span><span class="sxs-lookup"><span data-stu-id="11dd2-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="11dd2-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="11dd2-198">Request</span></span>
<span data-ttu-id="11dd2-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11dd2-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11dd2-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="11dd2-200">Response</span></span>
<span data-ttu-id="11dd2-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="11dd2-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



