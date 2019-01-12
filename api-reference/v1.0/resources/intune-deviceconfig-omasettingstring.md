---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0524e077c210f2b13744534b9f42b2bb19d6359b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911765"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="bfeca-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="bfeca-103">omaSettingString resource type</span></span>

> <span data-ttu-id="bfeca-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bfeca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfeca-105">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="bfeca-105">OMA Settings String definition.</span></span>

<span data-ttu-id="bfeca-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bfeca-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bfeca-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfeca-107">Properties</span></span>
|<span data-ttu-id="bfeca-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfeca-108">Property</span></span>|<span data-ttu-id="bfeca-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bfeca-109">Type</span></span>|<span data-ttu-id="bfeca-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bfeca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfeca-111">displayName</span><span class="sxs-lookup"><span data-stu-id="bfeca-111">displayName</span></span>|<span data-ttu-id="bfeca-112">Строка</span><span class="sxs-lookup"><span data-stu-id="bfeca-112">String</span></span>|<span data-ttu-id="bfeca-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="bfeca-113">Display Name.</span></span> <span data-ttu-id="bfeca-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bfeca-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bfeca-115">описание</span><span class="sxs-lookup"><span data-stu-id="bfeca-115">description</span></span>|<span data-ttu-id="bfeca-116">Строка</span><span class="sxs-lookup"><span data-stu-id="bfeca-116">String</span></span>|<span data-ttu-id="bfeca-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="bfeca-117">Description.</span></span> <span data-ttu-id="bfeca-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bfeca-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bfeca-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="bfeca-119">omaUri</span></span>|<span data-ttu-id="bfeca-120">Строка</span><span class="sxs-lookup"><span data-stu-id="bfeca-120">String</span></span>|<span data-ttu-id="bfeca-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="bfeca-121">OMA.</span></span> <span data-ttu-id="bfeca-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="bfeca-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bfeca-123">value</span><span class="sxs-lookup"><span data-stu-id="bfeca-123">value</span></span>|<span data-ttu-id="bfeca-124">Строка</span><span class="sxs-lookup"><span data-stu-id="bfeca-124">String</span></span>|<span data-ttu-id="bfeca-125">Значение</span><span class="sxs-lookup"><span data-stu-id="bfeca-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfeca-126">Связи</span><span class="sxs-lookup"><span data-stu-id="bfeca-126">Relationships</span></span>
<span data-ttu-id="bfeca-127">Нет</span><span class="sxs-lookup"><span data-stu-id="bfeca-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bfeca-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfeca-128">JSON Representation</span></span>
<span data-ttu-id="bfeca-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfeca-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



