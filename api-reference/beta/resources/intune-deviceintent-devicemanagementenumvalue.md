---
title: Тип ресурса Девицеманажементенумвалуе
description: Сведения об определении значения перечисления
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ade5c3c10354d8697ca40f553c0941751cd26c1a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366625"
---
# <a name="devicemanagementenumvalue-resource-type"></a><span data-ttu-id="b2894-103">Тип ресурса Девицеманажементенумвалуе</span><span class="sxs-lookup"><span data-stu-id="b2894-103">deviceManagementEnumValue resource type</span></span>

> <span data-ttu-id="b2894-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2894-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2894-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2894-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2894-106">Сведения об определении значения перечисления</span><span class="sxs-lookup"><span data-stu-id="b2894-106">Definition information for an enum value</span></span>

## <a name="properties"></a><span data-ttu-id="b2894-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2894-107">Properties</span></span>
|<span data-ttu-id="b2894-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2894-108">Property</span></span>|<span data-ttu-id="b2894-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b2894-109">Type</span></span>|<span data-ttu-id="b2894-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b2894-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2894-111">значение</span><span class="sxs-lookup"><span data-stu-id="b2894-111">value</span></span>|<span data-ttu-id="b2894-112">String</span><span class="sxs-lookup"><span data-stu-id="b2894-112">String</span></span>|<span data-ttu-id="b2894-113">Необработанный текст значения перечисления</span><span class="sxs-lookup"><span data-stu-id="b2894-113">The raw enum value text</span></span>|
|<span data-ttu-id="b2894-114">displayName</span><span class="sxs-lookup"><span data-stu-id="b2894-114">displayName</span></span>|<span data-ttu-id="b2894-115">String</span><span class="sxs-lookup"><span data-stu-id="b2894-115">String</span></span>|<span data-ttu-id="b2894-116">Отображаемое имя для этого значения перечисления</span><span class="sxs-lookup"><span data-stu-id="b2894-116">Display name for this enum value</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2894-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="b2894-117">Relationships</span></span>
<span data-ttu-id="b2894-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b2894-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2894-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2894-119">JSON Representation</span></span>
<span data-ttu-id="b2894-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2894-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumValue",
  "value": "String",
  "displayName": "String"
}
```



