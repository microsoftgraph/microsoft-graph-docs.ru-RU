---
title: 'Едукатионсинчронизатионпрофиле: адрес uploadurl'
description: Получение подписи общего доступа (SAS) для отправки исходных файлов в хранилище BLOB-объектов Azure для определенного профиля синхронизации данных School в клиенте. Срок действия маркера SAS — 1 час.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d49f64a6ed809388e2e60b84c8ba0bb89ca2b2f1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259390"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="ed7d0-104">Едукатионсинчронизатионпрофиле: адрес uploadurl</span><span class="sxs-lookup"><span data-stu-id="ed7d0-104">educationSynchronizationProfile: uploadUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed7d0-105">Получение подписи общего доступа (SAS) для отправки исходных файлов в хранилище BLOB-объектов Azure для определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-105">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="ed7d0-106">Срок действия маркера SAS — 1 час.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-106">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="ed7d0-107">URL-адрес отправки предоставляется только для [поставщика данных в формате CSV](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="ed7d0-107">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="ed7d0-108">**Примечание:** Чтобы получить доступ к хранилищу больших двоичных объектов с маркером SAS, используйте пакеты SDK или [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy) [хранилища Azure](https://github.com/search?q=org%3AAzure+azure-storage) .</span><span class="sxs-lookup"><span data-stu-id="ed7d0-108">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed7d0-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed7d0-109">Permissions</span></span>
<span data-ttu-id="ed7d0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed7d0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed7d0-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed7d0-112">Permission type</span></span> | <span data-ttu-id="ed7d0-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed7d0-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ed7d0-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed7d0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ed7d0-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed7d0-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="ed7d0-116">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed7d0-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ed7d0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-117">Not supported.</span></span>|
|<span data-ttu-id="ed7d0-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed7d0-118">Application</span></span>|<span data-ttu-id="ed7d0-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed7d0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed7d0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="ed7d0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed7d0-121">Request headers</span></span>
| <span data-ttu-id="ed7d0-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ed7d0-122">Name</span></span>       | <span data-ttu-id="ed7d0-123">Тип</span><span class="sxs-lookup"><span data-stu-id="ed7d0-123">Type</span></span> | <span data-ttu-id="ed7d0-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ed7d0-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ed7d0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed7d0-125">Authorization</span></span>  | <span data-ttu-id="ed7d0-126">string</span><span class="sxs-lookup"><span data-stu-id="ed7d0-126">string</span></span>  | <span data-ttu-id="ed7d0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed7d0-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed7d0-129">Request body</span></span>
<span data-ttu-id="ed7d0-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ed7d0-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed7d0-131">Response</span></span>
<span data-ttu-id="ed7d0-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и URL-адрес SAS для [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-132">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="ed7d0-133">Если предыдущий запрос по-прежнему обрабатывается, этот метод возвращает значение `409 Conflict` , указывающее на то, что отправка в [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md)заблокирована.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-133">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="ed7d0-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ed7d0-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed7d0-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed7d0-135">Request</span></span>
<span data-ttu-id="ed7d0-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a><span data-ttu-id="ed7d0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed7d0-137">Response</span></span>
<span data-ttu-id="ed7d0-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-138">The following is an example of the response.</span></span> 

><span data-ttu-id="ed7d0-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed7d0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ed7d0-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ed7d0-141">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ed7d0-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="ed7d0-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_uploadurl-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="ed7d0-143">C#</span><span class="sxs-lookup"><span data-stu-id="ed7d0-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_uploadurl-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ed7d0-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ed7d0-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_uploadurl-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-uploadurl.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-uploadurl.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-uploadurl.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
