---
title: Тип ресурса dataSource
description: Объект DataSource — абстрактный базовый класс
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 645ae33eb6c43972122623e52bfecf17f39491e4
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597830"
---
# <a name="datasource-resource-type"></a><span data-ttu-id="ac5f5-103">Тип ресурса dataSource</span><span class="sxs-lookup"><span data-stu-id="ac5f5-103">dataSource resource type</span></span>

<span data-ttu-id="ac5f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac5f5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac5f5-105">Сущность dataSource — это абстрактный объект BaseClass, используемый для определения источников контента для обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="ac5f5-105">The dataSource entity is an abstract baseclass used to identify sources of content for eDiscovery.</span></span>

## <a name="methods"></a><span data-ttu-id="ac5f5-106">Methods</span><span class="sxs-lookup"><span data-stu-id="ac5f5-106">Methods</span></span>

<span data-ttu-id="ac5f5-107">Нет</span><span class="sxs-lookup"><span data-stu-id="ac5f5-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="ac5f5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac5f5-108">Properties</span></span>

|<span data-ttu-id="ac5f5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac5f5-109">Property</span></span>|<span data-ttu-id="ac5f5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ac5f5-110">Type</span></span>|<span data-ttu-id="ac5f5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ac5f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac5f5-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="ac5f5-112">createdBy</span></span>|[<span data-ttu-id="ac5f5-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="ac5f5-113">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="ac5f5-114">Пользователь, создавший **источник данных**.</span><span class="sxs-lookup"><span data-stu-id="ac5f5-114">The user who created the **dataSource**.</span></span>|
|<span data-ttu-id="ac5f5-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac5f5-115">createdDateTime</span></span>|<span data-ttu-id="ac5f5-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac5f5-116">DateTimeOffset</span></span>|<span data-ttu-id="ac5f5-117">Дата и время создания **источника данных** .</span><span class="sxs-lookup"><span data-stu-id="ac5f5-117">The date and time the **dataSource** was created.</span></span>|
|<span data-ttu-id="ac5f5-118">displayName</span><span class="sxs-lookup"><span data-stu-id="ac5f5-118">displayName</span></span>|<span data-ttu-id="ac5f5-119">String</span><span class="sxs-lookup"><span data-stu-id="ac5f5-119">String</span></span>|<span data-ttu-id="ac5f5-120">Отображаемое имя **источника данных**.</span><span class="sxs-lookup"><span data-stu-id="ac5f5-120">The display name of the **dataSource**.</span></span> <span data-ttu-id="ac5f5-121">Это будет имя сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ac5f5-121">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="ac5f5-122">id</span><span class="sxs-lookup"><span data-stu-id="ac5f5-122">id</span></span>|<span data-ttu-id="ac5f5-123">String</span><span class="sxs-lookup"><span data-stu-id="ac5f5-123">String</span></span>| <span data-ttu-id="ac5f5-124">Идентификатор **источника данных**.</span><span class="sxs-lookup"><span data-stu-id="ac5f5-124">The ID of the **dataSource**.</span></span> <span data-ttu-id="ac5f5-125">Это значение не является ИДЕНТИФИКАТОРом действительного сайта.</span><span class="sxs-lookup"><span data-stu-id="ac5f5-125">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac5f5-126">Связи</span><span class="sxs-lookup"><span data-stu-id="ac5f5-126">Relationships</span></span>

<span data-ttu-id="ac5f5-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ac5f5-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac5f5-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ac5f5-128">JSON representation</span></span>

<span data-ttu-id="ac5f5-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac5f5-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSource",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
