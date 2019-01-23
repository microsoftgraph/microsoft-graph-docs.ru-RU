---
title: Тип ресурса iPv4Range
description: Описание ресурсов iPv4Range из Microsoft Graph API для Intune, которая поддерживает несколько рабочих процессов.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9ac2656b7c79cceba70879fe478aec65a5bd7250
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425227"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="ea4c2-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="ea4c2-103">iPv4Range resource type</span></span>

> <span data-ttu-id="ea4c2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ea4c2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea4c2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea4c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea4c2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ea4c2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea4c2-107">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="ea4c2-107">IP V4 range</span></span>

<span data-ttu-id="ea4c2-108">Наследуется от [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="ea4c2-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea4c2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea4c2-109">Properties</span></span>
|<span data-ttu-id="ea4c2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea4c2-110">Property</span></span>|<span data-ttu-id="ea4c2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ea4c2-111">Type</span></span>|<span data-ttu-id="ea4c2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ea4c2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea4c2-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="ea4c2-113">lowerAddress</span></span>|<span data-ttu-id="ea4c2-114">String</span><span class="sxs-lookup"><span data-stu-id="ea4c2-114">String</span></span>|<span data-ttu-id="ea4c2-115">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="ea4c2-115">Lower IP Address</span></span>|
|<span data-ttu-id="ea4c2-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="ea4c2-116">upperAddress</span></span>|<span data-ttu-id="ea4c2-117">String</span><span class="sxs-lookup"><span data-stu-id="ea4c2-117">String</span></span>|<span data-ttu-id="ea4c2-118">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="ea4c2-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea4c2-119">Связи</span><span class="sxs-lookup"><span data-stu-id="ea4c2-119">Relationships</span></span>
<span data-ttu-id="ea4c2-120">Нет</span><span class="sxs-lookup"><span data-stu-id="ea4c2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea4c2-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea4c2-121">JSON Representation</span></span>
<span data-ttu-id="ea4c2-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea4c2-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



