---
title: Тип ресурса win32LobAppProductCodeDetection
description: Содержит код продукта и свойства версии для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: baceeb2cbc3ddfe28e81871159fb24db96accd64
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280867"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="e401e-103">Тип ресурса win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="e401e-103">win32LobAppProductCodeDetection resource type</span></span>

<span data-ttu-id="e401e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e401e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e401e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e401e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e401e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e401e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e401e-107">Содержит код продукта и свойства версии для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="e401e-107">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="e401e-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="e401e-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e401e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e401e-109">Properties</span></span>
|<span data-ttu-id="e401e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e401e-110">Property</span></span>|<span data-ttu-id="e401e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e401e-111">Type</span></span>|<span data-ttu-id="e401e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e401e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e401e-113">productCode</span><span class="sxs-lookup"><span data-stu-id="e401e-113">productCode</span></span>|<span data-ttu-id="e401e-114">String</span><span class="sxs-lookup"><span data-stu-id="e401e-114">String</span></span>|<span data-ttu-id="e401e-115">Код продукта для бизнес-приложения Win32 (LoB).</span><span class="sxs-lookup"><span data-stu-id="e401e-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e401e-116">продуктверсионоператор</span><span class="sxs-lookup"><span data-stu-id="e401e-116">productVersionOperator</span></span>|[<span data-ttu-id="e401e-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="e401e-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="e401e-118">Оператор для определения версии продукта.</span><span class="sxs-lookup"><span data-stu-id="e401e-118">The operator to detect product version.</span></span> <span data-ttu-id="e401e-119">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="e401e-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="e401e-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="e401e-120">productVersion</span></span>|<span data-ttu-id="e401e-121">String</span><span class="sxs-lookup"><span data-stu-id="e401e-121">String</span></span>|<span data-ttu-id="e401e-122">Версия приложения, на котором установлен продукт Win32 бизнес (LoB).</span><span class="sxs-lookup"><span data-stu-id="e401e-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e401e-123">Связи</span><span class="sxs-lookup"><span data-stu-id="e401e-123">Relationships</span></span>
<span data-ttu-id="e401e-124">Нет</span><span class="sxs-lookup"><span data-stu-id="e401e-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e401e-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e401e-125">JSON Representation</span></span>
<span data-ttu-id="e401e-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e401e-126">Here is a JSON representation of the resource.</span></span>
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




