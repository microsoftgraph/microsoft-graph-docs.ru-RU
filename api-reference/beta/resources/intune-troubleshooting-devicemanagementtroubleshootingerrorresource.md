---
title: Тип ресурса Девицеманажементтраублешутинжеррорресаурце
description: Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 18537e1fa81fd082cc7fd78d2675540535195a32
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075786"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="dc4aa-103">Тип ресурса Девицеманажементтраублешутинжеррорресаурце</span><span class="sxs-lookup"><span data-stu-id="dc4aa-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

<span data-ttu-id="dc4aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc4aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc4aa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc4aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc4aa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc4aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc4aa-107">Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.</span><span class="sxs-lookup"><span data-stu-id="dc4aa-107">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="dc4aa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc4aa-108">Properties</span></span>
|<span data-ttu-id="dc4aa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc4aa-109">Property</span></span>|<span data-ttu-id="dc4aa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dc4aa-110">Type</span></span>|<span data-ttu-id="dc4aa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dc4aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc4aa-112">text</span><span class="sxs-lookup"><span data-stu-id="dc4aa-112">text</span></span>|<span data-ttu-id="dc4aa-113">String</span><span class="sxs-lookup"><span data-stu-id="dc4aa-113">String</span></span>|<span data-ttu-id="dc4aa-114">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="dc4aa-114">Not yet documented</span></span>|
|<span data-ttu-id="dc4aa-115">ссылка</span><span class="sxs-lookup"><span data-stu-id="dc4aa-115">link</span></span>|<span data-ttu-id="dc4aa-116">String</span><span class="sxs-lookup"><span data-stu-id="dc4aa-116">String</span></span>|<span data-ttu-id="dc4aa-117">Ссылка на веб-ресурс.</span><span class="sxs-lookup"><span data-stu-id="dc4aa-117">The link to the web resource.</span></span> <span data-ttu-id="dc4aa-118">Может содержать любой из следующих форматеров: {{UPN}}, {{Девицегуид}}, {{Усергуид}}</span><span class="sxs-lookup"><span data-stu-id="dc4aa-118">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc4aa-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="dc4aa-119">Relationships</span></span>
<span data-ttu-id="dc4aa-120">Нет</span><span class="sxs-lookup"><span data-stu-id="dc4aa-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc4aa-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc4aa-121">JSON Representation</span></span>
<span data-ttu-id="dc4aa-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc4aa-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```






