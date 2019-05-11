---
title: Тип ресурса Девицеманажементтраублешутинжеррорресаурце
description: Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 712832420b556517be8ef053cc6cd292acfeed86
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939863"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="d3a22-103">Тип ресурса Девицеманажементтраублешутинжеррорресаурце</span><span class="sxs-lookup"><span data-stu-id="d3a22-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="d3a22-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3a22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3a22-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3a22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3a22-106">Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d3a22-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="d3a22-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3a22-107">Properties</span></span>
|<span data-ttu-id="d3a22-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3a22-108">Property</span></span>|<span data-ttu-id="d3a22-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d3a22-109">Type</span></span>|<span data-ttu-id="d3a22-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d3a22-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3a22-111">text</span><span class="sxs-lookup"><span data-stu-id="d3a22-111">text</span></span>|<span data-ttu-id="d3a22-112">String</span><span class="sxs-lookup"><span data-stu-id="d3a22-112">String</span></span>|<span data-ttu-id="d3a22-113">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="d3a22-113">Not yet documented</span></span>|
|<span data-ttu-id="d3a22-114">ссылка</span><span class="sxs-lookup"><span data-stu-id="d3a22-114">link</span></span>|<span data-ttu-id="d3a22-115">Строка</span><span class="sxs-lookup"><span data-stu-id="d3a22-115">String</span></span>|<span data-ttu-id="d3a22-116">Ссылка на веб-ресурс.</span><span class="sxs-lookup"><span data-stu-id="d3a22-116">The link to the web resource.</span></span> <span data-ttu-id="d3a22-117">Может содержать любой из следующих форматеров: {{UPN}}, {{Девицегуид}}, {{Усергуид}}</span><span class="sxs-lookup"><span data-stu-id="d3a22-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3a22-118">Связи</span><span class="sxs-lookup"><span data-stu-id="d3a22-118">Relationships</span></span>
<span data-ttu-id="d3a22-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d3a22-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3a22-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3a22-120">JSON Representation</span></span>
<span data-ttu-id="d3a22-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3a22-121">Here is a JSON representation of the resource.</span></span>
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




