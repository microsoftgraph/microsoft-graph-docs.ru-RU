---
title: Тип ресурса synchronizationJobApplicationParameters
description: Представляет объекты, которые необходимо получить, и правила, которые выполняются во время предоставления по требованию.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 2c17d67f766a398f94ab4962850a762fc62f6e53
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133926"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a><span data-ttu-id="56307-103">Тип ресурса synchronizationJobApplicationParameters</span><span class="sxs-lookup"><span data-stu-id="56307-103">synchronizationJobApplicationParameters resource type</span></span>

<span data-ttu-id="56307-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56307-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56307-105">Представляет объекты, которые будут быть выполнены с выполнением правил синхронизации.</span><span class="sxs-lookup"><span data-stu-id="56307-105">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="56307-106">Ресурс в основном используется для предоставления по требованию.</span><span class="sxs-lookup"><span data-stu-id="56307-106">The resource is primarily used for on-demand provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="56307-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="56307-107">Properties</span></span>
|<span data-ttu-id="56307-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="56307-108">Property</span></span>|<span data-ttu-id="56307-109">Тип</span><span class="sxs-lookup"><span data-stu-id="56307-109">Type</span></span>|<span data-ttu-id="56307-110">Описание</span><span class="sxs-lookup"><span data-stu-id="56307-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56307-111">ruleId</span><span class="sxs-lookup"><span data-stu-id="56307-111">ruleId</span></span>|<span data-ttu-id="56307-112">Строка</span><span class="sxs-lookup"><span data-stu-id="56307-112">String</span></span>|<span data-ttu-id="56307-113">Идентификатор применяемого synchronizationRule.</span><span class="sxs-lookup"><span data-stu-id="56307-113">The identifier of a the synchronizationRule to be applied.</span></span>|
|<span data-ttu-id="56307-114">subjects</span><span class="sxs-lookup"><span data-stu-id="56307-114">subjects</span></span>|<span data-ttu-id="56307-115">[Коллекция synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)</span><span class="sxs-lookup"><span data-stu-id="56307-115">[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) collection</span></span>|<span data-ttu-id="56307-116">Идентификаторы одного или более объектов, к которым необходимо применить synchronizationJob.</span><span class="sxs-lookup"><span data-stu-id="56307-116">The identifiers of one or more objects to which a synchronizationJob is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56307-117">Связи</span><span class="sxs-lookup"><span data-stu-id="56307-117">Relationships</span></span>
<span data-ttu-id="56307-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="56307-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="56307-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="56307-119">JSON representation</span></span>
<span data-ttu-id="56307-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56307-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobApplicationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobApplicationParameters",
  "ruleId": "String",
  "subjects": [
    {
      "@odata.type": "microsoft.graph.synchronizationJobSubject"
    }
  ]
}
```


