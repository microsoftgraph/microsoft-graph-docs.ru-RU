---
title: Тип ресурса Девицеманажементтраублешутинжеррорресаурце
description: Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eaf3cc39efb52bb7f603c636a69d13e3d025ce5f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347740"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="1aba9-103">Тип ресурса Девицеманажементтраублешутинжеррорресаурце</span><span class="sxs-lookup"><span data-stu-id="1aba9-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="1aba9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1aba9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1aba9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1aba9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aba9-106">Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1aba9-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="1aba9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1aba9-107">Properties</span></span>
|<span data-ttu-id="1aba9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1aba9-108">Property</span></span>|<span data-ttu-id="1aba9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1aba9-109">Type</span></span>|<span data-ttu-id="1aba9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1aba9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aba9-111">text</span><span class="sxs-lookup"><span data-stu-id="1aba9-111">text</span></span>|<span data-ttu-id="1aba9-112">String</span><span class="sxs-lookup"><span data-stu-id="1aba9-112">String</span></span>|<span data-ttu-id="1aba9-113">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="1aba9-113">Not yet documented</span></span>|
|<span data-ttu-id="1aba9-114">ссылка</span><span class="sxs-lookup"><span data-stu-id="1aba9-114">link</span></span>|<span data-ttu-id="1aba9-115">String</span><span class="sxs-lookup"><span data-stu-id="1aba9-115">String</span></span>|<span data-ttu-id="1aba9-116">Ссылка на веб-ресурс.</span><span class="sxs-lookup"><span data-stu-id="1aba9-116">The link to the web resource.</span></span> <span data-ttu-id="1aba9-117">Может содержать любой из следующих форматеров: {{UPN}}, {{Девицегуид}}, {{Усергуид}}</span><span class="sxs-lookup"><span data-stu-id="1aba9-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aba9-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="1aba9-118">Relationships</span></span>
<span data-ttu-id="1aba9-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1aba9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1aba9-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1aba9-120">JSON Representation</span></span>
<span data-ttu-id="1aba9-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1aba9-121">Here is a JSON representation of the resource.</span></span>
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



