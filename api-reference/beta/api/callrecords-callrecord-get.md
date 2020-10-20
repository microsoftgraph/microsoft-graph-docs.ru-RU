---
title: Получение callRecord
description: Получение свойств и связей объекта каллрекорд.
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7660af536659ad6c2baf1e2ad12938ee10a46c9d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601120"
---
# <a name="get-callrecord"></a><span data-ttu-id="e3a8e-103">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="e3a8e-103">Get callRecord</span></span>

<span data-ttu-id="e3a8e-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="e3a8e-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3a8e-105">Получение свойств и связей объекта [каллрекорд](../resources/callrecords-callrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="e3a8e-105">Retrieve the properties and relationships of a [callRecord](../resources/callrecords-callrecord.md) object.</span></span>

<span data-ttu-id="e3a8e-106">Существует два способа получения **идентификатора** **каллрекорд**:</span><span class="sxs-lookup"><span data-stu-id="e3a8e-106">There are two ways to get the **id** of a **callRecord**:</span></span>

* <span data-ttu-id="e3a8e-107">Подпишитесь, чтобы [изменить уведомления](/graph/api/resources/webhooks?view=graph-rest-beta) для `/communications/callRecords` конечной точки.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-107">Subscribe to [change notifications](/graph/api/resources/webhooks?view=graph-rest-beta) to the `/communications/callRecords` endpoint.</span></span>
* <span data-ttu-id="e3a8e-108">Используйте свойство **каллчаинид** [вызова](../resources/call.md).</span><span class="sxs-lookup"><span data-stu-id="e3a8e-108">Use the **callChainId** property of a [call](../resources/call.md).</span></span> <span data-ttu-id="e3a8e-109">Запись вызова доступна только после завершения связанного вызова.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-109">The call record is available only after the associated call is completed.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3a8e-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3a8e-110">Permissions</span></span>

<span data-ttu-id="e3a8e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3a8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e3a8e-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3a8e-113">Permission type</span></span>                        | <span data-ttu-id="e3a8e-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3a8e-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e3a8e-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3a8e-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e3a8e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-116">Not supported.</span></span> |
| <span data-ttu-id="e3a8e-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3a8e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3a8e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-118">Not supported.</span></span> |
| <span data-ttu-id="e3a8e-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="e3a8e-119">Application</span></span>                            | <span data-ttu-id="e3a8e-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3a8e-120">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3a8e-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3a8e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/callRecords/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3a8e-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e3a8e-122">Optional query parameters</span></span>

<span data-ttu-id="e3a8e-123">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-123">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e3a8e-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e3a8e-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3a8e-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3a8e-125">Request headers</span></span>

| <span data-ttu-id="e3a8e-126">Имя</span><span class="sxs-lookup"><span data-stu-id="e3a8e-126">Name</span></span>      |<span data-ttu-id="e3a8e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="e3a8e-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3a8e-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3a8e-128">Authorization</span></span> | <span data-ttu-id="e3a8e-129">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="e3a8e-129">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3a8e-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e3a8e-130">Request body</span></span>

<span data-ttu-id="e3a8e-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3a8e-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3a8e-132">Response</span></span>

<span data-ttu-id="e3a8e-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [Microsoft. Graph. Каллрекордс. каллрекорд](../resources/callrecords-callrecord.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-133">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3a8e-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="e3a8e-134">Examples</span></span>

### <a name="example-1-get-basic-details"></a><span data-ttu-id="e3a8e-135">Пример 1: получение основных сведений</span><span class="sxs-lookup"><span data-stu-id="e3a8e-135">Example 1: Get basic details</span></span>

#### <a name="request"></a><span data-ttu-id="e3a8e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3a8e-136">Request</span></span>

<span data-ttu-id="e3a8e-137">Ниже приведен пример запроса на получение основных сведений из [каллрекорд](../resources/callrecords-callrecord.md).</span><span class="sxs-lookup"><span data-stu-id="e3a8e-137">The following is an example of the request to get the basic details from a [callRecord](../resources/callrecords-callrecord.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_callrecord"
}-->

```http
GET https://graph.microsoft.com/beta/communications/callRecords/{id}
```

#### <a name="response"></a><span data-ttu-id="e3a8e-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3a8e-138">Response</span></span>

<span data-ttu-id="e3a8e-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-139">The following is an example of the response.</span></span>

> <span data-ttu-id="e3a8e-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.callRecord"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords/$entity",
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

### <a name="example-2-get-full-details"></a><span data-ttu-id="e3a8e-142">Пример 2: получение полных сведений</span><span class="sxs-lookup"><span data-stu-id="e3a8e-142">Example 2: Get full details</span></span>

#### <a name="request"></a><span data-ttu-id="e3a8e-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3a8e-143">Request</span></span>

<span data-ttu-id="e3a8e-144">Ниже приведен пример запроса на получение полных сведений из [каллрекорд](../resources/callrecords-callrecord.md), включая компоненты Session и Segment.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-144">The following is an example of the request to get the full details from a [callRecord](../resources/callrecords-callrecord.md), including session and segment components.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_callrecord_expanded"
}-->

```http
GET https://graph.microsoft.com/beta/communications/callRecords/{id}?$expand=sessions($expand=segments)
```

#### <a name="response"></a><span data-ttu-id="e3a8e-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="e3a8e-145">Response</span></span>

<span data-ttu-id="e3a8e-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-146">The following is an example of the response.</span></span> <span data-ttu-id="e3a8e-147">Если список сеансов усекается, `sessions@odata.nextLink` будет предоставлено значение для получения следующей страницы сеансов.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-147">If the sessions list is truncated, a `sessions@odata.nextLink` value will be provided to retrieve the next page of sessions.</span></span>

> <span data-ttu-id="e3a8e-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e3a8e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.callRecord"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords(sessions(segments()))/$entity",
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
    "sessions@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions(segments())",
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
            "segments@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions('e523d2ed-2966-4b6b-925b-754a88034cc5')/segments",
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
    "sessions@odata.nextLink": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions?$expand=segments&$skiptoken=abc"
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


