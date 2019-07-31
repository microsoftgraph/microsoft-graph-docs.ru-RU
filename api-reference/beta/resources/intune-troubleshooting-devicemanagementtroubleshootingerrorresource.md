---
title: Тип ресурса Девицеманажементтраублешутинжеррорресаурце
description: Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6454bad98938bc73d4cde8d48229f6146d07c0bb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010310"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="7b9d4-103">Тип ресурса Девицеманажементтраублешутинжеррорресаурце</span><span class="sxs-lookup"><span data-stu-id="7b9d4-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="7b9d4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b9d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b9d4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b9d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b9d4-106">Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7b9d4-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="7b9d4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b9d4-107">Properties</span></span>
|<span data-ttu-id="7b9d4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b9d4-108">Property</span></span>|<span data-ttu-id="7b9d4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7b9d4-109">Type</span></span>|<span data-ttu-id="7b9d4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7b9d4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b9d4-111">text</span><span class="sxs-lookup"><span data-stu-id="7b9d4-111">text</span></span>|<span data-ttu-id="7b9d4-112">String</span><span class="sxs-lookup"><span data-stu-id="7b9d4-112">String</span></span>|<span data-ttu-id="7b9d4-113">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="7b9d4-113">Not yet documented</span></span>|
|<span data-ttu-id="7b9d4-114">ссылка</span><span class="sxs-lookup"><span data-stu-id="7b9d4-114">link</span></span>|<span data-ttu-id="7b9d4-115">String</span><span class="sxs-lookup"><span data-stu-id="7b9d4-115">String</span></span>|<span data-ttu-id="7b9d4-116">Ссылка на веб-ресурс.</span><span class="sxs-lookup"><span data-stu-id="7b9d4-116">The link to the web resource.</span></span> <span data-ttu-id="7b9d4-117">Может содержать любой из следующих форматеров: {{UPN}}, {{Девицегуид}}, {{Усергуид}}</span><span class="sxs-lookup"><span data-stu-id="7b9d4-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b9d4-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="7b9d4-118">Relationships</span></span>
<span data-ttu-id="7b9d4-119">Нет</span><span class="sxs-lookup"><span data-stu-id="7b9d4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b9d4-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b9d4-120">JSON Representation</span></span>
<span data-ttu-id="7b9d4-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b9d4-121">Here is a JSON representation of the resource.</span></span>
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





