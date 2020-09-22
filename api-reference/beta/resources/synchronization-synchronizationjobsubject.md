---
title: Тип ресурса Синчронизатионжобсубжект
description: Представляет объекты, которые будут подготовлены при подготовке по запросу.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f1f7421e00fbf3f974039878e9250f07a2bcbd0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023837"
---
# <a name="synchronizationjobsubject-resource-type"></a><span data-ttu-id="95ab6-103">Тип ресурса Синчронизатионжобсубжект</span><span class="sxs-lookup"><span data-stu-id="95ab6-103">synchronizationJobSubject resource type</span></span>

<span data-ttu-id="95ab6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95ab6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95ab6-105">Представляет объекты, которые будут подготовлены при подготовке по запросу.</span><span class="sxs-lookup"><span data-stu-id="95ab6-105">Represents the objects that will be provisioned during on-demand provisioning.</span></span>

## <a name="properties"></a><span data-ttu-id="95ab6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="95ab6-106">Properties</span></span>
|<span data-ttu-id="95ab6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="95ab6-107">Property</span></span>|<span data-ttu-id="95ab6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="95ab6-108">Type</span></span>|<span data-ttu-id="95ab6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="95ab6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95ab6-110">objectId</span><span class="sxs-lookup"><span data-stu-id="95ab6-110">objectId</span></span>|<span data-ttu-id="95ab6-111">String</span><span class="sxs-lookup"><span data-stu-id="95ab6-111">String</span></span>|<span data-ttu-id="95ab6-112">Идентификатор объекта, к которому применяется Синчронизатионжоб.</span><span class="sxs-lookup"><span data-stu-id="95ab6-112">The identifier of an object to which a synchronizationJob  is to be applied.</span></span>|
|<span data-ttu-id="95ab6-113">обжекттипенаме</span><span class="sxs-lookup"><span data-stu-id="95ab6-113">objectTypeName</span></span>|<span data-ttu-id="95ab6-114">String</span><span class="sxs-lookup"><span data-stu-id="95ab6-114">String</span></span>|<span data-ttu-id="95ab6-115">Тип объекта, к которому применяется Синчронизатионжоб.</span><span class="sxs-lookup"><span data-stu-id="95ab6-115">The type of the object to which a synchronizationJob  is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95ab6-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="95ab6-116">Relationships</span></span>
<span data-ttu-id="95ab6-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="95ab6-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95ab6-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="95ab6-118">JSON representation</span></span>
<span data-ttu-id="95ab6-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95ab6-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobSubject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobSubject",
  "objectId": "String",
  "objectTypeName": "String"
}
```


