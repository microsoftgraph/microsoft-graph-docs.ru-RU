---
title: Тип ресурса Ассигнментордер
description: Используется для определения порядка атрибутов, собранных в пользовательском движении.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 41b75e1adf5459279b5675278a8f00a82110b457
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581338"
---
# <a name="assignmentorder-resource-type"></a><span data-ttu-id="a639f-103">Тип ресурса Ассигнментордер</span><span class="sxs-lookup"><span data-stu-id="a639f-103">assignmentOrder resource type</span></span>

<span data-ttu-id="a639f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a639f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a639f-105">Используется для определения порядка атрибутов, собранных в пользовательском движении.</span><span class="sxs-lookup"><span data-stu-id="a639f-105">Used to define the order of the attributes being collected within a user flow.</span></span> <span data-ttu-id="a639f-106">Этот параметр определяет способ отображения страницы коллекции атрибутов, когда пользователь подписывается через пользовательский ход.</span><span class="sxs-lookup"><span data-stu-id="a639f-106">THis determines how the attribute collection page is displayed when a user signs up via a user flow.</span></span>

## <a name="properties"></a><span data-ttu-id="a639f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a639f-107">Properties</span></span>

|<span data-ttu-id="a639f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a639f-108">Property</span></span>|<span data-ttu-id="a639f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a639f-109">Type</span></span>|<span data-ttu-id="a639f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a639f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a639f-111">порядке</span><span class="sxs-lookup"><span data-stu-id="a639f-111">order</span></span>|<span data-ttu-id="a639f-112">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a639f-112">String collection</span></span>|<span data-ttu-id="a639f-113">Список идентификаторов Идентитюсерфловаттрибуте, предоставляемых для определения порядка, в котором атрибуты должны быть собраны в пользовательском цикле.</span><span class="sxs-lookup"><span data-stu-id="a639f-113">A list of identityUserFlowAttribute IDs provided to determine the order in which attributes should be collected within a user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a639f-114">Связи</span><span class="sxs-lookup"><span data-stu-id="a639f-114">Relationships</span></span>

<span data-ttu-id="a639f-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a639f-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a639f-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a639f-116">JSON representation</span></span>

<span data-ttu-id="a639f-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a639f-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentOrder"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.assignmentOrder",
  "order": [
    "String"
  ]
}
```
