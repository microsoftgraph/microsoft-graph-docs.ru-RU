---
title: Тип ресурса omaSettingBoolean
description: Логическое определение параметров OMA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2c555093e129bd3faedbaa1962505046b01cf822
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273167"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="eb94a-103">Тип ресурса omaSettingBoolean</span><span class="sxs-lookup"><span data-stu-id="eb94a-103">omaSettingBoolean resource type</span></span>

<span data-ttu-id="eb94a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb94a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb94a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb94a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb94a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb94a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb94a-107">Логическое определение параметров OMA.</span><span class="sxs-lookup"><span data-stu-id="eb94a-107">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="eb94a-108">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eb94a-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb94a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb94a-109">Properties</span></span>
|<span data-ttu-id="eb94a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb94a-110">Property</span></span>|<span data-ttu-id="eb94a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="eb94a-111">Type</span></span>|<span data-ttu-id="eb94a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="eb94a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb94a-113">displayName</span><span class="sxs-lookup"><span data-stu-id="eb94a-113">displayName</span></span>|<span data-ttu-id="eb94a-114">String</span><span class="sxs-lookup"><span data-stu-id="eb94a-114">String</span></span>|<span data-ttu-id="eb94a-115">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="eb94a-115">Display Name.</span></span> <span data-ttu-id="eb94a-116">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eb94a-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eb94a-117">description</span><span class="sxs-lookup"><span data-stu-id="eb94a-117">description</span></span>|<span data-ttu-id="eb94a-118">String</span><span class="sxs-lookup"><span data-stu-id="eb94a-118">String</span></span>|<span data-ttu-id="eb94a-119">Описание.</span><span class="sxs-lookup"><span data-stu-id="eb94a-119">Description.</span></span> <span data-ttu-id="eb94a-120">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eb94a-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eb94a-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="eb94a-121">omaUri</span></span>|<span data-ttu-id="eb94a-122">String</span><span class="sxs-lookup"><span data-stu-id="eb94a-122">String</span></span>|<span data-ttu-id="eb94a-123">OMA.</span><span class="sxs-lookup"><span data-stu-id="eb94a-123">OMA.</span></span> <span data-ttu-id="eb94a-124">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eb94a-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eb94a-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="eb94a-125">isEncrypted</span></span>|<span data-ttu-id="eb94a-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb94a-126">Boolean</span></span>|<span data-ttu-id="eb94a-127">Указывает, зашифровано ли поле "значение".</span><span class="sxs-lookup"><span data-stu-id="eb94a-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="eb94a-128">Наследуется от [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eb94a-128">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="eb94a-129">value</span><span class="sxs-lookup"><span data-stu-id="eb94a-129">value</span></span>|<span data-ttu-id="eb94a-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb94a-130">Boolean</span></span>|<span data-ttu-id="eb94a-131">Значение</span><span class="sxs-lookup"><span data-stu-id="eb94a-131">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb94a-132">Связи</span><span class="sxs-lookup"><span data-stu-id="eb94a-132">Relationships</span></span>
<span data-ttu-id="eb94a-133">Нет</span><span class="sxs-lookup"><span data-stu-id="eb94a-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb94a-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb94a-134">JSON Representation</span></span>
<span data-ttu-id="eb94a-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb94a-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "isEncrypted": true,
  "value": true
}
```




