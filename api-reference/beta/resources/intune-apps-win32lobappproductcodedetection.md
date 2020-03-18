---
title: Тип ресурса win32LobAppProductCodeDetection
description: Содержит код продукта и свойства версии для обнаружения приложения Win32
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 98d510d2a42666924adbdb9c2a2e05d9f3b60762
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797593"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="7804a-103">Тип ресурса win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="7804a-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="7804a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7804a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7804a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7804a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7804a-106">Содержит код продукта и свойства версии для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="7804a-106">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="7804a-107">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="7804a-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7804a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7804a-108">Properties</span></span>
|<span data-ttu-id="7804a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7804a-109">Property</span></span>|<span data-ttu-id="7804a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7804a-110">Type</span></span>|<span data-ttu-id="7804a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7804a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7804a-112">productCode</span><span class="sxs-lookup"><span data-stu-id="7804a-112">productCode</span></span>|<span data-ttu-id="7804a-113">String</span><span class="sxs-lookup"><span data-stu-id="7804a-113">String</span></span>|<span data-ttu-id="7804a-114">Код продукта для бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="7804a-114">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7804a-115">продуктверсионоператор</span><span class="sxs-lookup"><span data-stu-id="7804a-115">productVersionOperator</span></span>|[<span data-ttu-id="7804a-116">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="7804a-116">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="7804a-117">Оператор для определения версии продукта.</span><span class="sxs-lookup"><span data-stu-id="7804a-117">The operator to detect product version.</span></span> <span data-ttu-id="7804a-118">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="7804a-118">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="7804a-119">productVersion</span><span class="sxs-lookup"><span data-stu-id="7804a-119">productVersion</span></span>|<span data-ttu-id="7804a-120">String</span><span class="sxs-lookup"><span data-stu-id="7804a-120">String</span></span>|<span data-ttu-id="7804a-121">Версия приложения, на котором установлен продукт Win32 бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="7804a-121">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7804a-122">Связи</span><span class="sxs-lookup"><span data-stu-id="7804a-122">Relationships</span></span>
<span data-ttu-id="7804a-123">Нет</span><span class="sxs-lookup"><span data-stu-id="7804a-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7804a-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7804a-124">JSON Representation</span></span>
<span data-ttu-id="7804a-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7804a-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeDetection",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```



