---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dc59c22933b888227678db70d9a48d601d699a8e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990248"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="689da-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="689da-103">omaSettingString resource type</span></span>

> <span data-ttu-id="689da-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="689da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="689da-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="689da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="689da-106">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="689da-106">OMA Settings String definition.</span></span>


<span data-ttu-id="689da-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="689da-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="689da-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="689da-108">Properties</span></span>
|<span data-ttu-id="689da-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="689da-109">Property</span></span>|<span data-ttu-id="689da-110">Тип</span><span class="sxs-lookup"><span data-stu-id="689da-110">Type</span></span>|<span data-ttu-id="689da-111">Описание</span><span class="sxs-lookup"><span data-stu-id="689da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="689da-112">displayName</span><span class="sxs-lookup"><span data-stu-id="689da-112">displayName</span></span>|<span data-ttu-id="689da-113">Строка</span><span class="sxs-lookup"><span data-stu-id="689da-113">String</span></span>|<span data-ttu-id="689da-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="689da-114">Display Name.</span></span> <span data-ttu-id="689da-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="689da-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="689da-116">description</span><span class="sxs-lookup"><span data-stu-id="689da-116">description</span></span>|<span data-ttu-id="689da-117">String</span><span class="sxs-lookup"><span data-stu-id="689da-117">String</span></span>|<span data-ttu-id="689da-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="689da-118">Description.</span></span> <span data-ttu-id="689da-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="689da-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="689da-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="689da-120">omaUri</span></span>|<span data-ttu-id="689da-121">String</span><span class="sxs-lookup"><span data-stu-id="689da-121">String</span></span>|<span data-ttu-id="689da-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="689da-122">OMA.</span></span> <span data-ttu-id="689da-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="689da-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="689da-124">value</span><span class="sxs-lookup"><span data-stu-id="689da-124">value</span></span>|<span data-ttu-id="689da-125">Строка</span><span class="sxs-lookup"><span data-stu-id="689da-125">String</span></span>|<span data-ttu-id="689da-126">Значение</span><span class="sxs-lookup"><span data-stu-id="689da-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="689da-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="689da-127">Relationships</span></span>
<span data-ttu-id="689da-128">Нет</span><span class="sxs-lookup"><span data-stu-id="689da-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="689da-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="689da-129">JSON Representation</span></span>
<span data-ttu-id="689da-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="689da-130">Here is a JSON representation of the resource.</span></span>
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





