---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad9845dc06a320ad993327e29d92d6b099d62344
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965689"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="efc05-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="efc05-103">auditProperty resource type</span></span>

<span data-ttu-id="efc05-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efc05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efc05-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efc05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efc05-106">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="efc05-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="efc05-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="efc05-107">Properties</span></span>
|<span data-ttu-id="efc05-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="efc05-108">Property</span></span>|<span data-ttu-id="efc05-109">Тип</span><span class="sxs-lookup"><span data-stu-id="efc05-109">Type</span></span>|<span data-ttu-id="efc05-110">Описание</span><span class="sxs-lookup"><span data-stu-id="efc05-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efc05-111">displayName</span><span class="sxs-lookup"><span data-stu-id="efc05-111">displayName</span></span>|<span data-ttu-id="efc05-112">String</span><span class="sxs-lookup"><span data-stu-id="efc05-112">String</span></span>|<span data-ttu-id="efc05-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="efc05-113">Display name.</span></span>|
|<span data-ttu-id="efc05-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="efc05-114">oldValue</span></span>|<span data-ttu-id="efc05-115">String</span><span class="sxs-lookup"><span data-stu-id="efc05-115">String</span></span>|<span data-ttu-id="efc05-116">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="efc05-116">Old value.</span></span>|
|<span data-ttu-id="efc05-117">newValue</span><span class="sxs-lookup"><span data-stu-id="efc05-117">newValue</span></span>|<span data-ttu-id="efc05-118">String</span><span class="sxs-lookup"><span data-stu-id="efc05-118">String</span></span>|<span data-ttu-id="efc05-119">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="efc05-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efc05-120">Связи</span><span class="sxs-lookup"><span data-stu-id="efc05-120">Relationships</span></span>
<span data-ttu-id="efc05-121">Нет</span><span class="sxs-lookup"><span data-stu-id="efc05-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efc05-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efc05-122">JSON Representation</span></span>
<span data-ttu-id="efc05-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efc05-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```









