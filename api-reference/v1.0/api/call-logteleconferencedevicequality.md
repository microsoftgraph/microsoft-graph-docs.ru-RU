---
title: 'call: logTeleconferenceDeviceQuality'
description: Запись в журнал данных о качестве устройств для видеоконференций.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: a6cbacb3ce97ca1b9b09b12e0185757d5c8392ac
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786049"
---
# <a name="call-logteleconferencedevicequality"></a><span data-ttu-id="cde88-103">call: logTeleconferenceDeviceQuality</span><span class="sxs-lookup"><span data-stu-id="cde88-103">call: logTeleconferenceDeviceQuality</span></span>

<span data-ttu-id="cde88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cde88-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cde88-105">Запись в журнал данных о качестве устройств для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="cde88-105">Log video teleconferencing device quality data.</span></span>

<span data-ttu-id="cde88-106">Бот Cloud Video Interop (CVI) представляет устройства видео телеконференции (VTC) и выступает в качестве обратного агента для устройства VTC во время конференц-связи.</span><span class="sxs-lookup"><span data-stu-id="cde88-106">The Cloud Video Interop (CVI) bot represents video teleconferencing (VTC) devices and acts as a back-to-back agent for a VTC device in a conference call.</span></span> <span data-ttu-id="cde88-107">Так как бот CVI находится в центре VTC и Microsoft Teams в качестве прокси-сервера VTC, он имеет две области мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="cde88-107">Because a CVI bot is in the middle of the VTC and Microsoft Teams infrastructure as a VTC proxy, it has two media legs.</span></span> <span data-ttu-id="cde88-108">Один этап мультимедиа находится между ботом CVI и Teams инфраструктурой, например сервером Teams конференции или Teams клиентом.</span><span class="sxs-lookup"><span data-stu-id="cde88-108">One media leg is between the CVI bot and Teams infrastructure, such as Teams conference server or a Teams client.</span></span> <span data-ttu-id="cde88-109">Другой этап мультимедиа находится между CVI-ботом и устройством VTC.</span><span class="sxs-lookup"><span data-stu-id="cde88-109">The other media leg is between the CVI bot and the VTC device.</span></span> 

<span data-ttu-id="cde88-110">Сторонние партнеры владеют медиа-ногой VTC, а инфраструктура Teams не может получить доступ к качественным данным сторонного вызова.</span><span class="sxs-lookup"><span data-stu-id="cde88-110">The third-party partners own the VTC media leg and the Teams infrastructure cannot access the quality data of the third-party call leg.</span></span>  <span data-ttu-id="cde88-111">Этот метод позволяет партнерам CVI предоставлять данные о качестве мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="cde88-111">This method is only for the CVI partners to provide their media quality data.</span></span>

## <a name="permissions"></a><span data-ttu-id="cde88-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cde88-112">Permissions</span></span>

<span data-ttu-id="cde88-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cde88-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cde88-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cde88-115">Permission type</span></span>                        | <span data-ttu-id="cde88-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cde88-116">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cde88-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cde88-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="cde88-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cde88-118">Not supported.</span></span> |
| <span data-ttu-id="cde88-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cde88-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cde88-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cde88-120">Not supported.</span></span> |
| <span data-ttu-id="cde88-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cde88-121">Application</span></span>                            | <span data-ttu-id="cde88-122">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="cde88-122">Calls.AccessMedia.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cde88-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cde88-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /communications/calls/logTeleconferenceDeviceQuality
```

## <a name="request-headers"></a><span data-ttu-id="cde88-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cde88-124">Request headers</span></span>

| <span data-ttu-id="cde88-125">Имя</span><span class="sxs-lookup"><span data-stu-id="cde88-125">Name</span></span>          | <span data-ttu-id="cde88-126">Описание</span><span class="sxs-lookup"><span data-stu-id="cde88-126">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cde88-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cde88-127">Authorization</span></span> | <span data-ttu-id="cde88-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cde88-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cde88-130">User-Agent</span><span class="sxs-lookup"><span data-stu-id="cde88-130">User-Agent</span></span>    | <span data-ttu-id="cde88-131">Описывает имя и версию вызываемого приложения.</span><span class="sxs-lookup"><span data-stu-id="cde88-131">Describes the name and version of the calling application.</span></span> <span data-ttu-id="cde88-132">Сведения будут всплыть в Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="cde88-132">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="cde88-133">Рекомендуемый формат — ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="cde88-133">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="cde88-134">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="cde88-134">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cde88-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cde88-135">Request body</span></span>

<span data-ttu-id="cde88-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="cde88-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="cde88-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="cde88-137">Parameter</span></span>    | <span data-ttu-id="cde88-138">Тип</span><span class="sxs-lookup"><span data-stu-id="cde88-138">Type</span></span>        | <span data-ttu-id="cde88-139">Описание</span><span class="sxs-lookup"><span data-stu-id="cde88-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cde88-140">качество</span><span class="sxs-lookup"><span data-stu-id="cde88-140">quality</span></span>|[<span data-ttu-id="cde88-141">teleconferenceDeviceQuality</span><span class="sxs-lookup"><span data-stu-id="cde88-141">teleconferenceDeviceQuality</span></span>](../resources/teleconferencedevicequality.md)|<span data-ttu-id="cde88-142">Качественные данные ногой мультимедиа VTC.</span><span class="sxs-lookup"><span data-stu-id="cde88-142">Quality data of VTC media leg.</span></span>|

## <a name="response"></a><span data-ttu-id="cde88-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="cde88-143">Response</span></span>

<span data-ttu-id="cde88-p106">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cde88-p106">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cde88-146">Примеры</span><span class="sxs-lookup"><span data-stu-id="cde88-146">Examples</span></span>

<span data-ttu-id="cde88-147">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="cde88-147">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="cde88-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="cde88-148">Request</span></span>

<span data-ttu-id="cde88-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cde88-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cde88-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="cde88-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call_logteleconferencedevicequality"
}-->

```http
POST https://graph.microsoft.com/v1.0/communications/calls/logTeleconferenceDeviceQuality
Content-type: application/json

