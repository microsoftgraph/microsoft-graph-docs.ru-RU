---
title: тип ресурса printerCreateOperation
description: Представляет собой операцию длительной регистрации принтера. Производный от printOperation.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 31d872ba84df3fcdd4f246cbd32b3668d21e57d5
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517344"
---
# <a name="printercreateoperation-resource-type"></a><span data-ttu-id="20a06-104">тип ресурса printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="20a06-104">printerCreateOperation resource type</span></span>

<span data-ttu-id="20a06-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20a06-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="20a06-106">Представляет собой операцию длительной регистрации принтера.</span><span class="sxs-lookup"><span data-stu-id="20a06-106">Represents a long-running printer registration operation.</span></span> <span data-ttu-id="20a06-107">Производные от [printOperation](printoperation.md).</span><span class="sxs-lookup"><span data-stu-id="20a06-107">Derived from [printOperation](printoperation.md).</span></span>

<span data-ttu-id="20a06-108">Наследует [от printOperation](printoperation.md).</span><span class="sxs-lookup"><span data-stu-id="20a06-108">Inherits from [printOperation](printoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="20a06-109">Методы</span><span class="sxs-lookup"><span data-stu-id="20a06-109">Methods</span></span>
|<span data-ttu-id="20a06-110">Метод</span><span class="sxs-lookup"><span data-stu-id="20a06-110">Method</span></span>|<span data-ttu-id="20a06-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="20a06-111">Return type</span></span>|<span data-ttu-id="20a06-112">Описание</span><span class="sxs-lookup"><span data-stu-id="20a06-112">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="20a06-113">Получить операцию</span><span class="sxs-lookup"><span data-stu-id="20a06-113">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="20a06-114">printOperation</span><span class="sxs-lookup"><span data-stu-id="20a06-114">printOperation</span></span>](printoperation.md) | <span data-ttu-id="20a06-115">Извлечение длительной операции в текущем пользователе или клиенте приложения.</span><span class="sxs-lookup"><span data-stu-id="20a06-115">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="20a06-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="20a06-116">Properties</span></span>
|<span data-ttu-id="20a06-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="20a06-117">Property</span></span>|<span data-ttu-id="20a06-118">Тип</span><span class="sxs-lookup"><span data-stu-id="20a06-118">Type</span></span>|<span data-ttu-id="20a06-119">Описание</span><span class="sxs-lookup"><span data-stu-id="20a06-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20a06-120">id</span><span class="sxs-lookup"><span data-stu-id="20a06-120">id</span></span>|<span data-ttu-id="20a06-121">Строка</span><span class="sxs-lookup"><span data-stu-id="20a06-121">String</span></span>|<span data-ttu-id="20a06-122">Идентификатор операции.</span><span class="sxs-lookup"><span data-stu-id="20a06-122">The operation's identifier.</span></span> <span data-ttu-id="20a06-123">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20a06-123">Read-only.</span></span>|
|<span data-ttu-id="20a06-124">status</span><span class="sxs-lookup"><span data-stu-id="20a06-124">status</span></span>|[<span data-ttu-id="20a06-125">printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="20a06-125">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="20a06-126">Состояние операции регистрации.</span><span class="sxs-lookup"><span data-stu-id="20a06-126">The status of the registration operation.</span></span> <span data-ttu-id="20a06-127">Содержит ход операции и ее успешное завершения.</span><span class="sxs-lookup"><span data-stu-id="20a06-127">Contains the operation's progress and whether it completed successfully.</span></span> <span data-ttu-id="20a06-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20a06-128">Read-only.</span></span>|
|<span data-ttu-id="20a06-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20a06-129">createdDateTime</span></span>|<span data-ttu-id="20a06-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20a06-130">DateTimeOffset</span></span>|<span data-ttu-id="20a06-131">DateTimeOffset, когда была создана операция.</span><span class="sxs-lookup"><span data-stu-id="20a06-131">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="20a06-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20a06-132">Read-only.</span></span>|
|<span data-ttu-id="20a06-133">certificate</span><span class="sxs-lookup"><span data-stu-id="20a06-133">certificate</span></span>|<span data-ttu-id="20a06-134">String</span><span class="sxs-lookup"><span data-stu-id="20a06-134">String</span></span>|<span data-ttu-id="20a06-135">Подписанный сертификат, созданный в процессе регистрации.</span><span class="sxs-lookup"><span data-stu-id="20a06-135">The signed certificate created during the registration process.</span></span> <span data-ttu-id="20a06-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20a06-136">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20a06-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="20a06-137">Relationships</span></span>
|<span data-ttu-id="20a06-138">Связь</span><span class="sxs-lookup"><span data-stu-id="20a06-138">Relationship</span></span>|<span data-ttu-id="20a06-139">Тип</span><span class="sxs-lookup"><span data-stu-id="20a06-139">Type</span></span>|<span data-ttu-id="20a06-140">Описание</span><span class="sxs-lookup"><span data-stu-id="20a06-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20a06-141">printer</span><span class="sxs-lookup"><span data-stu-id="20a06-141">printer</span></span>|[<span data-ttu-id="20a06-142">printer</span><span class="sxs-lookup"><span data-stu-id="20a06-142">printer</span></span>](printer.md)|<span data-ttu-id="20a06-143">Созданный объект принтера.</span><span class="sxs-lookup"><span data-stu-id="20a06-143">The created printer entity.</span></span> <span data-ttu-id="20a06-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20a06-144">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20a06-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20a06-145">JSON representation</span></span>
<span data-ttu-id="20a06-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20a06-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "baseType": "microsoft.graph.printOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCreateOperation",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printOperationStatus"
  },
  "createdDateTime": "String (timestamp)",
  "certificate": "String"
}
```

