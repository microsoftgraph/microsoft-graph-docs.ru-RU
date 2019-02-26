---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d10a1039c0186238504836c0f719ab19ae4c4882
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261763"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="94c94-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="94c94-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="94c94-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94c94-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94c94-105">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="94c94-105">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="94c94-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="94c94-106">Properties</span></span>
|<span data-ttu-id="94c94-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="94c94-107">Property</span></span>|<span data-ttu-id="94c94-108">Тип</span><span class="sxs-lookup"><span data-stu-id="94c94-108">Type</span></span>|<span data-ttu-id="94c94-109">Описание</span><span class="sxs-lookup"><span data-stu-id="94c94-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94c94-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="94c94-110">encryptionMethod</span></span>|[<span data-ttu-id="94c94-111">Битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="94c94-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="94c94-112">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="94c94-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="94c94-113">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="94c94-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="94c94-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="94c94-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="94c94-115">Логический</span><span class="sxs-lookup"><span data-stu-id="94c94-115">Boolean</span></span>|<span data-ttu-id="94c94-116">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="94c94-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="94c94-117">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="94c94-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="94c94-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="94c94-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="94c94-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="94c94-119">Boolean</span></span>|<span data-ttu-id="94c94-120">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="94c94-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94c94-121">Связи</span><span class="sxs-lookup"><span data-stu-id="94c94-121">Relationships</span></span>
<span data-ttu-id="94c94-122">Нет</span><span class="sxs-lookup"><span data-stu-id="94c94-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94c94-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94c94-123">JSON Representation</span></span>
<span data-ttu-id="94c94-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94c94-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```



