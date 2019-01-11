---
title: Тип ресурса airPrintDestination
description: Представляет целевой объект AirPrint.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6d1548737956d35d42fc077afe92de1885a54581
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878591"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="3f919-103">Тип ресурса airPrintDestination</span><span class="sxs-lookup"><span data-stu-id="3f919-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="3f919-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3f919-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f919-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f919-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f919-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3f919-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f919-107">Представляет целевой объект AirPrint.</span><span class="sxs-lookup"><span data-stu-id="3f919-107">Represents an AirPrint destination.</span></span>
## <a name="properties"></a><span data-ttu-id="3f919-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f919-108">Properties</span></span>
|<span data-ttu-id="3f919-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f919-109">Property</span></span>|<span data-ttu-id="3f919-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3f919-110">Type</span></span>|<span data-ttu-id="3f919-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3f919-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f919-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="3f919-112">ipAddress</span></span>|<span data-ttu-id="3f919-113">String</span><span class="sxs-lookup"><span data-stu-id="3f919-113">String</span></span>|<span data-ttu-id="3f919-114">IP-адрес назначения AirPrint.</span><span class="sxs-lookup"><span data-stu-id="3f919-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="3f919-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="3f919-115">resourcePath</span></span>|<span data-ttu-id="3f919-116">Строка</span><span class="sxs-lookup"><span data-stu-id="3f919-116">String</span></span>|<span data-ttu-id="3f919-117">Путь к ресурсу, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="3f919-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="3f919-118">Это соответствует параметру rp _ipps.tcp Bonjour записи.</span><span class="sxs-lookup"><span data-stu-id="3f919-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="3f919-119">Например: принтеры/Canon_MG5300_series, принтеры/Xerox_Phaser_7600, ipp/print Epson_IPP_Printer.</span><span class="sxs-lookup"><span data-stu-id="3f919-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="3f919-120">port</span><span class="sxs-lookup"><span data-stu-id="3f919-120">port</span></span>|<span data-ttu-id="3f919-121">Int32</span><span class="sxs-lookup"><span data-stu-id="3f919-121">Int32</span></span>|<span data-ttu-id="3f919-122">Прослушивающий порт назначения AirPrint.</span><span class="sxs-lookup"><span data-stu-id="3f919-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="3f919-123">Если этот ключ не указан AirPrint будет использовать порт по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3f919-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="3f919-124">Доступные в iOS 11.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="3f919-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="3f919-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="3f919-125">forceTls</span></span>|<span data-ttu-id="3f919-126">Логический</span><span class="sxs-lookup"><span data-stu-id="3f919-126">Boolean</span></span>|<span data-ttu-id="3f919-127">Если значение true, AirPrint подключения будут защищены по безопасности TLS (Transport Layer).</span><span class="sxs-lookup"><span data-stu-id="3f919-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="3f919-128">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="3f919-128">Default is false.</span></span> <span data-ttu-id="3f919-129">Доступные в iOS 11.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="3f919-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f919-130">Связи</span><span class="sxs-lookup"><span data-stu-id="3f919-130">Relationships</span></span>
<span data-ttu-id="3f919-131">Нет</span><span class="sxs-lookup"><span data-stu-id="3f919-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3f919-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f919-132">JSON Representation</span></span>
<span data-ttu-id="3f919-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f919-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.airPrintDestination"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.airPrintDestination",
  "ipAddress": "String",
  "resourcePath": "String",
  "port": 1024,
  "forceTls": true
}
```





