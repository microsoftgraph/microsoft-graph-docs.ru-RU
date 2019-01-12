---
title: Обновление объекта iosVppEBook
description: Обновление свойств объекта iosVppEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 27fa80b36ab049ead5b3aa8f56b27eeecfb31430
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915020"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="7bd10-103">Обновление объекта iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="7bd10-103">Update iosVppEBook</span></span>

> <span data-ttu-id="7bd10-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7bd10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7bd10-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bd10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bd10-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7bd10-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7bd10-107">Обновление свойств объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="7bd10-107">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7bd10-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7bd10-108">Prerequisites</span></span>
<span data-ttu-id="7bd10-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bd10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bd10-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bd10-111">Permission type</span></span>|<span data-ttu-id="7bd10-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bd10-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7bd10-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bd10-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7bd10-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bd10-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7bd10-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bd10-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7bd10-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bd10-116">Not supported.</span></span>|
|<span data-ttu-id="7bd10-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bd10-117">Application</span></span>|<span data-ttu-id="7bd10-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bd10-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7bd10-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bd10-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="7bd10-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bd10-120">Request headers</span></span>
|<span data-ttu-id="7bd10-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7bd10-121">Header</span></span>|<span data-ttu-id="7bd10-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7bd10-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7bd10-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7bd10-123">Authorization</span></span>|<span data-ttu-id="7bd10-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7bd10-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7bd10-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7bd10-125">Accept</span></span>|<span data-ttu-id="7bd10-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7bd10-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7bd10-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7bd10-127">Request body</span></span>
<span data-ttu-id="7bd10-128">В теле запроса добавьте представление объекта [iosVppEBook](../resources/intune-books-iosvppebook.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bd10-128">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="7bd10-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="7bd10-129">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="7bd10-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bd10-130">Property</span></span>|<span data-ttu-id="7bd10-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7bd10-131">Type</span></span>|<span data-ttu-id="7bd10-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7bd10-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bd10-133">id</span><span class="sxs-lookup"><span data-stu-id="7bd10-133">id</span></span>|<span data-ttu-id="7bd10-134">String</span><span class="sxs-lookup"><span data-stu-id="7bd10-134">String</span></span>|<span data-ttu-id="7bd10-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7bd10-135">Key of the entity.</span></span> <span data-ttu-id="7bd10-136">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7bd10-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="7bd10-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7bd10-137">displayName</span></span>|<span data-ttu-id="7bd10-138">String</span><span class="sxs-lookup"><span data-stu-id="7bd10-138">String</span></span>|<span data-ttu-id="7bd10-139">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="7bd10-139">Name of the eBook.</span></span> <span data-ttu-id="7bd10-140">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7bd10-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="7bd10-141">описание</span><span class="sxs-lookup"><span data-stu-id="7bd10-141">description</span></span>|<span data-ttu-id="7bd10-142">String</span><span class="sxs-lookup"><span data-stu-id="7bd10-142">String</span></span>|<span data-ttu-id="7bd10-143">Описание.</span><span class="sxs-lookup"><span data-stu-id="7bd10-143">Description.</span></span> <span data-ttu-id="7bd10-144">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7bd10-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="7bd10-145">publisher</span><span class="sxs-lookup"><span data-stu-id="7bd10-145">publisher</span></span>|<span data-ttu-id="7bd10-146">String</span><span class="sxs-lookup"><span data-stu-id="7bd10-146">String</span></span>|<span data-ttu-id="7bd10-147">Издатель.</span><span class="sxs-lookup"><span data-stu-id="7bd10-147">Publisher.</span></span> <span data-ttu-id="7bd10-148">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7bd10-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="7bd10-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bd10-149">publishedDateTime</span></span>|<span data-ttu-id="7bd10-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bd10-150">DateTimeOffset</span></span>|<span data-ttu-id="7bd10-151">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="7bd10-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="7bd10-152">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7bd10-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="7bd10-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="7bd10-153">largeCover</span></span>|[<span data-ttu-id="7bd10-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7bd10-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7bd10-155">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="7bd10-155">Book cover.</span></span> <span data-ttu-id="7bd10-156">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7bd10-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="7bd10-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7bd10-157">createdDateTime</span></span>|<span data-ttu-id="7bd10-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bd10-158">DateTimeOffset</span></span>|<span data-ttu-id="7bd10-159">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="7bd10-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="7bd10-160">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7bd10-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="7bd10-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bd10-161">lastModifiedDateTime</span></span>|<span data-ttu-id="7bd10-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bd10-162">DateTimeOffset</span></span>|<span data-ttu-id="7bd10-163">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="7bd10-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="7bd10-164">Унаследован от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="7bd10-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="7bd10-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7bd10-165">informationUrl</span></span>|<span data-ttu-id="7bd10-166">String</span><span class="sxs-lookup"><span data-stu-id="7bd10-166">String</span></span>|<span data-ttu-id="7bd10-167">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="7bd10-167">The more information Url.</span></span> <span data-ttu-id="7bd10-168">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7bd10-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="7bd10-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7bd10-169">privacyInformationUrl</span></span>|<span data-ttu-id="7bd10-170">String</span><span class="sxs-lookup"><span data-stu-id="7bd10-170">String</span></span>|<span data-ttu-id="7bd10-171">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="7bd10-171">The privacy statement Url.</span></span> <span data-ttu-id="7bd10-172">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="7bd10-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="7bd10-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="7bd10-173">vppTokenId</span></span>|<span data-ttu-id="7bd10-174">Guid</span><span class="sxs-lookup"><span data-stu-id="7bd10-174">Guid</span></span>|<span data-ttu-id="7bd10-175">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="7bd10-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="7bd10-176">appleId</span><span class="sxs-lookup"><span data-stu-id="7bd10-176">appleId</span></span>|<span data-ttu-id="7bd10-177">String</span><span class="sxs-lookup"><span data-stu-id="7bd10-177">String</span></span>|<span data-ttu-id="7bd10-178">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="7bd10-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="7bd10-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="7bd10-179">vppOrganizationName</span></span>|<span data-ttu-id="7bd10-180">String</span><span class="sxs-lookup"><span data-stu-id="7bd10-180">String</span></span>|<span data-ttu-id="7bd10-181">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="7bd10-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="7bd10-182">genres</span><span class="sxs-lookup"><span data-stu-id="7bd10-182">genres</span></span>|<span data-ttu-id="7bd10-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7bd10-183">String collection</span></span>|<span data-ttu-id="7bd10-184">Жанры.</span><span class="sxs-lookup"><span data-stu-id="7bd10-184">Genres.</span></span>|
|<span data-ttu-id="7bd10-185">language</span><span class="sxs-lookup"><span data-stu-id="7bd10-185">language</span></span>|<span data-ttu-id="7bd10-186">String</span><span class="sxs-lookup"><span data-stu-id="7bd10-186">String</span></span>|<span data-ttu-id="7bd10-187">Язык.</span><span class="sxs-lookup"><span data-stu-id="7bd10-187">Language.</span></span>|
|<span data-ttu-id="7bd10-188">seller</span><span class="sxs-lookup"><span data-stu-id="7bd10-188">seller</span></span>|<span data-ttu-id="7bd10-189">String</span><span class="sxs-lookup"><span data-stu-id="7bd10-189">String</span></span>|<span data-ttu-id="7bd10-190">Продавец.</span><span class="sxs-lookup"><span data-stu-id="7bd10-190">Seller.</span></span>|
|<span data-ttu-id="7bd10-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7bd10-191">totalLicenseCount</span></span>|<span data-ttu-id="7bd10-192">Int32</span><span class="sxs-lookup"><span data-stu-id="7bd10-192">Int32</span></span>|<span data-ttu-id="7bd10-193">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="7bd10-193">Total license count.</span></span>|
|<span data-ttu-id="7bd10-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7bd10-194">usedLicenseCount</span></span>|<span data-ttu-id="7bd10-195">Int32</span><span class="sxs-lookup"><span data-stu-id="7bd10-195">Int32</span></span>|<span data-ttu-id="7bd10-196">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="7bd10-196">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="7bd10-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bd10-197">Response</span></span>
<span data-ttu-id="7bd10-198">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7bd10-198">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bd10-199">Пример</span><span class="sxs-lookup"><span data-stu-id="7bd10-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="7bd10-200">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bd10-200">Request</span></span>
<span data-ttu-id="7bd10-201">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bd10-201">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
Content-type: application/json
Content-length: 806

{
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

### <a name="response"></a><span data-ttu-id="7bd10-202">Ответ</span><span class="sxs-lookup"><span data-stu-id="7bd10-202">Response</span></span>
<span data-ttu-id="7bd10-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7bd10-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





