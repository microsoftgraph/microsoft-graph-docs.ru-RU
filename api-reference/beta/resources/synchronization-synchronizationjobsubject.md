---
title: Тип ресурса synchronizationJobSubject
description: Представляет объекты, которые будут быть представлены во время предоставления по требованию.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c9e6d83ed7024556954740e89edcc18f7b56ba04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132001"
---
# <a name="synchronizationjobsubject-resource-type"></a><span data-ttu-id="4e0e2-103">Тип ресурса synchronizationJobSubject</span><span class="sxs-lookup"><span data-stu-id="4e0e2-103">synchronizationJobSubject resource type</span></span>

<span data-ttu-id="4e0e2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e0e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e0e2-105">Представляет объекты, которые будут быть представлены во время предоставления по требованию.</span><span class="sxs-lookup"><span data-stu-id="4e0e2-105">Represents the objects that will be provisioned during on-demand provisioning.</span></span>

## <a name="properties"></a><span data-ttu-id="4e0e2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e0e2-106">Properties</span></span>
|<span data-ttu-id="4e0e2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e0e2-107">Property</span></span>|<span data-ttu-id="4e0e2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4e0e2-108">Type</span></span>|<span data-ttu-id="4e0e2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4e0e2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e0e2-110">objectId</span><span class="sxs-lookup"><span data-stu-id="4e0e2-110">objectId</span></span>|<span data-ttu-id="4e0e2-111">String</span><span class="sxs-lookup"><span data-stu-id="4e0e2-111">String</span></span>|<span data-ttu-id="4e0e2-112">Идентификатор объекта, к которому применяется synchronizationJob.</span><span class="sxs-lookup"><span data-stu-id="4e0e2-112">The identifier of an object to which a synchronizationJob  is to be applied.</span></span>|
|<span data-ttu-id="4e0e2-113">objectTypeName</span><span class="sxs-lookup"><span data-stu-id="4e0e2-113">objectTypeName</span></span>|<span data-ttu-id="4e0e2-114">Строка</span><span class="sxs-lookup"><span data-stu-id="4e0e2-114">String</span></span>|<span data-ttu-id="4e0e2-115">Тип объекта, к которому применяется synchronizationJob.</span><span class="sxs-lookup"><span data-stu-id="4e0e2-115">The type of the object to which a synchronizationJob  is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e0e2-116">Связи</span><span class="sxs-lookup"><span data-stu-id="4e0e2-116">Relationships</span></span>
<span data-ttu-id="4e0e2-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4e0e2-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e0e2-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4e0e2-118">JSON representation</span></span>
<span data-ttu-id="4e0e2-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e0e2-119">The following is a JSON representation of the resource.</span></span>
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


