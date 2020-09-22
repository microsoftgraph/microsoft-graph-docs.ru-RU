---
title: Тип ресурса Девицеманажементсеттингпрофилеконстраинт
description: Ограничение на применение заданной метаданных профиля
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2244b0fcafb1eb983388a220662c0ce7c874c73f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061163"
---
# <a name="devicemanagementsettingprofileconstraint-resource-type"></a><span data-ttu-id="e94ee-103">Тип ресурса Девицеманажементсеттингпрофилеконстраинт</span><span class="sxs-lookup"><span data-stu-id="e94ee-103">deviceManagementSettingProfileConstraint resource type</span></span>

<span data-ttu-id="e94ee-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e94ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e94ee-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e94ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e94ee-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e94ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e94ee-107">Ограничение на применение заданной метаданных профиля</span><span class="sxs-lookup"><span data-stu-id="e94ee-107">Constraint enforcing a given profile metadata</span></span>


<span data-ttu-id="e94ee-108">Наследуется от [девицеманажементконстраинт](../resources/intune-deviceintent-devicemanagementconstraint.md)</span><span class="sxs-lookup"><span data-stu-id="e94ee-108">Inherits from [deviceManagementConstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e94ee-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e94ee-109">Properties</span></span>
|<span data-ttu-id="e94ee-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e94ee-110">Property</span></span>|<span data-ttu-id="e94ee-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e94ee-111">Type</span></span>|<span data-ttu-id="e94ee-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e94ee-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e94ee-113">source</span><span class="sxs-lookup"><span data-stu-id="e94ee-113">source</span></span>|<span data-ttu-id="e94ee-114">String</span><span class="sxs-lookup"><span data-stu-id="e94ee-114">String</span></span>|<span data-ttu-id="e94ee-115">Источник объекта</span><span class="sxs-lookup"><span data-stu-id="e94ee-115">The source of the entity</span></span>|
|<span data-ttu-id="e94ee-116">types</span><span class="sxs-lookup"><span data-stu-id="e94ee-116">types</span></span>|<span data-ttu-id="e94ee-117">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e94ee-117">String collection</span></span>|<span data-ttu-id="e94ee-118">Коллекция типов, которые несет данный объект</span><span class="sxs-lookup"><span data-stu-id="e94ee-118">A collection of types this entity carries</span></span>|

## <a name="relationships"></a><span data-ttu-id="e94ee-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e94ee-119">Relationships</span></span>
<span data-ttu-id="e94ee-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e94ee-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e94ee-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e94ee-121">JSON Representation</span></span>
<span data-ttu-id="e94ee-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e94ee-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingProfileConstraint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingProfileConstraint",
  "source": "String",
  "types": [
    "String"
  ]
}
```






