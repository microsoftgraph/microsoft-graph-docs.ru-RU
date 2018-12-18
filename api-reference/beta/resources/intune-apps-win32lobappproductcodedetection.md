---
title: Тип ресурса win32LobAppProductCodeDetection
description: Содержит свойства кода и версия продукта для обнаружения приложений Win32
author: tfitzmac
ms.openlocfilehash: d66dab5a43a11c480e0e30f70eb8aecbe47e1fa7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353986"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="ad680-103">Тип ресурса win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="ad680-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="ad680-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ad680-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad680-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad680-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad680-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ad680-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad680-107">Содержит свойства кода и версия продукта для обнаружения приложений Win32</span><span class="sxs-lookup"><span data-stu-id="ad680-107">Contains product code and version properties to detect a Win32 App</span></span>

<span data-ttu-id="ad680-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="ad680-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ad680-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad680-109">Properties</span></span>
|<span data-ttu-id="ad680-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad680-110">Property</span></span>|<span data-ttu-id="ad680-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ad680-111">Type</span></span>|<span data-ttu-id="ad680-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ad680-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad680-113">productCode</span><span class="sxs-lookup"><span data-stu-id="ad680-113">productCode</span></span>|<span data-ttu-id="ad680-114">String</span><span class="sxs-lookup"><span data-stu-id="ad680-114">String</span></span>|<span data-ttu-id="ad680-115">Код продукта Win32 строки из бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ad680-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ad680-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="ad680-116">productVersionOperator</span></span>|[<span data-ttu-id="ad680-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="ad680-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="ad680-118">Оператор для обнаружения версии данного продукта.</span><span class="sxs-lookup"><span data-stu-id="ad680-118">The operator to detect product version.</span></span> <span data-ttu-id="ad680-119">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="ad680-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="ad680-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="ad680-120">productVersion</span></span>|<span data-ttu-id="ad680-121">String</span><span class="sxs-lookup"><span data-stu-id="ad680-121">String</span></span>|<span data-ttu-id="ad680-122">Версия продукта Win32 строки из бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ad680-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad680-123">Связи</span><span class="sxs-lookup"><span data-stu-id="ad680-123">Relationships</span></span>
<span data-ttu-id="ad680-124">Нет</span><span class="sxs-lookup"><span data-stu-id="ad680-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ad680-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad680-125">JSON Representation</span></span>
<span data-ttu-id="ad680-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad680-126">Here is a JSON representation of the resource.</span></span>
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





