---
title: Тип ресурса Аирпринтдестинатион
description: Представляет целевой объект Аирпринт.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b0f77b9f0ee3ff3abe46a41b0c6760a15d7aa2c1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797208"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="579a7-103">Тип ресурса Аирпринтдестинатион</span><span class="sxs-lookup"><span data-stu-id="579a7-103">airPrintDestination resource type</span></span>

> <span data-ttu-id="579a7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="579a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="579a7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="579a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="579a7-106">Представляет целевой объект Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="579a7-106">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="579a7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="579a7-107">Properties</span></span>
|<span data-ttu-id="579a7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="579a7-108">Property</span></span>|<span data-ttu-id="579a7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="579a7-109">Type</span></span>|<span data-ttu-id="579a7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="579a7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="579a7-111">ipAddress</span><span class="sxs-lookup"><span data-stu-id="579a7-111">ipAddress</span></span>|<span data-ttu-id="579a7-112">String</span><span class="sxs-lookup"><span data-stu-id="579a7-112">String</span></span>|<span data-ttu-id="579a7-113">IP-адрес назначения Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="579a7-113">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="579a7-114">resourcePath</span><span class="sxs-lookup"><span data-stu-id="579a7-114">resourcePath</span></span>|<span data-ttu-id="579a7-115">String</span><span class="sxs-lookup"><span data-stu-id="579a7-115">String</span></span>|<span data-ttu-id="579a7-116">Путь к ресурсу, связанный с принтером.</span><span class="sxs-lookup"><span data-stu-id="579a7-116">The Resource Path associated with the printer.</span></span> <span data-ttu-id="579a7-117">Соответствует _ipps параметру RP записи Бонжаур. TCP.</span><span class="sxs-lookup"><span data-stu-id="579a7-117">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="579a7-118">Например: Printers/Canon_MG5300_series, Printers/Xerox_Phaser_7600, IPP/Print, Epson_IPP_Printer.</span><span class="sxs-lookup"><span data-stu-id="579a7-118">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="579a7-119">порта</span><span class="sxs-lookup"><span data-stu-id="579a7-119">port</span></span>|<span data-ttu-id="579a7-120">Int32</span><span class="sxs-lookup"><span data-stu-id="579a7-120">Int32</span></span>|<span data-ttu-id="579a7-121">Прослушивающий порт назначения Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="579a7-121">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="579a7-122">Если этот ключ не указан, Аирпринт будет использовать порт по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="579a7-122">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="579a7-123">Доступно в iOS 11,0 и более поздних версиях.</span><span class="sxs-lookup"><span data-stu-id="579a7-123">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="579a7-124">форцетлс</span><span class="sxs-lookup"><span data-stu-id="579a7-124">forceTls</span></span>|<span data-ttu-id="579a7-125">Логический</span><span class="sxs-lookup"><span data-stu-id="579a7-125">Boolean</span></span>|<span data-ttu-id="579a7-126">Если задано значение true, подключения Аирпринт защищены с помощью протокола TLS.</span><span class="sxs-lookup"><span data-stu-id="579a7-126">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="579a7-127">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="579a7-127">Default is false.</span></span> <span data-ttu-id="579a7-128">Доступно в iOS 11,0 и более поздних версиях.</span><span class="sxs-lookup"><span data-stu-id="579a7-128">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="579a7-129">Связи</span><span class="sxs-lookup"><span data-stu-id="579a7-129">Relationships</span></span>
<span data-ttu-id="579a7-130">Нет</span><span class="sxs-lookup"><span data-stu-id="579a7-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="579a7-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="579a7-131">JSON Representation</span></span>
<span data-ttu-id="579a7-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="579a7-132">Here is a JSON representation of the resource.</span></span>
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



