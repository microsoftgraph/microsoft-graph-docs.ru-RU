---
title: Тип ресурса win32LobAppProductCodeDetection
description: Содержит код продукта и свойства версии для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 33a27e35843c3bda7a2e5ef5560f6b5487948d6a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692578"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="003bd-103">Тип ресурса win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="003bd-103">win32LobAppProductCodeDetection resource type</span></span>

<span data-ttu-id="003bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="003bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="003bd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="003bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="003bd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="003bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="003bd-107">Содержит код продукта и свойства версии для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="003bd-107">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="003bd-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="003bd-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="003bd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="003bd-109">Properties</span></span>
|<span data-ttu-id="003bd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="003bd-110">Property</span></span>|<span data-ttu-id="003bd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="003bd-111">Type</span></span>|<span data-ttu-id="003bd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="003bd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="003bd-113">productCode</span><span class="sxs-lookup"><span data-stu-id="003bd-113">productCode</span></span>|<span data-ttu-id="003bd-114">String</span><span class="sxs-lookup"><span data-stu-id="003bd-114">String</span></span>|<span data-ttu-id="003bd-115">Код продукта для бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="003bd-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="003bd-116">продуктверсионоператор</span><span class="sxs-lookup"><span data-stu-id="003bd-116">productVersionOperator</span></span>|[<span data-ttu-id="003bd-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="003bd-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="003bd-118">Оператор для определения версии продукта.</span><span class="sxs-lookup"><span data-stu-id="003bd-118">The operator to detect product version.</span></span> <span data-ttu-id="003bd-119">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="003bd-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="003bd-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="003bd-120">productVersion</span></span>|<span data-ttu-id="003bd-121">String</span><span class="sxs-lookup"><span data-stu-id="003bd-121">String</span></span>|<span data-ttu-id="003bd-122">Версия приложения, на котором установлен продукт Win32 бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="003bd-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="003bd-123">Связи</span><span class="sxs-lookup"><span data-stu-id="003bd-123">Relationships</span></span>
<span data-ttu-id="003bd-124">Нет</span><span class="sxs-lookup"><span data-stu-id="003bd-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="003bd-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="003bd-125">JSON Representation</span></span>
<span data-ttu-id="003bd-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="003bd-126">Here is a JSON representation of the resource.</span></span>
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