{
  "quality": {
    "@odata.type": "#microsoft.graph.teleconferenceDeviceQuality",
    "callChainId": "0622673d-9f69-49b3-9d4f-5ec64f42ecce",
    "participantId": "ea078406-b5d4-4d3c-b85e-90103dcec7f6",
    "mediaLegId": "bd9ee398-4b9d-42c7-8b8d-4e8efad9435f",
    "deviceName": "TestAgent",
    "deviceDescription": "TestDescription",
    "mediaQualityList": [
      {
        "@odata.type": "#microsoft.graph.teleconferenceDeviceAudioQuality",
        "channelIndex": 1,
        "mediaDuration": "PT20M",
        "networkLinkSpeedInBytes": 13000,
        "localIPAddress": "127.0.0.1",
        "localPort": 6300,
        "remoteIPAddress": "102.1.1.101",
        "remotePort": 6301,
        "inboundPackets": 5500,
        "outboundPackets": 5400,
        "averageInboundPacketLossRateInPercentage": 0.01,
        "averageOutboundPacketLossRateInPercentage": 0.02,
        "maximumInboundPacketLossRateInPercentage": 0.05,
        "maximumOutboundPacketLossRateInPercentage": 0.06,
        "averageInboundRoundTripDelay": "PT0.03S",
        "averageOutboundRoundTripDelay": "PT0.04S",
        "maximumInboundRoundTripDelay": "PT0.13S",
        "maximumOutboundRoundTripDelay": "PT0.14S",
        "averageInboundJitter": "PT0.01S",
        "averageOutboundJitter": "PT0.015S",
        "maximumInboundJitter": "PT0.023S",
        "maximumOutboundJitter": "PT0.024S"
      },
      {
        "@odata.type": "#microsoft.graph.teleconferenceDeviceVideoQuality",
        "channelIndex": 1,
        "mediaDuration": "PT20M",
        "networkLinkSpeedInBytes": 13000,
        "localIPAddress": "127.0.0.1",
        "localPort": 6300,
        "remoteIPAddress": "102.1.1.101",
        "remotePort": 6301,
        "inboundPackets": 5500,
        "outboundPackets": 5400,
        "averageInboundPacketLossRateInPercentage": 0.01,
        "averageOutboundPacketLossRateInPercentage": 0.02,
        "maximumInboundPacketLossRateInPercentage": 0.05,
        "maximumOutboundPacketLossRateInPercentage": 0.06,
        "averageInboundRoundTripDelay": "PT0.03S",
        "averageOutboundRoundTripDelay": "PT0.04S",
        "maximumInboundRoundTripDelay": "PT0.13S",
        "maximumOutboundRoundTripDelay": "PT0.14S",
        "averageInboundJitter": "PT0.01S",
        "averageOutboundJitter": "PT0.015S",
        "maximumInboundJitter": "PT0.023S",
        "maximumOutboundJitter": "PT0.024S"
      },
      {
        "@odata.type": "#microsoft.graph.teleconferenceDeviceScreenSharingQuality",
        "channelIndex": 1,
        "mediaDuration": "PT20M",
        "networkLinkSpeedInBytes": 13000,
        "localIPAddress": "127.0.0.1",
        "localPort": 6300,
        "remoteIPAddress": "102.1.1.101",
        "remotePort": 6301,
        "inboundPackets": 5500,
        "outboundPackets": 5400,
        "averageInboundPacketLossRateInPercentage": 0.01,
        "averageOutboundPacketLossRateInPercentage": 0.02,
        "maximumInboundPacketLossRateInPercentage": 0.05,
        "maximumOutboundPacketLossRateInPercentage": 0.06,
        "averageInboundRoundTripDelay": "PT0.03S",
        "averageOutboundRoundTripDelay": "PT0.04S",
        "maximumInboundRoundTripDelay": "PT0.13S",
        "maximumOutboundRoundTripDelay": "PT0.14S",
        "averageInboundJitter": "PT0.01S",
        "averageOutboundJitter": "PT0.015S",
        "maximumInboundJitter": "PT0.023S",
        "maximumOutboundJitter": "PT0.024S"
      }
    ]
  }
}
```
# <a name="c"></a>[<span data-ttu-id="cde88-151">C#</span><span class="sxs-lookup"><span data-stu-id="cde88-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-logteleconferencedevicequality-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cde88-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cde88-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-logteleconferencedevicequality-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cde88-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cde88-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-logteleconferencedevicequality-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cde88-154">Java</span><span class="sxs-lookup"><span data-stu-id="cde88-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/call-logteleconferencedevicequality-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cde88-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="cde88-155">Response</span></span>

<span data-ttu-id="cde88-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cde88-156">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "call: logTeleconferenceDeviceQuality",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

