---
title: Тип ресурса Девицеинфо
description: Тип Девицеинфо
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8387926d7b6c8b0f5bf2ea774dc8d248d956c916
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492060"
---
# <a name="deviceinfo-resource-type"></a><span data-ttu-id="0daa7-103">Тип ресурса Девицеинфо</span><span class="sxs-lookup"><span data-stu-id="0daa7-103">deviceInfo resource type</span></span>

<span data-ttu-id="0daa7-104">Пространство имен: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="0daa7-104">Namespace: microsoft.graph.callRecords</span></span>

<span data-ttu-id="0daa7-105">Представляет сведения о устройстве (микрофон, динамик, Камера и т. д.), используемые при вызове.</span><span class="sxs-lookup"><span data-stu-id="0daa7-105">Represents information about a device (microphone, speaker, camera, etc.) used in a call.</span></span>

## <a name="properties"></a><span data-ttu-id="0daa7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0daa7-106">Properties</span></span>

| <span data-ttu-id="0daa7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0daa7-107">Property</span></span>     | <span data-ttu-id="0daa7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0daa7-108">Type</span></span>        | <span data-ttu-id="0daa7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0daa7-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0daa7-110">каптуредевицедривер</span><span class="sxs-lookup"><span data-stu-id="0daa7-110">captureDeviceDriver</span></span>|<span data-ttu-id="0daa7-111">String</span><span class="sxs-lookup"><span data-stu-id="0daa7-111">String</span></span>|<span data-ttu-id="0daa7-112">Имя драйвера устройства захвата, используемого конечной точкой мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="0daa7-112">Name of the capture device driver used by the media endpoint.</span></span>|
|<span data-ttu-id="0daa7-113">каптуредевиценаме</span><span class="sxs-lookup"><span data-stu-id="0daa7-113">captureDeviceName</span></span>|<span data-ttu-id="0daa7-114">String</span><span class="sxs-lookup"><span data-stu-id="0daa7-114">String</span></span>|<span data-ttu-id="0daa7-115">Имя устройства захвата, используемого конечной точкой носителя.</span><span class="sxs-lookup"><span data-stu-id="0daa7-115">Name of the capture device used by the media endpoint.</span></span>|
|<span data-ttu-id="0daa7-116">каптуренотфунктионинжевентратио</span><span class="sxs-lookup"><span data-stu-id="0daa7-116">captureNotFunctioningEventRatio</span></span>|<span data-ttu-id="0daa7-117">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0daa7-117">Double</span></span>|<span data-ttu-id="0daa7-118">Доля звонка, когда конечная точка мультимедиа обнаружила, что устройство захвата не работает должным образом.</span><span class="sxs-lookup"><span data-stu-id="0daa7-118">Fraction of the call that the media endpoint detected the capture device was not working properly.</span></span>|
|<span data-ttu-id="0daa7-119">кпуинсуффицентевентратио</span><span class="sxs-lookup"><span data-stu-id="0daa7-119">cpuInsufficentEventRatio</span></span>|<span data-ttu-id="0daa7-120">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0daa7-120">Double</span></span>|<span data-ttu-id="0daa7-121">Доля звонка, когда конечная точка мультимедиа обнаружила, что ресурсы ЦП недостаточны и вызвали низкое качество отправленного и полученного звукового сигнала.</span><span class="sxs-lookup"><span data-stu-id="0daa7-121">Fraction of the call that the media endpoint detected the CPU resources available were insufficient and caused poor quality of the audio sent and received.</span></span>|
|<span data-ttu-id="0daa7-122">девицеклиппинжевентратио</span><span class="sxs-lookup"><span data-stu-id="0daa7-122">deviceClippingEventRatio</span></span>|<span data-ttu-id="0daa7-123">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0daa7-123">Double</span></span>|<span data-ttu-id="0daa7-124">Доля звонка, когда конечная точка мультимедиа обнаружила обрезку в записанном звуке, которая вызвала низкое качество отправляемого звука.</span><span class="sxs-lookup"><span data-stu-id="0daa7-124">Fraction of the call that the media endpoint detected clipping in the captured audio that caused poor quality of the audio being sent.</span></span>|
|<span data-ttu-id="0daa7-125">девицеглитчевентратио</span><span class="sxs-lookup"><span data-stu-id="0daa7-125">deviceGlitchEventRatio</span></span>|<span data-ttu-id="0daa7-126">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0daa7-126">Double</span></span>|<span data-ttu-id="0daa7-127">Доля звонка, когда конечная точка мультимедиа обнаружила ошибки или перерывы в воспроизводимом или захваченном звуке, что привело к неудовлетворительному качеству отправляемого или принимаемого звука.</span><span class="sxs-lookup"><span data-stu-id="0daa7-127">Fraction of the call that the media endpoint detected glitches or gaps in the audio played or captured that caused poor quality of the audio being sent or received.</span></span>|
|<span data-ttu-id="0daa7-128">ховлинжевенткаунт</span><span class="sxs-lookup"><span data-stu-id="0daa7-128">howlingEventCount</span></span>|<span data-ttu-id="0daa7-129">Int32</span><span class="sxs-lookup"><span data-stu-id="0daa7-129">Int32</span></span>|<span data-ttu-id="0daa7-130">Количество вызовов, в течение которых конечная точка мультимедиа обнаружила ховлинг или скричинг Audio.</span><span class="sxs-lookup"><span data-stu-id="0daa7-130">Number of times during the call that the media endpoint detected howling or screeching audio.</span></span>|
|<span data-ttu-id="0daa7-131">инитиалсигналлевелрутмеанскуаре</span><span class="sxs-lookup"><span data-stu-id="0daa7-131">initialSignalLevelRootMeanSquare</span></span>|<span data-ttu-id="0daa7-132">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0daa7-132">Double</span></span>|<span data-ttu-id="0daa7-133">Средняя средняя квадрат (RMS) входящего сигнала до первого 30 секунд вызова.</span><span class="sxs-lookup"><span data-stu-id="0daa7-133">The root mean square (RMS) of the incoming signal of up to the first 30 seconds of the call.</span></span>|
|<span data-ttu-id="0daa7-134">ловспичлевелевентратио</span><span class="sxs-lookup"><span data-stu-id="0daa7-134">lowSpeechLevelEventRatio</span></span>|<span data-ttu-id="0daa7-135">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0daa7-135">Double</span></span>|<span data-ttu-id="0daa7-136">Доля звонка, когда конечная точка мультимедиа обнаружила слабый уровень речи, который вызвал низкое качество отправляемого звука.</span><span class="sxs-lookup"><span data-stu-id="0daa7-136">Fraction of the call that the media endpoint detected low speech level that caused poor quality of the audio being sent.</span></span>|
|<span data-ttu-id="0daa7-137">ловспичтоноисивентратио</span><span class="sxs-lookup"><span data-stu-id="0daa7-137">lowSpeechToNoiseEventRatio</span></span>|<span data-ttu-id="0daa7-138">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0daa7-138">Double</span></span>|<span data-ttu-id="0daa7-139">Доля звонка, когда конечная точка мультимедиа обнаружила низкую речь до уровня шума, который вызвал низкое качество отправляемого звука.</span><span class="sxs-lookup"><span data-stu-id="0daa7-139">Fraction of the call that the media endpoint detected low speech to noise level that caused poor quality of the audio being sent.</span></span>|
|<span data-ttu-id="0daa7-140">микглитчрате</span><span class="sxs-lookup"><span data-stu-id="0daa7-140">micGlitchRate</span></span>|<span data-ttu-id="0daa7-141">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0daa7-141">Double</span></span>|<span data-ttu-id="0daa7-142">Число сбоев для микрофона конечной точки носителя в течение 5 минут.</span><span class="sxs-lookup"><span data-stu-id="0daa7-142">Glitches per 5 minute interval for the media endpoint's microphone.</span></span>|
|<span data-ttu-id="0daa7-143">рецеиведноиселевел</span><span class="sxs-lookup"><span data-stu-id="0daa7-143">receivedNoiseLevel</span></span>|<span data-ttu-id="0daa7-144">Int32</span><span class="sxs-lookup"><span data-stu-id="0daa7-144">Int32</span></span>|<span data-ttu-id="0daa7-145">Средний уровень энергии принятого звука для звука, классифицированного как моно шум, или левый канал стерео шума конечной точки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="0daa7-145">Average energy level of received audio for audio classified as mono noise or left channel of stereo noise by the media endpoint.</span></span>|
|<span data-ttu-id="0daa7-146">рецеиведсигналлевел</span><span class="sxs-lookup"><span data-stu-id="0daa7-146">receivedSignalLevel</span></span>|<span data-ttu-id="0daa7-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0daa7-147">Int32</span></span>|<span data-ttu-id="0daa7-148">Средний уровень энергии принятого звука, классифицированного как моно речь, или левый канал стерео речи конечной точки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="0daa7-148">Average energy level of received audio for audio classified as mono speech, or left channel of stereo speech by the media endpoint.</span></span>|
|<span data-ttu-id="0daa7-149">рендердевицедривер</span><span class="sxs-lookup"><span data-stu-id="0daa7-149">renderDeviceDriver</span></span>|<span data-ttu-id="0daa7-150">String</span><span class="sxs-lookup"><span data-stu-id="0daa7-150">String</span></span>|<span data-ttu-id="0daa7-151">Имя драйвера устройства отрисовки, используемого конечной точкой мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="0daa7-151">Name of the render device driver used by the media endpoint.</span></span>|
|<span data-ttu-id="0daa7-152">рендердевиценаме</span><span class="sxs-lookup"><span data-stu-id="0daa7-152">renderDeviceName</span></span>|<span data-ttu-id="0daa7-153">String</span><span class="sxs-lookup"><span data-stu-id="0daa7-153">String</span></span>|<span data-ttu-id="0daa7-154">Имя устройства отрисовки, используемого конечной точкой мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="0daa7-154">Name of the render device used by the media endpoint.</span></span>|
|<span data-ttu-id="0daa7-155">рендермутивентратио</span><span class="sxs-lookup"><span data-stu-id="0daa7-155">renderMuteEventRatio</span></span>|<span data-ttu-id="0daa7-156">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0daa7-156">Double</span></span>|<span data-ttu-id="0daa7-157">Доля звонка, когда конечная точка Media обнаружила, что устройство отображения устройства отключено.</span><span class="sxs-lookup"><span data-stu-id="0daa7-157">Fraction of the call that media endpoint detected device render is muted.</span></span>|
|<span data-ttu-id="0daa7-158">рендернотфунктионинжевентратио</span><span class="sxs-lookup"><span data-stu-id="0daa7-158">renderNotFunctioningEventRatio</span></span>|<span data-ttu-id="0daa7-159">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0daa7-159">Double</span></span>|<span data-ttu-id="0daa7-160">Доля звонка, когда конечная точка мультимедиа обнаружила, что устройство отображения не работает должным образом.</span><span class="sxs-lookup"><span data-stu-id="0daa7-160">Fraction of the call that the media endpoint detected the render device was not working properly.</span></span>|
|<span data-ttu-id="0daa7-161">рендерзероволумивентратио</span><span class="sxs-lookup"><span data-stu-id="0daa7-161">renderZeroVolumeEventRatio</span></span>|<span data-ttu-id="0daa7-162">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0daa7-162">Double</span></span>|<span data-ttu-id="0daa7-163">Доля звонка, когда конечная точка Media обнаружила, что для тома отображения устройства задано значение 0.</span><span class="sxs-lookup"><span data-stu-id="0daa7-163">Fraction of the call that media endpoint detected device render volume is set to 0.</span></span>|
|<span data-ttu-id="0daa7-164">сентноиселевел</span><span class="sxs-lookup"><span data-stu-id="0daa7-164">sentNoiseLevel</span></span>|<span data-ttu-id="0daa7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0daa7-165">Int32</span></span>|<span data-ttu-id="0daa7-166">Средний уровень энергии отправленного звука для звука, классифицированного как моно шум, или левый канал стерео шума конечной точки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="0daa7-166">Average energy level of sent audio for audio classified as mono noise or left channel of stereo noise by the media endpoint.</span></span>|
|<span data-ttu-id="0daa7-167">сентсигналлевел</span><span class="sxs-lookup"><span data-stu-id="0daa7-167">sentSignalLevel</span></span>|<span data-ttu-id="0daa7-168">Int32</span><span class="sxs-lookup"><span data-stu-id="0daa7-168">Int32</span></span>|<span data-ttu-id="0daa7-169">Средний уровень энергии отправленного звука, классифицированного как моно речь, или левый канал стерео речи конечной точки мультимедиа.</span><span class="sxs-lookup"><span data-stu-id="0daa7-169">Average energy level of sent audio for audio classified as mono speech, or left channel of stereo speech by the media endpoint.</span></span>|
|<span data-ttu-id="0daa7-170">спеакерглитчрате</span><span class="sxs-lookup"><span data-stu-id="0daa7-170">speakerGlitchRate</span></span>|<span data-ttu-id="0daa7-171">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="0daa7-171">Double</span></span>|<span data-ttu-id="0daa7-172">Число сбоев в течение 5 минут внутренней для лаудспеакер конечной точки носителя.</span><span class="sxs-lookup"><span data-stu-id="0daa7-172">Glitches per 5 minute internal for the media endpoint's loudspeaker.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="0daa7-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0daa7-173">JSON representation</span></span>

<span data-ttu-id="0daa7-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0daa7-174">The following is a JSON representation of the resource.</span></span>

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