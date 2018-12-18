---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: tfitzmac
ms.openlocfilehash: a62f6dee2bf0f5a9ca96488625a84ceef5f7c785
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311202"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="b07cf-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="b07cf-103">omaSettingString resource type</span></span>

> <span data-ttu-id="b07cf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b07cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b07cf-105">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="b07cf-105">OMA Settings String definition.</span></span>

<span data-ttu-id="b07cf-106">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b07cf-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b07cf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b07cf-107">Properties</span></span>
|<span data-ttu-id="b07cf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b07cf-108">Property</span></span>|<span data-ttu-id="b07cf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b07cf-109">Type</span></span>|<span data-ttu-id="b07cf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b07cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b07cf-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b07cf-111">displayName</span></span>|<span data-ttu-id="b07cf-112">Строка</span><span class="sxs-lookup"><span data-stu-id="b07cf-112">String</span></span>|<span data-ttu-id="b07cf-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="b07cf-113">Display Name.</span></span> <span data-ttu-id="b07cf-114">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b07cf-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b07cf-115">описание</span><span class="sxs-lookup"><span data-stu-id="b07cf-115">description</span></span>|<span data-ttu-id="b07cf-116">Строка</span><span class="sxs-lookup"><span data-stu-id="b07cf-116">String</span></span>|<span data-ttu-id="b07cf-117">Описание.</span><span class="sxs-lookup"><span data-stu-id="b07cf-117">Description.</span></span> <span data-ttu-id="b07cf-118">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b07cf-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b07cf-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="b07cf-119">omaUri</span></span>|<span data-ttu-id="b07cf-120">Строка</span><span class="sxs-lookup"><span data-stu-id="b07cf-120">String</span></span>|<span data-ttu-id="b07cf-121">OMA.</span><span class="sxs-lookup"><span data-stu-id="b07cf-121">OMA.</span></span> <span data-ttu-id="b07cf-122">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b07cf-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b07cf-123">value</span><span class="sxs-lookup"><span data-stu-id="b07cf-123">value</span></span>|<span data-ttu-id="b07cf-124">Строка</span><span class="sxs-lookup"><span data-stu-id="b07cf-124">String</span></span>|<span data-ttu-id="b07cf-125">Значение</span><span class="sxs-lookup"><span data-stu-id="b07cf-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b07cf-126">Связи</span><span class="sxs-lookup"><span data-stu-id="b07cf-126">Relationships</span></span>
<span data-ttu-id="b07cf-127">Нет</span><span class="sxs-lookup"><span data-stu-id="b07cf-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b07cf-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b07cf-128">JSON Representation</span></span>
<span data-ttu-id="b07cf-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b07cf-129">Here is a JSON representation of the resource.</span></span>
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



