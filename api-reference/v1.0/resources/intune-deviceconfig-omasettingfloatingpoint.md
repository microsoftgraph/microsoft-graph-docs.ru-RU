---
title: Тип ресурса omaSettingFloatingPoint
description: Определение плавающей запятой параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddb11f40faf9db58fefb984fcc08a9fedd66e97d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951553"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="afee5-103">Тип ресурса omaSettingFloatingPoint</span><span class="sxs-lookup"><span data-stu-id="afee5-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="afee5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="afee5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afee5-105">Определение плавающей запятой параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="afee5-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="afee5-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="afee5-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="afee5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="afee5-107">Properties</span></span>
|<span data-ttu-id="afee5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="afee5-108">Property</span></span>|<span data-ttu-id="afee5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="afee5-109">Type</span></span>|<span data-ttu-id="afee5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="afee5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afee5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="afee5-111">displayName</span></span>|<span data-ttu-id="afee5-112">Строка</span><span class="sxs-lookup"><span data-stu-id="afee5-112">String</span></span>|<span data-ttu-id="afee5-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="afee5-113">Display Name.</span></span> <span data-ttu-id="afee5-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="afee5-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="afee5-115">описание</span><span class="sxs-lookup"><span data-stu-id="afee5-115">description</span></span>|<span data-ttu-id="afee5-116">Строка</span><span class="sxs-lookup"><span data-stu-id="afee5-116">String</span></span>|<span data-ttu-id="afee5-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="afee5-117">Description.</span></span> <span data-ttu-id="afee5-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="afee5-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="afee5-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="afee5-119">omaUri</span></span>|<span data-ttu-id="afee5-120">Строка</span><span class="sxs-lookup"><span data-stu-id="afee5-120">String</span></span>|<span data-ttu-id="afee5-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="afee5-121">OMA.</span></span> <span data-ttu-id="afee5-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="afee5-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="afee5-123">value</span><span class="sxs-lookup"><span data-stu-id="afee5-123">value</span></span>|<span data-ttu-id="afee5-124">Single</span><span class="sxs-lookup"><span data-stu-id="afee5-124">Single</span></span>|<span data-ttu-id="afee5-125">Значение.</span><span class="sxs-lookup"><span data-stu-id="afee5-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="afee5-126">Связи</span><span class="sxs-lookup"><span data-stu-id="afee5-126">Relationships</span></span>
<span data-ttu-id="afee5-127">Нет</span><span class="sxs-lookup"><span data-stu-id="afee5-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="afee5-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="afee5-128">JSON Representation</span></span>
<span data-ttu-id="afee5-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="afee5-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



