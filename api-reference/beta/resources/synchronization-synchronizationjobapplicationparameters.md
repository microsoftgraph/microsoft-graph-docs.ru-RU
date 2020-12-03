---
title: Тип ресурса Синчронизатионжобаппликатионпараметерс
description: Представляет объекты, которые необходимо подготовить, и правила, выполняемые при подготовке по требованию.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ca91021ccb9fbc4cf8ec6c61b4edea979bb7c833
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523205"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a><span data-ttu-id="2d168-103">Тип ресурса Синчронизатионжобаппликатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="2d168-103">synchronizationJobApplicationParameters resource type</span></span>

<span data-ttu-id="2d168-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d168-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d168-105">Представляет объекты, которые будут подготовлены к работе, и выполняемые правила синхронизации.</span><span class="sxs-lookup"><span data-stu-id="2d168-105">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="2d168-106">Ресурс в основном используется для подготовки по требованию.</span><span class="sxs-lookup"><span data-stu-id="2d168-106">The resource is primarily used for on-demand provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="2d168-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d168-107">Properties</span></span>
|<span data-ttu-id="2d168-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d168-108">Property</span></span>|<span data-ttu-id="2d168-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2d168-109">Type</span></span>|<span data-ttu-id="2d168-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2d168-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d168-111">ruleId</span><span class="sxs-lookup"><span data-stu-id="2d168-111">ruleId</span></span>|<span data-ttu-id="2d168-112">String</span><span class="sxs-lookup"><span data-stu-id="2d168-112">String</span></span>|<span data-ttu-id="2d168-113">Идентификатор Синчронизатионруле, который требуется применить.</span><span class="sxs-lookup"><span data-stu-id="2d168-113">The identifier of a the synchronizationRule to be applied.</span></span>|
|<span data-ttu-id="2d168-114">вопросов</span><span class="sxs-lookup"><span data-stu-id="2d168-114">subjects</span></span>|<span data-ttu-id="2d168-115">Коллекция [синчронизатионжобсубжект](../resources/synchronization-synchronizationjobsubject.md)</span><span class="sxs-lookup"><span data-stu-id="2d168-115">[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) collection</span></span>|<span data-ttu-id="2d168-116">Идентификаторы одного или нескольких объектов, к которым применяется Синчронизатионжоб.</span><span class="sxs-lookup"><span data-stu-id="2d168-116">The identifiers of one or more objects to which a synchronizationJob is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d168-117">Связи</span><span class="sxs-lookup"><span data-stu-id="2d168-117">Relationships</span></span>
<span data-ttu-id="2d168-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2d168-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d168-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2d168-119">JSON representation</span></span>
<span data-ttu-id="2d168-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d168-120">The following is a JSON representation of the resource.</span></span>
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


