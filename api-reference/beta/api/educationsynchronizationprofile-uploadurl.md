---
title: 'educationSynchronizationProfile: uploadUrl'
description: Получение доступа к общим подписи (SAS) для загрузки исходных файлов в хранилище Azure больших двоичных объектов для синхронизации профиля данных конкретного school в клиентов. Маркер SAS имеет допустимость часа.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 2f6b10bda218bafbe18698defed138c39a45cc7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894147"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="56234-104">educationSynchronizationProfile: uploadUrl</span><span class="sxs-lookup"><span data-stu-id="56234-104">educationSynchronizationProfile: uploadUrl</span></span>

> <span data-ttu-id="56234-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="56234-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56234-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56234-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56234-107">Получение доступа к общим подписи (SAS) для загрузки исходных файлов в хранилище Azure больших двоичных объектов для конкретных школа данных [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="56234-107">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="56234-108">Маркер SAS имеет допустимость часа.</span><span class="sxs-lookup"><span data-stu-id="56234-108">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="56234-109">Передача URL-адрес предоставляется только для [поставщика данных CSV](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="56234-109">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="56234-110">**Примечание:** Для доступа к хранилища больших двоичных объектов с маркером SAS, с помощью [хранилища Azure SDK](https://github.com/search?q=org%3AAzure+azure-storage) или [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span><span class="sxs-lookup"><span data-stu-id="56234-110">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="56234-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56234-111">Permissions</span></span>
<span data-ttu-id="56234-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56234-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56234-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56234-114">Permission type</span></span> | <span data-ttu-id="56234-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="56234-115">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="56234-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56234-116">Delegated (work or school account)</span></span> | <span data-ttu-id="56234-117">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56234-117">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="56234-118">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="56234-118">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="56234-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56234-119">Not supported.</span></span>|
|<span data-ttu-id="56234-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56234-120">Application</span></span>|<span data-ttu-id="56234-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56234-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56234-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56234-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="56234-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56234-123">Request headers</span></span>
| <span data-ttu-id="56234-124">Имя</span><span class="sxs-lookup"><span data-stu-id="56234-124">Name</span></span>       | <span data-ttu-id="56234-125">Тип</span><span class="sxs-lookup"><span data-stu-id="56234-125">Type</span></span> | <span data-ttu-id="56234-126">Описание</span><span class="sxs-lookup"><span data-stu-id="56234-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="56234-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="56234-127">Authorization</span></span>  | <span data-ttu-id="56234-128">string</span><span class="sxs-lookup"><span data-stu-id="56234-128">string</span></span>  | <span data-ttu-id="56234-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56234-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="56234-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56234-131">Request body</span></span>
<span data-ttu-id="56234-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56234-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="56234-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="56234-133">Response</span></span>
<span data-ttu-id="56234-134">Успешно завершена, этот метод возвращает `200 OK` код ответа и URL-адрес SAS [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="56234-134">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="56234-135">Если по-прежнему обрабатывается предыдущего запроса, этот метод возвращает `409 Conflict` , указывающее, что загрузка в настоящее время заблокирован по [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span><span class="sxs-lookup"><span data-stu-id="56234-135">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="56234-136">Пример</span><span class="sxs-lookup"><span data-stu-id="56234-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56234-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="56234-137">Request</span></span>
<span data-ttu-id="56234-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56234-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a><span data-ttu-id="56234-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="56234-139">Response</span></span>
<span data-ttu-id="56234-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56234-140">The following is an example of the response.</span></span> 

><span data-ttu-id="56234-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56234-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
