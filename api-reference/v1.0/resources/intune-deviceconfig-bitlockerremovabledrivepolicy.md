---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 78ce6f77c90e3b9356ccc75a6a202a9983b11874
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449105"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="27f38-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="27f38-103">bitLockerRemovableDrivePolicy resource type</span></span>

<span data-ttu-id="27f38-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27f38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27f38-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27f38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27f38-106">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="27f38-106">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="27f38-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="27f38-107">Properties</span></span>
|<span data-ttu-id="27f38-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="27f38-108">Property</span></span>|<span data-ttu-id="27f38-109">Тип</span><span class="sxs-lookup"><span data-stu-id="27f38-109">Type</span></span>|<span data-ttu-id="27f38-110">Описание</span><span class="sxs-lookup"><span data-stu-id="27f38-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27f38-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="27f38-111">encryptionMethod</span></span>|[<span data-ttu-id="27f38-112">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="27f38-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="27f38-113">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="27f38-113">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="27f38-114">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="27f38-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="27f38-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="27f38-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="27f38-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="27f38-116">Boolean</span></span>|<span data-ttu-id="27f38-117">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="27f38-117">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="27f38-118">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="27f38-118">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="27f38-119">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="27f38-119">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="27f38-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="27f38-120">Boolean</span></span>|<span data-ttu-id="27f38-121">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="27f38-121">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27f38-122">Связи</span><span class="sxs-lookup"><span data-stu-id="27f38-122">Relationships</span></span>
<span data-ttu-id="27f38-123">Нет</span><span class="sxs-lookup"><span data-stu-id="27f38-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27f38-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27f38-124">JSON Representation</span></span>
<span data-ttu-id="27f38-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27f38-125">Here is a JSON representation of the resource.</span></span>
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







