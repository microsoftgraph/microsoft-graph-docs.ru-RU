---
title: Тип ресурса Нетворкинфо
description: Тип Нетворкинфо
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4e7054fa425a38e90cd62b4b69ea8a034d26d6b0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601685"
---
# <a name="networkinfo-resource-type"></a><span data-ttu-id="4444c-103">Тип ресурса Нетворкинфо</span><span class="sxs-lookup"><span data-stu-id="4444c-103">networkInfo resource type</span></span>

<span data-ttu-id="4444c-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="4444c-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4444c-105">Представляет сведения о сети, используемой в вызове.</span><span class="sxs-lookup"><span data-stu-id="4444c-105">Represents information about the network used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="4444c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4444c-106">Properties</span></span>

| <span data-ttu-id="4444c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4444c-107">Property</span></span>     | <span data-ttu-id="4444c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4444c-108">Type</span></span>        | <span data-ttu-id="4444c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4444c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4444c-110">бандвидсловевентратио</span><span class="sxs-lookup"><span data-stu-id="4444c-110">bandwidthLowEventRatio</span></span>|<span data-ttu-id="4444c-111">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4444c-111">Double</span></span>|<span data-ttu-id="4444c-112">Доля звонка, когда конечная точка мультимедиа обнаружила доступную пропускную способность или политику пропускной способности, достаточно низкой, чтобы снизить качество передачи звука.</span><span class="sxs-lookup"><span data-stu-id="4444c-112">Fraction of the call that the media endpoint detected the available bandwidth or bandwidth policy was low enough to cause poor quality of the audio sent.</span></span>|
|<span data-ttu-id="4444c-113">басиксервицесетидентифиер</span><span class="sxs-lookup"><span data-stu-id="4444c-113">basicServiceSetIdentifier</span></span>|<span data-ttu-id="4444c-114">String</span><span class="sxs-lookup"><span data-stu-id="4444c-114">String</span></span>|<span data-ttu-id="4444c-115">Идентификатор набора служб беспроводной локальной сети для конечной точки носителя, используемой для подключения к сети.</span><span class="sxs-lookup"><span data-stu-id="4444c-115">The wireless LAN basic service set identifier of the media endpoint used to connect to the network.</span></span>|
|<span data-ttu-id="4444c-116">connectionType</span><span class="sxs-lookup"><span data-stu-id="4444c-116">connectionType</span></span>|<span data-ttu-id="4444c-117">Microsoft. Graph. Каллрекордс. Нетворкконнектионтипе</span><span class="sxs-lookup"><span data-stu-id="4444c-117">microsoft.graph.callRecords.networkConnectionType</span></span>|<span data-ttu-id="4444c-118">Тип сети, используемой конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-118">Type of network used by the media endpoint.</span></span> <span data-ttu-id="4444c-119">Возможные значения: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4444c-119">Possible values are: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4444c-120">делайевентратио</span><span class="sxs-lookup"><span data-stu-id="4444c-120">delayEventRatio</span></span>|<span data-ttu-id="4444c-121">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4444c-121">Double</span></span>|<span data-ttu-id="4444c-122">Доля звонка, когда конечная точка мультимедиа обнаружила, что задержка в сети была достаточно большой, чтобы повлиять на возможность двусторонней связи в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="4444c-122">Fraction of the call that the media endpoint detected the network delay was significant enough to impact the ability to have real-time two-way communication.</span></span>|
|<span data-ttu-id="4444c-123">днссуффикс</span><span class="sxs-lookup"><span data-stu-id="4444c-123">dnsSuffix</span></span>|<span data-ttu-id="4444c-124">String</span><span class="sxs-lookup"><span data-stu-id="4444c-124">String</span></span>|<span data-ttu-id="4444c-125">DNS-суффикс, связанный с сетевым адаптером конечной точки носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-125">DNS suffix associated with the network adapter of the media endpoint.</span></span>|
|<span data-ttu-id="4444c-126">ipAddress</span><span class="sxs-lookup"><span data-stu-id="4444c-126">ipAddress</span></span>|<span data-ttu-id="4444c-127">String</span><span class="sxs-lookup"><span data-stu-id="4444c-127">String</span></span>|<span data-ttu-id="4444c-128">IP-адрес конечной точки носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-128">IP address of the media endpoint.</span></span>|
|<span data-ttu-id="4444c-129">линкспид</span><span class="sxs-lookup"><span data-stu-id="4444c-129">linkSpeed</span></span>|<span data-ttu-id="4444c-130">Int64</span><span class="sxs-lookup"><span data-stu-id="4444c-130">Int64</span></span>|<span data-ttu-id="4444c-131">Скорость канала в битах в секунду, сообщаемая сетевым адаптером, используемым конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-131">Link speed in bits per second reported by the network adapter used by the media endpoint.</span></span>|
|<span data-ttu-id="4444c-132">macAddress</span><span class="sxs-lookup"><span data-stu-id="4444c-132">macAddress</span></span>|<span data-ttu-id="4444c-133">String</span><span class="sxs-lookup"><span data-stu-id="4444c-133">String</span></span>|<span data-ttu-id="4444c-134">MAC-адрес сетевого устройства конечной точки носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-134">The media access control (MAC) address of the media endpoint's network device.</span></span>|
|<span data-ttu-id="4444c-135">порта</span><span class="sxs-lookup"><span data-stu-id="4444c-135">port</span></span>|<span data-ttu-id="4444c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4444c-136">Int32</span></span>|<span data-ttu-id="4444c-137">Номер сетевого порта, используемый конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-137">Network port number used by media endpoint.</span></span>|
|<span data-ttu-id="4444c-138">рецеиведкуалитевентратио</span><span class="sxs-lookup"><span data-stu-id="4444c-138">receivedQualityEventRatio</span></span>|<span data-ttu-id="4444c-139">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4444c-139">Double</span></span>|<span data-ttu-id="4444c-140">Доля звонка, когда конечная точка мультимедиа обнаружила, что сеть привела к низкому качеству полученного звука.</span><span class="sxs-lookup"><span data-stu-id="4444c-140">Fraction of the call that the media endpoint detected the network was causing poor quality of the audio received.</span></span>|
|<span data-ttu-id="4444c-141">рефлексивеипаддресс</span><span class="sxs-lookup"><span data-stu-id="4444c-141">reflexiveIPAddress</span></span>|<span data-ttu-id="4444c-142">String</span><span class="sxs-lookup"><span data-stu-id="4444c-142">String</span></span>|<span data-ttu-id="4444c-143">IP-адрес конечной точки носителя, отображаемый сервером ретрансляции мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="4444c-143">IP address of the media endpoint as seen by the media relay server.</span></span> <span data-ttu-id="4444c-144">Обычно это общедоступный IP-адрес в Интернете, связанный с конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="4444c-144">This is typically the public internet IP address associated to the endpoint.</span></span>|
|<span data-ttu-id="4444c-145">релайипаддресс</span><span class="sxs-lookup"><span data-stu-id="4444c-145">relayIPAddress</span></span>|<span data-ttu-id="4444c-146">String</span><span class="sxs-lookup"><span data-stu-id="4444c-146">String</span></span>|<span data-ttu-id="4444c-147">IP-адрес сервера ретрансляции мультимедиа, выделенный конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-147">IP address of the media relay server allocated by the media endpoint.</span></span>|
|<span data-ttu-id="4444c-148">релайпорт</span><span class="sxs-lookup"><span data-stu-id="4444c-148">relayPort</span></span>|<span data-ttu-id="4444c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="4444c-149">Int32</span></span>|<span data-ttu-id="4444c-150">Номер сетевого порта, выделенный на сервере ретрансляции мультимедиа конечной точкой мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="4444c-150">Network port number allocated on the media relay server by the media endpoint.</span></span>|
|<span data-ttu-id="4444c-151">сенткуалитевентратио</span><span class="sxs-lookup"><span data-stu-id="4444c-151">sentQualityEventRatio</span></span>|<span data-ttu-id="4444c-152">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="4444c-152">Double</span></span>|<span data-ttu-id="4444c-153">Доля звонка, когда конечная точка мультимедиа обнаружила, что сеть привела к низкому качеству отправленного звука.</span><span class="sxs-lookup"><span data-stu-id="4444c-153">Fraction of the call that the media endpoint detected the network was causing poor quality of the audio sent.</span></span>|
|<span data-ttu-id="4444c-154">подсети</span><span class="sxs-lookup"><span data-stu-id="4444c-154">subnet</span></span>|<span data-ttu-id="4444c-155">String</span><span class="sxs-lookup"><span data-stu-id="4444c-155">String</span></span>|<span data-ttu-id="4444c-156">Подсеть, используемая конечной точкой мультимедиа для потока мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="4444c-156">Subnet used for media stream by the media endpoint.</span></span>|
|<span data-ttu-id="4444c-157">вифибанд</span><span class="sxs-lookup"><span data-stu-id="4444c-157">wifiBand</span></span>|<span data-ttu-id="4444c-158">Microsoft. Graph. Каллрекордс. Вифибанд</span><span class="sxs-lookup"><span data-stu-id="4444c-158">microsoft.graph.callRecords.wifiBand</span></span>|<span data-ttu-id="4444c-159">Полоса Wi-Fi, используемая конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-159">WiFi band used by the media endpoint.</span></span> <span data-ttu-id="4444c-160">Возможные значения: `unknown`, `frequency24GHz`, `frequency50GHz`, `frequency60GHz`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4444c-160">Possible values are: `unknown`, `frequency24GHz`, `frequency50GHz`, `frequency60GHz`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4444c-161">вифибаттеричарже</span><span class="sxs-lookup"><span data-stu-id="4444c-161">wifiBatteryCharge</span></span>|<span data-ttu-id="4444c-162">Int32</span><span class="sxs-lookup"><span data-stu-id="4444c-162">Int32</span></span>|<span data-ttu-id="4444c-163">Оценка оставшегося заряда батареи в процентах от конечной точки носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-163">Estimated remaining battery charge in percentage reported by the media endpoint.</span></span>|
|<span data-ttu-id="4444c-164">вифичаннел</span><span class="sxs-lookup"><span data-stu-id="4444c-164">wifiChannel</span></span>|<span data-ttu-id="4444c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4444c-165">Int32</span></span>|<span data-ttu-id="4444c-166">Канал Wi-Fi, используемый конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-166">WiFi channel used by the media endpoint.</span></span>|
|<span data-ttu-id="4444c-167">вифимикрософтдривер</span><span class="sxs-lookup"><span data-stu-id="4444c-167">wifiMicrosoftDriver</span></span>|<span data-ttu-id="4444c-168">String</span><span class="sxs-lookup"><span data-stu-id="4444c-168">String</span></span>|<span data-ttu-id="4444c-169">Имя драйвера Microsoft WiFi, используемого конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-169">Name of the Microsoft WiFi driver used by the media endpoint.</span></span> <span data-ttu-id="4444c-170">Значение может быть локализовано на основе языка, используемого конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="4444c-170">Value may be localized based on the language used by endpoint.</span></span>|
|<span data-ttu-id="4444c-171">вифимикрософтдриверверсион</span><span class="sxs-lookup"><span data-stu-id="4444c-171">wifiMicrosoftDriverVersion</span></span>|<span data-ttu-id="4444c-172">String</span><span class="sxs-lookup"><span data-stu-id="4444c-172">String</span></span>|<span data-ttu-id="4444c-173">Версия драйвера Wi-Fi (Майкрософт), используемая конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-173">Version of the Microsoft WiFi driver used by the media endpoint.</span></span>|
|<span data-ttu-id="4444c-174">вифирадиотипе</span><span class="sxs-lookup"><span data-stu-id="4444c-174">wifiRadioType</span></span>|<span data-ttu-id="4444c-175">Microsoft. Graph. Каллрекордс. Вифирадиотипе</span><span class="sxs-lookup"><span data-stu-id="4444c-175">microsoft.graph.callRecords.wifiRadioType</span></span>|<span data-ttu-id="4444c-176">Тип радиосвязи Wi-Fi, используемый конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-176">Type of WiFi radio used by the media endpoint.</span></span> <span data-ttu-id="4444c-177">Возможные значения: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="4444c-177">Possible values are: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="4444c-178">вифисигналстренгс</span><span class="sxs-lookup"><span data-stu-id="4444c-178">wifiSignalStrength</span></span>|<span data-ttu-id="4444c-179">Int32</span><span class="sxs-lookup"><span data-stu-id="4444c-179">Int32</span></span>|<span data-ttu-id="4444c-180">Сила сигнала Wi-Fi в процентном отношении, сообщаемая конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-180">WiFi signal strength in percentage reported by the media endpoint.</span></span>|
|<span data-ttu-id="4444c-181">вифивендордривер</span><span class="sxs-lookup"><span data-stu-id="4444c-181">wifiVendorDriver</span></span>|<span data-ttu-id="4444c-182">String</span><span class="sxs-lookup"><span data-stu-id="4444c-182">String</span></span>|<span data-ttu-id="4444c-183">Имя драйвера Wi-Fi, используемого конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-183">Name of the WiFi driver used by the media endpoint.</span></span> <span data-ttu-id="4444c-184">Значение может быть локализовано на основе языка, используемого конечной точкой.</span><span class="sxs-lookup"><span data-stu-id="4444c-184">Value may be localized based on the language used by endpoint.</span></span>|
|<span data-ttu-id="4444c-185">вифивендордриверверсион</span><span class="sxs-lookup"><span data-stu-id="4444c-185">wifiVendorDriverVersion</span></span>|<span data-ttu-id="4444c-186">String</span><span class="sxs-lookup"><span data-stu-id="4444c-186">String</span></span>|<span data-ttu-id="4444c-187">Версия драйвера Wi-Fi, используемая конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="4444c-187">Version of the WiFi driver used by the media endpoint.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4444c-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4444c-188">JSON representation</span></span>

<span data-ttu-id="4444c-189">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4444c-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.networkInfo",
  "baseType": null
}-->

```json
{
  "bandwidthLowEventRatio": "Double",
  "basicServiceSetIdentifier": "String",
  "connectionType": "String",
  "delayEventRatio": "Double",
  "dnsSuffix": "String",
  "ipAddress": "String",
  "linkSpeed": 1024,
  "macAddress": "String",
  "port": 1024,
  "receivedQualityEventRatio": "Double",
  "reflexiveIPAddress": "String",
  "relayIPAddress": "String",
  "relayPort": 1024,
  "sentQualityEventRatio": "Double",
  "subnet": "String",
  "wifiBand": "String",
  "wifiBatteryCharge": 1024,
  "wifiChannel": 1024,
  "wifiMicrosoftDriver": "String",
  "wifiMicrosoftDriverVersion": "String",
  "wifiRadioType": "String",
  "wifiSignalStrength": 1024,
  "wifiVendorDriver": "String",
  "wifiVendorDriverVersion": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

