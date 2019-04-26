---
title: Тип ресурса omaSettingString
description: Определение строки параметра OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a22c69270126349d8d1d4afca4555abd18768aa3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566789"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="fcd08-103">Тип ресурса omaSettingString</span><span class="sxs-lookup"><span data-stu-id="fcd08-103">omaSettingString resource type</span></span>

> <span data-ttu-id="fcd08-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcd08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fcd08-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fcd08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcd08-106">Определение строки параметра OMA.</span><span class="sxs-lookup"><span data-stu-id="fcd08-106">OMA Settings String definition.</span></span>


<span data-ttu-id="fcd08-107">Наследуется от ресурса [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fcd08-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fcd08-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcd08-108">Properties</span></span>
|<span data-ttu-id="fcd08-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcd08-109">Property</span></span>|<span data-ttu-id="fcd08-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fcd08-110">Type</span></span>|<span data-ttu-id="fcd08-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fcd08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcd08-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fcd08-112">displayName</span></span>|<span data-ttu-id="fcd08-113">String</span><span class="sxs-lookup"><span data-stu-id="fcd08-113">String</span></span>|<span data-ttu-id="fcd08-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="fcd08-114">Display Name.</span></span> <span data-ttu-id="fcd08-115">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fcd08-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fcd08-116">description</span><span class="sxs-lookup"><span data-stu-id="fcd08-116">description</span></span>|<span data-ttu-id="fcd08-117">String</span><span class="sxs-lookup"><span data-stu-id="fcd08-117">String</span></span>|<span data-ttu-id="fcd08-118">Описание.</span><span class="sxs-lookup"><span data-stu-id="fcd08-118">Description.</span></span> <span data-ttu-id="fcd08-119">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fcd08-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fcd08-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="fcd08-120">omaUri</span></span>|<span data-ttu-id="fcd08-121">String</span><span class="sxs-lookup"><span data-stu-id="fcd08-121">String</span></span>|<span data-ttu-id="fcd08-122">OMA.</span><span class="sxs-lookup"><span data-stu-id="fcd08-122">OMA.</span></span> <span data-ttu-id="fcd08-123">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fcd08-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fcd08-124">value</span><span class="sxs-lookup"><span data-stu-id="fcd08-124">value</span></span>|<span data-ttu-id="fcd08-125">Строка</span><span class="sxs-lookup"><span data-stu-id="fcd08-125">String</span></span>|<span data-ttu-id="fcd08-126">Значение</span><span class="sxs-lookup"><span data-stu-id="fcd08-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcd08-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="fcd08-127">Relationships</span></span>
<span data-ttu-id="fcd08-128">Нет</span><span class="sxs-lookup"><span data-stu-id="fcd08-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcd08-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcd08-129">JSON Representation</span></span>
<span data-ttu-id="fcd08-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcd08-130">Here is a JSON representation of the resource.</span></span>
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





