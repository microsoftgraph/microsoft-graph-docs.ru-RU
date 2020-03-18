---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 829f73ec2d5eb205e6cacdb46ee209760334cb3a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788445"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="1a177-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="1a177-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="1a177-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a177-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a177-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1a177-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a177-106">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="1a177-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="1a177-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1a177-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a177-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a177-108">Properties</span></span>
|<span data-ttu-id="1a177-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a177-109">Property</span></span>|<span data-ttu-id="1a177-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1a177-110">Type</span></span>|<span data-ttu-id="1a177-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1a177-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a177-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1a177-112">displayName</span></span>|<span data-ttu-id="1a177-113">Строка</span><span class="sxs-lookup"><span data-stu-id="1a177-113">String</span></span>|<span data-ttu-id="1a177-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="1a177-114">Display Name.</span></span> <span data-ttu-id="1a177-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1a177-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1a177-116">description</span><span class="sxs-lookup"><span data-stu-id="1a177-116">description</span></span>|<span data-ttu-id="1a177-117">String</span><span class="sxs-lookup"><span data-stu-id="1a177-117">String</span></span>|<span data-ttu-id="1a177-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="1a177-118">Description.</span></span> <span data-ttu-id="1a177-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1a177-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1a177-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="1a177-120">omaUri</span></span>|<span data-ttu-id="1a177-121">String</span><span class="sxs-lookup"><span data-stu-id="1a177-121">String</span></span>|<span data-ttu-id="1a177-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="1a177-122">OMA.</span></span> <span data-ttu-id="1a177-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1a177-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="1a177-124">value</span><span class="sxs-lookup"><span data-stu-id="1a177-124">value</span></span>|<span data-ttu-id="1a177-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1a177-125">Int32</span></span>|<span data-ttu-id="1a177-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="1a177-126">Value.</span></span>|
|<span data-ttu-id="1a177-127">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="1a177-127">isReadOnly</span></span>|<span data-ttu-id="1a177-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a177-128">Boolean</span></span>|<span data-ttu-id="1a177-129">Если задано значение true, CSP (поставщик услуг по настройке), указанный в OMA-URI, будет выполнять Get, а не Set</span><span class="sxs-lookup"><span data-stu-id="1a177-129">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a177-130">Связи</span><span class="sxs-lookup"><span data-stu-id="1a177-130">Relationships</span></span>
<span data-ttu-id="1a177-131">Нет</span><span class="sxs-lookup"><span data-stu-id="1a177-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a177-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a177-132">JSON Representation</span></span>
<span data-ttu-id="1a177-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a177-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024,
  "isReadOnly": true
}
```



