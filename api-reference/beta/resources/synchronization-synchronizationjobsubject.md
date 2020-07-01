---
title: Тип ресурса Синчронизатионжобсубжект
description: Представляет объекты, которые будут подготовлены при подготовке по запросу.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54f8271d3b11cce55cc3e7042ffcba84a330d798
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007208"
---
# <a name="synchronizationjobsubject-resource-type"></a><span data-ttu-id="5ec80-103">Тип ресурса Синчронизатионжобсубжект</span><span class="sxs-lookup"><span data-stu-id="5ec80-103">synchronizationJobSubject resource type</span></span>

<span data-ttu-id="5ec80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ec80-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ec80-105">Представляет объекты, которые будут подготовлены при подготовке по запросу.</span><span class="sxs-lookup"><span data-stu-id="5ec80-105">Represents the objects that will be provisioned during on-demand provisioning.</span></span>

## <a name="properties"></a><span data-ttu-id="5ec80-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ec80-106">Properties</span></span>
|<span data-ttu-id="5ec80-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ec80-107">Property</span></span>|<span data-ttu-id="5ec80-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5ec80-108">Type</span></span>|<span data-ttu-id="5ec80-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5ec80-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ec80-110">objectId</span><span class="sxs-lookup"><span data-stu-id="5ec80-110">objectId</span></span>|<span data-ttu-id="5ec80-111">String</span><span class="sxs-lookup"><span data-stu-id="5ec80-111">String</span></span>|<span data-ttu-id="5ec80-112">Идентификатор объекта, к которому применяется Синчронизатионжоб.</span><span class="sxs-lookup"><span data-stu-id="5ec80-112">The identifier of an object to which a synchronizationJob  is to be applied.</span></span>|
|<span data-ttu-id="5ec80-113">обжекттипенаме</span><span class="sxs-lookup"><span data-stu-id="5ec80-113">objectTypeName</span></span>|<span data-ttu-id="5ec80-114">String</span><span class="sxs-lookup"><span data-stu-id="5ec80-114">String</span></span>|<span data-ttu-id="5ec80-115">Тип объекта, к которому применяется Синчронизатионжоб.</span><span class="sxs-lookup"><span data-stu-id="5ec80-115">The type of the object to which a synchronizationJob  is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ec80-116">Связи</span><span class="sxs-lookup"><span data-stu-id="5ec80-116">Relationships</span></span>
<span data-ttu-id="5ec80-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5ec80-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ec80-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5ec80-118">JSON representation</span></span>
<span data-ttu-id="5ec80-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ec80-119">The following is a JSON representation of the resource.</span></span>
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
