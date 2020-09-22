---
title: Тип ресурса Аирпринтдестинатион
description: Представляет целевой объект Аирпринт.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84575b172dee1f07d114abb202b3868ab936ce9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076185"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="8bca2-103">Тип ресурса Аирпринтдестинатион</span><span class="sxs-lookup"><span data-stu-id="8bca2-103">airPrintDestination resource type</span></span>

<span data-ttu-id="8bca2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bca2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8bca2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bca2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bca2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bca2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bca2-107">Представляет целевой объект Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="8bca2-107">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="8bca2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bca2-108">Properties</span></span>
|<span data-ttu-id="8bca2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bca2-109">Property</span></span>|<span data-ttu-id="8bca2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8bca2-110">Type</span></span>|<span data-ttu-id="8bca2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8bca2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bca2-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="8bca2-112">ipAddress</span></span>|<span data-ttu-id="8bca2-113">String</span><span class="sxs-lookup"><span data-stu-id="8bca2-113">String</span></span>|<span data-ttu-id="8bca2-114">IP-адрес назначения Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="8bca2-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="8bca2-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="8bca2-115">resourcePath</span></span>|<span data-ttu-id="8bca2-116">String</span><span class="sxs-lookup"><span data-stu-id="8bca2-116">String</span></span>|<span data-ttu-id="8bca2-117">Путь к ресурсу, связанный с принтером.</span><span class="sxs-lookup"><span data-stu-id="8bca2-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="8bca2-118">Соответствует _ipps параметру RP записи Бонжаур. TCP.</span><span class="sxs-lookup"><span data-stu-id="8bca2-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="8bca2-119">Например: Printers/Canon_MG5300_series, Printers/Xerox_Phaser_7600, IPP/Print, Epson_IPP_Printer.</span><span class="sxs-lookup"><span data-stu-id="8bca2-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="8bca2-120">порта</span><span class="sxs-lookup"><span data-stu-id="8bca2-120">port</span></span>|<span data-ttu-id="8bca2-121">Int32</span><span class="sxs-lookup"><span data-stu-id="8bca2-121">Int32</span></span>|<span data-ttu-id="8bca2-122">Прослушивающий порт назначения Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="8bca2-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="8bca2-123">Если этот ключ не указан, Аирпринт будет использовать порт по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8bca2-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="8bca2-124">Доступно в iOS 11,0 и более поздних версиях.</span><span class="sxs-lookup"><span data-stu-id="8bca2-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="8bca2-125">форцетлс</span><span class="sxs-lookup"><span data-stu-id="8bca2-125">forceTls</span></span>|<span data-ttu-id="8bca2-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bca2-126">Boolean</span></span>|<span data-ttu-id="8bca2-127">Если задано значение true, подключения Аирпринт защищены с помощью протокола TLS.</span><span class="sxs-lookup"><span data-stu-id="8bca2-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="8bca2-128">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="8bca2-128">Default is false.</span></span> <span data-ttu-id="8bca2-129">Доступно в iOS 11,0 и более поздних версиях.</span><span class="sxs-lookup"><span data-stu-id="8bca2-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bca2-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="8bca2-130">Relationships</span></span>
<span data-ttu-id="8bca2-131">Нет</span><span class="sxs-lookup"><span data-stu-id="8bca2-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bca2-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bca2-132">JSON Representation</span></span>
<span data-ttu-id="8bca2-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bca2-133">Here is a JSON representation of the resource.</span></span>
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






