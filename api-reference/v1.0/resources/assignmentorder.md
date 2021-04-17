---
title: тип ресурса assignmentOrder
description: Определяет порядок атрибутов, собираемого в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c5faed250c07d5c4416c91a5452f1276c6b728e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883061"
---
# <a name="assignmentorder-resource-type"></a><span data-ttu-id="33753-103">тип ресурса assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="33753-103">assignmentOrder resource type</span></span>

<span data-ttu-id="33753-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33753-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33753-105">Используется для определения порядка атрибутов, собираемого в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="33753-105">Used to define the order of the attributes being collected within a user flow.</span></span> <span data-ttu-id="33753-106">Порядок определяет отображение страницы коллекции атрибутов при записи пользователя с помощью пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="33753-106">The order determines how the attribute collection page is displayed when a user signs up using a user flow.</span></span>

## <a name="properties"></a><span data-ttu-id="33753-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="33753-107">Properties</span></span>

|<span data-ttu-id="33753-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="33753-108">Property</span></span>|<span data-ttu-id="33753-109">Тип</span><span class="sxs-lookup"><span data-stu-id="33753-109">Type</span></span>|<span data-ttu-id="33753-110">Описание</span><span class="sxs-lookup"><span data-stu-id="33753-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33753-111">порядок</span><span class="sxs-lookup"><span data-stu-id="33753-111">order</span></span>|<span data-ttu-id="33753-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="33753-112">String collection</span></span>|<span data-ttu-id="33753-113">Список идентификаторов объектов identityUserFlowAttribute, определяющих порядок сбора атрибутов в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="33753-113">A list of identityUserFlowAttribute object identifiers that determine the order in which attributes should be collected within a user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33753-114">Связи</span><span class="sxs-lookup"><span data-stu-id="33753-114">Relationships</span></span>

<span data-ttu-id="33753-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="33753-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="33753-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="33753-116">JSON representation</span></span>

<span data-ttu-id="33753-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33753-117">The following is a JSON representation of the resource.</span></span>
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
