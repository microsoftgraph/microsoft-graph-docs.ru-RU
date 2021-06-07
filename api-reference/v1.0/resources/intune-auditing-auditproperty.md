---
title: Тип ресурса auditProperty
description: Класс, содержащий свойства для свойства аудита.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 900e493ce77fd47a232626ad73999ce3482d4fe6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748998"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="5c781-103">Тип ресурса auditProperty</span><span class="sxs-lookup"><span data-stu-id="5c781-103">auditProperty resource type</span></span>

<span data-ttu-id="5c781-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c781-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5c781-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5c781-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c781-106">Класс, содержащий свойства для свойства аудита.</span><span class="sxs-lookup"><span data-stu-id="5c781-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="5c781-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c781-107">Properties</span></span>
|<span data-ttu-id="5c781-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c781-108">Property</span></span>|<span data-ttu-id="5c781-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5c781-109">Type</span></span>|<span data-ttu-id="5c781-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5c781-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c781-111">displayName</span><span class="sxs-lookup"><span data-stu-id="5c781-111">displayName</span></span>|<span data-ttu-id="5c781-112">String</span><span class="sxs-lookup"><span data-stu-id="5c781-112">String</span></span>|<span data-ttu-id="5c781-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="5c781-113">Display name.</span></span>|
|<span data-ttu-id="5c781-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="5c781-114">oldValue</span></span>|<span data-ttu-id="5c781-115">String</span><span class="sxs-lookup"><span data-stu-id="5c781-115">String</span></span>|<span data-ttu-id="5c781-116">Старое значение.</span><span class="sxs-lookup"><span data-stu-id="5c781-116">Old value.</span></span>|
|<span data-ttu-id="5c781-117">newValue</span><span class="sxs-lookup"><span data-stu-id="5c781-117">newValue</span></span>|<span data-ttu-id="5c781-118">String</span><span class="sxs-lookup"><span data-stu-id="5c781-118">String</span></span>|<span data-ttu-id="5c781-119">Новое значение.</span><span class="sxs-lookup"><span data-stu-id="5c781-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c781-120">Связи</span><span class="sxs-lookup"><span data-stu-id="5c781-120">Relationships</span></span>
<span data-ttu-id="5c781-121">Нет</span><span class="sxs-lookup"><span data-stu-id="5c781-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c781-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c781-122">JSON Representation</span></span>
<span data-ttu-id="5c781-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c781-123">Here is a JSON representation of the resource.</span></span>
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




