---
title: 'Едукатионсинчронизатионпрофиле: адрес uploadurl'
description: Получение подписи общего доступа (SAS) для отправки исходных файлов в хранилище BLOB-объектов Azure для определенного профиля синхронизации данных School в клиенте. Срок действия маркера SAS — 1 час.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ea5806cc0f95d19d1b3b9b63ab4139272ba50c76
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323901"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="613a4-104">Едукатионсинчронизатионпрофиле: адрес uploadurl</span><span class="sxs-lookup"><span data-stu-id="613a4-104">educationSynchronizationProfile: uploadUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="613a4-105">Получение подписи общего доступа (SAS) для отправки исходных файлов в хранилище BLOB-объектов Azure для определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="613a4-105">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="613a4-106">Срок действия маркера SAS — 1 час.</span><span class="sxs-lookup"><span data-stu-id="613a4-106">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="613a4-107">URL-адрес отправки предоставляется только для [поставщика данных в формате CSV](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="613a4-107">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="613a4-108">**Примечание:** Чтобы получить доступ к хранилищу больших двоичных объектов с маркером SAS, используйте пакеты SDK или [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy) [хранилища Azure](https://github.com/search?q=org%3AAzure+azure-storage) .</span><span class="sxs-lookup"><span data-stu-id="613a4-108">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="613a4-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="613a4-109">Permissions</span></span>
<span data-ttu-id="613a4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="613a4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="613a4-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="613a4-112">Permission type</span></span> | <span data-ttu-id="613a4-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="613a4-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="613a4-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="613a4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="613a4-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="613a4-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="613a4-116">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="613a4-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="613a4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="613a4-117">Not supported.</span></span>|
|<span data-ttu-id="613a4-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="613a4-118">Application</span></span>|<span data-ttu-id="613a4-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="613a4-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="613a4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="613a4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="613a4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="613a4-121">Request headers</span></span>
| <span data-ttu-id="613a4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="613a4-122">Name</span></span>       | <span data-ttu-id="613a4-123">Тип</span><span class="sxs-lookup"><span data-stu-id="613a4-123">Type</span></span> | <span data-ttu-id="613a4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="613a4-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="613a4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="613a4-125">Authorization</span></span>  | <span data-ttu-id="613a4-126">string</span><span class="sxs-lookup"><span data-stu-id="613a4-126">string</span></span>  | <span data-ttu-id="613a4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="613a4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="613a4-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="613a4-129">Request body</span></span>
<span data-ttu-id="613a4-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="613a4-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="613a4-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="613a4-131">Response</span></span>
<span data-ttu-id="613a4-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и URL-адрес SAS для [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="613a4-132">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="613a4-133">Если предыдущий запрос по-прежнему обрабатывается, этот метод возвращает значение `409 Conflict` , указывающее на то, что отправка в [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md)заблокирована.</span><span class="sxs-lookup"><span data-stu-id="613a4-133">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="613a4-134">Пример</span><span class="sxs-lookup"><span data-stu-id="613a4-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="613a4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="613a4-135">Request</span></span>
<span data-ttu-id="613a4-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="613a4-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="613a4-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="613a4-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="613a4-138">C#</span><span class="sxs-lookup"><span data-stu-id="613a4-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-uploadurl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="613a4-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="613a4-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-uploadurl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="613a4-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="613a4-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-uploadurl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="613a4-141">Java</span><span class="sxs-lookup"><span data-stu-id="613a4-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-uploadurl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="613a4-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="613a4-142">Response</span></span>
<span data-ttu-id="613a4-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="613a4-143">The following is an example of the response.</span></span> 

><span data-ttu-id="613a4-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="613a4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
