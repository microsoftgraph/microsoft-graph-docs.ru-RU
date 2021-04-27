---
title: 'educationSynchronizationProfile: uploadUrl'
description: Извлечение подписи общего доступа (SAS) для отправки исходных файлов в хранилище BLOB Azure для определенного профиля синхронизации школьных данных в клиенте. Срок действия маркера SAS - один час.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8e3abb8a558ed26b2a47467faabf30fffba2409d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042956"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="c2dd4-104">educationSynchronizationProfile: uploadUrl</span><span class="sxs-lookup"><span data-stu-id="c2dd4-104">educationSynchronizationProfile: uploadUrl</span></span>

<span data-ttu-id="c2dd4-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2dd4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2dd4-106">Извлечение подписи общего доступа (SAS) для отправки исходных файлов в хранилище BLOB Azure для определенного профиля синхронизации школьных данных [в](../resources/educationsynchronizationprofile.md) клиенте.</span><span class="sxs-lookup"><span data-stu-id="c2dd4-106">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="c2dd4-107">Срок действия маркера SAS - один час.</span><span class="sxs-lookup"><span data-stu-id="c2dd4-107">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="c2dd4-108">URL-адрес загрузки предоставляется только поставщику [данных CSV.](../resources/educationcsvdataprovider.md)</span><span class="sxs-lookup"><span data-stu-id="c2dd4-108">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="c2dd4-109">**Примечание:** Чтобы получить доступ к хранилище blob с помощью маркера SAS, используйте [SDKs](https://github.com/search?q=org%3AAzure+azure-storage) хранилища Azure или [AzCopy.](/azure/storage/storage-use-azcopy)</span><span class="sxs-lookup"><span data-stu-id="c2dd4-109">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2dd4-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2dd4-110">Permissions</span></span>
<span data-ttu-id="c2dd4-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2dd4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2dd4-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2dd4-113">Permission type</span></span> | <span data-ttu-id="c2dd4-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2dd4-114">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c2dd4-115">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2dd4-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c2dd4-116">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2dd4-116">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="c2dd4-117">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2dd4-117">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c2dd4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2dd4-118">Not supported.</span></span>|
|<span data-ttu-id="c2dd4-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2dd4-119">Application</span></span>|<span data-ttu-id="c2dd4-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2dd4-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2dd4-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2dd4-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="c2dd4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2dd4-122">Request headers</span></span>
| <span data-ttu-id="c2dd4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="c2dd4-123">Name</span></span>       | <span data-ttu-id="c2dd4-124">Тип</span><span class="sxs-lookup"><span data-stu-id="c2dd4-124">Type</span></span> | <span data-ttu-id="c2dd4-125">Описание</span><span class="sxs-lookup"><span data-stu-id="c2dd4-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c2dd4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2dd4-126">Authorization</span></span>  | <span data-ttu-id="c2dd4-127">string</span><span class="sxs-lookup"><span data-stu-id="c2dd4-127">string</span></span>  | <span data-ttu-id="c2dd4-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2dd4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2dd4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2dd4-130">Request body</span></span>
<span data-ttu-id="c2dd4-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2dd4-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c2dd4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2dd4-132">Response</span></span>
<span data-ttu-id="c2dd4-133">В случае успешной работы этот метод возвращает код отклика и `200 OK` URL-адрес SAS для [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c2dd4-133">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="c2dd4-134">Если предыдущий запрос еще обрабатывается, этот метод возвращает указание на то, что загрузка в настоящее время заблокирована для `409 Conflict` [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="c2dd4-134">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="c2dd4-135">Пример</span><span class="sxs-lookup"><span data-stu-id="c2dd4-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c2dd4-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2dd4-136">Request</span></span>
<span data-ttu-id="c2dd4-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2dd4-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2dd4-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2dd4-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```
# <a name="c"></a>[<span data-ttu-id="c2dd4-139">C#</span><span class="sxs-lookup"><span data-stu-id="c2dd4-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-uploadurl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2dd4-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2dd4-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-uploadurl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2dd4-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2dd4-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-uploadurl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2dd4-142">Java</span><span class="sxs-lookup"><span data-stu-id="c2dd4-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-uploadurl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c2dd4-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2dd4-143">Response</span></span>
<span data-ttu-id="c2dd4-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c2dd4-144">The following is an example of the response.</span></span>

><span data-ttu-id="c2dd4-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c2dd4-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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


