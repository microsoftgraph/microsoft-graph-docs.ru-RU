---
title: 'Едукатионсинчронизатионпрофиле: адрес uploadurl'
description: Получение подписи общего доступа (SAS) для отправки исходных файлов в хранилище BLOB-объектов Azure для определенного профиля синхронизации данных School в клиенте. Срок действия маркера SAS — 1 час.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: abab00a78e9160e4c1cfe856bc31e8ee691bdf9f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424227"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="ed858-104">Едукатионсинчронизатионпрофиле: адрес uploadurl</span><span class="sxs-lookup"><span data-stu-id="ed858-104">educationSynchronizationProfile: uploadUrl</span></span>

<span data-ttu-id="ed858-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed858-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed858-106">Получение подписи общего доступа (SAS) для отправки исходных файлов в хранилище BLOB-объектов Azure для определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ed858-106">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="ed858-107">Срок действия маркера SAS — 1 час.</span><span class="sxs-lookup"><span data-stu-id="ed858-107">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="ed858-108">URL-адрес отправки предоставляется только для [поставщика данных в формате CSV](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="ed858-108">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="ed858-109">**Примечание:** Чтобы получить доступ к хранилищу больших двоичных объектов с маркером SAS, используйте пакеты SDK или [AzCopy](/azure/storage/storage-use-azcopy) [хранилища Azure](https://github.com/search?q=org%3AAzure+azure-storage) .</span><span class="sxs-lookup"><span data-stu-id="ed858-109">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed858-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed858-110">Permissions</span></span>
<span data-ttu-id="ed858-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed858-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed858-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ed858-113">Permission type</span></span> | <span data-ttu-id="ed858-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ed858-114">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ed858-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ed858-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ed858-116">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed858-116">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="ed858-117">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ed858-117">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ed858-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed858-118">Not supported.</span></span>|
|<span data-ttu-id="ed858-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ed858-119">Application</span></span>|<span data-ttu-id="ed858-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed858-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed858-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ed858-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="ed858-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ed858-122">Request headers</span></span>
| <span data-ttu-id="ed858-123">Имя</span><span class="sxs-lookup"><span data-stu-id="ed858-123">Name</span></span>       | <span data-ttu-id="ed858-124">Тип</span><span class="sxs-lookup"><span data-stu-id="ed858-124">Type</span></span> | <span data-ttu-id="ed858-125">Описание</span><span class="sxs-lookup"><span data-stu-id="ed858-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ed858-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed858-126">Authorization</span></span>  | <span data-ttu-id="ed858-127">string</span><span class="sxs-lookup"><span data-stu-id="ed858-127">string</span></span>  | <span data-ttu-id="ed858-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ed858-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed858-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ed858-130">Request body</span></span>
<span data-ttu-id="ed858-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ed858-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ed858-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="ed858-132">Response</span></span>
<span data-ttu-id="ed858-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и URL-адрес SAS для [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ed858-133">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="ed858-134">Если предыдущий запрос по-прежнему обрабатывается, этот метод возвращает значение `409 Conflict` , указывающее на то, что отправка в [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md)заблокирована.</span><span class="sxs-lookup"><span data-stu-id="ed858-134">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="ed858-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ed858-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed858-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ed858-136">Request</span></span>
<span data-ttu-id="ed858-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ed858-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed858-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed858-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```
# <a name="c"></a>[<span data-ttu-id="ed858-139">C#</span><span class="sxs-lookup"><span data-stu-id="ed858-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-uploadurl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed858-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed858-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-uploadurl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed858-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed858-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-uploadurl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ed858-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ed858-142">Response</span></span>
<span data-ttu-id="ed858-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ed858-143">The following is an example of the response.</span></span>

><span data-ttu-id="ed858-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ed858-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
