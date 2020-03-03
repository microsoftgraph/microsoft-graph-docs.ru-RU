---
title: Тип ресурса Девицеинфо
description: Тип Девицеинфо
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 17ebc8d0a7ffe9a59dd5225439e90af41aaa688a
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394865"
---
# <a name="deviceinfo-resource-type"></a><span data-ttu-id="8b6b9-103">Тип ресурса Девицеинфо</span><span class="sxs-lookup"><span data-stu-id="8b6b9-103">deviceInfo resource type</span></span>

<span data-ttu-id="8b6b9-104">Пространство имен: Microsoft. Graph. Каллрекордс</span><span class="sxs-lookup"><span data-stu-id="8b6b9-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b6b9-105">Представляет сведения о устройстве (микрофон, динамик, Камера и т. д.), используемые при вызове.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-105">Represents information about a device (microphone, speaker, camera, etc.) used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="8b6b9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b6b9-106">Properties</span></span>

| <span data-ttu-id="8b6b9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b6b9-107">Property</span></span>     | <span data-ttu-id="8b6b9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8b6b9-108">Type</span></span>        | <span data-ttu-id="8b6b9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8b6b9-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8b6b9-110">каптуредевицедривер</span><span class="sxs-lookup"><span data-stu-id="8b6b9-110">captureDeviceDriver</span></span>|<span data-ttu-id="8b6b9-111">String</span><span class="sxs-lookup"><span data-stu-id="8b6b9-111">String</span></span>|<span data-ttu-id="8b6b9-112">Имя драйвера устройства захвата, используемого конечной точкой мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-112">Name of the capture device driver used by the media endpoint.</span></span>|
|<span data-ttu-id="8b6b9-113">каптуредевиценаме</span><span class="sxs-lookup"><span data-stu-id="8b6b9-113">captureDeviceName</span></span>|<span data-ttu-id="8b6b9-114">String</span><span class="sxs-lookup"><span data-stu-id="8b6b9-114">String</span></span>|<span data-ttu-id="8b6b9-115">Имя устройства захвата, используемого конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-115">Name of the capture device used by the media endpoint.</span></span>|
|<span data-ttu-id="8b6b9-116">каптуренотфунктионинжевентратио</span><span class="sxs-lookup"><span data-stu-id="8b6b9-116">captureNotFunctioningEventRatio</span></span>|<span data-ttu-id="8b6b9-117">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b6b9-117">Double</span></span>|<span data-ttu-id="8b6b9-118">Доля звонка, когда конечная точка мультимедиа обнаружила, что устройство захвата не работает должным образом.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-118">Fraction of the call that the media endpoint detected the capture device was not working properly.</span></span>|
|<span data-ttu-id="8b6b9-119">кпуинсуффицентевентратио</span><span class="sxs-lookup"><span data-stu-id="8b6b9-119">cpuInsufficentEventRatio</span></span>|<span data-ttu-id="8b6b9-120">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b6b9-120">Double</span></span>|<span data-ttu-id="8b6b9-121">Доля звонка, когда конечная точка мультимедиа обнаружила, что ресурсы ЦП недостаточны и вызвали низкое качество отправленного и полученного звукового сигнала.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-121">Fraction of the call that the media endpoint detected the CPU resources available were insufficient and caused poor quality of the audio sent and received.</span></span>|
|<span data-ttu-id="8b6b9-122">девицеклиппинжевентратио</span><span class="sxs-lookup"><span data-stu-id="8b6b9-122">deviceClippingEventRatio</span></span>|<span data-ttu-id="8b6b9-123">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b6b9-123">Double</span></span>|<span data-ttu-id="8b6b9-124">Доля звонка, когда конечная точка мультимедиа обнаружила обрезку в записанном звуке, которая вызвала низкое качество отправляемого звука.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-124">Fraction of the call that the media endpoint detected clipping in the captured audio that caused poor quality of the audio being sent.</span></span>|
|<span data-ttu-id="8b6b9-125">девицеглитчевентратио</span><span class="sxs-lookup"><span data-stu-id="8b6b9-125">deviceGlitchEventRatio</span></span>|<span data-ttu-id="8b6b9-126">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b6b9-126">Double</span></span>|<span data-ttu-id="8b6b9-127">Доля звонка, когда конечная точка мультимедиа обнаружила ошибки или перерывы в воспроизводимом или захваченном звуке, что привело к неудовлетворительному качеству отправляемого или принимаемого звука.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-127">Fraction of the call that the media endpoint detected glitches or gaps in the audio played or captured that caused poor quality of the audio being sent or received.</span></span>|
|<span data-ttu-id="8b6b9-128">ховлинжевенткаунт</span><span class="sxs-lookup"><span data-stu-id="8b6b9-128">howlingEventCount</span></span>|<span data-ttu-id="8b6b9-129">Int32</span><span class="sxs-lookup"><span data-stu-id="8b6b9-129">Int32</span></span>|<span data-ttu-id="8b6b9-130">Количество вызовов, в течение которых конечная точка мультимедиа обнаружила ховлинг или скричинг Audio.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-130">Number of times during the call that the media endpoint detected howling or screeching audio.</span></span>|
|<span data-ttu-id="8b6b9-131">инитиалсигналлевелрутмеанскуаре</span><span class="sxs-lookup"><span data-stu-id="8b6b9-131">initialSignalLevelRootMeanSquare</span></span>|<span data-ttu-id="8b6b9-132">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b6b9-132">Double</span></span>|<span data-ttu-id="8b6b9-133">Средняя средняя квадрат (RMS) входящего сигнала до первого 30 секунд вызова.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-133">The root mean square (RMS) of the incoming signal of up to the first 30 seconds of the call.</span></span>|
|<span data-ttu-id="8b6b9-134">ловспичлевелевентратио</span><span class="sxs-lookup"><span data-stu-id="8b6b9-134">lowSpeechLevelEventRatio</span></span>|<span data-ttu-id="8b6b9-135">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b6b9-135">Double</span></span>|<span data-ttu-id="8b6b9-136">Доля звонка, когда конечная точка мультимедиа обнаружила слабый уровень речи, который вызвал низкое качество отправляемого звука.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-136">Fraction of the call that the media endpoint detected low speech level that caused poor quality of the audio being sent.</span></span>|
|<span data-ttu-id="8b6b9-137">ловспичтоноисивентратио</span><span class="sxs-lookup"><span data-stu-id="8b6b9-137">lowSpeechToNoiseEventRatio</span></span>|<span data-ttu-id="8b6b9-138">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b6b9-138">Double</span></span>|<span data-ttu-id="8b6b9-139">Доля звонка, когда конечная точка мультимедиа обнаружила низкую речь до уровня шума, который вызвал низкое качество отправляемого звука.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-139">Fraction of the call that the media endpoint detected low speech to noise level that caused poor quality of the audio being sent.</span></span>|
|<span data-ttu-id="8b6b9-140">микглитчрате</span><span class="sxs-lookup"><span data-stu-id="8b6b9-140">micGlitchRate</span></span>|<span data-ttu-id="8b6b9-141">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b6b9-141">Double</span></span>|<span data-ttu-id="8b6b9-142">Число сбоев для микрофона конечной точки носителя в течение 5 минут.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-142">Glitches per 5 minute interval for the media endpoint's microphone.</span></span>|
|<span data-ttu-id="8b6b9-143">рецеиведноиселевел</span><span class="sxs-lookup"><span data-stu-id="8b6b9-143">receivedNoiseLevel</span></span>|<span data-ttu-id="8b6b9-144">Int32</span><span class="sxs-lookup"><span data-stu-id="8b6b9-144">Int32</span></span>|<span data-ttu-id="8b6b9-145">Средний уровень энергии принятого звука для звука, классифицированного как моно шум, или левый канал стерео шума конечной точки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-145">Average energy level of received audio for audio classified as mono noise or left channel of stereo noise by the media endpoint.</span></span>|
|<span data-ttu-id="8b6b9-146">рецеиведсигналлевел</span><span class="sxs-lookup"><span data-stu-id="8b6b9-146">receivedSignalLevel</span></span>|<span data-ttu-id="8b6b9-147">Int32</span><span class="sxs-lookup"><span data-stu-id="8b6b9-147">Int32</span></span>|<span data-ttu-id="8b6b9-148">Средний уровень энергии принятого звука, классифицированного как моно речь, или левый канал стерео речи конечной точки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-148">Average energy level of received audio for audio classified as mono speech, or left channel of stereo speech by the media endpoint.</span></span>|
|<span data-ttu-id="8b6b9-149">рендердевицедривер</span><span class="sxs-lookup"><span data-stu-id="8b6b9-149">renderDeviceDriver</span></span>|<span data-ttu-id="8b6b9-150">String</span><span class="sxs-lookup"><span data-stu-id="8b6b9-150">String</span></span>|<span data-ttu-id="8b6b9-151">Имя драйвера устройства отрисовки, используемого конечной точкой мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-151">Name of the render device driver used by the media endpoint.</span></span>|
|<span data-ttu-id="8b6b9-152">рендердевиценаме</span><span class="sxs-lookup"><span data-stu-id="8b6b9-152">renderDeviceName</span></span>|<span data-ttu-id="8b6b9-153">String</span><span class="sxs-lookup"><span data-stu-id="8b6b9-153">String</span></span>|<span data-ttu-id="8b6b9-154">Имя устройства отрисовки, используемого конечной точкой мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-154">Name of the render device used by the media endpoint.</span></span>|
|<span data-ttu-id="8b6b9-155">рендермутивентратио</span><span class="sxs-lookup"><span data-stu-id="8b6b9-155">renderMuteEventRatio</span></span>|<span data-ttu-id="8b6b9-156">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b6b9-156">Double</span></span>|<span data-ttu-id="8b6b9-157">Доля звонка, когда конечная точка Media обнаружила, что устройство отображения устройства отключено.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-157">Fraction of the call that media endpoint detected device render is muted.</span></span>|
|<span data-ttu-id="8b6b9-158">рендернотфунктионинжевентратио</span><span class="sxs-lookup"><span data-stu-id="8b6b9-158">renderNotFunctioningEventRatio</span></span>|<span data-ttu-id="8b6b9-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b6b9-159">Double</span></span>|<span data-ttu-id="8b6b9-160">Доля звонка, когда конечная точка мультимедиа обнаружила, что устройство отображения не работает должным образом.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-160">Fraction of the call that the media endpoint detected the render device was not working properly.</span></span>|
|<span data-ttu-id="8b6b9-161">рендерзероволумивентратио</span><span class="sxs-lookup"><span data-stu-id="8b6b9-161">renderZeroVolumeEventRatio</span></span>|<span data-ttu-id="8b6b9-162">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b6b9-162">Double</span></span>|<span data-ttu-id="8b6b9-163">Доля звонка, когда конечная точка Media обнаружила, что для тома отображения устройства задано значение 0.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-163">Fraction of the call that media endpoint detected device render volume is set to 0.</span></span>|
|<span data-ttu-id="8b6b9-164">сентноиселевел</span><span class="sxs-lookup"><span data-stu-id="8b6b9-164">sentNoiseLevel</span></span>|<span data-ttu-id="8b6b9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8b6b9-165">Int32</span></span>|<span data-ttu-id="8b6b9-166">Средний уровень энергии отправленного звука для звука, классифицированного как моно шум, или левый канал стерео шума конечной точки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-166">Average energy level of sent audio for audio classified as mono noise or left channel of stereo noise by the media endpoint.</span></span>|
|<span data-ttu-id="8b6b9-167">сентсигналлевел</span><span class="sxs-lookup"><span data-stu-id="8b6b9-167">sentSignalLevel</span></span>|<span data-ttu-id="8b6b9-168">Int32</span><span class="sxs-lookup"><span data-stu-id="8b6b9-168">Int32</span></span>|<span data-ttu-id="8b6b9-169">Средний уровень энергии отправленного звука, классифицированного как моно речь, или левый канал стерео речи конечной точки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-169">Average energy level of sent audio for audio classified as mono speech, or left channel of stereo speech by the media endpoint.</span></span>|
|<span data-ttu-id="8b6b9-170">спеакерглитчрате</span><span class="sxs-lookup"><span data-stu-id="8b6b9-170">speakerGlitchRate</span></span>|<span data-ttu-id="8b6b9-171">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="8b6b9-171">Double</span></span>|<span data-ttu-id="8b6b9-172">Число сбоев в течение 5 минут внутренней для лаудспеакер конечной точки носителя.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-172">Glitches per 5 minute internal for the media endpoint's loudspeaker.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="8b6b9-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b6b9-173">JSON representation</span></span>

<span data-ttu-id="8b6b9-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b6b9-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.deviceInfo",
  "baseType": null
}-->

```json
{
  "captureDeviceDriver": "String",
  "captureDeviceName": "String",
  "captureNotFunctioningEventRatio": "Double",
  "cpuInsufficentEventRatio": "Double",
  "deviceClippingEventRatio": "Double",
  "deviceGlitchEventRatio": "Double",
  "howlingEventCount": 1024,
  "initialSignalLevelRootMeanSquare": "Double",
  "lowSpeechLevelEventRatio": "Double",
  "lowSpeechToNoiseEventRatio": "Double",
  "micGlitchRate": "Double",
  "receivedNoiseLevel": 1024,
  "receivedSignalLevel": 1024,
  "renderDeviceDriver": "String",
  "renderDeviceName": "String",
  "renderMuteEventRatio": "Double",
  "renderNotFunctioningEventRatio": "Double",
  "renderZeroVolumeEventRatio": "Double",
  "sentNoiseLevel": 1024,
  "sentSignalLevel": 1024,
  "speakerGlitchRate": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->