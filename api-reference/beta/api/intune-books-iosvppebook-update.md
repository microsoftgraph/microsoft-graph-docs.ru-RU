---
title: Обновление объекта iosVppEBook
description: Обновление свойств объекта iosVppEBook.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7279b8da1ffe159dba56f4a5a10345243703da1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393748"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="ff646-103">Обновление объекта iosVppEBook</span><span class="sxs-lookup"><span data-stu-id="ff646-103">Update iosVppEBook</span></span>

> <span data-ttu-id="ff646-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ff646-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ff646-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff646-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff646-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff646-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff646-107">Обновление свойств объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="ff646-107">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff646-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ff646-108">Prerequisites</span></span>
<span data-ttu-id="ff646-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ff646-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ff646-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff646-111">Permission type</span></span>|<span data-ttu-id="ff646-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff646-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff646-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff646-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff646-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff646-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff646-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff646-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff646-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff646-116">Not supported.</span></span>|
|<span data-ttu-id="ff646-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff646-117">Application</span></span>|<span data-ttu-id="ff646-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff646-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff646-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff646-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="ff646-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff646-120">Request headers</span></span>
|<span data-ttu-id="ff646-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ff646-121">Header</span></span>|<span data-ttu-id="ff646-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ff646-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff646-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff646-123">Authorization</span></span>|<span data-ttu-id="ff646-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ff646-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff646-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ff646-125">Accept</span></span>|<span data-ttu-id="ff646-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff646-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff646-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ff646-127">Request body</span></span>
<span data-ttu-id="ff646-128">В теле запроса добавьте представление объекта [iosVppEBook](../resources/intune-books-iosvppebook.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff646-128">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="ff646-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="ff646-129">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="ff646-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff646-130">Property</span></span>|<span data-ttu-id="ff646-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ff646-131">Type</span></span>|<span data-ttu-id="ff646-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ff646-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff646-133">id</span><span class="sxs-lookup"><span data-stu-id="ff646-133">id</span></span>|<span data-ttu-id="ff646-134">String</span><span class="sxs-lookup"><span data-stu-id="ff646-134">String</span></span>|<span data-ttu-id="ff646-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ff646-135">Key of the entity.</span></span> <span data-ttu-id="ff646-136">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="ff646-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ff646-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ff646-137">displayName</span></span>|<span data-ttu-id="ff646-138">String</span><span class="sxs-lookup"><span data-stu-id="ff646-138">String</span></span>|<span data-ttu-id="ff646-139">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ff646-139">Name of the eBook.</span></span> <span data-ttu-id="ff646-140">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="ff646-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ff646-141">description</span><span class="sxs-lookup"><span data-stu-id="ff646-141">description</span></span>|<span data-ttu-id="ff646-142">String</span><span class="sxs-lookup"><span data-stu-id="ff646-142">String</span></span>|<span data-ttu-id="ff646-143">Описание.</span><span class="sxs-lookup"><span data-stu-id="ff646-143">Description.</span></span> <span data-ttu-id="ff646-144">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="ff646-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ff646-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ff646-145">publisher</span></span>|<span data-ttu-id="ff646-146">String</span><span class="sxs-lookup"><span data-stu-id="ff646-146">String</span></span>|<span data-ttu-id="ff646-147">Издатель.</span><span class="sxs-lookup"><span data-stu-id="ff646-147">Publisher.</span></span> <span data-ttu-id="ff646-148">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="ff646-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ff646-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff646-149">publishedDateTime</span></span>|<span data-ttu-id="ff646-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff646-150">DateTimeOffset</span></span>|<span data-ttu-id="ff646-151">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ff646-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="ff646-152">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="ff646-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ff646-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="ff646-153">largeCover</span></span>|[<span data-ttu-id="ff646-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ff646-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ff646-155">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="ff646-155">Book cover.</span></span> <span data-ttu-id="ff646-156">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="ff646-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ff646-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff646-157">createdDateTime</span></span>|<span data-ttu-id="ff646-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff646-158">DateTimeOffset</span></span>|<span data-ttu-id="ff646-159">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ff646-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="ff646-160">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="ff646-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ff646-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff646-161">lastModifiedDateTime</span></span>|<span data-ttu-id="ff646-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff646-162">DateTimeOffset</span></span>|<span data-ttu-id="ff646-163">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="ff646-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="ff646-164">Унаследован от объекта [managedEBook](../resources/intune-books-managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="ff646-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ff646-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ff646-165">informationUrl</span></span>|<span data-ttu-id="ff646-166">String</span><span class="sxs-lookup"><span data-stu-id="ff646-166">String</span></span>|<span data-ttu-id="ff646-167">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="ff646-167">The more information Url.</span></span> <span data-ttu-id="ff646-168">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="ff646-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ff646-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ff646-169">privacyInformationUrl</span></span>|<span data-ttu-id="ff646-170">String</span><span class="sxs-lookup"><span data-stu-id="ff646-170">String</span></span>|<span data-ttu-id="ff646-171">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="ff646-171">The privacy statement Url.</span></span> <span data-ttu-id="ff646-172">Наследуется от [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="ff646-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ff646-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="ff646-173">vppTokenId</span></span>|<span data-ttu-id="ff646-174">Guid</span><span class="sxs-lookup"><span data-stu-id="ff646-174">Guid</span></span>|<span data-ttu-id="ff646-175">Идентификатор токена VPP.</span><span class="sxs-lookup"><span data-stu-id="ff646-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="ff646-176">appleId</span><span class="sxs-lookup"><span data-stu-id="ff646-176">appleId</span></span>|<span data-ttu-id="ff646-177">String</span><span class="sxs-lookup"><span data-stu-id="ff646-177">String</span></span>|<span data-ttu-id="ff646-178">Идентификатор Apple ID, связанный с токеном VPP.</span><span class="sxs-lookup"><span data-stu-id="ff646-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="ff646-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="ff646-179">vppOrganizationName</span></span>|<span data-ttu-id="ff646-180">String</span><span class="sxs-lookup"><span data-stu-id="ff646-180">String</span></span>|<span data-ttu-id="ff646-181">Название организации для токена VPP.</span><span class="sxs-lookup"><span data-stu-id="ff646-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="ff646-182">genres</span><span class="sxs-lookup"><span data-stu-id="ff646-182">genres</span></span>|<span data-ttu-id="ff646-183">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ff646-183">String collection</span></span>|<span data-ttu-id="ff646-184">Жанры.</span><span class="sxs-lookup"><span data-stu-id="ff646-184">Genres.</span></span>|
|<span data-ttu-id="ff646-185">language</span><span class="sxs-lookup"><span data-stu-id="ff646-185">language</span></span>|<span data-ttu-id="ff646-186">String</span><span class="sxs-lookup"><span data-stu-id="ff646-186">String</span></span>|<span data-ttu-id="ff646-187">Язык.</span><span class="sxs-lookup"><span data-stu-id="ff646-187">Language.</span></span>|
|<span data-ttu-id="ff646-188">seller</span><span class="sxs-lookup"><span data-stu-id="ff646-188">seller</span></span>|<span data-ttu-id="ff646-189">String</span><span class="sxs-lookup"><span data-stu-id="ff646-189">String</span></span>|<span data-ttu-id="ff646-190">Продавец.</span><span class="sxs-lookup"><span data-stu-id="ff646-190">Seller.</span></span>|
|<span data-ttu-id="ff646-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ff646-191">totalLicenseCount</span></span>|<span data-ttu-id="ff646-192">Int32</span><span class="sxs-lookup"><span data-stu-id="ff646-192">Int32</span></span>|<span data-ttu-id="ff646-193">Общее число лицензий.</span><span class="sxs-lookup"><span data-stu-id="ff646-193">Total license count.</span></span>|
|<span data-ttu-id="ff646-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ff646-194">usedLicenseCount</span></span>|<span data-ttu-id="ff646-195">Int32</span><span class="sxs-lookup"><span data-stu-id="ff646-195">Int32</span></span>|<span data-ttu-id="ff646-196">Число используемых лицензий.</span><span class="sxs-lookup"><span data-stu-id="ff646-196">Used license count.</span></span>|
|<span data-ttu-id="ff646-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff646-197">roleScopeTagIds</span></span>|<span data-ttu-id="ff646-198">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ff646-198">String collection</span></span>|<span data-ttu-id="ff646-199">Список областей теги для данного экземпляра сущности.</span><span class="sxs-lookup"><span data-stu-id="ff646-199">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="ff646-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff646-200">Response</span></span>
<span data-ttu-id="ff646-201">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosVppEBook](../resources/intune-books-iosvppebook.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ff646-201">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff646-202">Пример</span><span class="sxs-lookup"><span data-stu-id="ff646-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff646-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff646-203">Request</span></span>
<span data-ttu-id="ff646-204">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff646-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ff646-205">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff646-205">Response</span></span>
<span data-ttu-id="ff646-p113">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ff646-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




