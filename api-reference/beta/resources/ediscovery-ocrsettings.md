---
title: тип ресурса ocrSettings
description: Параметры OCR для дела об обнаружении электронной почты
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 648e0ad63f558f211591d1c8aa976c2689dd271d
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080893"
---
# <a name="ocrsettings-resource-type"></a><span data-ttu-id="60631-103">тип ресурса ocrSettings</span><span class="sxs-lookup"><span data-stu-id="60631-103">ocrSettings resource type</span></span>

<span data-ttu-id="60631-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="60631-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60631-105">Параметры OCR (Optical Character Recognition) для дела об обнаружении электронных обнаружений.</span><span class="sxs-lookup"><span data-stu-id="60631-105">The OCR (Optical Character Recognition) settings for the eDiscovery case.</span></span>

## <a name="properties"></a><span data-ttu-id="60631-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="60631-106">Properties</span></span>

|<span data-ttu-id="60631-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="60631-107">Property</span></span>|<span data-ttu-id="60631-108">Тип</span><span class="sxs-lookup"><span data-stu-id="60631-108">Type</span></span>|<span data-ttu-id="60631-109">Описание</span><span class="sxs-lookup"><span data-stu-id="60631-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60631-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="60631-110">isEnabled</span></span>|<span data-ttu-id="60631-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="60631-111">Boolean</span></span>|<span data-ttu-id="60631-112">Указывает, включен ли OCR для дела.</span><span class="sxs-lookup"><span data-stu-id="60631-112">Indicates whether or not OCR is enabled for the case.</span></span>|
|<span data-ttu-id="60631-113">maxImageSize</span><span class="sxs-lookup"><span data-stu-id="60631-113">maxImageSize</span></span>|<span data-ttu-id="60631-114">Int32</span><span class="sxs-lookup"><span data-stu-id="60631-114">Int32</span></span>|<span data-ttu-id="60631-115">Максимальный размер изображения, который будет обрабатываться в КБ).</span><span class="sxs-lookup"><span data-stu-id="60631-115">Maximum image size that will be processed in KB).</span></span>|
|<span data-ttu-id="60631-116">timeout</span><span class="sxs-lookup"><span data-stu-id="60631-116">timeout</span></span>|<span data-ttu-id="60631-117">Duration</span><span class="sxs-lookup"><span data-stu-id="60631-117">Duration</span></span>|<span data-ttu-id="60631-118">Продолжительность периода времени для двигателя OCR.</span><span class="sxs-lookup"><span data-stu-id="60631-118">The timeout duration for the OCR engine.</span></span> <span data-ttu-id="60631-119">Более длительный период времени может повысить успешность OCR, но может увеличить общее время обработки.</span><span class="sxs-lookup"><span data-stu-id="60631-119">A longer timeout may increase success of OCR, but may add to the total processing time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60631-120">Связи</span><span class="sxs-lookup"><span data-stu-id="60631-120">Relationships</span></span>

<span data-ttu-id="60631-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="60631-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="60631-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="60631-122">JSON representation</span></span>

<span data-ttu-id="60631-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60631-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.ocrSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.ocrSettings",
  "isEnabled": "Boolean",
  "maxImageSize": "Integer",
  "timeout": "String (duration)"
}
```
