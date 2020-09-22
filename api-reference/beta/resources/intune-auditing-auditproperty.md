---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2d30f44bdf5ca002f71ac5e1f935081b032379ec
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076304"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="04869-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="04869-103">auditProperty resource type</span></span>

<span data-ttu-id="04869-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04869-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04869-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04869-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04869-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04869-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04869-107">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="04869-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="04869-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="04869-108">Properties</span></span>
|<span data-ttu-id="04869-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="04869-109">Property</span></span>|<span data-ttu-id="04869-110">Тип</span><span class="sxs-lookup"><span data-stu-id="04869-110">Type</span></span>|<span data-ttu-id="04869-111">Описание</span><span class="sxs-lookup"><span data-stu-id="04869-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04869-112">displayName</span><span class="sxs-lookup"><span data-stu-id="04869-112">displayName</span></span>|<span data-ttu-id="04869-113">String</span><span class="sxs-lookup"><span data-stu-id="04869-113">String</span></span>|<span data-ttu-id="04869-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="04869-114">Display name.</span></span>|
|<span data-ttu-id="04869-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="04869-115">oldValue</span></span>|<span data-ttu-id="04869-116">String</span><span class="sxs-lookup"><span data-stu-id="04869-116">String</span></span>|<span data-ttu-id="04869-117">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="04869-117">Old value.</span></span>|
|<span data-ttu-id="04869-118">newValue</span><span class="sxs-lookup"><span data-stu-id="04869-118">newValue</span></span>|<span data-ttu-id="04869-119">String</span><span class="sxs-lookup"><span data-stu-id="04869-119">String</span></span>|<span data-ttu-id="04869-120">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="04869-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04869-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="04869-121">Relationships</span></span>
<span data-ttu-id="04869-122">Нет</span><span class="sxs-lookup"><span data-stu-id="04869-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04869-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04869-123">JSON Representation</span></span>
<span data-ttu-id="04869-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04869-124">Here is a JSON representation of the resource.</span></span>
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






