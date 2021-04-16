---
title: Get onlineMeeting
description: Извлечение свойств и связей объекта собраний в Интернете.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 02466f23b1ffbb7e91cfffba6c5bf5748cdc1892
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51870018"
---
# <a name="get-onlinemeeting"></a><span data-ttu-id="4238e-103">Get onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="4238e-103">Get onlineMeeting</span></span>

<span data-ttu-id="4238e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4238e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4238e-105">Извлечение свойств и связей [объекта onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="4238e-105">Retrieve the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span> <span data-ttu-id="4238e-106">Сведения о onlineMeeting можно получить с помощью [VideoTeleconferenceId](#example-1-retrieve-an-online-meeting-by-videoteleconferenceid) или [ID собрания.](#example-2-retrieve-an-online-meeting-by-meeting-id)</span><span class="sxs-lookup"><span data-stu-id="4238e-106">You can get details of an onlineMeeting using [VideoTeleconferenceId](#example-1-retrieve-an-online-meeting-by-videoteleconferenceid) or [meeting ID](#example-2-retrieve-an-online-meeting-by-meeting-id).</span></span>


## <a name="permissions"></a><span data-ttu-id="4238e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4238e-107">Permissions</span></span>

<span data-ttu-id="4238e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4238e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4238e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4238e-110">Permission type</span></span>                        | <span data-ttu-id="4238e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4238e-111">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="4238e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4238e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4238e-113">OnlineMeetings.Read, OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4238e-113">OnlineMeetings.Read, OnlineMeetings.ReadWrite</span></span>         |
| <span data-ttu-id="4238e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4238e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4238e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4238e-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="4238e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4238e-116">Application</span></span>                            | <span data-ttu-id="4238e-117">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="4238e-117">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All\*</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="4238e-118">\*Администраторы должны [](/graph/cloud-communication-online-meeting-application-access-policy) создать политику доступа к приложениям и предоставить ее пользователю, уполномочив приложение, настроенного в политике, получить онлайн-собрание от имени этого пользователя (пользовательский ID, указанный в пути запроса).</span><span class="sxs-lookup"><span data-stu-id="4238e-118">\* Administrators must create an [application access policy](/graph/cloud-communication-online-meeting-application-access-policy) and grant it to a user, authorizing the app configured in the policy to retrieve an online meeting on behalf of that user (user ID specified in the request path).</span></span>

## <a name="http-request"></a><span data-ttu-id="4238e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4238e-119">HTTP request</span></span>
<span data-ttu-id="4238e-120">Чтобы получить указанный onlineMeeting с помощью ID собрания с делегированным маркером:</span><span class="sxs-lookup"><span data-stu-id="4238e-120">To get the specified onlineMeeting using meeting ID with delegated token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onlineMeetings/{meetingId}
```

<span data-ttu-id="4238e-121">Чтобы получить указанный onlineMeeting с помощью ИД собрания с маркером приложения:</span><span class="sxs-lookup"><span data-stu-id="4238e-121">To get the specified onlineMeeting using meeting ID with application token:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{userId}/onlineMeetings/{meetingId}
```

<span data-ttu-id="4238e-122">Чтобы получить указанный onlineMeeting с помощью \*\*videoTeleconferenceId\*\*\*:</span><span class="sxs-lookup"><span data-stu-id="4238e-122">To get the specified onlineMeeting using \*\*videoTeleconferenceId\*\*\*:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{videoTeleconferenceId}'
```

> [!NOTE]
> - <span data-ttu-id="4238e-123">`userId`— это объектный ID пользователя на портале [управления пользователями Azure.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)</span><span class="sxs-lookup"><span data-stu-id="4238e-123">`userId` is the object ID of a user in [Azure user management portal](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade).</span></span> <span data-ttu-id="4238e-124">Дополнительные сведения см. в [политике доступа к приложениям.](/graph/cloud-communication-online-meeting-application-access-policy)</span><span class="sxs-lookup"><span data-stu-id="4238e-124">For more details, see [application access policy](/graph/cloud-communication-online-meeting-application-access-policy).</span></span>
> - <span data-ttu-id="4238e-125">`meetingId`является **id** объекта [onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="4238e-125">`meetingId` is the **id** of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>
> - <span data-ttu-id="4238e-126">**VideoTeleconferenceId** создается для лицензированных пользователей Cloud-Video-Interop и может быть найден в [объекте onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="4238e-126">**videoTeleconferenceId** is generated for Cloud-Video-Interop licensed users and can be found in an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span> <span data-ttu-id="4238e-127">Дополнительные сведения можно получить в ID конференции [VTC.](/microsoftteams/cloud-video-interop-for-teams-set-up)</span><span class="sxs-lookup"><span data-stu-id="4238e-127">Refer to [VTC conference id](/microsoftteams/cloud-video-interop-for-teams-set-up) for more details.</span></span>
> - <span data-ttu-id="4238e-128">\* Этот сценарий поддерживает только маркер приложений и не поддерживает политику доступа к приложениям.</span><span class="sxs-lookup"><span data-stu-id="4238e-128">\* This scenario only supports application token and does not support application access policy.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="4238e-129">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4238e-129">Optional query parameters</span></span>
<span data-ttu-id="4238e-130">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4238e-130">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4238e-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4238e-131">Request headers</span></span>
| <span data-ttu-id="4238e-132">Имя</span><span class="sxs-lookup"><span data-stu-id="4238e-132">Name</span></span>          | <span data-ttu-id="4238e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4238e-133">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4238e-134">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4238e-134">Authorization</span></span> | <span data-ttu-id="4238e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4238e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4238e-137">Принять-Язык</span><span class="sxs-lookup"><span data-stu-id="4238e-137">Accept-Language</span></span>  | <span data-ttu-id="4238e-138">Язык.</span><span class="sxs-lookup"><span data-stu-id="4238e-138">Language.</span></span> <span data-ttu-id="4238e-139">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4238e-139">Optional.</span></span> |

<span data-ttu-id="4238e-140">Если запрос содержит `Accept-Language` HTTP-заголовок, то `content` из `joinInformation` будет указан на языке и языкового стандарта, указанного в заголовке `Accept-Language`.</span><span class="sxs-lookup"><span data-stu-id="4238e-140">If the request contains an `Accept-Language` HTTP header, the `content` of `joinInformation` will be in the language and locale variant specified in the `Accept-Language` header.</span></span> <span data-ttu-id="4238e-141">Контент по умолчанию будет на английском языке.</span><span class="sxs-lookup"><span data-stu-id="4238e-141">The default content will be in English.</span></span>

## <a name="request-body"></a><span data-ttu-id="4238e-142">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4238e-142">Request body</span></span>
<span data-ttu-id="4238e-143">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4238e-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4238e-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="4238e-144">Response</span></span>
<span data-ttu-id="4238e-145">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [onlineMeeting](../resources/onlinemeeting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4238e-145">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4238e-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="4238e-146">Examples</span></span>

### <a name="example-1-retrieve-an-online-meeting-by-videoteleconferenceid"></a><span data-ttu-id="4238e-147">Пример 1. Извлечение собрания в Интернете с помощью VideoTeleconferenceId</span><span class="sxs-lookup"><span data-stu-id="4238e-147">Example 1: Retrieve an online meeting by VideoTeleconferenceId</span></span>

#### <a name="request"></a><span data-ttu-id="4238e-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="4238e-148">Request</span></span>
<span data-ttu-id="4238e-149">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4238e-149">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4238e-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="4238e-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["123456789"],
  "name": "get-onlineMeeting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="c"></a>[<span data-ttu-id="4238e-151">C#</span><span class="sxs-lookup"><span data-stu-id="4238e-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4238e-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4238e-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4238e-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4238e-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4238e-154">Java</span><span class="sxs-lookup"><span data-stu-id="4238e-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

><span data-ttu-id="4238e-155">**Примечание.** если указан японский язык, в ответ будут включены перечисленные ниже данные.</span><span class="sxs-lookup"><span data-stu-id="4238e-155">**Note:** If 'Accept-Language: ja' is specified to indicate Japanese, for example, the response will include the following.</span></span>
```json
    "joinInformation": {
        "content": "data%3Atext%2Fhtml%2C%0A++%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A%09+%3C%2Fdiv%3E%0A++++%3Cdiv+class%3D%22me-email-text%22+style%3D%22color%3A%23252424%3Bfont-family%3A'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3B%22%3E%0A+++%3Cdiv+style%3D%22margin-top%3A+24px%3B+margin-bottom%3A+10px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-headline%22%0A++++++++++++++style%3D%22font-size%3A+18px%3Bfont-family%3A'Segoe+UI+Semibold'%2C'Segoe+UI'%2C'Helvetica+Neue'%2CHelvetica%2CArial%2Csans-serif%3Btext-decoration%3A+underline%3Bcolor%3A+%236264a7%3B%22%0A++++++++++++++href%3D%22https%3A%2F%2Fteams.microsoft.com%2Fl%2Fmeetup-join%2F19%253ameeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%2540thread.v2%2F0%3Fcontext%3D%257b%2522Tid%2522%253a%252279a788bf-86f1-41af-91ab-000000000000%2522%252c%2522Oid%2522%253a%2522d4a060b5-a8fc-450c-837b-000000000000%2522%257d%22%0A++++++++++++++target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3EMicrosoft+Teams+%E4%BC%9A%E8%AD%B0%E3%81%AB%E5%8F%82%E5%8A%A0%3C%2Fa%3E%0A++++++%3C%2Fdiv%3E%0A%09+%3Cdiv%3E%0A++++%0A++++++%3Cdiv%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+14px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22%0A++++++++++href%3D%22tel%3A%2B16477490000%2C%2C11160000%26%2335%3B+%22+target%3D%22_blank%22+rel%3D%22noreferrer+noopener%22%3E%2B16477490000%3C%2Fa%3E%0A++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%26nbsp%3B++(%E6%9C%89%E6%96%99)+%3C%2Fspan%3E%0A++++++%3C%2Fdiv%3E%0A++++%0A++%3C%2Fdiv%3E%0A%0A%09+%0A++++++%3Cdiv+style%3D%22margin-top%3A+10px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Cspan+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++++++%E4%BC%9A%E8%AD%B0+ID%3A%0A++++++++%3C%2Fspan%3E%0A++++++%3Cspan+style%3D%22font-size%3A+14px%3B%22%3E%0A++++++++111+000+00%23%0A++++++%3C%2Fspan%3E%0A++++%3C%2Fdiv%3E%0A++++%0A%09+%0A++++++++%3Cdiv+style%3D%22margin-bottom%3A+24px%3B%22%3E%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fdialin.teams.microsoft.com%2F8bf6e654-57eb-4b85-aeaf-36c84429b2fe%3Fid%3D11160000%22+rel%3D%22noreferrer+noopener%22%3E%E6%9C%80%E5%AF%84%E3%82%8A%E3%81%AE%E5%9B%BD%E3%81%AE%E9%9B%BB%E8%A9%B1%E7%95%AA%E5%8F%B7%E3%82%92%E6%A4%9C%E7%B4%A2%3C%2Fa%3E%0A+++++++++%7C%0A++++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fmysettings.lync.com%2Fpstnconferencing%22+rel%3D%22noreferrer+noopener%22%3E%0A++++++++PIN+%E3%82%92%E3%83%AA%E3%82%BB%E3%83%83%E3%83%88%3C%2Fa%3E%0A+++++++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Faka.ms%2FJoinTeamsMeeting%22+rel%3D%22noreferrer+noopener%22%3ETeams+%E3%81%AE%E8%A9%B3%E7%B4%B0%E3%82%92%E8%A1%A8%E7%A4%BA%3C%2Fa%3E%0A+++++%7C+%3Ca+class%3D%22me-email-link%22+style%3D%22font-size%3A+12px%3Btext-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+target%3D%22_blank%22+href%3D%22https%3A%2F%2Fteams.microsoft.com%2FmeetingOptions%2F%3ForganizerId%3Dd4a060b5-a8fc-450c-837b-000000000000%26tenantId%3D79a788bf-86f1-41af-91ab-000000000000%26threadId%3D19_meeting_NDRiZjRiMmUtODI5OC00MzRlLTk1ZWEtMGY1000000000000%40thread.v2%26messageId%3D0%26language%3Dja%22+rel%3D%22noreferrer+noopener%22%3E%E4%BC%9A%E8%AD%B0%E3%81%AE%E3%82%AA%E3%83%97%E3%82%B7%E3%83%A7%E3%83%B3%3C%2Fa%3E%0A++++%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%E3%83%93%E3%83%87%E3%82%AA%E4%BC%9A%E8%AD%B0%E3%83%87%E3%83%90%E3%82%A4%E3%82%B9%E3%81%A7%E5%8F%82%E5%8A%A0%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A12px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22%22%3E000000000%40t.abcd.vc%3C%2Fa%3E+VTC+%E4%BC%9A%E8%AD%B0+ID%3A+0180300000%0A++++++++%3C%2Fdiv%3E%0A%0A++++++++%3Cdiv+style%3D%22font-size%3A+12px%3B+margin-bottom%3A+20px%3B%22%3E%0A++++++++%3Ca+class%3D%22me-email-link%22+style%3D%22text-decoration%3A+none%3Bcolor%3A+%236264a7%3B%22+href%3D%22https%3A%2F%2Fdialin.abcd.vc%2Fteams%2F%3Fkey%3D000000000%26conf%3D0180308922%22%3E%E4%BB%A3%E6%9B%BF+VTC+%E3%81%AE%E3%83%80%E3%82%A4%E3%83%A4%E3%83%AB%E6%96%B9%E6%B3%95%3C%2Fa%3E%0A++++++++%3C%2Fdiv%3E%0A++++%0A+++++%0A++++++%3Cdiv+style%3D%22font-size%3A+14px%3B+margin-bottom%3A+4px%3B%22%3E%0A++++++++%0A++++++%3C%2Fdiv%3E%0A++++++%3Cdiv+style%3D%22font-size%3A+12px%3B%22%3E%0A++++++%0A++++++%3C%2Fdiv%3E%0A++++%0A+++++%3C%2Fdiv%3E%0A%09+%3Cdiv+style%3D%22width%3A100%25%3Bheight%3A+20px%3B%22%3E%0A%09%09%3Cspan+style%3D%22white-space%3Anowrap%3Bcolor%3Agray%3Bopacity%3A.36%3B%22%3E________________________________________________________________________________%3C%2Fspan%3E%0A++%3C%2Fdiv%3E%22%2C%0A",
        "contentType": "Html"
    }  
```

#### <a name="response"></a><span data-ttu-id="4238e-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4238e-156">Response</span></span>

> <span data-ttu-id="4238e-p108">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4238e-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "55525634478",
    "tollFreeNumber": "55566390588",
    "ConferenceId": "9999999",
    "dialinUrl": "https://dialin.teams.microsoft.com/6787A136-B9B8-4D39-846C-C0F1FF937F10?id=xxxxxxx"
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "creationDateTime": "2018-05-30T00:12:19.0726086Z",
  "endDateTime": "2018-05-30T01:00:00Z",
  "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8_19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3a:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context=%7b%22Tid%22%3a%aa67bd4c-8475-432d-bd41-39f255720e0a%22%2c%22Oid%22%3a%22112f7296-5fa4-42ca-bae8-6a692b15d4b8%22%7d",
  "participants": {
  "@odata.type": "#microsoft.graph.meetingParticipants",
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.identitySet",
        "identity": {
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8",
            "displayName": "Tyler Stein"
          }
        },
        "upn": "upn-value"
      }
    ],
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
          "displayName": "Jasmine Miller"
        }
      },
      "upn": "upn-value"
    }
  },
  "startDateTime": "2018-05-30T00:30:00Z",
  "subject": "Test Meeting.",
  "videoTeleconferenceId": "123456789",
  "lobbyBypassSettings": {
    "scope": "everyone",
    "isDialInBypassEnabled": true
  },
  "isEntryExitAnnounced": true,
  "allowedPresenters": "everyone"
}
```

### <a name="example-2-retrieve-an-online-meeting-by-meeting-id"></a><span data-ttu-id="4238e-159">Пример 2. Извлечение собрания в Интернете с помощью ИД собрания</span><span class="sxs-lookup"><span data-stu-id="4238e-159">Example 2: Retrieve an online meeting by meeting ID</span></span>
<span data-ttu-id="4238e-160">Сведения о собраниях можно получить с помощью ИД собрания с помощью маркера пользователя или приложения.</span><span class="sxs-lookup"><span data-stu-id="4238e-160">You can retrieve meeting information via meeting ID with either a user or application token.</span></span> <span data-ttu-id="4238e-161">ID собрания предоставляется в объекте ответа при создании [onlineMeeting.](../resources/onlinemeeting.md)</span><span class="sxs-lookup"><span data-stu-id="4238e-161">The meeting ID is provided in the response object when creating an [onlineMeeting](../resources/onlinemeeting.md).</span></span> <span data-ttu-id="4238e-162">Этот параметр доступен для поддержки случаев использования, в которых известен ID собрания, например, когда приложение сначала создает онлайн-собрание с помощью API Graph, а затем извлекает сведения о собраниях позже в качестве отдельного действия.</span><span class="sxs-lookup"><span data-stu-id="4238e-162">This option is available to support use cases where the meeting ID is known, such as when an application first creates the online meeting using Graph API first then retrieves meeting information later as a separate action.</span></span>

#### <a name="request"></a><span data-ttu-id="4238e-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="4238e-163">Request</span></span>

> <span data-ttu-id="4238e-164">**Примечание:** ID собрания был усечен для чтения.</span><span class="sxs-lookup"><span data-stu-id="4238e-164">**Note:** The meeting ID has been truncated for readability.</span></span>

<span data-ttu-id="4238e-165">В следующем запросе используется маркер пользователя.</span><span class="sxs-lookup"><span data-stu-id="4238e-165">The following request uses a user token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy
```

<span data-ttu-id="4238e-166">В следующем запросе используется маркер приложения.</span><span class="sxs-lookup"><span data-stu-id="4238e-166">The following request uses an app token.</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/users/dc17674c-81d9-4adb-bfb2-8f6a442e4622/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy
```

#### <a name="response"></a><span data-ttu-id="4238e-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="4238e-167">Response</span></span>

> <span data-ttu-id="4238e-168">**Примечание.** Объект отклика, показанный здесь, сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4238e-168">**Note:** The response object shown here has been shortened for readability.</span></span> <span data-ttu-id="4238e-169">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4238e-169">All the properties will be returned from an actual call.</span></span>

```json
{
    "id": "MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZiMi04ZdFpHRTNaR1F6WGhyZWFkLnYy",
    "creationDateTime": "2020-09-29T22:35:33.1594516Z",
    "startDateTime": "2020-09-29T22:35:31.389759Z",
    "endDateTime": "2020-09-29T23:35:31.389759Z",
    "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_MGQ4MDQyNTEtNTQ2NS00YjQxLTlkM2EtZWVkODYxODYzMmY2%40thread.v2/0?context=%7b%22Tid%22%3a%22909c6581-5130-43e9-88f3-fcb3582cde37%22%2c%22Oid%22%3a%22dc17674c-81d9-4adb-bfb2-8f6a442e4622%22%7d",
    "subject": null,
    "autoAdmittedUsers": "EveryoneInCompany",
    "isEntryExitAnnounced": true,
    "allowedPresenters": "everyone",
    "videoTeleconferenceId": "(redacted)",
    "participants": {
        "organizer": {
            "upn": "(redacted)",
            "role": "presenter",
            "identity": {
                "user": {
                    "id": "dc17674c-81d9-4adb-bfb2-8f6a442e4622",
                    "displayName": null,
                    "tenantId": "909c6581-5130-43e9-88f3-fcb3582cde38",
                    "identityProvider": "AAD"
                }
            }
        },
        "attendees": [],
        "producers": [],
        "contributors": []
    },
    "lobbyBypassSettings": {
        "scope": "organization",
        "isDialInBypassEnabled": false
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
