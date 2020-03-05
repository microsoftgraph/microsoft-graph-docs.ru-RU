---
title: Тип ресурса Аирпринтдестинатион
description: Представляет целевой объект Аирпринт.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 99693cbdfa77895e0116ac5228fdf58d95afeacb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42487363"
---
# <a name="airprintdestination-resource-type"></a><span data-ttu-id="73b18-103">Тип ресурса Аирпринтдестинатион</span><span class="sxs-lookup"><span data-stu-id="73b18-103">airPrintDestination resource type</span></span>

<span data-ttu-id="73b18-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="73b18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73b18-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="73b18-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73b18-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="73b18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73b18-107">Представляет целевой объект Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="73b18-107">Represents an AirPrint destination.</span></span>

## <a name="properties"></a><span data-ttu-id="73b18-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="73b18-108">Properties</span></span>
|<span data-ttu-id="73b18-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="73b18-109">Property</span></span>|<span data-ttu-id="73b18-110">Тип</span><span class="sxs-lookup"><span data-stu-id="73b18-110">Type</span></span>|<span data-ttu-id="73b18-111">Описание</span><span class="sxs-lookup"><span data-stu-id="73b18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73b18-112">ipAddress</span><span class="sxs-lookup"><span data-stu-id="73b18-112">ipAddress</span></span>|<span data-ttu-id="73b18-113">String</span><span class="sxs-lookup"><span data-stu-id="73b18-113">String</span></span>|<span data-ttu-id="73b18-114">IP-адрес назначения Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="73b18-114">The IP Address of the AirPrint destination.</span></span>|
|<span data-ttu-id="73b18-115">resourcePath</span><span class="sxs-lookup"><span data-stu-id="73b18-115">resourcePath</span></span>|<span data-ttu-id="73b18-116">String</span><span class="sxs-lookup"><span data-stu-id="73b18-116">String</span></span>|<span data-ttu-id="73b18-117">Путь к ресурсу, связанный с принтером.</span><span class="sxs-lookup"><span data-stu-id="73b18-117">The Resource Path associated with the printer.</span></span> <span data-ttu-id="73b18-118">Соответствует _ipps параметру RP записи Бонжаур. TCP.</span><span class="sxs-lookup"><span data-stu-id="73b18-118">This corresponds to the rp parameter of the _ipps.tcp Bonjour record.</span></span> <span data-ttu-id="73b18-119">Например: Printers/Canon_MG5300_series, Printers/Xerox_Phaser_7600, IPP/Print, Epson_IPP_Printer.</span><span class="sxs-lookup"><span data-stu-id="73b18-119">For example: printers/Canon_MG5300_series, printers/Xerox_Phaser_7600, ipp/print, Epson_IPP_Printer.</span></span>|
|<span data-ttu-id="73b18-120">порта</span><span class="sxs-lookup"><span data-stu-id="73b18-120">port</span></span>|<span data-ttu-id="73b18-121">Int32</span><span class="sxs-lookup"><span data-stu-id="73b18-121">Int32</span></span>|<span data-ttu-id="73b18-122">Прослушивающий порт назначения Аирпринт.</span><span class="sxs-lookup"><span data-stu-id="73b18-122">The listening port of the AirPrint destination.</span></span> <span data-ttu-id="73b18-123">Если этот ключ не указан, Аирпринт будет использовать порт по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="73b18-123">If this key is not specified AirPrint will use the default port.</span></span> <span data-ttu-id="73b18-124">Доступно в iOS 11,0 и более поздних версиях.</span><span class="sxs-lookup"><span data-stu-id="73b18-124">Available in iOS 11.0 and later.</span></span>|
|<span data-ttu-id="73b18-125">форцетлс</span><span class="sxs-lookup"><span data-stu-id="73b18-125">forceTls</span></span>|<span data-ttu-id="73b18-126">Логический</span><span class="sxs-lookup"><span data-stu-id="73b18-126">Boolean</span></span>|<span data-ttu-id="73b18-127">Если задано значение true, подключения Аирпринт защищены с помощью протокола TLS.</span><span class="sxs-lookup"><span data-stu-id="73b18-127">If true AirPrint connections are secured by Transport Layer Security (TLS).</span></span> <span data-ttu-id="73b18-128">Значение по умолчанию: false.</span><span class="sxs-lookup"><span data-stu-id="73b18-128">Default is false.</span></span> <span data-ttu-id="73b18-129">Доступно в iOS 11,0 и более поздних версиях.</span><span class="sxs-lookup"><span data-stu-id="73b18-129">Available in iOS 11.0 and later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73b18-130">Связи</span><span class="sxs-lookup"><span data-stu-id="73b18-130">Relationships</span></span>
<span data-ttu-id="73b18-131">Нет</span><span class="sxs-lookup"><span data-stu-id="73b18-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73b18-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="73b18-132">JSON Representation</span></span>
<span data-ttu-id="73b18-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="73b18-133">Here is a JSON representation of the resource.</span></span>
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



