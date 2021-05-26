---
title: Начните синхронизацию после отправки файлов в educationSynchronizationProfile
description: Проверка файлов, загруженных в определенный профиль синхронизации школьных данных в клиенте. Если проверка будет успешной, в профиле начнется синхронизация. В противном случае ответ будет содержать ошибки и предупреждения. Если ответ содержит ошибки, синхронизация не начнется. Если ответ содержит только предупреждения, начнется синхронизация.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2150fd1e54cdb4d5afa2ecbd9a451104d00f2a38
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664722"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="1c73a-107">Начните синхронизацию после отправки файлов в educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="1c73a-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

<span data-ttu-id="1c73a-108">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c73a-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c73a-109">Проверка файлов, загруженных в определенный профиль синхронизации школьных данных [в](../resources/educationsynchronizationprofile.md) клиенте.</span><span class="sxs-lookup"><span data-stu-id="1c73a-109">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="1c73a-110">Если проверка будет успешной, в профиле начнется синхронизация.</span><span class="sxs-lookup"><span data-stu-id="1c73a-110">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="1c73a-111">В противном случае ответ будет содержать ошибки и предупреждения.</span><span class="sxs-lookup"><span data-stu-id="1c73a-111">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="1c73a-112">Если ответ содержит ошибки, синхронизация не начнется.</span><span class="sxs-lookup"><span data-stu-id="1c73a-112">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="1c73a-113">Если ответ содержит только предупреждения, начнется синхронизация.</span><span class="sxs-lookup"><span data-stu-id="1c73a-113">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="1c73a-114">**Примечание:** Используйте этот метод только в том случае, если поставщик данных имеет тип [educationcsvdataprovider.](../resources/educationcsvdataprovider.md)</span><span class="sxs-lookup"><span data-stu-id="1c73a-114">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="1c73a-115">Кроме того, перед началом работы необходимо предварительно прозаить состояние свойства профиля.</span><span class="sxs-lookup"><span data-stu-id="1c73a-115">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="1c73a-116">Опрос объекта профиля, чтобы проверить его свойство состояния.</span><span class="sxs-lookup"><span data-stu-id="1c73a-116">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c73a-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c73a-117">Permissions</span></span>
<span data-ttu-id="1c73a-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c73a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c73a-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c73a-120">Permission type</span></span> | <span data-ttu-id="1c73a-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c73a-121">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="1c73a-122">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c73a-122">Delegated (work or school account)</span></span> | <span data-ttu-id="1c73a-123">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c73a-123">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="1c73a-124">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c73a-124">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1c73a-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c73a-125">Not supported.</span></span>|
|<span data-ttu-id="1c73a-126">Приложение</span><span class="sxs-lookup"><span data-stu-id="1c73a-126">Application</span></span>|<span data-ttu-id="1c73a-127">EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c73a-127">EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c73a-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c73a-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="1c73a-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c73a-129">Request headers</span></span>
| <span data-ttu-id="1c73a-130">Имя</span><span class="sxs-lookup"><span data-stu-id="1c73a-130">Name</span></span>       | <span data-ttu-id="1c73a-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1c73a-131">Type</span></span> | <span data-ttu-id="1c73a-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1c73a-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1c73a-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c73a-133">Authorization</span></span>  | <span data-ttu-id="1c73a-134">string</span><span class="sxs-lookup"><span data-stu-id="1c73a-134">string</span></span>  | <span data-ttu-id="1c73a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c73a-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1c73a-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c73a-137">Request body</span></span>
<span data-ttu-id="1c73a-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c73a-138">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1c73a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c73a-139">Response</span></span>
<span data-ttu-id="1c73a-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1c73a-140">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="1c73a-141">В случае неудачи `400 Bad Request` возвращается .</span><span class="sxs-lookup"><span data-stu-id="1c73a-141">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="1c73a-142">Ответ содержит коллекцию объектов [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) в составе тела отклика, если были найдены ошибки или предупреждения.</span><span class="sxs-lookup"><span data-stu-id="1c73a-142">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="1c73a-143">Пример</span><span class="sxs-lookup"><span data-stu-id="1c73a-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c73a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c73a-144">Request</span></span>
<span data-ttu-id="1c73a-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c73a-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c73a-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c73a-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```
# <a name="c"></a>[<span data-ttu-id="1c73a-147">C#</span><span class="sxs-lookup"><span data-stu-id="1c73a-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c73a-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c73a-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c73a-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c73a-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c73a-150">Java</span><span class="sxs-lookup"><span data-stu-id="1c73a-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1c73a-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c73a-151">Response</span></span>
<span data-ttu-id="1c73a-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1c73a-152">Here is an example of the response.</span></span> 

><span data-ttu-id="1c73a-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c73a-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2105

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/Collection(microsoft.graph.verificationMessage)",
    "value": [
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have missing data for the field - SIS ID"
        },
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have an invalid format for the field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "125 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "35 row(s) have referenced data not found in source. Field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "10 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "91 row(s) have referenced data not found in source. Field - SIS ID"
        }
    ]
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


