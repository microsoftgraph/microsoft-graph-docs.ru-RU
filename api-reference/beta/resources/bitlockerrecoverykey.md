---
title: Тип ресурса Битлоккеррековерикэй
description: Ресурс ключа восстановления BitLocker
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 038feb77f7ca57d426a44c04b3d9c93ae29e5aa4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082074"
---
# <a name="bitlockerrecoverykey-resource-type"></a><span data-ttu-id="58560-103">Тип ресурса Битлоккеррековерикэй</span><span class="sxs-lookup"><span data-stu-id="58560-103">bitlockerRecoveryKey resource type</span></span>

<span data-ttu-id="58560-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58560-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58560-105">Представляет сохраненный ключ BitLocker, который содержит фактический ключ восстановления с помощью **ключевого** свойства.</span><span class="sxs-lookup"><span data-stu-id="58560-105">Represents a stored BitLocker key that contains the actual recovery key via the **key** property.</span></span>

## <a name="methods"></a><span data-ttu-id="58560-106">Методы</span><span class="sxs-lookup"><span data-stu-id="58560-106">Methods</span></span>
|<span data-ttu-id="58560-107">Метод</span><span class="sxs-lookup"><span data-stu-id="58560-107">Method</span></span>|<span data-ttu-id="58560-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="58560-108">Return type</span></span>|<span data-ttu-id="58560-109">Описание</span><span class="sxs-lookup"><span data-stu-id="58560-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="58560-110">Список Рековерикэйс</span><span class="sxs-lookup"><span data-stu-id="58560-110">List recoveryKeys</span></span>](../api/bitlocker-list-recoverykeys.md)|<span data-ttu-id="58560-111">Коллекция [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="58560-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span>|<span data-ttu-id="58560-112">Получение списка объектов [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) и их свойств.</span><span class="sxs-lookup"><span data-stu-id="58560-112">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span>|
|[<span data-ttu-id="58560-113">Получение Битлоккеррековерикэй</span><span class="sxs-lookup"><span data-stu-id="58560-113">Get bitlockerRecoveryKey</span></span>](../api/bitlockerrecoverykey-get.md)|[<span data-ttu-id="58560-114">битлоккеррековерикэй</span><span class="sxs-lookup"><span data-stu-id="58560-114">bitlockerRecoveryKey</span></span>](../resources/bitlockerrecoverykey.md)|<span data-ttu-id="58560-115">Получение свойств и связей объекта [битлоккеррековерикэй](../resources/bitlockerrecoverykey.md) .</span><span class="sxs-lookup"><span data-stu-id="58560-115">Retrieve the properties and relationships of a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object.</span></span> <span data-ttu-id="58560-116">Note: свойство **Key** не возвращается по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="58560-116">Note: The **key** property is not returned by default.</span></span>|

> <span data-ttu-id="58560-117">**Note**: только некоторые роли имеют разрешения на вызов этих API.</span><span class="sxs-lookup"><span data-stu-id="58560-117">**Note**: Only some roles have the permissions to call these APIs.</span></span>

## <a name="properties"></a><span data-ttu-id="58560-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="58560-118">Properties</span></span>
|<span data-ttu-id="58560-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="58560-119">Property</span></span>|<span data-ttu-id="58560-120">Тип</span><span class="sxs-lookup"><span data-stu-id="58560-120">Type</span></span>|<span data-ttu-id="58560-121">Описание</span><span class="sxs-lookup"><span data-stu-id="58560-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58560-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58560-122">createdDateTime</span></span>|<span data-ttu-id="58560-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58560-123">DateTimeOffset</span></span>|<span data-ttu-id="58560-124">Дата и время первоначального резервного копирования ключа в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="58560-124">The date and time when the key was originally backed up to Azure Active Directory.</span></span>|
|<span data-ttu-id="58560-125">deviceId</span><span class="sxs-lookup"><span data-stu-id="58560-125">deviceId</span></span>|<span data-ttu-id="58560-126">String</span><span class="sxs-lookup"><span data-stu-id="58560-126">String</span></span>|<span data-ttu-id="58560-127">ИДЕНТИФИКАТОР устройства, с которого создана резервная копия ключа BitLocker.</span><span class="sxs-lookup"><span data-stu-id="58560-127">ID of the device the BitLocker key is originally backed up from.</span></span>|
|<span data-ttu-id="58560-128">id</span><span class="sxs-lookup"><span data-stu-id="58560-128">id</span></span>|<span data-ttu-id="58560-129">Строка</span><span class="sxs-lookup"><span data-stu-id="58560-129">String</span></span>|<span data-ttu-id="58560-130">Уникальный идентификатор для ключа BitLocker.</span><span class="sxs-lookup"><span data-stu-id="58560-130">The unique identifier for the BitLocker key.</span></span>|
|<span data-ttu-id="58560-131">ключа</span><span class="sxs-lookup"><span data-stu-id="58560-131">key</span></span>|<span data-ttu-id="58560-132">Строка</span><span class="sxs-lookup"><span data-stu-id="58560-132">String</span></span>|<span data-ttu-id="58560-133">Ключ восстановления BitLocker.</span><span class="sxs-lookup"><span data-stu-id="58560-133">The BitLocker recovery key.</span></span>|
|<span data-ttu-id="58560-134">волуметипе</span><span class="sxs-lookup"><span data-stu-id="58560-134">volumeType</span></span>|<span data-ttu-id="58560-135">волуметипе</span><span class="sxs-lookup"><span data-stu-id="58560-135">volumeType</span></span>|<span data-ttu-id="58560-136">Указывает тип тома, с которым связан ключ BitLocker.</span><span class="sxs-lookup"><span data-stu-id="58560-136">Indicates the type of volume the BitLocker key is associated with.</span></span> <span data-ttu-id="58560-137">Возможные значения: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="58560-137">Possible values are: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58560-138">Связи</span><span class="sxs-lookup"><span data-stu-id="58560-138">Relationships</span></span>
<span data-ttu-id="58560-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="58560-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="58560-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="58560-140">JSON representation</span></span>
<span data-ttu-id="58560-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58560-141">The following is a JSON representation of the resource.</span></span>
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

