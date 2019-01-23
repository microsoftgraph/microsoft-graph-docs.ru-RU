---
title: Тип ресурса airPrintDestination
description: Представляет целевой объект AirPrint.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f56578427427d45a69c4c64fe9fde3cf31f8fd9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422497"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="7c995-103">Тип ресурса airPrintDestination</span><span class="sxs-lookup"><span data-stu-id="7c995-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="7c995-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7c995-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7c995-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c995-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c995-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c995-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c995-107">Представляет целевой объект AirPrint.</span><span class="sxs-lookup"><span data-stu-id="7c995-107">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="7c995-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c995-108">Properties</span></span>
|<span data-ttu-id="7c995-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c995-109">Property</span></span>|<span data-ttu-id="7c995-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7c995-110">Type</span></span>|<span data-ttu-id="7c995-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7c995-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c995-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="7c995-112">ipAddress</span></span>|<span data-ttu-id="7c995-113">String</span><span class="sxs-lookup"><span data-stu-id="7c995-113">String</span></span>|<span data-ttu-id="7c995-114">IP-адрес назначения AirPrint.</span><span class="sxs-lookup"><span data-stu-id="7c995-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="7c995-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="7c995-115">resourcePath</span></span>|<span data-ttu-id="7c995-116">String</span><span class="sxs-lookup"><span data-stu-id="7c995-116">String</span></span>|<span data-ttu-id="7c995-117">Путь к ресурсу, связанных с принтером.</span><span class="sxs-lookup"><span data-stu-id="7c995-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="7c995-118">Это соответствует параметру rp _ipps.tcp Bonjour записи.</span><span class="sxs-lookup"><span data-stu-id="7c995-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="7c995-119">Например: принтеры/Canon_MG5300_series, принтеры/Xerox_Phaser_7600, ipp/print Epson_IPP_Printer.</span><span class="sxs-lookup"><span data-stu-id="7c995-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="7c995-120">port</span><span class="sxs-lookup"><span data-stu-id="7c995-120">port</span></span>|<span data-ttu-id="7c995-121">Int32</span><span class="sxs-lookup"><span data-stu-id="7c995-121">Int32</span></span>|<span data-ttu-id="7c995-122">Прослушивающий порт назначения AirPrint.</span><span class="sxs-lookup"><span data-stu-id="7c995-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="7c995-123">Если этот ключ не указан AirPrint будет использовать порт по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7c995-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="7c995-124">Доступные в iOS 11.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="7c995-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="7c995-125">forceTls</span><span class="sxs-lookup"><span data-stu-id="7c995-125">forceTls</span></span>|<span data-ttu-id="7c995-126">Логический</span><span class="sxs-lookup"><span data-stu-id="7c995-126">Boolean</span></span>|<span data-ttu-id="7c995-127">Если значение true, AirPrint подключения будут защищены по безопасности TLS (Transport Layer).</span><span class="sxs-lookup"><span data-stu-id="7c995-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="7c995-128">Значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="7c995-128">Default is false.</span></span> <span data-ttu-id="7c995-129">Доступные в iOS 11.0 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="7c995-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c995-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="7c995-130">Relationships</span></span>
<span data-ttu-id="7c995-131">Нет</span><span class="sxs-lookup"><span data-stu-id="7c995-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c995-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c995-132">JSON Representation</span></span>
<span data-ttu-id="7c995-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c995-133">Here is a JSON representation of the resource.</span></span>
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




