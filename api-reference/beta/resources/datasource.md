---
title: Тип ресурса dataSource
description: Объект Datasource — абстрактный базовый класс
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: c019a6b8338180584a31382c0741018791973184
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161924"
---
# <a name="datasource-resource-type"></a><span data-ttu-id="3aa0a-103">Тип ресурса dataSource</span><span class="sxs-lookup"><span data-stu-id="3aa0a-103">dataSource resource type</span></span>

<span data-ttu-id="3aa0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3aa0a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3aa0a-105">Объект dataSource — это абстрактный базовый класс, используемый для определения источников контента для eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="3aa0a-105">The dataSource entity is an abstract baseclass used to identify sources of content for eDiscovery.</span></span>

## <a name="methods"></a><span data-ttu-id="3aa0a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="3aa0a-106">Methods</span></span>

<span data-ttu-id="3aa0a-107">Нет</span><span class="sxs-lookup"><span data-stu-id="3aa0a-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="3aa0a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3aa0a-108">Properties</span></span>

|<span data-ttu-id="3aa0a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3aa0a-109">Property</span></span>|<span data-ttu-id="3aa0a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3aa0a-110">Type</span></span>|<span data-ttu-id="3aa0a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3aa0a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3aa0a-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="3aa0a-112">createdBy</span></span>|[<span data-ttu-id="3aa0a-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="3aa0a-113">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="3aa0a-114">Пользователь, создавший **dataSource.**</span><span class="sxs-lookup"><span data-stu-id="3aa0a-114">The user who created the **dataSource**.</span></span>|
|<span data-ttu-id="3aa0a-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3aa0a-115">createdDateTime</span></span>|<span data-ttu-id="3aa0a-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3aa0a-116">DateTimeOffset</span></span>|<span data-ttu-id="3aa0a-117">Дата и время создания **dataSource.**</span><span class="sxs-lookup"><span data-stu-id="3aa0a-117">The date and time the **dataSource** was created.</span></span>|
|<span data-ttu-id="3aa0a-118">displayName</span><span class="sxs-lookup"><span data-stu-id="3aa0a-118">displayName</span></span>|<span data-ttu-id="3aa0a-119">String</span><span class="sxs-lookup"><span data-stu-id="3aa0a-119">String</span></span>|<span data-ttu-id="3aa0a-120">Отображаемого имени **dataSource**.</span><span class="sxs-lookup"><span data-stu-id="3aa0a-120">The display name of the **dataSource**.</span></span> <span data-ttu-id="3aa0a-121">Это имя сайта SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3aa0a-121">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="3aa0a-122">id</span><span class="sxs-lookup"><span data-stu-id="3aa0a-122">id</span></span>|<span data-ttu-id="3aa0a-123">String</span><span class="sxs-lookup"><span data-stu-id="3aa0a-123">String</span></span>| <span data-ttu-id="3aa0a-124">ИД **dataSource.**</span><span class="sxs-lookup"><span data-stu-id="3aa0a-124">The ID of the **dataSource**.</span></span> <span data-ttu-id="3aa0a-125">Это не ИД фактического сайта.</span><span class="sxs-lookup"><span data-stu-id="3aa0a-125">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3aa0a-126">Связи</span><span class="sxs-lookup"><span data-stu-id="3aa0a-126">Relationships</span></span>

<span data-ttu-id="3aa0a-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3aa0a-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3aa0a-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3aa0a-128">JSON representation</span></span>

<span data-ttu-id="3aa0a-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3aa0a-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSource",
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
