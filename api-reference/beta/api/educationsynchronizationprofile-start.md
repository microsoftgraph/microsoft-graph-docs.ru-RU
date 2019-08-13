---
title: Запуск синхронизации после отправки файлов в Едукатионсинчронизатионпрофиле
description: Проверьте, что файлы переданы в определенный профиль синхронизации данных учебного заведения в клиенте. Если проверка прошла успешно, синхронизация начнется в профиле. В противном случае ответ будет содержать ошибки и предупреждения. Если ответ содержит ошибки, синхронизация не начнется. Если ответ содержит только предупреждения, синхронизация начнется.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2247bdfc519bfc07ac0436058b07c3e593ddbb5f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323818"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="de050-107">Запуск синхронизации после отправки файлов в Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="de050-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de050-108">Проверьте, что файлы переданы в определенный [профиль синхронизации](../resources/educationsynchronizationprofile.md) данных учебного заведения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="de050-108">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="de050-109">Если проверка прошла успешно, синхронизация начнется в профиле.</span><span class="sxs-lookup"><span data-stu-id="de050-109">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="de050-110">В противном случае ответ будет содержать ошибки и предупреждения.</span><span class="sxs-lookup"><span data-stu-id="de050-110">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="de050-111">Если ответ содержит ошибки, синхронизация не начнется.</span><span class="sxs-lookup"><span data-stu-id="de050-111">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="de050-112">Если ответ содержит только предупреждения, синхронизация начнется.</span><span class="sxs-lookup"><span data-stu-id="de050-112">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="de050-113">**Примечание:** Используйте этот метод только в том случае, если поставщик данных относится к типу [едукатионксвдатапровидер](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="de050-113">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="de050-114">Кроме того, необходимо подготовить свойство состояния профиля, прежде чем его можно будет запустить.</span><span class="sxs-lookup"><span data-stu-id="de050-114">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="de050-115">Опросить объект Profile, чтобы проверить его свойство State.</span><span class="sxs-lookup"><span data-stu-id="de050-115">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="de050-116">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de050-116">Permissions</span></span>
<span data-ttu-id="de050-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de050-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de050-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de050-119">Permission type</span></span> | <span data-ttu-id="de050-120">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de050-120">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="de050-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de050-121">Delegated (work or school account)</span></span> | <span data-ttu-id="de050-122">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de050-122">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="de050-123">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de050-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="de050-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de050-124">Not supported.</span></span>|
|<span data-ttu-id="de050-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de050-125">Application</span></span>|<span data-ttu-id="de050-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de050-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de050-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de050-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="de050-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de050-128">Request headers</span></span>
| <span data-ttu-id="de050-129">Имя</span><span class="sxs-lookup"><span data-stu-id="de050-129">Name</span></span>       | <span data-ttu-id="de050-130">Тип</span><span class="sxs-lookup"><span data-stu-id="de050-130">Type</span></span> | <span data-ttu-id="de050-131">Описание</span><span class="sxs-lookup"><span data-stu-id="de050-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="de050-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="de050-132">Authorization</span></span>  | <span data-ttu-id="de050-133">string</span><span class="sxs-lookup"><span data-stu-id="de050-133">string</span></span>  | <span data-ttu-id="de050-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de050-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de050-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de050-136">Request body</span></span>
<span data-ttu-id="de050-137">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de050-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="de050-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="de050-138">Response</span></span>
<span data-ttu-id="de050-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="de050-139">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="de050-140">Если операция завершилась неудачно, `400 Bad Request`возвращается значение.</span><span class="sxs-lookup"><span data-stu-id="de050-140">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="de050-141">Ответ содержит коллекцию объектов [едукатионфилесинчронизатионверификатионмессаже](../resources/educationfilesynchronizationverificationmessage.md) в теле отклика, если обнаружены какие-либо ошибки или предупреждения.</span><span class="sxs-lookup"><span data-stu-id="de050-141">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="de050-142">Пример</span><span class="sxs-lookup"><span data-stu-id="de050-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de050-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="de050-143">Request</span></span>
<span data-ttu-id="de050-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de050-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="de050-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="de050-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de050-146">C#</span><span class="sxs-lookup"><span data-stu-id="de050-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de050-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de050-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de050-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="de050-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="de050-149">Java</span><span class="sxs-lookup"><span data-stu-id="de050-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="de050-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="de050-150">Response</span></span>
<span data-ttu-id="de050-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de050-151">Here is an example of the response.</span></span> 

><span data-ttu-id="de050-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de050-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
