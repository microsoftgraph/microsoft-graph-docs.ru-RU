---
title: тип ресурса assignmentOrder
description: Используется для определения порядка атрибутов, собираемого в потоке пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7d7716cb4b13917aad33cd88afeb364a2891e3df
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761242"
---
# <a name="assignmentorder-resource-type"></a><span data-ttu-id="fc2db-103">тип ресурса assignmentOrder</span><span class="sxs-lookup"><span data-stu-id="fc2db-103">assignmentOrder resource type</span></span>

<span data-ttu-id="fc2db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc2db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc2db-105">Используется для определения порядка атрибутов, собираемого в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="fc2db-105">Used to define the order of the attributes being collected within a user flow.</span></span> <span data-ttu-id="fc2db-106">THis определяет отображение страницы коллекции атрибутов при записи пользователя в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="fc2db-106">THis determines how the attribute collection page is displayed when a user signs up via a user flow.</span></span>

## <a name="properties"></a><span data-ttu-id="fc2db-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc2db-107">Properties</span></span>

|<span data-ttu-id="fc2db-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc2db-108">Property</span></span>|<span data-ttu-id="fc2db-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fc2db-109">Type</span></span>|<span data-ttu-id="fc2db-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fc2db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc2db-111">порядок</span><span class="sxs-lookup"><span data-stu-id="fc2db-111">order</span></span>|<span data-ttu-id="fc2db-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc2db-112">String collection</span></span>|<span data-ttu-id="fc2db-113">Список идентификаторов identityUserFlowAttribute, предоставленных для определения порядка сбора атрибутов в потоке пользователей.</span><span class="sxs-lookup"><span data-stu-id="fc2db-113">A list of identityUserFlowAttribute IDs provided to determine the order in which attributes should be collected within a user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc2db-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="fc2db-114">Relationships</span></span>

<span data-ttu-id="fc2db-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fc2db-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc2db-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fc2db-116">JSON representation</span></span>

<span data-ttu-id="fc2db-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc2db-117">The following is a JSON representation of the resource.</span></span>
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
