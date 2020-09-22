---
title: Запуск синхронизации после отправки файлов в Едукатионсинчронизатионпрофиле
description: Проверьте, что файлы переданы в определенный профиль синхронизации данных учебного заведения в клиенте. Если проверка прошла успешно, синхронизация начнется в профиле. В противном случае ответ будет содержать ошибки и предупреждения. Если ответ содержит ошибки, синхронизация не начнется. Если ответ содержит только предупреждения, синхронизация начнется.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2671920a997e1cf561e2be77a13f168efe6842e4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007116"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="2a15e-107">Запуск синхронизации после отправки файлов в Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="2a15e-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

<span data-ttu-id="2a15e-108">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a15e-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a15e-109">Проверьте, что файлы переданы в определенный [профиль синхронизации](../resources/educationsynchronizationprofile.md) данных учебного заведения в клиенте.</span><span class="sxs-lookup"><span data-stu-id="2a15e-109">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="2a15e-110">Если проверка прошла успешно, синхронизация начнется в профиле.</span><span class="sxs-lookup"><span data-stu-id="2a15e-110">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="2a15e-111">В противном случае ответ будет содержать ошибки и предупреждения.</span><span class="sxs-lookup"><span data-stu-id="2a15e-111">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="2a15e-112">Если ответ содержит ошибки, синхронизация не начнется.</span><span class="sxs-lookup"><span data-stu-id="2a15e-112">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="2a15e-113">Если ответ содержит только предупреждения, синхронизация начнется.</span><span class="sxs-lookup"><span data-stu-id="2a15e-113">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="2a15e-114">**Примечание:** Используйте этот метод только в том случае, если поставщик данных относится к типу [едукатионксвдатапровидер](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="2a15e-114">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="2a15e-115">Кроме того, необходимо подготовить свойство состояния профиля, прежде чем его можно будет запустить.</span><span class="sxs-lookup"><span data-stu-id="2a15e-115">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="2a15e-116">Опросить объект Profile, чтобы проверить его свойство State.</span><span class="sxs-lookup"><span data-stu-id="2a15e-116">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a15e-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a15e-117">Permissions</span></span>
<span data-ttu-id="2a15e-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a15e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a15e-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a15e-120">Permission type</span></span> | <span data-ttu-id="2a15e-121">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a15e-121">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="2a15e-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a15e-122">Delegated (work or school account)</span></span> | <span data-ttu-id="2a15e-123">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a15e-123">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="2a15e-124">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a15e-124">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2a15e-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a15e-125">Not supported.</span></span>|
|<span data-ttu-id="2a15e-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a15e-126">Application</span></span>|<span data-ttu-id="2a15e-127">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a15e-127">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a15e-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a15e-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="2a15e-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a15e-129">Request headers</span></span>
| <span data-ttu-id="2a15e-130">Имя</span><span class="sxs-lookup"><span data-stu-id="2a15e-130">Name</span></span>       | <span data-ttu-id="2a15e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2a15e-131">Type</span></span> | <span data-ttu-id="2a15e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2a15e-132">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2a15e-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a15e-133">Authorization</span></span>  | <span data-ttu-id="2a15e-134">string</span><span class="sxs-lookup"><span data-stu-id="2a15e-134">string</span></span>  | <span data-ttu-id="2a15e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a15e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a15e-137">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2a15e-137">Request body</span></span>
<span data-ttu-id="2a15e-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a15e-138">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2a15e-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a15e-139">Response</span></span>
<span data-ttu-id="2a15e-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="2a15e-140">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="2a15e-141">Если операция завершилась неудачно, возвращается значение `400 Bad Request` .</span><span class="sxs-lookup"><span data-stu-id="2a15e-141">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="2a15e-142">Ответ содержит коллекцию объектов [едукатионфилесинчронизатионверификатионмессаже](../resources/educationfilesynchronizationverificationmessage.md) в теле отклика, если обнаружены какие-либо ошибки или предупреждения.</span><span class="sxs-lookup"><span data-stu-id="2a15e-142">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="2a15e-143">Пример</span><span class="sxs-lookup"><span data-stu-id="2a15e-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2a15e-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a15e-144">Request</span></span>
<span data-ttu-id="2a15e-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a15e-145">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a15e-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a15e-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```
# <a name="c"></a>[<span data-ttu-id="2a15e-147">C#</span><span class="sxs-lookup"><span data-stu-id="2a15e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a15e-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a15e-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a15e-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a15e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2a15e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a15e-150">Response</span></span>
<span data-ttu-id="2a15e-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2a15e-151">Here is an example of the response.</span></span> 

><span data-ttu-id="2a15e-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a15e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


