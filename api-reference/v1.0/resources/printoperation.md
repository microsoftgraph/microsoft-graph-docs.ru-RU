---
title: тип ресурса printOperation
description: Представляет собой долгосрочную операцию универсальной печати. Базовый класс для типов операций, таких как printerCreateOperation.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9a397a0166ad62a503027499e9e0f5fd4f127b1e
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518057"
---
# <a name="printoperation-resource-type"></a><span data-ttu-id="4ac8e-104">тип ресурса printOperation</span><span class="sxs-lookup"><span data-stu-id="4ac8e-104">printOperation resource type</span></span>

<span data-ttu-id="4ac8e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ac8e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="4ac8e-106">Представляет собой долгосрочную операцию универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="4ac8e-106">Represents a long-running Universal Print operation.</span></span> <span data-ttu-id="4ac8e-107">Базовый класс для типов операций, таких как [printerCreateOperation.](printercreateoperation.md)</span><span class="sxs-lookup"><span data-stu-id="4ac8e-107">Base class for operation types such as [printerCreateOperation](printercreateoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4ac8e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4ac8e-108">Methods</span></span>
|<span data-ttu-id="4ac8e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4ac8e-109">Method</span></span>|<span data-ttu-id="4ac8e-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="4ac8e-110">Return type</span></span>|<span data-ttu-id="4ac8e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4ac8e-111">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="4ac8e-112">Получить операцию</span><span class="sxs-lookup"><span data-stu-id="4ac8e-112">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="4ac8e-113">printOperation</span><span class="sxs-lookup"><span data-stu-id="4ac8e-113">printOperation</span></span>](printoperation.md) | <span data-ttu-id="4ac8e-114">Извлечение длительной операции в текущем пользователе или клиенте приложения.</span><span class="sxs-lookup"><span data-stu-id="4ac8e-114">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="4ac8e-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ac8e-115">Properties</span></span>
|<span data-ttu-id="4ac8e-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ac8e-116">Property</span></span>|<span data-ttu-id="4ac8e-117">Тип</span><span class="sxs-lookup"><span data-stu-id="4ac8e-117">Type</span></span>|<span data-ttu-id="4ac8e-118">Описание</span><span class="sxs-lookup"><span data-stu-id="4ac8e-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ac8e-119">id</span><span class="sxs-lookup"><span data-stu-id="4ac8e-119">id</span></span>|<span data-ttu-id="4ac8e-120">Строка</span><span class="sxs-lookup"><span data-stu-id="4ac8e-120">String</span></span>|<span data-ttu-id="4ac8e-121">Идентификатор операции.</span><span class="sxs-lookup"><span data-stu-id="4ac8e-121">The operation's identifier.</span></span> <span data-ttu-id="4ac8e-122">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ac8e-122">Read-only.</span></span>|
|<span data-ttu-id="4ac8e-123">status</span><span class="sxs-lookup"><span data-stu-id="4ac8e-123">status</span></span>|[<span data-ttu-id="4ac8e-124">printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="4ac8e-124">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="4ac8e-125">Состояние операции.</span><span class="sxs-lookup"><span data-stu-id="4ac8e-125">The status of the operation.</span></span> <span data-ttu-id="4ac8e-126">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ac8e-126">Read-only.</span></span>|
|<span data-ttu-id="4ac8e-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ac8e-127">createdDateTime</span></span>|<span data-ttu-id="4ac8e-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ac8e-128">DateTimeOffset</span></span>|<span data-ttu-id="4ac8e-129">DateTimeOffset, когда была создана операция.</span><span class="sxs-lookup"><span data-stu-id="4ac8e-129">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="4ac8e-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ac8e-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ac8e-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="4ac8e-131">Relationships</span></span>
<span data-ttu-id="4ac8e-132">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4ac8e-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ac8e-133">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4ac8e-133">JSON representation</span></span>
<span data-ttu-id="4ac8e-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ac8e-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printOperation",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printOperationStatus"
  },
  "createdDateTime": "String (timestamp)"
}
```

