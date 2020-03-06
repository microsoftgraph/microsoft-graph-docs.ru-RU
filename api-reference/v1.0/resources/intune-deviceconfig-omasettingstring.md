---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 885f2c275cea1df033a3cdfe791297d6b5d70c4c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530575"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="13290-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="13290-103">omaSettingString resource type</span></span>

<span data-ttu-id="13290-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13290-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13290-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="13290-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13290-106">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="13290-106">OMA Settings String definition.</span></span>


<span data-ttu-id="13290-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="13290-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="13290-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="13290-108">Properties</span></span>
|<span data-ttu-id="13290-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="13290-109">Property</span></span>|<span data-ttu-id="13290-110">Тип</span><span class="sxs-lookup"><span data-stu-id="13290-110">Type</span></span>|<span data-ttu-id="13290-111">Описание</span><span class="sxs-lookup"><span data-stu-id="13290-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13290-112">displayName</span><span class="sxs-lookup"><span data-stu-id="13290-112">displayName</span></span>|<span data-ttu-id="13290-113">Строка</span><span class="sxs-lookup"><span data-stu-id="13290-113">String</span></span>|<span data-ttu-id="13290-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="13290-114">Display Name.</span></span> <span data-ttu-id="13290-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="13290-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="13290-116">description</span><span class="sxs-lookup"><span data-stu-id="13290-116">description</span></span>|<span data-ttu-id="13290-117">String</span><span class="sxs-lookup"><span data-stu-id="13290-117">String</span></span>|<span data-ttu-id="13290-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="13290-118">Description.</span></span> <span data-ttu-id="13290-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="13290-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="13290-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="13290-120">omaUri</span></span>|<span data-ttu-id="13290-121">String</span><span class="sxs-lookup"><span data-stu-id="13290-121">String</span></span>|<span data-ttu-id="13290-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="13290-122">OMA.</span></span> <span data-ttu-id="13290-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="13290-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="13290-124">value</span><span class="sxs-lookup"><span data-stu-id="13290-124">value</span></span>|<span data-ttu-id="13290-125">Строка</span><span class="sxs-lookup"><span data-stu-id="13290-125">String</span></span>|<span data-ttu-id="13290-126">Значение</span><span class="sxs-lookup"><span data-stu-id="13290-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13290-127">Связи</span><span class="sxs-lookup"><span data-stu-id="13290-127">Relationships</span></span>
<span data-ttu-id="13290-128">Нет</span><span class="sxs-lookup"><span data-stu-id="13290-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13290-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13290-129">JSON Representation</span></span>
<span data-ttu-id="13290-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13290-130">Here is a JSON representation of the resource.</span></span>
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




