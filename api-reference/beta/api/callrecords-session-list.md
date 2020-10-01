---
title: Список сеансов Каллрекорд
description: Получение списка объектов Session для объекта Каллрекорд.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 51ef8e1e9cd56d5f969615cb9364ce26f8bd5d8e
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48329971"
---
# <a name="list-callrecord-sessions"></a><span data-ttu-id="ba6cc-103">Список сеансов Каллрекорд</span><span class="sxs-lookup"><span data-stu-id="ba6cc-103">List callRecord sessions</span></span>

<span data-ttu-id="ba6cc-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="ba6cc-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba6cc-105">Получение списка [сеансов](../resources/callrecords-session.md) , связанных с объектом [каллрекорд](../resources/callrecords-callrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="ba6cc-105">Retrieve the list of [sessions](../resources/callrecords-session.md) associated with a [callRecord](../resources/callrecords-callrecord.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba6cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba6cc-106">Permissions</span></span>

<span data-ttu-id="ba6cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba6cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba6cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba6cc-109">Permission type</span></span>                        | <span data-ttu-id="ba6cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba6cc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba6cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba6cc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba6cc-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba6cc-112">Not supported.</span></span> |
| <span data-ttu-id="ba6cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba6cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba6cc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba6cc-114">Not supported.</span></span> |
| <span data-ttu-id="ba6cc-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="ba6cc-115">Application</span></span>                            | <span data-ttu-id="ba6cc-116">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba6cc-116">CallRecords.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba6cc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba6cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /communications/callRecords/{id}/sessions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba6cc-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ba6cc-118">Optional query parameters</span></span>

<span data-ttu-id="ba6cc-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ba6cc-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ba6cc-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ba6cc-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba6cc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba6cc-121">Request headers</span></span>

| <span data-ttu-id="ba6cc-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ba6cc-122">Name</span></span>      |<span data-ttu-id="ba6cc-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ba6cc-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba6cc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba6cc-124">Authorization</span></span> | <span data-ttu-id="ba6cc-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ba6cc-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba6cc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba6cc-126">Request body</span></span>

<span data-ttu-id="ba6cc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba6cc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba6cc-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba6cc-128">Response</span></span>

<span data-ttu-id="ba6cc-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенные объекты [Session](../resources/callrecords-session.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ba6cc-129">If successful, this method returns a `200 OK` response code and the requested [session](../resources/callrecords-session.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba6cc-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="ba6cc-130">Examples</span></span>

### <a name="example-1-get-session-list"></a><span data-ttu-id="ba6cc-131">Пример 1: получение списка сеансов</span><span class="sxs-lookup"><span data-stu-id="ba6cc-131">Example 1: Get session list</span></span>

#### <a name="request"></a><span data-ttu-id="ba6cc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba6cc-132">Request</span></span>

<span data-ttu-id="ba6cc-133">Ниже приведен пример запроса на получение списка [сеансов](../resources/callrecords-session.md) для [каллрекорд](../resources/callrecords-callrecord.md).</span><span class="sxs-lookup"><span data-stu-id="ba6cc-133">The following is an example of the request to get the list of [sessions](../resources/callrecords-session.md) for a [callRecord](../resources/callrecords-callrecord.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_callrecord_sessions"
}-->

```http
GET https://graph.microsoft.com/beta/communications/callRecords/{id}/sessions
```

#### <a name="response"></a><span data-ttu-id="ba6cc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba6cc-134">Response</span></span>

<span data-ttu-id="ba6cc-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba6cc-135">The following is an example of the response.</span></span>

> <span data-ttu-id="ba6cc-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba6cc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.session",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions",
    "value": [
        {
            "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
            "modalities": [
                "audio"
            ],
            "startDateTime": "2020-02-25T18:52:21.2169889Z",
            "endDateTime": "2020-02-25T18:52:46.7640013Z",
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
            }
        }
    ],
    "@odata.nextLink": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions?$skiptoken=abc"
}
```

### <a name="example-2-get-session-list-with-segments"></a><span data-ttu-id="ba6cc-138">Пример 2: получение списка сеансов с сегментами</span><span class="sxs-lookup"><span data-stu-id="ba6cc-138">Example 2: Get session list with segments</span></span>

#### <a name="request"></a><span data-ttu-id="ba6cc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba6cc-139">Request</span></span>

<span data-ttu-id="ba6cc-140">Ниже приведен пример запроса на получение списка [сеансов](../resources/callrecords-session.md) для [каллрекорд](../resources/callrecords-callrecord.md) с включенными [сегментами](../resources/callrecords-segment.md) .</span><span class="sxs-lookup"><span data-stu-id="ba6cc-140">The following is an example of the request to get the list of [sessions](../resources/callrecords-session.md) for a [callRecord](../resources/callrecords-callrecord.md) with [segments](../resources/callrecords-segment.md) included.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_callrecord_sessions_expanded"
}-->

```http
GET https://graph.microsoft.com/beta/communications/callRecords/{id}/sessions?$expand=segments
```

#### <a name="response"></a><span data-ttu-id="ba6cc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba6cc-141">Response</span></span>

<span data-ttu-id="ba6cc-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba6cc-142">The following is an example of the response.</span></span>

> <span data-ttu-id="ba6cc-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba6cc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.session",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions",
    "value": [
        {
            "id": "e523d2ed-2966-4b6b-925b-754a88034cc5",
            "modalities": [
                "audio"
            ],
            "startDateTime": "2020-02-25T18:52:21.2169889Z",
            "endDateTime": "2020-02-25T18:52:46.7640013Z",
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
    "@odata.nextLink": "https://graph.microsoft.com/beta/$metadata#communications/callRecords('e523d2ed-2966-4b6b-925b-754a88034cc5')/sessions?$expand=segments&$skiptoken=abc"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


