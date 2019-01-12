---
title: Запуск синхронизации после загрузки файлов educationSynchronizationProfile
description: Проверьте файлы, отправленные в конкретных школа профиль синхронизации данных клиента. Если проверка выполнена успешно, в профиле будет запустить синхронизацию. В противном случае ответ будет содержать ошибки и предупреждения. Если ответ содержит ошибки, не запустится синхронизации. Если ответ содержит только предупреждения, будет запущен процесс синхронизации.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: efdc0863a1de58f7ebf46492b662e632972275c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915251"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="4563b-107">Запуск синхронизации после загрузки файлов educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="4563b-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

> <span data-ttu-id="4563b-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4563b-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4563b-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4563b-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4563b-110">Проверьте файлы, загруженные в конкретных школа данных [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="4563b-110">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="4563b-111">Если проверка выполнена успешно, в профиле будет запустить синхронизацию.</span><span class="sxs-lookup"><span data-stu-id="4563b-111">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="4563b-112">В противном случае ответ будет содержать ошибки и предупреждения.</span><span class="sxs-lookup"><span data-stu-id="4563b-112">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="4563b-113">Если ответ содержит ошибки, не запустится синхронизации.</span><span class="sxs-lookup"><span data-stu-id="4563b-113">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="4563b-114">Если ответ содержит только предупреждения, будет запущен процесс синхронизации.</span><span class="sxs-lookup"><span data-stu-id="4563b-114">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="4563b-115">**Примечание:** Этот метод используется только в том случае, если поставщик данных имеет тип [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="4563b-115">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="4563b-116">Кроме того свойство профиля в состоянии необходимо подготовить к работе с прежде чем можно будет начать.</span><span class="sxs-lookup"><span data-stu-id="4563b-116">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="4563b-117">Опрос объект профиля, чтобы проверить значение свойства состояний.</span><span class="sxs-lookup"><span data-stu-id="4563b-117">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="4563b-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4563b-118">Permissions</span></span>
<span data-ttu-id="4563b-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4563b-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4563b-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4563b-121">Permission type</span></span> | <span data-ttu-id="4563b-122">Permissions</span><span class="sxs-lookup"><span data-stu-id="4563b-122">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4563b-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4563b-123">Delegated (work or school account)</span></span> | <span data-ttu-id="4563b-124">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4563b-124">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="4563b-125">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="4563b-125">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="4563b-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4563b-126">Not supported.</span></span>|
|<span data-ttu-id="4563b-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4563b-127">Application</span></span>|<span data-ttu-id="4563b-128">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4563b-128">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4563b-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4563b-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="4563b-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4563b-130">Request headers</span></span>
| <span data-ttu-id="4563b-131">Имя</span><span class="sxs-lookup"><span data-stu-id="4563b-131">Name</span></span>       | <span data-ttu-id="4563b-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4563b-132">Type</span></span> | <span data-ttu-id="4563b-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4563b-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4563b-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="4563b-134">Authorization</span></span>  | <span data-ttu-id="4563b-135">string</span><span class="sxs-lookup"><span data-stu-id="4563b-135">string</span></span>  | <span data-ttu-id="4563b-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4563b-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4563b-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4563b-138">Request body</span></span>
<span data-ttu-id="4563b-139">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4563b-139">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4563b-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="4563b-140">Response</span></span>
<span data-ttu-id="4563b-141">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4563b-141">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="4563b-142">Если неудачно, возвращается `400 Bad Request`.</span><span class="sxs-lookup"><span data-stu-id="4563b-142">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="4563b-143">Ответ содержит коллекцию объектов [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) как часть тела ответа, если найдены ошибки и предупреждения.</span><span class="sxs-lookup"><span data-stu-id="4563b-143">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="4563b-144">Пример</span><span class="sxs-lookup"><span data-stu-id="4563b-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4563b-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="4563b-145">Request</span></span>
<span data-ttu-id="4563b-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4563b-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```

##### <a name="response"></a><span data-ttu-id="4563b-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="4563b-147">Response</span></span>
<span data-ttu-id="4563b-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4563b-148">Here is an example of the response.</span></span> 

><span data-ttu-id="4563b-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4563b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
