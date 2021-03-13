---
title: тип bitlocker
description: Ресурс BitLocker
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3e714015b3834051371861880355360f02d12166
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761837"
---
# <a name="bitlocker-resource-type"></a><span data-ttu-id="76d92-103">тип ресурса bitlocker</span><span class="sxs-lookup"><span data-stu-id="76d92-103">bitlocker resource type</span></span>

<span data-ttu-id="76d92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76d92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76d92-105">Родительский ресурс для сохраненного ключа BitLocker с свойством навигации **bitlockerRecoveryKey,** который содержит фактический ключ восстановления.</span><span class="sxs-lookup"><span data-stu-id="76d92-105">The parent resource for a stored BitLocker key with the navigation property **bitlockerRecoveryKey** which contains the actual recovery key.</span></span>

## <a name="methods"></a><span data-ttu-id="76d92-106">Методы</span><span class="sxs-lookup"><span data-stu-id="76d92-106">Methods</span></span>
|<span data-ttu-id="76d92-107">Метод</span><span class="sxs-lookup"><span data-stu-id="76d92-107">Method</span></span>|<span data-ttu-id="76d92-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="76d92-108">Return type</span></span>|<span data-ttu-id="76d92-109">Описание</span><span class="sxs-lookup"><span data-stu-id="76d92-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="76d92-110">Список recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="76d92-110">List recoveryKeys</span></span>](../api/bitlocker-list-recoverykeys.md)|<span data-ttu-id="76d92-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span><span class="sxs-lookup"><span data-stu-id="76d92-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span>|<span data-ttu-id="76d92-112">Получите список объектов bitlockerRecoveryKey и их свойств.</span><span class="sxs-lookup"><span data-stu-id="76d92-112">Get a list of the bitlockerRecoveryKey objects and their properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="76d92-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="76d92-113">Properties</span></span>
<span data-ttu-id="76d92-114">Нет</span><span class="sxs-lookup"><span data-stu-id="76d92-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="76d92-115">Связи</span><span class="sxs-lookup"><span data-stu-id="76d92-115">Relationships</span></span>
| <span data-ttu-id="76d92-116">Связь</span><span class="sxs-lookup"><span data-stu-id="76d92-116">Relationship</span></span> | <span data-ttu-id="76d92-117">Тип</span><span class="sxs-lookup"><span data-stu-id="76d92-117">Type</span></span> | <span data-ttu-id="76d92-118">Описание</span><span class="sxs-lookup"><span data-stu-id="76d92-118">Description</span></span> |
|--|--|--|
| <span data-ttu-id="76d92-119">recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="76d92-119">recoveryKeys</span></span> | <span data-ttu-id="76d92-120">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span><span class="sxs-lookup"><span data-stu-id="76d92-120">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span> | <span data-ttu-id="76d92-121">Ключи восстановления, связанные с объектом bitlocker.</span><span class="sxs-lookup"><span data-stu-id="76d92-121">The recovery keys associated with the bitlocker entity.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="76d92-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76d92-122">JSON representation</span></span>
<span data-ttu-id="76d92-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76d92-123">The following is a JSON representation of the resource.</span></span>
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

