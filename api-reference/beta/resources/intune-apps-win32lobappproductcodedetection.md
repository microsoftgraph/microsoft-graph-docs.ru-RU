---
title: Тип ресурса win32LobAppProductCodeDetection
description: Содержит код продукта и свойства версии для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8e4b2469dff93e34495f9b376c96abe7a4ede98c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092820"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="d1283-103">Тип ресурса win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="d1283-103">win32LobAppProductCodeDetection resource type</span></span>

<span data-ttu-id="d1283-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1283-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1283-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1283-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1283-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d1283-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1283-107">Содержит код продукта и свойства версии для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="d1283-107">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="d1283-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="d1283-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d1283-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1283-109">Properties</span></span>
|<span data-ttu-id="d1283-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1283-110">Property</span></span>|<span data-ttu-id="d1283-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d1283-111">Type</span></span>|<span data-ttu-id="d1283-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d1283-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1283-113">productCode</span><span class="sxs-lookup"><span data-stu-id="d1283-113">productCode</span></span>|<span data-ttu-id="d1283-114">String</span><span class="sxs-lookup"><span data-stu-id="d1283-114">String</span></span>|<span data-ttu-id="d1283-115">Код продукта для бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="d1283-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d1283-116">продуктверсионоператор</span><span class="sxs-lookup"><span data-stu-id="d1283-116">productVersionOperator</span></span>|[<span data-ttu-id="d1283-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="d1283-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="d1283-118">Оператор для определения версии продукта.</span><span class="sxs-lookup"><span data-stu-id="d1283-118">The operator to detect product version.</span></span> <span data-ttu-id="d1283-119">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="d1283-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="d1283-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="d1283-120">productVersion</span></span>|<span data-ttu-id="d1283-121">String</span><span class="sxs-lookup"><span data-stu-id="d1283-121">String</span></span>|<span data-ttu-id="d1283-122">Версия приложения, на котором установлен продукт Win32 бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="d1283-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1283-123">Связи</span><span class="sxs-lookup"><span data-stu-id="d1283-123">Relationships</span></span>
<span data-ttu-id="d1283-124">Нет</span><span class="sxs-lookup"><span data-stu-id="d1283-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1283-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1283-125">JSON Representation</span></span>
<span data-ttu-id="d1283-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1283-126">Here is a JSON representation of the resource.</span></span>
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






