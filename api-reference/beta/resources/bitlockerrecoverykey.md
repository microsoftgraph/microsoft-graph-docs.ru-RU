---
title: тип ресурса bitlockerRecoveryKey
description: Ресурс ключа восстановления BitLocker
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 466a5d907b3deb589ec1b70351903e24aba0ab32
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443155"
---
# <a name="bitlockerrecoverykey-resource-type"></a><span data-ttu-id="e6e10-103">тип ресурса bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="e6e10-103">bitlockerRecoveryKey resource type</span></span>

<span data-ttu-id="e6e10-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6e10-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6e10-105">Представляет сохраненный ключ BitLocker, содержащий фактический ключ восстановления с помощью **свойства ключа.**</span><span class="sxs-lookup"><span data-stu-id="e6e10-105">Represents a stored BitLocker key that contains the actual recovery key via the **key** property.</span></span>

## <a name="methods"></a><span data-ttu-id="e6e10-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e6e10-106">Methods</span></span>
|<span data-ttu-id="e6e10-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e6e10-107">Method</span></span>|<span data-ttu-id="e6e10-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="e6e10-108">Return type</span></span>|<span data-ttu-id="e6e10-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e6e10-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6e10-110">Список recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="e6e10-110">List recoveryKeys</span></span>](../api/bitlocker-list-recoverykeys.md)|<span data-ttu-id="e6e10-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span><span class="sxs-lookup"><span data-stu-id="e6e10-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span>|<span data-ttu-id="e6e10-112">Получите список объектов [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="e6e10-112">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span>|
|[<span data-ttu-id="e6e10-113">Get bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="e6e10-113">Get bitlockerRecoveryKey</span></span>](../api/bitlockerrecoverykey-get.md)|[<span data-ttu-id="e6e10-114">bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="e6e10-114">bitlockerRecoveryKey</span></span>](../resources/bitlockerrecoverykey.md)|<span data-ttu-id="e6e10-115">Извлечение свойств и связей [объекта bitlockerRecoveryKey.](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="e6e10-115">Retrieve the properties and relationships of a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object.</span></span> <span data-ttu-id="e6e10-116">Примечание. **Свойство ключа** не возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e6e10-116">Note: The **key** property is not returned by default.</span></span>|

> <span data-ttu-id="e6e10-117">**Примечание.** Только некоторые роли имеют разрешения на вызов этих API.</span><span class="sxs-lookup"><span data-stu-id="e6e10-117">**Note**: Only some roles have the permissions to call these APIs.</span></span>

## <a name="properties"></a><span data-ttu-id="e6e10-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6e10-118">Properties</span></span>
|<span data-ttu-id="e6e10-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6e10-119">Property</span></span>|<span data-ttu-id="e6e10-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e6e10-120">Type</span></span>|<span data-ttu-id="e6e10-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e6e10-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6e10-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6e10-122">createdDateTime</span></span>|<span data-ttu-id="e6e10-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6e10-123">DateTimeOffset</span></span>|<span data-ttu-id="e6e10-124">Дата и время, когда клавиша изначально была отсвеяна в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e6e10-124">The date and time when the key was originally backed up to Azure Active Directory.</span></span>|
|<span data-ttu-id="e6e10-125">deviceId</span><span class="sxs-lookup"><span data-stu-id="e6e10-125">deviceId</span></span>|<span data-ttu-id="e6e10-126">String</span><span class="sxs-lookup"><span data-stu-id="e6e10-126">String</span></span>|<span data-ttu-id="e6e10-127">ID устройства с ключом BitLocker изначально отсвеяли.</span><span class="sxs-lookup"><span data-stu-id="e6e10-127">ID of the device the BitLocker key is originally backed up from.</span></span>|
|<span data-ttu-id="e6e10-128">id</span><span class="sxs-lookup"><span data-stu-id="e6e10-128">id</span></span>|<span data-ttu-id="e6e10-129">String</span><span class="sxs-lookup"><span data-stu-id="e6e10-129">String</span></span>|<span data-ttu-id="e6e10-130">Уникальный идентификатор для ключа BitLocker.</span><span class="sxs-lookup"><span data-stu-id="e6e10-130">The unique identifier for the BitLocker key.</span></span>|
|<span data-ttu-id="e6e10-131">ключа</span><span class="sxs-lookup"><span data-stu-id="e6e10-131">key</span></span>|<span data-ttu-id="e6e10-132">String</span><span class="sxs-lookup"><span data-stu-id="e6e10-132">String</span></span>|<span data-ttu-id="e6e10-133">Ключ восстановления BitLocker.</span><span class="sxs-lookup"><span data-stu-id="e6e10-133">The BitLocker recovery key.</span></span>|
|<span data-ttu-id="e6e10-134">volumeType</span><span class="sxs-lookup"><span data-stu-id="e6e10-134">volumeType</span></span>|<span data-ttu-id="e6e10-135">volumeType</span><span class="sxs-lookup"><span data-stu-id="e6e10-135">volumeType</span></span>|<span data-ttu-id="e6e10-136">Указывает тип тома, с чем связан ключ BitLocker.</span><span class="sxs-lookup"><span data-stu-id="e6e10-136">Indicates the type of volume the BitLocker key is associated with.</span></span> <span data-ttu-id="e6e10-137">Возможные значения: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e6e10-137">Possible values are: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6e10-138">Связи</span><span class="sxs-lookup"><span data-stu-id="e6e10-138">Relationships</span></span>
<span data-ttu-id="e6e10-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e6e10-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6e10-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e6e10-140">JSON representation</span></span>
<span data-ttu-id="e6e10-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6e10-141">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
  "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
  "createdDateTime": "2020-06-15T13:45:30.0000000Z",
  "volumeType": 1,
  "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
  "key": "123456-231453-873456-213546-654678-765689-123456-324565"
}
```

