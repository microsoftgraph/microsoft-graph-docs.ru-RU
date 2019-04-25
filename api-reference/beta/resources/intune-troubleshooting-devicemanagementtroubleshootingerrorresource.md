---
title: Тип ресурса Девицеманажементтраублешутинжеррорресаурце
description: Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5905f62a1da0329db1b311ae586cdb64517a2b5d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554053"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="102f6-103">Тип ресурса Девицеманажементтраублешутинжеррорресаурце</span><span class="sxs-lookup"><span data-stu-id="102f6-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="102f6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="102f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="102f6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="102f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="102f6-106">Объект, представляющий ссылку на информацию об устранении неполадок, ссылка на портал Azure или документ Microsoft.</span><span class="sxs-lookup"><span data-stu-id="102f6-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="102f6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="102f6-107">Properties</span></span>
|<span data-ttu-id="102f6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="102f6-108">Property</span></span>|<span data-ttu-id="102f6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="102f6-109">Type</span></span>|<span data-ttu-id="102f6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="102f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="102f6-111">text</span><span class="sxs-lookup"><span data-stu-id="102f6-111">text</span></span>|<span data-ttu-id="102f6-112">String</span><span class="sxs-lookup"><span data-stu-id="102f6-112">String</span></span>|<span data-ttu-id="102f6-113">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="102f6-113">Not yet documented</span></span>|
|<span data-ttu-id="102f6-114">ссылка</span><span class="sxs-lookup"><span data-stu-id="102f6-114">link</span></span>|<span data-ttu-id="102f6-115">String</span><span class="sxs-lookup"><span data-stu-id="102f6-115">String</span></span>|<span data-ttu-id="102f6-116">Ссылка на веб-ресурс.</span><span class="sxs-lookup"><span data-stu-id="102f6-116">The link to the web resource.</span></span> <span data-ttu-id="102f6-117">Может содержать любой из следующих форматеров: {{UPN}}, {{Девицегуид}}, {{Усергуид}}</span><span class="sxs-lookup"><span data-stu-id="102f6-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="102f6-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="102f6-118">Relationships</span></span>
<span data-ttu-id="102f6-119">Нет</span><span class="sxs-lookup"><span data-stu-id="102f6-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="102f6-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="102f6-120">JSON Representation</span></span>
<span data-ttu-id="102f6-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="102f6-121">Here is a JSON representation of the resource.</span></span>
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



