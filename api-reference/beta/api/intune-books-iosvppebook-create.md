---
title: Create iosVppEBook
description: Создание объекта iosVppEBook.
author: tfitzmac
ms.openlocfilehash: d50e698668c177069934fe6eb33aec4f3475fe17
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314121"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="3357e-103">Create iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="3357e-103">Create iosVppEBook</span></span>

> <span data-ttu-id="3357e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3357e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3357e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3357e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3357e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3357e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3357e-107">Создание объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="3357e-107">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3357e-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3357e-108">Prerequisites</span></span>
<span data-ttu-id="3357e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3357e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3357e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3357e-111">Permission type</span></span>|<span data-ttu-id="3357e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3357e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3357e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3357e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3357e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3357e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3357e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3357e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3357e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3357e-116">Not supported.</span></span>|
|<span data-ttu-id="3357e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3357e-117">Application</span></span>|<span data-ttu-id="3357e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3357e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3357e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3357e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="3357e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3357e-120">Request headers</span></span>
|<span data-ttu-id="3357e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3357e-121">Header</span></span>|<span data-ttu-id="3357e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3357e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3357e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3357e-123">Authorization</span></span>|<span data-ttu-id="3357e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3357e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3357e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3357e-125">Accept</span></span>|<span data-ttu-id="3357e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3357e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3357e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3357e-127">Request body</span></span>
<span data-ttu-id="3357e-128">В теле запроса добавьте представление объекта iosVppEBook в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3357e-128">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="3357e-129">Ниже показаны свойства, которые необходимо указать при создании объекта iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="3357e-129">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="3357e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3357e-130">Property</span></span>|<span data-ttu-id="3357e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3357e-131">Type</span></span>|<span data-ttu-id="3357e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3357e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3357e-133">id</span><span class="sxs-lookup"><span data-stu-id="3357e-133">id</span></span>|<span data-ttu-id="3357e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3357e-134">String</span></span>|<span data-ttu-id="3357e-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3357e-135">Key of the entity.</span></span> <span data-ttu-id="3357e-136">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3357e-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3357e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3357e-137">displayName</span></span>|<span data-ttu-id="3357e-138">String</span><span class="sxs-lookup"><span data-stu-id="3357e-138">String</span></span>|<span data-ttu-id="3357e-139">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3357e-139">Name of the eBook.</span></span> <span data-ttu-id="3357e-140">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3357e-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3357e-141">описание</span><span class="sxs-lookup"><span data-stu-id="3357e-141">description</span></span>|<span data-ttu-id="3357e-142">Строка</span><span class="sxs-lookup"><span data-stu-id="3357e-142">String</span></span>|<span data-ttu-id="3357e-143">Описание.</span><span class="sxs-lookup"><span data-stu-id="3357e-143">Description.</span></span> <span data-ttu-id="3357e-144">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3357e-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3357e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3357e-145">publisher</span></span>|<span data-ttu-id="3357e-146">String</span><span class="sxs-lookup"><span data-stu-id="3357e-146">String</span></span>|<span data-ttu-id="3357e-147">Издатель.</span><span class="sxs-lookup"><span data-stu-id="3357e-147">Publisher.</span></span> <span data-ttu-id="3357e-148">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3357e-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3357e-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="3357e-149">publishedDateTime</span></span>|<span data-ttu-id="3357e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3357e-150">DateTimeOffset</span></span>|<span data-ttu-id="3357e-151">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3357e-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="3357e-152">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3357e-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3357e-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="3357e-153">largeCover</span></span>|[<span data-ttu-id="3357e-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3357e-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3357e-155">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="3357e-155">Book cover.</span></span> <span data-ttu-id="3357e-156">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3357e-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3357e-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3357e-157">createdDateTime</span></span>|<span data-ttu-id="3357e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3357e-158">DateTimeOffset</span></span>|<span data-ttu-id="3357e-159">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3357e-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="3357e-160">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3357e-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3357e-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3357e-161">lastModifiedDateTime</span></span>|<span data-ttu-id="3357e-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3357e-162">DateTimeOffset</span></span>|<span data-ttu-id="3357e-163">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="3357e-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="3357e-164">Унаследован от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="3357e-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3357e-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3357e-165">informationUrl</span></span>|<span data-ttu-id="3357e-166">String</span><span class="sxs-lookup"><span data-stu-id="3357e-166">String</span></span>|<span data-ttu-id="3357e-167">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3357e-167">The more information Url.</span></span> <span data-ttu-id="3357e-168">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3357e-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3357e-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3357e-169">privacyInformationUrl</span></span>|<span data-ttu-id="3357e-170">String</span><span class="sxs-lookup"><span data-stu-id="3357e-170">String</span></span>|<span data-ttu-id="3357e-171">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3357e-171">The privacy statement Url.</span></span> <span data-ttu-id="3357e-172">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="3357e-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="3357e-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="3357e-173">vppTokenId</span></span>|<span data-ttu-id="3357e-174">Guid</span><span class="sxs-lookup"><span data-stu-id="3357e-174">Guid</span></span>|<span data-ttu-id="3357e-175">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="3357e-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="3357e-176">appleId</span><span class="sxs-lookup"><span data-stu-id="3357e-176">appleId</span></span>|<span data-ttu-id="3357e-177">String</span><span class="sxs-lookup"><span data-stu-id="3357e-177">String</span></span>|<span data-ttu-id="3357e-178">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="3357e-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="3357e-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="3357e-179">vppOrganizationName</span></span>|<span data-ttu-id="3357e-180">String</span><span class="sxs-lookup"><span data-stu-id="3357e-180">String</span></span>|<span data-ttu-id="3357e-181">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="3357e-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="3357e-182">genres</span><span class="sxs-lookup"><span data-stu-id="3357e-182">genres</span></span>|<span data-ttu-id="3357e-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3357e-183">String collection</span></span>|<span data-ttu-id="3357e-184">Жанры.</span><span class="sxs-lookup"><span data-stu-id="3357e-184">Genres.</span></span>|
|<span data-ttu-id="3357e-185">language</span><span class="sxs-lookup"><span data-stu-id="3357e-185">language</span></span>|<span data-ttu-id="3357e-186">String</span><span class="sxs-lookup"><span data-stu-id="3357e-186">String</span></span>|<span data-ttu-id="3357e-187">Язык.</span><span class="sxs-lookup"><span data-stu-id="3357e-187">Language.</span></span>|
|<span data-ttu-id="3357e-188">seller</span><span class="sxs-lookup"><span data-stu-id="3357e-188">seller</span></span>|<span data-ttu-id="3357e-189">String</span><span class="sxs-lookup"><span data-stu-id="3357e-189">String</span></span>|<span data-ttu-id="3357e-190">Продавец.</span><span class="sxs-lookup"><span data-stu-id="3357e-190">Seller.</span></span>|
|<span data-ttu-id="3357e-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3357e-191">totalLicenseCount</span></span>|<span data-ttu-id="3357e-192">Int32</span><span class="sxs-lookup"><span data-stu-id="3357e-192">Int32</span></span>|<span data-ttu-id="3357e-193">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="3357e-193">Total license count.</span></span>|
|<span data-ttu-id="3357e-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="3357e-194">usedLicenseCount</span></span>|<span data-ttu-id="3357e-195">Int32</span><span class="sxs-lookup"><span data-stu-id="3357e-195">Int32</span></span>|<span data-ttu-id="3357e-196">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="3357e-196">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="3357e-197">Ответ</span><span class="sxs-lookup"><span data-stu-id="3357e-197">Response</span></span>
<span data-ttu-id="3357e-198">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3357e-198">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3357e-199">Пример</span><span class="sxs-lookup"><span data-stu-id="3357e-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="3357e-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="3357e-200">Request</span></span>
<span data-ttu-id="3357e-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3357e-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 856

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

### <a name="response"></a><span data-ttu-id="3357e-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="3357e-202">Response</span></span>
<span data-ttu-id="3357e-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3357e-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





