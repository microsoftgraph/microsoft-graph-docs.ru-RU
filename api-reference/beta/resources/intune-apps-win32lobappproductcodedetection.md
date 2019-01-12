---
title: Тип ресурса win32LobAppProductCodeDetection
description: Содержит свойства кода и версия продукта для обнаружения приложений Win32
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5536384178ac197d3b52609cb767fef82befd3b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928530"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="30a67-103">Тип ресурса win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="30a67-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="30a67-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="30a67-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30a67-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30a67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30a67-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="30a67-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30a67-107">Содержит свойства кода и версия продукта для обнаружения приложений Win32</span><span class="sxs-lookup"><span data-stu-id="30a67-107">Contains product code and version properties to detect a Win32 App</span></span>

<span data-ttu-id="30a67-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="30a67-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="30a67-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="30a67-109">Properties</span></span>
|<span data-ttu-id="30a67-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="30a67-110">Property</span></span>|<span data-ttu-id="30a67-111">Тип</span><span class="sxs-lookup"><span data-stu-id="30a67-111">Type</span></span>|<span data-ttu-id="30a67-112">Описание</span><span class="sxs-lookup"><span data-stu-id="30a67-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30a67-113">productCode</span><span class="sxs-lookup"><span data-stu-id="30a67-113">productCode</span></span>|<span data-ttu-id="30a67-114">String</span><span class="sxs-lookup"><span data-stu-id="30a67-114">String</span></span>|<span data-ttu-id="30a67-115">Код продукта Win32 строки из бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="30a67-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="30a67-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="30a67-116">productVersionOperator</span></span>|[<span data-ttu-id="30a67-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="30a67-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="30a67-118">Оператор для обнаружения версии данного продукта.</span><span class="sxs-lookup"><span data-stu-id="30a67-118">The operator to detect product version.</span></span> <span data-ttu-id="30a67-119">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="30a67-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="30a67-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="30a67-120">productVersion</span></span>|<span data-ttu-id="30a67-121">String</span><span class="sxs-lookup"><span data-stu-id="30a67-121">String</span></span>|<span data-ttu-id="30a67-122">Версия продукта Win32 строки из бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="30a67-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30a67-123">Связи</span><span class="sxs-lookup"><span data-stu-id="30a67-123">Relationships</span></span>
<span data-ttu-id="30a67-124">Нет</span><span class="sxs-lookup"><span data-stu-id="30a67-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="30a67-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30a67-125">JSON Representation</span></span>
<span data-ttu-id="30a67-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30a67-126">Here is a JSON representation of the resource.</span></span>
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





