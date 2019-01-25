---
title: 'educationSynchronizationProfile: uploadUrl'
description: Получение доступа к общим подписи (SAS) для загрузки исходных файлов в хранилище Azure больших двоичных объектов для синхронизации профиля данных конкретного school в клиентов. Маркер SAS имеет допустимость часа.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 74f37f5653147691c408cf83e3039920957352c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511599"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="cdcb5-104">educationSynchronizationProfile: uploadUrl</span><span class="sxs-lookup"><span data-stu-id="cdcb5-104">educationSynchronizationProfile: uploadUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cdcb5-105">Получение доступа к общим подписи (SAS) для загрузки исходных файлов в хранилище Azure больших двоичных объектов для конкретных школа данных [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="cdcb5-105">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="cdcb5-106">Маркер SAS имеет допустимость часа.</span><span class="sxs-lookup"><span data-stu-id="cdcb5-106">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="cdcb5-107">Передача URL-адрес предоставляется только для [поставщика данных CSV](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="cdcb5-107">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="cdcb5-108">**Примечание:** Для доступа к хранилища больших двоичных объектов с маркером SAS, с помощью [хранилища Azure SDK](https://github.com/search?q=org%3AAzure+azure-storage) или [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span><span class="sxs-lookup"><span data-stu-id="cdcb5-108">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="cdcb5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdcb5-109">Permissions</span></span>
<span data-ttu-id="cdcb5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdcb5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cdcb5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cdcb5-112">Permission type</span></span> | <span data-ttu-id="cdcb5-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cdcb5-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="cdcb5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cdcb5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cdcb5-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdcb5-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="cdcb5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cdcb5-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cdcb5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdcb5-117">Not supported.</span></span>|
|<span data-ttu-id="cdcb5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cdcb5-118">Application</span></span>|<span data-ttu-id="cdcb5-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdcb5-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdcb5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cdcb5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="cdcb5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cdcb5-121">Request headers</span></span>
| <span data-ttu-id="cdcb5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cdcb5-122">Name</span></span>       | <span data-ttu-id="cdcb5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="cdcb5-123">Type</span></span> | <span data-ttu-id="cdcb5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cdcb5-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cdcb5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdcb5-125">Authorization</span></span>  | <span data-ttu-id="cdcb5-126">string</span><span class="sxs-lookup"><span data-stu-id="cdcb5-126">string</span></span>  | <span data-ttu-id="cdcb5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cdcb5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cdcb5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cdcb5-129">Request body</span></span>
<span data-ttu-id="cdcb5-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cdcb5-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cdcb5-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdcb5-131">Response</span></span>
<span data-ttu-id="cdcb5-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и URL-адрес SAS [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cdcb5-132">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="cdcb5-133">Если по-прежнему обрабатывается предыдущего запроса, этот метод возвращает `409 Conflict` , указывающее, что загрузка в настоящее время заблокирован по [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="cdcb5-133">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="cdcb5-134">Пример</span><span class="sxs-lookup"><span data-stu-id="cdcb5-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdcb5-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="cdcb5-135">Request</span></span>
<span data-ttu-id="cdcb5-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cdcb5-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a><span data-ttu-id="cdcb5-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="cdcb5-137">Response</span></span>
<span data-ttu-id="cdcb5-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cdcb5-138">The following is an example of the response.</span></span> 

><span data-ttu-id="cdcb5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cdcb5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "String",
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 314

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#String",
    "value": "https://sdsstorage.blob.core.windows.net/86904b1e-c7d0-4ead-b13a-98f11fc400ee?sv=2015-07-08&sr=c&si=SharedAccessPolicy_20170704044441&sig=CH65vxxqXETCkQNH0Lfsu31cUo0s0XcEEo0OE2YiL6Q%3D&se=2017-07-04T08%3A43%3A01Z&sp=w"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-uploadurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
