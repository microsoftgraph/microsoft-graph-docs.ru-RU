---
title: Тип ресурса win32LobAppProductCodeDetection
description: Содержит свойства кода и версия продукта для обнаружения приложений Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f5af1cfc5fffe5241ef3b7883c3ebe6a2100278
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411206"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="35731-103">Тип ресурса win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="35731-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="35731-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35731-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="35731-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35731-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35731-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35731-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35731-107">Содержит свойства кода и версия продукта для обнаружения приложений Win32</span><span class="sxs-lookup"><span data-stu-id="35731-107">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="35731-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="35731-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="35731-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="35731-109">Properties</span></span>
|<span data-ttu-id="35731-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="35731-110">Property</span></span>|<span data-ttu-id="35731-111">Тип</span><span class="sxs-lookup"><span data-stu-id="35731-111">Type</span></span>|<span data-ttu-id="35731-112">Описание</span><span class="sxs-lookup"><span data-stu-id="35731-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35731-113">productCode</span><span class="sxs-lookup"><span data-stu-id="35731-113">productCode</span></span>|<span data-ttu-id="35731-114">String</span><span class="sxs-lookup"><span data-stu-id="35731-114">String</span></span>|<span data-ttu-id="35731-115">Код продукта Win32 строки из бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="35731-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="35731-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="35731-116">productVersionOperator</span></span>|[<span data-ttu-id="35731-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="35731-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="35731-118">Оператор для обнаружения версии данного продукта.</span><span class="sxs-lookup"><span data-stu-id="35731-118">The operator to detect product version.</span></span> <span data-ttu-id="35731-119">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="35731-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="35731-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="35731-120">productVersion</span></span>|<span data-ttu-id="35731-121">String</span><span class="sxs-lookup"><span data-stu-id="35731-121">String</span></span>|<span data-ttu-id="35731-122">Версия продукта Win32 строки из бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="35731-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35731-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="35731-123">Relationships</span></span>
<span data-ttu-id="35731-124">Нет</span><span class="sxs-lookup"><span data-stu-id="35731-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35731-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35731-125">JSON Representation</span></span>
<span data-ttu-id="35731-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35731-126">Here is a JSON representation of the resource.</span></span>
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




