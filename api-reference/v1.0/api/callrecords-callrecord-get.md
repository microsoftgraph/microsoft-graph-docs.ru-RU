---
title: Получение callRecord
description: Извлечение свойств и связей объекта callrecord.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: dc4a309e68f0fd05d99298194a30637014de5f70
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035864"
---
# <a name="get-callrecord"></a><span data-ttu-id="38567-103">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="38567-103">Get callRecord</span></span>

<span data-ttu-id="38567-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="38567-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="38567-105">Извлечение свойств и связей [объекта callRecord.](../resources/callrecords-callrecord.md)</span><span class="sxs-lookup"><span data-stu-id="38567-105">Retrieve the properties and relationships of a [callRecord](../resources/callrecords-callrecord.md) object.</span></span>

<span data-ttu-id="38567-106">Существует два способа получения **id** **callRecord:**</span><span class="sxs-lookup"><span data-stu-id="38567-106">There are two ways to get the **id** of a **callRecord**:</span></span>

* <span data-ttu-id="38567-107">[Подпишитесь на изменение уведомлений](/graph/api/resources/webhooks?view=graph-rest-1.0) в `/communications/callRecords` конечную точку.</span><span class="sxs-lookup"><span data-stu-id="38567-107">Subscribe to [change notifications](/graph/api/resources/webhooks?view=graph-rest-1.0) to the `/communications/callRecords` endpoint.</span></span>
* <span data-ttu-id="38567-108">Используйте **свойство callChainId** [вызова.](../resources/call.md)</span><span class="sxs-lookup"><span data-stu-id="38567-108">Use the **callChainId** property of a [call](../resources/call.md).</span></span> <span data-ttu-id="38567-109">Запись вызова доступна только после завершения связанного вызова.</span><span class="sxs-lookup"><span data-stu-id="38567-109">The call record is available only after the associated call is completed.</span></span>

## <a name="permissions"></a><span data-ttu-id="38567-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38567-110">Permissions</span></span>

<span data-ttu-id="38567-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38567-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38567-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38567-113">Permission type</span></span>                        | <span data-ttu-id="38567-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="38567-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="38567-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38567-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="38567-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38567-116">Not supported.</span></span> |
| <span data-ttu-id="38567-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38567-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38567-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38567-118">Not supported.</span></span> |
| <span data-ttu-id="38567-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38567-119">Application</span></span>                            | <span data-ttu-id="38567-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="38567-120">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="38567-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38567-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/callRecords/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="38567-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="38567-122">Optional query parameters</span></span>

<span data-ttu-id="38567-123">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="38567-123">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="38567-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="38567-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="38567-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38567-125">Request headers</span></span>

| <span data-ttu-id="38567-126">Имя</span><span class="sxs-lookup"><span data-stu-id="38567-126">Name</span></span>      |<span data-ttu-id="38567-127">Описание</span><span class="sxs-lookup"><span data-stu-id="38567-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="38567-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38567-128">Authorization</span></span> | <span data-ttu-id="38567-129">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="38567-129">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="38567-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38567-130">Request body</span></span>

<span data-ttu-id="38567-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38567-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38567-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="38567-132">Response</span></span>

