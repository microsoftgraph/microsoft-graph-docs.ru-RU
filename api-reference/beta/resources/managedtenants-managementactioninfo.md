---
title: тип ресурсов managementActionInfo
description: Представляет справочные сведения для действия управления.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: cde8e52b8329d03169eb5953dd92b897b3b8272e
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402712"
---
# <a name="managementactioninfo-resource-type"></a><span data-ttu-id="989fb-103">тип ресурсов managementActionInfo</span><span class="sxs-lookup"><span data-stu-id="989fb-103">managementActionInfo resource type</span></span>

<span data-ttu-id="989fb-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="989fb-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="989fb-105">Представляет справочные сведения для действия управления.</span><span class="sxs-lookup"><span data-stu-id="989fb-105">Represents reference information for a management action.</span></span>

## <a name="properties"></a><span data-ttu-id="989fb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="989fb-106">Properties</span></span>
|<span data-ttu-id="989fb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="989fb-107">Property</span></span>|<span data-ttu-id="989fb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="989fb-108">Type</span></span>|<span data-ttu-id="989fb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="989fb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="989fb-110">managementActionId</span><span class="sxs-lookup"><span data-stu-id="989fb-110">managementActionId</span></span>|<span data-ttu-id="989fb-111">String</span><span class="sxs-lookup"><span data-stu-id="989fb-111">String</span></span>|<span data-ttu-id="989fb-112">Идентификатор для действия управления.</span><span class="sxs-lookup"><span data-stu-id="989fb-112">The identifier for the management action.</span></span> <span data-ttu-id="989fb-113">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="989fb-113">Required.</span></span> <span data-ttu-id="989fb-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="989fb-114">Read-only.</span></span>|
|<span data-ttu-id="989fb-115">managementTemplateId</span><span class="sxs-lookup"><span data-stu-id="989fb-115">managementTemplateId</span></span>|<span data-ttu-id="989fb-116">String</span><span class="sxs-lookup"><span data-stu-id="989fb-116">String</span></span>|<span data-ttu-id="989fb-117">Идентификатор шаблона управления.</span><span class="sxs-lookup"><span data-stu-id="989fb-117">The identifier for the management template.</span></span> <span data-ttu-id="989fb-118">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="989fb-118">Required.</span></span> <span data-ttu-id="989fb-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="989fb-119">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="989fb-120">Связи</span><span class="sxs-lookup"><span data-stu-id="989fb-120">Relationships</span></span>
<span data-ttu-id="989fb-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="989fb-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="989fb-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="989fb-122">JSON representation</span></span>
<span data-ttu-id="989fb-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="989fb-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managementActionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managementActionInfo",
  "managementTemplateId": "String",
  "managementActionId": "String"
}
```
