---
title: Запуск синхронизации после отправки файлов в Едукатионсинчронизатионпрофиле
description: Проверьте, что файлы переданы в определенный профиль синхронизации данных учебного заведения в клиенте. Если проверка прошла успешно, синхронизация начнется в профиле. В противном случае ответ будет содержать ошибки и предупреждения. Если ответ содержит ошибки, синхронизация не начнется. Если ответ содержит только предупреждения, синхронизация начнется.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: e677090f925d336b47ab80e8e770ca1e2895b84b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259519"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="4c78b-107">Запуск синхронизации после отправки файлов в Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="4c78b-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c78b-108">Проверьте, что файлы переданы в определенный [профиль синхронизации](../resources/educationsynchronizationprofile.md) данных учебного заведения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="4c78b-108">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="4c78b-109">Если проверка прошла успешно, синхронизация начнется в профиле.</span><span class="sxs-lookup"><span data-stu-id="4c78b-109">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="4c78b-110">В противном случае ответ будет содержать ошибки и предупреждения.</span><span class="sxs-lookup"><span data-stu-id="4c78b-110">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="4c78b-111">Если ответ содержит ошибки, синхронизация не начнется.</span><span class="sxs-lookup"><span data-stu-id="4c78b-111">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="4c78b-112">Если ответ содержит только предупреждения, синхронизация начнется.</span><span class="sxs-lookup"><span data-stu-id="4c78b-112">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="4c78b-113">**Примечание:** Используйте этот метод только в том случае, если поставщик данных относится к типу [едукатионксвдатапровидер](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="4c78b-113">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="4c78b-114">Кроме того, необходимо подготовить свойство состояния профиля, прежде чем его можно будет запустить.</span><span class="sxs-lookup"><span data-stu-id="4c78b-114">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="4c78b-115">Опросить объект Profile, чтобы проверить его свойство State.</span><span class="sxs-lookup"><span data-stu-id="4c78b-115">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c78b-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c78b-116">Permissions</span></span>
<span data-ttu-id="4c78b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c78b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4c78b-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c78b-119">Permission type</span></span> | <span data-ttu-id="4c78b-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c78b-120">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4c78b-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c78b-121">Delegated (work or school account)</span></span> | <span data-ttu-id="4c78b-122">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c78b-122">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="4c78b-123">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c78b-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4c78b-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c78b-124">Not supported.</span></span>|
|<span data-ttu-id="4c78b-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c78b-125">Application</span></span>|<span data-ttu-id="4c78b-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c78b-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c78b-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c78b-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="4c78b-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c78b-128">Request headers</span></span>
| <span data-ttu-id="4c78b-129">Имя</span><span class="sxs-lookup"><span data-stu-id="4c78b-129">Name</span></span>       | <span data-ttu-id="4c78b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4c78b-130">Type</span></span> | <span data-ttu-id="4c78b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4c78b-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4c78b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c78b-132">Authorization</span></span>  | <span data-ttu-id="4c78b-133">string</span><span class="sxs-lookup"><span data-stu-id="4c78b-133">string</span></span>  | <span data-ttu-id="4c78b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c78b-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c78b-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c78b-136">Request body</span></span>
<span data-ttu-id="4c78b-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c78b-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4c78b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c78b-138">Response</span></span>
<span data-ttu-id="4c78b-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4c78b-139">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="4c78b-140">Если операция завершилась неудачно, `400 Bad Request`возвращается значение.</span><span class="sxs-lookup"><span data-stu-id="4c78b-140">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="4c78b-141">Ответ содержит коллекцию объектов [едукатионфилесинчронизатионверификатионмессаже](../resources/educationfilesynchronizationverificationmessage.md) в теле отклика, если обнаружены какие-либо ошибки или предупреждения.</span><span class="sxs-lookup"><span data-stu-id="4c78b-141">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="4c78b-142">Пример</span><span class="sxs-lookup"><span data-stu-id="4c78b-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c78b-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c78b-143">Request</span></span>
<span data-ttu-id="4c78b-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c78b-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```

##### <a name="response"></a><span data-ttu-id="4c78b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c78b-145">Response</span></span>
<span data-ttu-id="4c78b-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c78b-146">Here is an example of the response.</span></span> 

><span data-ttu-id="4c78b-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c78b-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="4c78b-149">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="4c78b-149">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c78b-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c78b-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_start-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="4c78b-151">C#</span><span class="sxs-lookup"><span data-stu-id="4c78b-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_start-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4c78b-152">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4c78b-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/post_educationSynchronizationProfile_start-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-start.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-start.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-start.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
