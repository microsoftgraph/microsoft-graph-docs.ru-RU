---
title: Тип ресурса win32LobAppProductCodeDetection
description: Содержит код продукта и свойства версии для обнаружения приложения Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 854d54b034b0e2e0dc0e7ce8e7f73466f37dd263
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173236"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="4475d-103">Тип ресурса win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="4475d-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="4475d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4475d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4475d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4475d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4475d-106">Содержит код продукта и свойства версии для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="4475d-106">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="4475d-107">НаСледуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="4475d-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4475d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4475d-108">Properties</span></span>
|<span data-ttu-id="4475d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4475d-109">Property</span></span>|<span data-ttu-id="4475d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4475d-110">Type</span></span>|<span data-ttu-id="4475d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4475d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4475d-112">productCode</span><span class="sxs-lookup"><span data-stu-id="4475d-112">productCode</span></span>|<span data-ttu-id="4475d-113">String</span><span class="sxs-lookup"><span data-stu-id="4475d-113">String</span></span>|<span data-ttu-id="4475d-114">Код продукта для бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="4475d-114">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4475d-115">Продуктверсионоператор</span><span class="sxs-lookup"><span data-stu-id="4475d-115">productVersionOperator</span></span>|[<span data-ttu-id="4475d-116">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="4475d-116">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="4475d-117">Оператор для определения версии продукта.</span><span class="sxs-lookup"><span data-stu-id="4475d-117">The operator to detect product version.</span></span> <span data-ttu-id="4475d-118">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="4475d-118">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="4475d-119">productVersion</span><span class="sxs-lookup"><span data-stu-id="4475d-119">productVersion</span></span>|<span data-ttu-id="4475d-120">String</span><span class="sxs-lookup"><span data-stu-id="4475d-120">String</span></span>|<span data-ttu-id="4475d-121">Версия приложения, на котором установлен продукт Win32 бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="4475d-121">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4475d-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="4475d-122">Relationships</span></span>
<span data-ttu-id="4475d-123">Нет</span><span class="sxs-lookup"><span data-stu-id="4475d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4475d-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4475d-124">JSON Representation</span></span>
<span data-ttu-id="4475d-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4475d-125">Here is a JSON representation of the resource.</span></span>
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




