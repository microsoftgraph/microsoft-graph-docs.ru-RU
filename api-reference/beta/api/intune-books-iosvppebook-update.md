---
title: Обновление объекта iosVppEBook
description: Обновление свойств объекта iosVppEBook.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af90d389eee0cf9c94233e7dddcc1343feb03c77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975691"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="2f684-103">Обновление объекта iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="2f684-103">Update iosVppEBook</span></span>

<span data-ttu-id="2f684-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f684-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f684-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f684-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f684-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f684-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f684-107">Обновление свойств объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="2f684-107">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f684-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f684-108">Prerequisites</span></span>
<span data-ttu-id="2f684-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f684-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f684-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f684-111">Permission type</span></span>|<span data-ttu-id="2f684-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f684-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f684-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f684-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f684-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f684-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f684-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f684-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f684-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f684-116">Not supported.</span></span>|
|<span data-ttu-id="2f684-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f684-117">Application</span></span>|<span data-ttu-id="2f684-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f684-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f684-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f684-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="2f684-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2f684-120">Request headers</span></span>
|<span data-ttu-id="2f684-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f684-121">Header</span></span>|<span data-ttu-id="2f684-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2f684-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f684-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f684-123">Authorization</span></span>|<span data-ttu-id="2f684-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f684-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f684-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2f684-125">Accept</span></span>|<span data-ttu-id="2f684-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f684-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f684-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f684-127">Request body</span></span>
<span data-ttu-id="2f684-128">В теле запроса добавьте представление объекта [iosVppEBook](../resources/intune-books-iosvppebook.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f684-128">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="2f684-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="2f684-129">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="2f684-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f684-130">Property</span></span>|<span data-ttu-id="2f684-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2f684-131">Type</span></span>|<span data-ttu-id="2f684-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2f684-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f684-133">id</span><span class="sxs-lookup"><span data-stu-id="2f684-133">id</span></span>|<span data-ttu-id="2f684-134">String</span><span class="sxs-lookup"><span data-stu-id="2f684-134">String</span></span>|<span data-ttu-id="2f684-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2f684-135">Key of the entity.</span></span> <span data-ttu-id="2f684-136">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="2f684-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2f684-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2f684-137">displayName</span></span>|<span data-ttu-id="2f684-138">String</span><span class="sxs-lookup"><span data-stu-id="2f684-138">String</span></span>|<span data-ttu-id="2f684-139">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="2f684-139">Name of the eBook.</span></span> <span data-ttu-id="2f684-140">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="2f684-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2f684-141">description</span><span class="sxs-lookup"><span data-stu-id="2f684-141">description</span></span>|<span data-ttu-id="2f684-142">String</span><span class="sxs-lookup"><span data-stu-id="2f684-142">String</span></span>|<span data-ttu-id="2f684-143">Описание.</span><span class="sxs-lookup"><span data-stu-id="2f684-143">Description.</span></span> <span data-ttu-id="2f684-144">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="2f684-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2f684-145">publisher</span><span class="sxs-lookup"><span data-stu-id="2f684-145">publisher</span></span>|<span data-ttu-id="2f684-146">String</span><span class="sxs-lookup"><span data-stu-id="2f684-146">String</span></span>|<span data-ttu-id="2f684-147">Издатель.</span><span class="sxs-lookup"><span data-stu-id="2f684-147">Publisher.</span></span> <span data-ttu-id="2f684-148">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="2f684-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2f684-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f684-149">publishedDateTime</span></span>|<span data-ttu-id="2f684-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f684-150">DateTimeOffset</span></span>|<span data-ttu-id="2f684-151">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="2f684-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="2f684-152">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="2f684-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2f684-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="2f684-153">largeCover</span></span>|[<span data-ttu-id="2f684-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2f684-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2f684-155">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="2f684-155">Book cover.</span></span> <span data-ttu-id="2f684-156">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="2f684-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2f684-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f684-157">createdDateTime</span></span>|<span data-ttu-id="2f684-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f684-158">DateTimeOffset</span></span>|<span data-ttu-id="2f684-159">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="2f684-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="2f684-160">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="2f684-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2f684-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f684-161">lastModifiedDateTime</span></span>|<span data-ttu-id="2f684-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f684-162">DateTimeOffset</span></span>|<span data-ttu-id="2f684-163">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="2f684-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="2f684-164">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="2f684-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2f684-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2f684-165">informationUrl</span></span>|<span data-ttu-id="2f684-166">String</span><span class="sxs-lookup"><span data-stu-id="2f684-166">String</span></span>|<span data-ttu-id="2f684-167">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="2f684-167">The more information Url.</span></span> <span data-ttu-id="2f684-168">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="2f684-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2f684-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2f684-169">privacyInformationUrl</span></span>|<span data-ttu-id="2f684-170">String</span><span class="sxs-lookup"><span data-stu-id="2f684-170">String</span></span>|<span data-ttu-id="2f684-171">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="2f684-171">The privacy statement Url.</span></span> <span data-ttu-id="2f684-172">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="2f684-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="2f684-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="2f684-173">vppTokenId</span></span>|<span data-ttu-id="2f684-174">Guid</span><span class="sxs-lookup"><span data-stu-id="2f684-174">Guid</span></span>|<span data-ttu-id="2f684-175">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="2f684-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="2f684-176">appleId</span><span class="sxs-lookup"><span data-stu-id="2f684-176">appleId</span></span>|<span data-ttu-id="2f684-177">String</span><span class="sxs-lookup"><span data-stu-id="2f684-177">String</span></span>|<span data-ttu-id="2f684-178">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="2f684-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="2f684-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="2f684-179">vppOrganizationName</span></span>|<span data-ttu-id="2f684-180">String</span><span class="sxs-lookup"><span data-stu-id="2f684-180">String</span></span>|<span data-ttu-id="2f684-181">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="2f684-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="2f684-182">genres</span><span class="sxs-lookup"><span data-stu-id="2f684-182">genres</span></span>|<span data-ttu-id="2f684-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2f684-183">String collection</span></span>|<span data-ttu-id="2f684-184">Жанры.</span><span class="sxs-lookup"><span data-stu-id="2f684-184">Genres.</span></span>|
|<span data-ttu-id="2f684-185">language</span><span class="sxs-lookup"><span data-stu-id="2f684-185">language</span></span>|<span data-ttu-id="2f684-186">String</span><span class="sxs-lookup"><span data-stu-id="2f684-186">String</span></span>|<span data-ttu-id="2f684-187">Язык.</span><span class="sxs-lookup"><span data-stu-id="2f684-187">Language.</span></span>|
|<span data-ttu-id="2f684-188">seller</span><span class="sxs-lookup"><span data-stu-id="2f684-188">seller</span></span>|<span data-ttu-id="2f684-189">String</span><span class="sxs-lookup"><span data-stu-id="2f684-189">String</span></span>|<span data-ttu-id="2f684-190">Продавец.</span><span class="sxs-lookup"><span data-stu-id="2f684-190">Seller.</span></span>|
|<span data-ttu-id="2f684-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2f684-191">totalLicenseCount</span></span>|<span data-ttu-id="2f684-192">Int32</span><span class="sxs-lookup"><span data-stu-id="2f684-192">Int32</span></span>|<span data-ttu-id="2f684-193">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="2f684-193">Total license count.</span></span>|
|<span data-ttu-id="2f684-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2f684-194">usedLicenseCount</span></span>|<span data-ttu-id="2f684-195">Int32</span><span class="sxs-lookup"><span data-stu-id="2f684-195">Int32</span></span>|<span data-ttu-id="2f684-196">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="2f684-196">Used license count.</span></span>|
|<span data-ttu-id="2f684-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f684-197">roleScopeTagIds</span></span>|<span data-ttu-id="2f684-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2f684-198">String collection</span></span>|<span data-ttu-id="2f684-199">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="2f684-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="2f684-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f684-200">Response</span></span>
<span data-ttu-id="2f684-201">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f684-201">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f684-202">Пример</span><span class="sxs-lookup"><span data-stu-id="2f684-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f684-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f684-203">Request</span></span>
<span data-ttu-id="2f684-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f684-204">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
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

### <a name="response"></a><span data-ttu-id="2f684-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f684-205">Response</span></span>
<span data-ttu-id="2f684-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f684-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