<span data-ttu-id="38567-133">В случае успешного решения этот метод возвращает код ответа и запрашиваемого `200 OK` [объекта microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="38567-133">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38567-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="38567-134">Examples</span></span>

### <a name="example-1-get-basic-details"></a><span data-ttu-id="38567-135">Пример 1. Получить основные сведения</span><span class="sxs-lookup"><span data-stu-id="38567-135">Example 1: Get basic details</span></span>

#### <a name="request"></a><span data-ttu-id="38567-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="38567-136">Request</span></span>

<span data-ttu-id="38567-137">Ниже приводится пример запроса на получения основных сведений из [callRecord.](../resources/callrecords-callrecord.md)</span><span class="sxs-lookup"><span data-stu-id="38567-137">The following is an example of the request to get the basic details from a [callRecord](../resources/callrecords-callrecord.md).</span></span>


# <a name="http"></a>[<span data-ttu-id="38567-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="38567-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callrecord"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/callRecords/{id}
```
# <a name="c"></a>[<span data-ttu-id="38567-139">C#</span><span class="sxs-lookup"><span data-stu-id="38567-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-callrecord-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38567-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38567-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-callrecord-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38567-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38567-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-callrecord-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38567-142">Java</span><span class="sxs-lookup"><span data-stu-id="38567-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-callrecord-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="38567-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="38567-143">Response</span></span>

<span data-ttu-id="38567-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="38567-144">The following is an example of the response.</span></span>

> <span data-ttu-id="38567-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="38567-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.callRecord"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords/$entity",
    "version": 1,
    "type": "peerToPeer",
    "modalities": [
        "audio"
    ],
    "lastModifiedDateTime": "2020-02-25T19:00:24.582757Z",
    "startDateTime": "2020-02-25T18:52:21.2169889Z",
    "endDateTime": "2020-02-25T18:52:46.7640013Z",
    "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
    "organizer": {
        "user": {
            "id": "821809f5-0000-0000-0000-3b5136c0e777",
            "displayName": "Abbie Wilkins",
            "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
        }
    },
    "participants": [
        {
            "user": {
                "id": "821809f5-0000-0000-0000-3b5136c0e777",
                "displayName": "Abbie Wilkins",
                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
            }
        },
        {
            "user": {
                "id": "f69e2c00-0000-0000-0000-185e5f5f5d8a",
                "displayName": "Owen Franklin",
                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
            }
        }
    ]
}
```

### <a name="example-2-get-full-details"></a><span data-ttu-id="38567-146">Пример 2. Получить полные сведения</span><span class="sxs-lookup"><span data-stu-id="38567-146">Example 2: Get full details</span></span>

#### <a name="request"></a><span data-ttu-id="38567-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="38567-147">Request</span></span>

<span data-ttu-id="38567-148">Ниже приводится пример запроса на получения полных сведений из [callRecord,](../resources/callrecords-callrecord.md)включая компоненты сеанса и сегмента.</span><span class="sxs-lookup"><span data-stu-id="38567-148">The following is an example of the request to get the full details from a [callRecord](../resources/callrecords-callrecord.md), including session and segment components.</span></span>


# <a name="http"></a>[<span data-ttu-id="38567-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="38567-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_callrecord_expanded"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/callRecords/{id}?$expand=sessions($expand=segments)
```
# <a name="c"></a>[<span data-ttu-id="38567-150">C#</span><span class="sxs-lookup"><span data-stu-id="38567-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-callrecord-expanded-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38567-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38567-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-callrecord-expanded-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38567-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38567-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-callrecord-expanded-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="38567-153">Java</span><span class="sxs-lookup"><span data-stu-id="38567-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-callrecord-expanded-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="38567-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="38567-154">Response</span></span>

<span data-ttu-id="38567-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="38567-155">The following is an example of the response.</span></span> <span data-ttu-id="38567-156">Если список сеансов усечен, для получения следующей страницы сеансов будет предоставлено `sessions@odata.nextLink` значение.</span><span class="sxs-lookup"><span data-stu-id="38567-156">If the sessions list is truncated, a `sessions@odata.nextLink` value will be provided to retrieve the next page of sessions.</span></span>

> <span data-ttu-id="38567-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="38567-157">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.callRecord"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords(sessions(segments()))/$entity",
    "version": 1,
    "type": "peerToPeer",
    "modalities": [
        "audio"
    ],
    "lastModifiedDateTime": "2020-02-25T19:00:24.582757Z",
    "startDateTime": "2020-02-25T18:52:21.2169889Z",
    "endDateTime": "2020-02-25T18:52:46.7640013Z",
    "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
    "organizer": {
        "user": {
            "id": "821809f5-0000-0000-0000-3b5136c0e777",
            "displayName": "Abbie Wilkins",
            "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
        }
    },
    "participants": [
        {
            "user": {
                "id": "821809f5-0000-0000-0000-3b5136c0e777",
                "displayName": "Abbie Wilkins",
                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
            }
        },
        {
            "user": {
                "id": "f69e2c00-0000-0000-0000-185e5f5f5d8a",
                "displayName": "Owen Franklin",
                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
            }
        }
    ],
    "sessions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions(segments())",
    "sessions": [
        {
            "modalities": [
                "audio"
            ],
            "startDateTime": "2020-02-25T18:52:21.2169889Z",
            "endDateTime": "2020-02-25T18:52:46.7640013Z",
            "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
            "caller": {
                "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
                "userAgent": {
                    "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
                    "headerValue": "RTCC/7.0.0.0 UCWA/7.0.0.0 AndroidLync/6.25.0.27 (SM-G930U Android 8.0.0)",
                    "platform": "android",
                    "productFamily": "skypeForBusiness"
                },
                "identity": {
                    "@odata.type": "#microsoft.graph.identitySet",
                    "user": {
                        "id": "821809f5-0000-0000-0000-3b5136c0e777",
                        "displayName": "Abbie Wilkins",
                        "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
                    }
                }
            },
            "callee": {
                "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
                "userAgent": {
                    "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
                    "headerValue": "UCCAPI/16.0.12527.20122 OC/16.0.12527.20194 (Skype for Business)",
                    "platform": "windows",
                    "productFamily": "skypeForBusiness"
                },
                "identity": {
                    "user": {
                        "id": "f69e2c00-0000-0000-0000-185e5f5f5d8a",
                        "displayName": "Owen Franklin",
                        "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
                    }
                },
                "feedback": {
                    "rating": "poor",
                    "tokens": {
                        "NoSound": false,
                        "OtherNoSound": false,
                        "Echo": false,
                        "Noisy": true,
                        "LowVolume": false,
                        "Stopped": false,
                        "DistortedSound": false,
                        "Interruptions": false
                    }
                }
            },
            "segments@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions('e523d2ed-2966-4b6b-925b-754a88034cc5')/segments",
            "segments": [
                {
                    "startDateTime": "2020-02-25T18:52:21.2169889Z",
                    "endDateTime": "2020-02-25T18:52:46.7640013Z",
                    "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
                    "caller": {
                        "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
                        "userAgent": {
                            "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
                            "headerValue": "RTCC/7.0.0.0 UCWA/7.0.0.0 AndroidLync/6.25.0.27 (SM-G930U Android 8.0.0)",
                            "platform": "android",
                            "productFamily": "skypeForBusiness"
                        },
                        "identity": {
                            "user": {
                                "id": "821809f5-0000-0000-0000-3b5136c0e777",
                                "displayName": "Abbie Wilkins",
                                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
                            }
                        }
                    },
                    "callee": {
                        "@odata.type": "#microsoft.graph.callRecords.participantEndpoint",
                        "userAgent": {
                            "@odata.type": "#microsoft.graph.callRecords.clientUserAgent",
                            "headerValue": "UCCAPI/16.0.12527.20122 OC/16.0.12527.20194 (Skype for Business)",
                            "platform": "windows",
                            "productFamily": "skypeForBusiness"
                        },
                        "identity": {
                            "user": {
                                "id": "f69e2c00-0000-0000-0000-185e5f5f5d8a",
                                "displayName": "Owen Franklin",
                                "tenantId": "dc368399-474c-4d40-900c-6265431fd81f"
                            }
                        }
                    },
                    "media": [
                        {
                            "label": "main-audio",
                            "callerNetwork": {
                                "ipAddress": "10.150.0.2",
                                "subnet": "10.150.0.0",
                                "linkSpeed": 54000000,
                                "connectionType": "wifi",
                                "port": 27288,
                                "reflexiveIPAddress": "127.0.0.2",
                                "relayIPAddress": "52.114.188.32",
                                "relayPort": 53889,
                                "macAddress": "00-00-00-00-00-00",
                                "dnsSuffix": null,
                                "sentQualityEventRatio": 0,
                                "receivedQualityEventRatio": 0.27,
                                "delayEventRatio": 0,
                                "bandwidthLowEventRatio": 0
                            },
                            "calleeNetwork": {
                                "ipAddress": "10.139.0.12",
                                "subnet": "10.139.80.0",
                                "linkSpeed": 4294967295,
                                "connectionType": "wired",
                                "port": 50011,
                                "reflexiveIPAddress": "127.0.0.2",
                                "relayIPAddress": "52.114.188.102",
                                "relayPort": 52810,
                                "macAddress": "00-00-00-00-00-00-00-00",
                                "dnsSuffix": null,
                                "sentQualityEventRatio": 0.31,
                                "receivedQualityEventRatio": 0,
                                "delayEventRatio": 0,
                                "bandwidthLowEventRatio": 0
                            },
                            "callerDevice": {
                                "captureDeviceName": "Default input device",
                                "renderDeviceName": "Default output device",
                                "receivedSignalLevel": -10,
                                "receivedNoiseLevel": -68,
                                "initialSignalLevelRootMeanSquare": 60.25816,
                                "renderZeroVolumeEventRatio": 1,
                                "renderMuteEventRatio": 1,
                                "micGlitchRate": 23,
                                "speakerGlitchRate": 3830
                            },
                            "calleeDevice": {
                                "captureDeviceName": "Microphone (Microsoft Virtual Audio Device (Simple) (WDM))",
                                "captureDeviceDriver": "Microsoft: 5.0.8638.1100",
                                "renderDeviceName": "Speakers (Microsoft Virtual Audio Device (Simple) (WDM))",
                                "renderDeviceDriver": "Microsoft: 5.0.8638.1100",
                                "receivedSignalLevel": -14,
                                "receivedNoiseLevel": -86,
                                "initialSignalLevelRootMeanSquare": 146.7885,
                                "micGlitchRate": 143,
                                "speakerGlitchRate": 182
                            },
                            "streams": [
                                {
                                    "streamId": "1504545584",
                                    "streamDirection": "callerToCallee",
                                    "averageAudioDegradation": null,
                                    "averageJitter": "PT0.016S",
                                    "maxJitter": "PT0.021S",
                                    "averagePacketLossRate": 0,
                                    "maxPacketLossRate": 0,
                                    "averageRatioOfConcealedSamples": null,
                                    "maxRatioOfConcealedSamples": null,
                                    "averageRoundTripTime": "PT0.061S",
                                    "maxRoundTripTime": "PT0.079S",
                                    "packetUtilization": 67,
                                    "averageBandwidthEstimate": 9965083,
                                    "wasMediaBypassed": false,
                                    "averageAudioNetworkJitter": "PT0.043S",
                                    "maxAudioNetworkJitter": "PT0.046S"
                                },
                                {
                                    "streamId": "1785122252",
                                    "streamDirection": "calleeToCaller",
                                    "averageAudioDegradation": 1.160898,
                                    "averageJitter": "PT0.007S",
                                    "maxJitter": "PT0.012S",
                                    "averagePacketLossRate": 0.01381693,
                                    "maxPacketLossRate": 0.03738318,
                                    "averageRatioOfConcealedSamples": 0.06233422,
                                    "maxRatioOfConcealedSamples": 0.07192807,
                                    "averageRoundTripTime": "PT0.064S",
                                    "maxRoundTripTime": "PT0.106S",
                                    "packetUtilization": 709,
                                    "averageBandwidthEstimate": 15644878,
                                    "wasMediaBypassed": false,
                                    "averageAudioNetworkJitter": "PT0.266S",
                                    "maxAudioNetworkJitter": "PT0.474S"
                                }
                            ]
                        }
                    ]
                }
            ]
        }
    ],
    "sessions@odata.nextLink": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions?$expand=segments&$skiptoken=abc"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get callRecord",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

