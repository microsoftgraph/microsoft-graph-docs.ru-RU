---
title: Обновление объекта iosVppEBook
description: Обновление свойств объекта iosVppEBook.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75923333d699e4cd8cd24a223231d3b720aea542
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328454"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="5e9e3-103">Обновление объекта iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="5e9e3-103">Update iosVppEBook</span></span>

> <span data-ttu-id="5e9e3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e9e3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e9e3-106">Обновление свойств объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e9e3-106">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e9e3-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5e9e3-107">Prerequisites</span></span>
<span data-ttu-id="5e9e3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e9e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e9e3-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e9e3-110">Permission type</span></span>|<span data-ttu-id="5e9e3-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e9e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e9e3-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e9e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5e9e3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e9e3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5e9e3-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e9e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e9e3-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-115">Not supported.</span></span>|
|<span data-ttu-id="5e9e3-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e9e3-116">Application</span></span>|<span data-ttu-id="5e9e3-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e9e3-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e9e3-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e9e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="5e9e3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e9e3-119">Request headers</span></span>
|<span data-ttu-id="5e9e3-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e9e3-120">Header</span></span>|<span data-ttu-id="5e9e3-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5e9e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e9e3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e9e3-122">Authorization</span></span>|<span data-ttu-id="5e9e3-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e9e3-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5e9e3-124">Accept</span></span>|<span data-ttu-id="5e9e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e9e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e9e3-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5e9e3-126">Request body</span></span>
<span data-ttu-id="5e9e3-127">В теле запроса добавьте представление объекта [iosVppEBook](../resources/intune-books-iosvppebook.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-127">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="5e9e3-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e9e3-128">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="5e9e3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e9e3-129">Property</span></span>|<span data-ttu-id="5e9e3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5e9e3-130">Type</span></span>|<span data-ttu-id="5e9e3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5e9e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e9e3-132">id</span><span class="sxs-lookup"><span data-stu-id="5e9e3-132">id</span></span>|<span data-ttu-id="5e9e3-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5e9e3-133">String</span></span>|<span data-ttu-id="5e9e3-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-134">Key of the entity.</span></span> <span data-ttu-id="5e9e3-135">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e9e3-135">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="5e9e3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5e9e3-136">displayName</span></span>|<span data-ttu-id="5e9e3-137">Строка</span><span class="sxs-lookup"><span data-stu-id="5e9e3-137">String</span></span>|<span data-ttu-id="5e9e3-138">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-138">Name of the eBook.</span></span> <span data-ttu-id="5e9e3-139">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e9e3-139">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="5e9e3-140">description</span><span class="sxs-lookup"><span data-stu-id="5e9e3-140">description</span></span>|<span data-ttu-id="5e9e3-141">String</span><span class="sxs-lookup"><span data-stu-id="5e9e3-141">String</span></span>|<span data-ttu-id="5e9e3-142">Описание.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-142">Description.</span></span> <span data-ttu-id="5e9e3-143">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e9e3-143">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="5e9e3-144">publisher</span><span class="sxs-lookup"><span data-stu-id="5e9e3-144">publisher</span></span>|<span data-ttu-id="5e9e3-145">String</span><span class="sxs-lookup"><span data-stu-id="5e9e3-145">String</span></span>|<span data-ttu-id="5e9e3-146">Издатель.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-146">Publisher.</span></span> <span data-ttu-id="5e9e3-147">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e9e3-147">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="5e9e3-148">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e9e3-148">publishedDateTime</span></span>|<span data-ttu-id="5e9e3-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e9e3-149">DateTimeOffset</span></span>|<span data-ttu-id="5e9e3-150">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-150">The date and time when the eBook was published.</span></span> <span data-ttu-id="5e9e3-151">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e9e3-151">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="5e9e3-152">largeCover</span><span class="sxs-lookup"><span data-stu-id="5e9e3-152">largeCover</span></span>|[<span data-ttu-id="5e9e3-153">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5e9e3-153">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5e9e3-154">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-154">Book cover.</span></span> <span data-ttu-id="5e9e3-155">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e9e3-155">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="5e9e3-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e9e3-156">createdDateTime</span></span>|<span data-ttu-id="5e9e3-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e9e3-157">DateTimeOffset</span></span>|<span data-ttu-id="5e9e3-158">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-158">The date and time when the eBook file was created.</span></span> <span data-ttu-id="5e9e3-159">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e9e3-159">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="5e9e3-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e9e3-160">lastModifiedDateTime</span></span>|<span data-ttu-id="5e9e3-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e9e3-161">DateTimeOffset</span></span>|<span data-ttu-id="5e9e3-162">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-162">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="5e9e3-163">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="5e9e3-163">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="5e9e3-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5e9e3-164">informationUrl</span></span>|<span data-ttu-id="5e9e3-165">String</span><span class="sxs-lookup"><span data-stu-id="5e9e3-165">String</span></span>|<span data-ttu-id="5e9e3-166">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-166">The more information Url.</span></span> <span data-ttu-id="5e9e3-167">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e9e3-167">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="5e9e3-168">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5e9e3-168">privacyInformationUrl</span></span>|<span data-ttu-id="5e9e3-169">String</span><span class="sxs-lookup"><span data-stu-id="5e9e3-169">String</span></span>|<span data-ttu-id="5e9e3-170">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-170">The privacy statement Url.</span></span> <span data-ttu-id="5e9e3-171">Наследуется от объекта [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="5e9e3-171">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="5e9e3-172">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="5e9e3-172">vppTokenId</span></span>|<span data-ttu-id="5e9e3-173">Guid</span><span class="sxs-lookup"><span data-stu-id="5e9e3-173">Guid</span></span>|<span data-ttu-id="5e9e3-174">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-174">The Vpp token ID.</span></span>|
|<span data-ttu-id="5e9e3-175">appleId</span><span class="sxs-lookup"><span data-stu-id="5e9e3-175">appleId</span></span>|<span data-ttu-id="5e9e3-176">Строка</span><span class="sxs-lookup"><span data-stu-id="5e9e3-176">String</span></span>|<span data-ttu-id="5e9e3-177">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-177">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="5e9e3-178">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="5e9e3-178">vppOrganizationName</span></span>|<span data-ttu-id="5e9e3-179">String</span><span class="sxs-lookup"><span data-stu-id="5e9e3-179">String</span></span>|<span data-ttu-id="5e9e3-180">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-180">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="5e9e3-181">genres</span><span class="sxs-lookup"><span data-stu-id="5e9e3-181">genres</span></span>|<span data-ttu-id="5e9e3-182">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5e9e3-182">String collection</span></span>|<span data-ttu-id="5e9e3-183">Жанры.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-183">Genres.</span></span>|
|<span data-ttu-id="5e9e3-184">language</span><span class="sxs-lookup"><span data-stu-id="5e9e3-184">language</span></span>|<span data-ttu-id="5e9e3-185">String</span><span class="sxs-lookup"><span data-stu-id="5e9e3-185">String</span></span>|<span data-ttu-id="5e9e3-186">Язык.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-186">Language.</span></span>|
|<span data-ttu-id="5e9e3-187">seller</span><span class="sxs-lookup"><span data-stu-id="5e9e3-187">seller</span></span>|<span data-ttu-id="5e9e3-188">String</span><span class="sxs-lookup"><span data-stu-id="5e9e3-188">String</span></span>|<span data-ttu-id="5e9e3-189">Продавец.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-189">Seller.</span></span>|
|<span data-ttu-id="5e9e3-190">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="5e9e3-190">totalLicenseCount</span></span>|<span data-ttu-id="5e9e3-191">Int32</span><span class="sxs-lookup"><span data-stu-id="5e9e3-191">Int32</span></span>|<span data-ttu-id="5e9e3-192">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-192">Total license count.</span></span>|
|<span data-ttu-id="5e9e3-193">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="5e9e3-193">usedLicenseCount</span></span>|<span data-ttu-id="5e9e3-194">Int32</span><span class="sxs-lookup"><span data-stu-id="5e9e3-194">Int32</span></span>|<span data-ttu-id="5e9e3-195">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-195">Used license count.</span></span>|
|<span data-ttu-id="5e9e3-196">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5e9e3-196">roleScopeTagIds</span></span>|<span data-ttu-id="5e9e3-197">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="5e9e3-197">String collection</span></span>|<span data-ttu-id="5e9e3-198">Список тегов областей для этого экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-198">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="5e9e3-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e9e3-199">Response</span></span>
<span data-ttu-id="5e9e3-200">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-200">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e9e3-201">Пример</span><span class="sxs-lookup"><span data-stu-id="5e9e3-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e9e3-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e9e3-202">Request</span></span>
<span data-ttu-id="5e9e3-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5e9e3-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e9e3-204">Response</span></span>
<span data-ttu-id="5e9e3-p112">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e9e3-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






