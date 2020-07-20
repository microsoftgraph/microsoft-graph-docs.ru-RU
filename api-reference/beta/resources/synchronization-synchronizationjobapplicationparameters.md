---
title: Тип ресурса Синчронизатионжобаппликатионпараметерс
description: Представляет объекты, которые необходимо подготовить, и правила, выполняемые при подготовке по требованию.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0f0b7cae5a3ce9c49ea64b603390ea65831144b
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007214"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a><span data-ttu-id="44c2b-103">Тип ресурса Синчронизатионжобаппликатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="44c2b-103">synchronizationJobApplicationParameters resource type</span></span>

<span data-ttu-id="44c2b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44c2b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44c2b-105">Представляет объекты, которые будут подготовлены к работе, и выполняемые правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="44c2b-105">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="44c2b-106">Ресурс в основном используется для подготовки по требованию.</span><span class="sxs-lookup"><span data-stu-id="44c2b-106">The resource is primarily used for on-demand provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="44c2b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="44c2b-107">Properties</span></span>
|<span data-ttu-id="44c2b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="44c2b-108">Property</span></span>|<span data-ttu-id="44c2b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="44c2b-109">Type</span></span>|<span data-ttu-id="44c2b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="44c2b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44c2b-111">ruleId</span><span class="sxs-lookup"><span data-stu-id="44c2b-111">ruleId</span></span>|<span data-ttu-id="44c2b-112">String</span><span class="sxs-lookup"><span data-stu-id="44c2b-112">String</span></span>|<span data-ttu-id="44c2b-113">Идентификатор Синчронизатионруле, который требуется применить; необязательно для Синчронизатионжоб с одним Синчронизатионруле.</span><span class="sxs-lookup"><span data-stu-id="44c2b-113">The identifier of a the synchronizationRule to be applied; optional for a synchronizationJob with a single synchronizationRule.</span></span>|
|<span data-ttu-id="44c2b-114">вопросов</span><span class="sxs-lookup"><span data-stu-id="44c2b-114">subjects</span></span>|<span data-ttu-id="44c2b-115">Коллекция [синчронизатионжобсубжект](../resources/synchronization-synchronizationjobsubject.md)</span><span class="sxs-lookup"><span data-stu-id="44c2b-115">[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) collection</span></span>|<span data-ttu-id="44c2b-116">Идентификаторы одного или нескольких объектов, к которым применяется Синчронизатионжоб.</span><span class="sxs-lookup"><span data-stu-id="44c2b-116">The identifiers of one or more objects to which a synchronizationJob is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44c2b-117">Связи</span><span class="sxs-lookup"><span data-stu-id="44c2b-117">Relationships</span></span>
<span data-ttu-id="44c2b-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="44c2b-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="44c2b-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="44c2b-119">JSON representation</span></span>
<span data-ttu-id="44c2b-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44c2b-120">The following is a JSON representation of the resource.</span></span>
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
