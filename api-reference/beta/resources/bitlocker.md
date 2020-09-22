---
title: Тип BitLocker
description: Ресурс BitLocker
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3ad8a05e82cd3f300bedf034fe18f67ce3359f16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038877"
---
# <a name="bitlocker-resource-type"></a><span data-ttu-id="8f541-103">Тип ресурса BitLocker</span><span class="sxs-lookup"><span data-stu-id="8f541-103">bitlocker resource type</span></span>

<span data-ttu-id="8f541-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f541-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f541-105">Родительский ресурс для сохраненного ключа BitLocker с помощью свойства навигации **битлоккеррековерикэй** , содержащего фактический ключ восстановления.</span><span class="sxs-lookup"><span data-stu-id="8f541-105">The parent resource for a stored BitLocker key with the navigation property **bitlockerRecoveryKey** which contains the actual recovery key.</span></span>

## <a name="methods"></a><span data-ttu-id="8f541-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8f541-106">Methods</span></span>
|<span data-ttu-id="8f541-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8f541-107">Method</span></span>|<span data-ttu-id="8f541-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="8f541-108">Return type</span></span>|<span data-ttu-id="8f541-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8f541-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8f541-110">Список Рековерикэйс</span><span class="sxs-lookup"><span data-stu-id="8f541-110">List recoveryKeys</span></span>](../api/bitlocker-list-recoverykeys.md)|<span data-ttu-id="8f541-111">Коллекция [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="8f541-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span>|<span data-ttu-id="8f541-112">Получение списка объектов Битлоккеррековерикэй и их свойств.</span><span class="sxs-lookup"><span data-stu-id="8f541-112">Get a list of the bitlockerRecoveryKey objects and their properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f541-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f541-113">Properties</span></span>
<span data-ttu-id="8f541-114">Нет</span><span class="sxs-lookup"><span data-stu-id="8f541-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="8f541-115">Связи</span><span class="sxs-lookup"><span data-stu-id="8f541-115">Relationships</span></span>
| <span data-ttu-id="8f541-116">Связь</span><span class="sxs-lookup"><span data-stu-id="8f541-116">Relationship</span></span> | <span data-ttu-id="8f541-117">Тип</span><span class="sxs-lookup"><span data-stu-id="8f541-117">Type</span></span> | <span data-ttu-id="8f541-118">Описание</span><span class="sxs-lookup"><span data-stu-id="8f541-118">Description</span></span> |
|--|--|--|
| <span data-ttu-id="8f541-119">рековерикэйс</span><span class="sxs-lookup"><span data-stu-id="8f541-119">recoveryKeys</span></span> | <span data-ttu-id="8f541-120">Коллекция [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="8f541-120">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span> | <span data-ttu-id="8f541-121">Ключи восстановления, связанные с сущностью BitLocker.</span><span class="sxs-lookup"><span data-stu-id="8f541-121">The recovery keys associated with the bitlocker entity.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8f541-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f541-122">JSON representation</span></span>
<span data-ttu-id="8f541-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f541-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitlocker",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitlocker"
}
```

