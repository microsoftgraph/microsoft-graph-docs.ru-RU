---
title: Получение callRecord
description: Получение свойств и связей объекта каллрекорд.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: ae239cd7bb559d8fc46cbaa43933a54d6ffe5e1c
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183654"
---
# <a name="get-callrecord"></a><span data-ttu-id="58e57-103">Получение callRecord</span><span class="sxs-lookup"><span data-stu-id="58e57-103">Get callRecord</span></span>

<span data-ttu-id="58e57-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="58e57-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="58e57-105">Получение свойств и связей объекта [каллрекорд](../resources/callrecords-callrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="58e57-105">Retrieve the properties and relationships of a [callRecord](../resources/callrecords-callrecord.md) object.</span></span>

<span data-ttu-id="58e57-106">Существует два способа получения **идентификатора** **каллрекорд**:</span><span class="sxs-lookup"><span data-stu-id="58e57-106">There are two ways to get the **id** of a **callRecord**:</span></span>

* <span data-ttu-id="58e57-107">Подпишитесь, чтобы [изменить уведомления](/graph/api/resources/webhooks?view=graph-rest-1.0) для `/communications/callRecords` конечной точки.</span><span class="sxs-lookup"><span data-stu-id="58e57-107">Subscribe to [change notifications](/graph/api/resources/webhooks?view=graph-rest-1.0) to the `/communications/callRecords` endpoint.</span></span>
* <span data-ttu-id="58e57-108">Используйте свойство **каллчаинид** [вызова](../resources/call.md).</span><span class="sxs-lookup"><span data-stu-id="58e57-108">Use the **callChainId** property of a [call](../resources/call.md).</span></span> <span data-ttu-id="58e57-109">Запись вызова доступна только после завершения связанного вызова.</span><span class="sxs-lookup"><span data-stu-id="58e57-109">The call record is available only after the associated call is completed.</span></span>

## <a name="permissions"></a><span data-ttu-id="58e57-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="58e57-110">Permissions</span></span>

<span data-ttu-id="58e57-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58e57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58e57-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58e57-113">Permission type</span></span>                        | <span data-ttu-id="58e57-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="58e57-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="58e57-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58e57-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="58e57-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58e57-116">Not supported.</span></span> |
| <span data-ttu-id="58e57-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58e57-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58e57-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58e57-118">Not supported.</span></span> |
| <span data-ttu-id="58e57-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="58e57-119">Application</span></span>                            | <span data-ttu-id="58e57-120">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="58e57-120">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58e57-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58e57-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/callRecords/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58e57-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="58e57-122">Optional query parameters</span></span>

<span data-ttu-id="58e57-123">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="58e57-123">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="58e57-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="58e57-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="58e57-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58e57-125">Request headers</span></span>

| <span data-ttu-id="58e57-126">Имя</span><span class="sxs-lookup"><span data-stu-id="58e57-126">Name</span></span>      |<span data-ttu-id="58e57-127">Описание</span><span class="sxs-lookup"><span data-stu-id="58e57-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="58e57-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="58e57-128">Authorization</span></span> | <span data-ttu-id="58e57-129">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="58e57-129">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="58e57-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="58e57-130">Request body</span></span>

<span data-ttu-id="58e57-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58e57-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58e57-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e57-132">Response</span></span>

<span data-ttu-id="58e57-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [Microsoft. Graph. Каллрекордс. каллрекорд](../resources/callrecords-callrecord.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="58e57-133">If successful, this method returns a `200 OK` response code and the requested [microsoft.graph.callRecords.callRecord](../resources/callrecords-callrecord.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58e57-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="58e57-134">Examples</span></span>

### <a name="example-1-get-basic-details"></a><span data-ttu-id="58e57-135">Пример 1: получение основных сведений</span><span class="sxs-lookup"><span data-stu-id="58e57-135">Example 1: Get basic details</span></span>

#### <a name="request"></a><span data-ttu-id="58e57-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="58e57-136">Request</span></span>

<span data-ttu-id="58e57-137">Ниже приведен пример запроса на получение основных сведений из [каллрекорд](../resources/callrecords-callrecord.md).</span><span class="sxs-lookup"><span data-stu-id="58e57-137">The following is an example of the request to get the basic details from a [callRecord](../resources/callrecords-callrecord.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_callrecord"
}-->

```http
GET https://graph.microsoft.com/v1.0/communications/callRecords/{id}
```

#### <a name="response"></a><span data-ttu-id="58e57-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e57-138">Response</span></span>

<span data-ttu-id="58e57-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="58e57-139">The following is an example of the response.</span></span>

> <span data-ttu-id="58e57-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58e57-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
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

### <a name="example-2-get-full-details"></a><span data-ttu-id="58e57-142">Пример 2: получение полных сведений</span><span class="sxs-lookup"><span data-stu-id="58e57-142">Example 2: Get full details</span></span>

#### <a name="request"></a><span data-ttu-id="58e57-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="58e57-143">Request</span></span>

<span data-ttu-id="58e57-144">Ниже приведен пример запроса на получение полных сведений из [каллрекорд](../resources/callrecords-callrecord.md), включая компоненты Session и Segment.</span><span class="sxs-lookup"><span data-stu-id="58e57-144">The following is an example of the request to get the full details from a [callRecord](../resources/callrecords-callrecord.md), including session and segment components.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_callrecord_expanded"
}-->

```http
GET https://graph.microsoft.com/v1.0/communications/callRecords/{id}?$expand=sessions($expand=segments)
```

#### <a name="response"></a><span data-ttu-id="58e57-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="58e57-145">Response</span></span>

<span data-ttu-id="58e57-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="58e57-146">The following is an example of the response.</span></span> <span data-ttu-id="58e57-147">Если список сеансов усекается, `sessions@odata.nextlink` будет предоставлено значение для получения следующей страницы сеансов.</span><span class="sxs-lookup"><span data-stu-id="58e57-147">If the sessions list is truncated, a `sessions@odata.nextlink` value will be provided to retrieve the next page of sessions.</span></span>

> <span data-ttu-id="58e57-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="58e57-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
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
    "sessions@odata.nextlink": "https://graph.microsoft.com/v1.0/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions?$expand=segments&$skiptoken=abc"
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
