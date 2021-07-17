---
title: тип ресурса connectionOperation
description: Описывает состояние асинхронного запроса для создания схемы Поиск (Майкрософт) подключения.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f81300c0fd2f895daccb816c86cdd7151c803b2d
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467478"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="e23d8-103">тип ресурса connectionOperation</span><span class="sxs-lookup"><span data-stu-id="e23d8-103">connectionOperation resource type</span></span>

<span data-ttu-id="e23d8-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="e23d8-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="e23d8-105">Описывает состояние асинхронного запроса для создания схемы Поиск (Майкрософт) [подключения.](externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="e23d8-105">Describes status of an asynchronous request to create a Microsoft Search connection [schema](externalconnectors-schema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e23d8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e23d8-106">Methods</span></span>
|<span data-ttu-id="e23d8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e23d8-107">Method</span></span>|<span data-ttu-id="e23d8-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="e23d8-108">Return type</span></span>|<span data-ttu-id="e23d8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e23d8-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e23d8-110">Get connectionOperation</span><span class="sxs-lookup"><span data-stu-id="e23d8-110">Get connectionOperation</span></span>](../api/externalconnectors-connectionoperation-get.md)|[<span data-ttu-id="e23d8-111">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="e23d8-111">connectionOperation</span></span>](../resources/externalconnectors-connectionoperation.md)|<span data-ttu-id="e23d8-112">Ознакомьтесь с свойствами и отношениями объекта [connectionOperation.](../resources/externalconnectors-connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="e23d8-112">Read the properties and relationships of a [connectionOperation](../resources/externalconnectors-connectionoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e23d8-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="e23d8-113">Properties</span></span>
|<span data-ttu-id="e23d8-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="e23d8-114">Property</span></span>|<span data-ttu-id="e23d8-115">Тип</span><span class="sxs-lookup"><span data-stu-id="e23d8-115">Type</span></span>|<span data-ttu-id="e23d8-116">Описание</span><span class="sxs-lookup"><span data-stu-id="e23d8-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e23d8-117">error</span><span class="sxs-lookup"><span data-stu-id="e23d8-117">error</span></span>|<span data-ttu-id="e23d8-118">publicError</span><span class="sxs-lookup"><span data-stu-id="e23d8-118">publicError</span></span>| <span data-ttu-id="e23d8-119">Если `status` это `failed` так, предоставляет дополнительные сведения об ошибке, которая привела к сбою.</span><span class="sxs-lookup"><span data-stu-id="e23d8-119">If `status` is `failed`, provides more information about the error that caused the failure.</span></span>|
|<span data-ttu-id="e23d8-120">id</span><span class="sxs-lookup"><span data-stu-id="e23d8-120">id</span></span>|<span data-ttu-id="e23d8-121">String</span><span class="sxs-lookup"><span data-stu-id="e23d8-121">String</span></span>| <span data-ttu-id="e23d8-122">Уникальный идентификатор для подключенияOperation.</span><span class="sxs-lookup"><span data-stu-id="e23d8-122">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="e23d8-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e23d8-123">Read-only.</span></span> |
|<span data-ttu-id="e23d8-124">status</span><span class="sxs-lookup"><span data-stu-id="e23d8-124">status</span></span>|<span data-ttu-id="e23d8-125">microsoft.graph.externalConnectors.connectionOperationStatus</span><span class="sxs-lookup"><span data-stu-id="e23d8-125">microsoft.graph.externalConnectors.connectionOperationStatus</span></span>| <span data-ttu-id="e23d8-126">Указывает состояние асинхронной операции.</span><span class="sxs-lookup"><span data-stu-id="e23d8-126">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="e23d8-127">Возможные значения: `unspecified`, `inprogress`, `completed`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e23d8-127">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e23d8-128">Связи</span><span class="sxs-lookup"><span data-stu-id="e23d8-128">Relationships</span></span>
<span data-ttu-id="e23d8-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e23d8-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e23d8-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e23d8-130">JSON representation</span></span>
<span data-ttu-id="e23d8-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e23d8-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "status": "String"
}
```

