---
title: Тип ресурса dataSource
description: Объект dataSource — это абстрактный базовый класс, используемый для определения источников контента для электронных данных.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 2f945ba74a5576a35146ee1832f3740b537ed23b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447383"
---
# <a name="datasource-resource-type"></a><span data-ttu-id="7c408-103">Тип ресурса dataSource</span><span class="sxs-lookup"><span data-stu-id="7c408-103">dataSource resource type</span></span>

<span data-ttu-id="7c408-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="7c408-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c408-105">Объект dataSource — это абстрактный базовый класс, используемый для определения источников контента для электронных данных.</span><span class="sxs-lookup"><span data-stu-id="7c408-105">The dataSource entity is an abstract base class used to identify sources of content for eDiscovery.</span></span>

## <a name="methods"></a><span data-ttu-id="7c408-106">Methods</span><span class="sxs-lookup"><span data-stu-id="7c408-106">Methods</span></span>

<span data-ttu-id="7c408-107">Нет</span><span class="sxs-lookup"><span data-stu-id="7c408-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="7c408-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c408-108">Properties</span></span>

|<span data-ttu-id="7c408-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c408-109">Property</span></span>|<span data-ttu-id="7c408-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7c408-110">Type</span></span>|<span data-ttu-id="7c408-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7c408-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c408-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="7c408-112">createdBy</span></span>|[<span data-ttu-id="7c408-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="7c408-113">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="7c408-114">Пользователь, создавший **dataSource.**</span><span class="sxs-lookup"><span data-stu-id="7c408-114">The user who created the **dataSource**.</span></span>|
|<span data-ttu-id="7c408-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c408-115">createdDateTime</span></span>|<span data-ttu-id="7c408-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c408-116">DateTimeOffset</span></span>|<span data-ttu-id="7c408-117">Дата и время **создания dataSource.**</span><span class="sxs-lookup"><span data-stu-id="7c408-117">The date and time the **dataSource** was created.</span></span>|
|<span data-ttu-id="7c408-118">displayName</span><span class="sxs-lookup"><span data-stu-id="7c408-118">displayName</span></span>|<span data-ttu-id="7c408-119">String</span><span class="sxs-lookup"><span data-stu-id="7c408-119">String</span></span>|<span data-ttu-id="7c408-120">Имя отображения **dataSource**.</span><span class="sxs-lookup"><span data-stu-id="7c408-120">The display name of the **dataSource**.</span></span> <span data-ttu-id="7c408-121">Это будет имя сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7c408-121">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="7c408-122">id</span><span class="sxs-lookup"><span data-stu-id="7c408-122">id</span></span>|<span data-ttu-id="7c408-123">String</span><span class="sxs-lookup"><span data-stu-id="7c408-123">String</span></span>| <span data-ttu-id="7c408-124">ID **dataSource**.</span><span class="sxs-lookup"><span data-stu-id="7c408-124">The ID of the **dataSource**.</span></span> <span data-ttu-id="7c408-125">Это не ID фактического сайта.</span><span class="sxs-lookup"><span data-stu-id="7c408-125">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c408-126">Связи</span><span class="sxs-lookup"><span data-stu-id="7c408-126">Relationships</span></span>

<span data-ttu-id="7c408-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7c408-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c408-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7c408-128">JSON representation</span></span>

<span data-ttu-id="7c408-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c408-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.dataSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
