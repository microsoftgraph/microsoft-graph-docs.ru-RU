---
title: Тип ресурса Девицеманажементтраублешутинжеррорресаурце
description: Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60a098774f8302ec23322fc18af1998ba6e14480
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388246"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="132be-103">Тип ресурса Девицеманажементтраублешутинжеррорресаурце</span><span class="sxs-lookup"><span data-stu-id="132be-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

<span data-ttu-id="132be-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="132be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="132be-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="132be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="132be-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="132be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="132be-107">Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.</span><span class="sxs-lookup"><span data-stu-id="132be-107">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="132be-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="132be-108">Properties</span></span>
|<span data-ttu-id="132be-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="132be-109">Property</span></span>|<span data-ttu-id="132be-110">Тип</span><span class="sxs-lookup"><span data-stu-id="132be-110">Type</span></span>|<span data-ttu-id="132be-111">Описание</span><span class="sxs-lookup"><span data-stu-id="132be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="132be-112">text</span><span class="sxs-lookup"><span data-stu-id="132be-112">text</span></span>|<span data-ttu-id="132be-113">String</span><span class="sxs-lookup"><span data-stu-id="132be-113">String</span></span>|<span data-ttu-id="132be-114">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="132be-114">Not yet documented</span></span>|
|<span data-ttu-id="132be-115">ссылка</span><span class="sxs-lookup"><span data-stu-id="132be-115">link</span></span>|<span data-ttu-id="132be-116">String</span><span class="sxs-lookup"><span data-stu-id="132be-116">String</span></span>|<span data-ttu-id="132be-117">Ссылка на веб-ресурс.</span><span class="sxs-lookup"><span data-stu-id="132be-117">The link to the web resource.</span></span> <span data-ttu-id="132be-118">Может содержать любой из следующих форматеров: {{UPN}}, {{Девицегуид}}, {{Усергуид}}</span><span class="sxs-lookup"><span data-stu-id="132be-118">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="132be-119">Связи</span><span class="sxs-lookup"><span data-stu-id="132be-119">Relationships</span></span>
<span data-ttu-id="132be-120">Нет</span><span class="sxs-lookup"><span data-stu-id="132be-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="132be-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="132be-121">JSON Representation</span></span>
<span data-ttu-id="132be-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="132be-122">Here is a JSON representation of the resource.</span></span>
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



