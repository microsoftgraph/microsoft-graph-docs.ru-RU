---
title: Тип ресурса Девицеманажементтраублешутинжеррорресаурце
description: Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5c0507a793585818e709ccbbb02cb93743e7502d
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42765673"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="588cc-103">Тип ресурса Девицеманажементтраублешутинжеррорресаурце</span><span class="sxs-lookup"><span data-stu-id="588cc-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="588cc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="588cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="588cc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="588cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="588cc-106">Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.</span><span class="sxs-lookup"><span data-stu-id="588cc-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="588cc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="588cc-107">Properties</span></span>
|<span data-ttu-id="588cc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="588cc-108">Property</span></span>|<span data-ttu-id="588cc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="588cc-109">Type</span></span>|<span data-ttu-id="588cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="588cc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="588cc-111">text</span><span class="sxs-lookup"><span data-stu-id="588cc-111">text</span></span>|<span data-ttu-id="588cc-112">String</span><span class="sxs-lookup"><span data-stu-id="588cc-112">String</span></span>|<span data-ttu-id="588cc-113">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="588cc-113">Not yet documented</span></span>|
|<span data-ttu-id="588cc-114">ссылка</span><span class="sxs-lookup"><span data-stu-id="588cc-114">link</span></span>|<span data-ttu-id="588cc-115">String</span><span class="sxs-lookup"><span data-stu-id="588cc-115">String</span></span>|<span data-ttu-id="588cc-116">Ссылка на веб-ресурс.</span><span class="sxs-lookup"><span data-stu-id="588cc-116">The link to the web resource.</span></span> <span data-ttu-id="588cc-117">Может содержать любой из следующих форматеров: {{UPN}}, {{Девицегуид}}, {{Усергуид}}</span><span class="sxs-lookup"><span data-stu-id="588cc-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="588cc-118">Связи</span><span class="sxs-lookup"><span data-stu-id="588cc-118">Relationships</span></span>
<span data-ttu-id="588cc-119">Нет</span><span class="sxs-lookup"><span data-stu-id="588cc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="588cc-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="588cc-120">JSON Representation</span></span>
<span data-ttu-id="588cc-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="588cc-121">Here is a JSON representation of the resource.</span></span>
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



