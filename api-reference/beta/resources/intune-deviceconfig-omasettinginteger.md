---
title: Тип ресурса omaSettingInteger
description: Определение целого числа параметра OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 58e668baadc854d2f73a3c9f9e52614905fe1a9f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011402"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="92981-103">Тип ресурса omaSettingInteger</span><span class="sxs-lookup"><span data-stu-id="92981-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="92981-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92981-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92981-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92981-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92981-106">Определение целого числа параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="92981-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="92981-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="92981-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92981-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="92981-108">Properties</span></span>
|<span data-ttu-id="92981-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="92981-109">Property</span></span>|<span data-ttu-id="92981-110">Тип</span><span class="sxs-lookup"><span data-stu-id="92981-110">Type</span></span>|<span data-ttu-id="92981-111">Описание</span><span class="sxs-lookup"><span data-stu-id="92981-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92981-112">displayName</span><span class="sxs-lookup"><span data-stu-id="92981-112">displayName</span></span>|<span data-ttu-id="92981-113">Строка</span><span class="sxs-lookup"><span data-stu-id="92981-113">String</span></span>|<span data-ttu-id="92981-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="92981-114">Display Name.</span></span> <span data-ttu-id="92981-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="92981-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="92981-116">description</span><span class="sxs-lookup"><span data-stu-id="92981-116">description</span></span>|<span data-ttu-id="92981-117">String</span><span class="sxs-lookup"><span data-stu-id="92981-117">String</span></span>|<span data-ttu-id="92981-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="92981-118">Description.</span></span> <span data-ttu-id="92981-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="92981-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="92981-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="92981-120">omaUri</span></span>|<span data-ttu-id="92981-121">String</span><span class="sxs-lookup"><span data-stu-id="92981-121">String</span></span>|<span data-ttu-id="92981-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="92981-122">OMA.</span></span> <span data-ttu-id="92981-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="92981-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="92981-124">value</span><span class="sxs-lookup"><span data-stu-id="92981-124">value</span></span>|<span data-ttu-id="92981-125">Int32</span><span class="sxs-lookup"><span data-stu-id="92981-125">Int32</span></span>|<span data-ttu-id="92981-126">Значение.</span><span class="sxs-lookup"><span data-stu-id="92981-126">Value.</span></span>|
|<span data-ttu-id="92981-127">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="92981-127">isReadOnly</span></span>|<span data-ttu-id="92981-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="92981-128">Boolean</span></span>|<span data-ttu-id="92981-129">Если задано значение true, CSP (поставщик услуг по настройке), указанный в OMA-URI, будет выполнять Get, а не Set</span><span class="sxs-lookup"><span data-stu-id="92981-129">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="92981-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="92981-130">Relationships</span></span>
<span data-ttu-id="92981-131">Нет</span><span class="sxs-lookup"><span data-stu-id="92981-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92981-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92981-132">JSON Representation</span></span>
<span data-ttu-id="92981-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92981-133">Here is a JSON representation of the resource.</span></span>
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





