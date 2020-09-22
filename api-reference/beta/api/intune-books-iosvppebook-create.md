---
title: Create iosVppEBook
description: Создание объекта iosVppEBook.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ebfba46a810dce455b7f6b538e5b1ea6934447fe
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975747"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="b995c-103">Create iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="b995c-103">Create iosVppEBook</span></span>

<span data-ttu-id="b995c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b995c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b995c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b995c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b995c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b995c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b995c-107">Создание объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="b995c-107">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b995c-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="b995c-108">Prerequisites</span></span>
<span data-ttu-id="b995c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b995c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b995c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b995c-111">Permission type</span></span>|<span data-ttu-id="b995c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b995c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b995c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b995c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b995c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b995c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b995c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b995c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b995c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b995c-116">Not supported.</span></span>|
|<span data-ttu-id="b995c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b995c-117">Application</span></span>|<span data-ttu-id="b995c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b995c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b995c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b995c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="b995c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b995c-120">Request headers</span></span>
|<span data-ttu-id="b995c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b995c-121">Header</span></span>|<span data-ttu-id="b995c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b995c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b995c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b995c-123">Authorization</span></span>|<span data-ttu-id="b995c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b995c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b995c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b995c-125">Accept</span></span>|<span data-ttu-id="b995c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b995c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b995c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b995c-127">Request body</span></span>
<span data-ttu-id="b995c-128">В теле запроса добавьте представление объекта iosVppEBook в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b995c-128">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="b995c-129">Ниже показаны свойства, которые необходимо указать при создании объекта iosVppEBook.</span><span class="sxs-lookup"><span data-stu-id="b995c-129">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="b995c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b995c-130">Property</span></span>|<span data-ttu-id="b995c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b995c-131">Type</span></span>|<span data-ttu-id="b995c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b995c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b995c-133">id</span><span class="sxs-lookup"><span data-stu-id="b995c-133">id</span></span>|<span data-ttu-id="b995c-134">String</span><span class="sxs-lookup"><span data-stu-id="b995c-134">String</span></span>|<span data-ttu-id="b995c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b995c-135">Key of the entity.</span></span> <span data-ttu-id="b995c-136">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b995c-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="b995c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b995c-137">displayName</span></span>|<span data-ttu-id="b995c-138">String</span><span class="sxs-lookup"><span data-stu-id="b995c-138">String</span></span>|<span data-ttu-id="b995c-139">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b995c-139">Name of the eBook.</span></span> <span data-ttu-id="b995c-140">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b995c-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="b995c-141">description</span><span class="sxs-lookup"><span data-stu-id="b995c-141">description</span></span>|<span data-ttu-id="b995c-142">String</span><span class="sxs-lookup"><span data-stu-id="b995c-142">String</span></span>|<span data-ttu-id="b995c-143">Описание.</span><span class="sxs-lookup"><span data-stu-id="b995c-143">Description.</span></span> <span data-ttu-id="b995c-144">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b995c-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="b995c-145">publisher</span><span class="sxs-lookup"><span data-stu-id="b995c-145">publisher</span></span>|<span data-ttu-id="b995c-146">String</span><span class="sxs-lookup"><span data-stu-id="b995c-146">String</span></span>|<span data-ttu-id="b995c-147">Издатель.</span><span class="sxs-lookup"><span data-stu-id="b995c-147">Publisher.</span></span> <span data-ttu-id="b995c-148">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b995c-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="b995c-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="b995c-149">publishedDateTime</span></span>|<span data-ttu-id="b995c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b995c-150">DateTimeOffset</span></span>|<span data-ttu-id="b995c-151">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b995c-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="b995c-152">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b995c-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="b995c-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="b995c-153">largeCover</span></span>|[<span data-ttu-id="b995c-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b995c-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b995c-155">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="b995c-155">Book cover.</span></span> <span data-ttu-id="b995c-156">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b995c-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="b995c-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b995c-157">createdDateTime</span></span>|<span data-ttu-id="b995c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b995c-158">DateTimeOffset</span></span>|<span data-ttu-id="b995c-159">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b995c-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="b995c-160">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b995c-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="b995c-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b995c-161">lastModifiedDateTime</span></span>|<span data-ttu-id="b995c-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b995c-162">DateTimeOffset</span></span>|<span data-ttu-id="b995c-163">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="b995c-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="b995c-164">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="b995c-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="b995c-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b995c-165">informationUrl</span></span>|<span data-ttu-id="b995c-166">String</span><span class="sxs-lookup"><span data-stu-id="b995c-166">String</span></span>|<span data-ttu-id="b995c-167">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="b995c-167">The more information Url.</span></span> <span data-ttu-id="b995c-168">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b995c-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="b995c-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b995c-169">privacyInformationUrl</span></span>|<span data-ttu-id="b995c-170">String</span><span class="sxs-lookup"><span data-stu-id="b995c-170">String</span></span>|<span data-ttu-id="b995c-171">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="b995c-171">The privacy statement Url.</span></span> <span data-ttu-id="b995c-172">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="b995c-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="b995c-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="b995c-173">vppTokenId</span></span>|<span data-ttu-id="b995c-174">Guid</span><span class="sxs-lookup"><span data-stu-id="b995c-174">Guid</span></span>|<span data-ttu-id="b995c-175">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="b995c-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="b995c-176">appleId</span><span class="sxs-lookup"><span data-stu-id="b995c-176">appleId</span></span>|<span data-ttu-id="b995c-177">String</span><span class="sxs-lookup"><span data-stu-id="b995c-177">String</span></span>|<span data-ttu-id="b995c-178">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="b995c-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="b995c-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="b995c-179">vppOrganizationName</span></span>|<span data-ttu-id="b995c-180">String</span><span class="sxs-lookup"><span data-stu-id="b995c-180">String</span></span>|<span data-ttu-id="b995c-181">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="b995c-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="b995c-182">genres</span><span class="sxs-lookup"><span data-stu-id="b995c-182">genres</span></span>|<span data-ttu-id="b995c-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b995c-183">String collection</span></span>|<span data-ttu-id="b995c-184">Жанры.</span><span class="sxs-lookup"><span data-stu-id="b995c-184">Genres.</span></span>|
|<span data-ttu-id="b995c-185">language</span><span class="sxs-lookup"><span data-stu-id="b995c-185">language</span></span>|<span data-ttu-id="b995c-186">String</span><span class="sxs-lookup"><span data-stu-id="b995c-186">String</span></span>|<span data-ttu-id="b995c-187">Язык.</span><span class="sxs-lookup"><span data-stu-id="b995c-187">Language.</span></span>|
|<span data-ttu-id="b995c-188">seller</span><span class="sxs-lookup"><span data-stu-id="b995c-188">seller</span></span>|<span data-ttu-id="b995c-189">String</span><span class="sxs-lookup"><span data-stu-id="b995c-189">String</span></span>|<span data-ttu-id="b995c-190">Продавец.</span><span class="sxs-lookup"><span data-stu-id="b995c-190">Seller.</span></span>|
|<span data-ttu-id="b995c-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b995c-191">totalLicenseCount</span></span>|<span data-ttu-id="b995c-192">Int32</span><span class="sxs-lookup"><span data-stu-id="b995c-192">Int32</span></span>|<span data-ttu-id="b995c-193">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="b995c-193">Total license count.</span></span>|
|<span data-ttu-id="b995c-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b995c-194">usedLicenseCount</span></span>|<span data-ttu-id="b995c-195">Int32</span><span class="sxs-lookup"><span data-stu-id="b995c-195">Int32</span></span>|<span data-ttu-id="b995c-196">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="b995c-196">Used license count.</span></span>|
|<span data-ttu-id="b995c-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b995c-197">roleScopeTagIds</span></span>|<span data-ttu-id="b995c-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b995c-198">String collection</span></span>|<span data-ttu-id="b995c-199">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="b995c-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="b995c-200">Ответ</span><span class="sxs-lookup"><span data-stu-id="b995c-200">Response</span></span>
<span data-ttu-id="b995c-201">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b995c-201">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b995c-202">Пример</span><span class="sxs-lookup"><span data-stu-id="b995c-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="b995c-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="b995c-203">Request</span></span>
<span data-ttu-id="b995c-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b995c-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b995c-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="b995c-205">Response</span></span>
<span data-ttu-id="b995c-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b995c-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






