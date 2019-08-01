---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5c474dc113d7d00bb0a43bef59c8196befddea3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028541"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="08e29-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="08e29-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="08e29-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08e29-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08e29-105">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="08e29-105">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="08e29-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="08e29-106">Properties</span></span>
|<span data-ttu-id="08e29-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="08e29-107">Property</span></span>|<span data-ttu-id="08e29-108">Тип</span><span class="sxs-lookup"><span data-stu-id="08e29-108">Type</span></span>|<span data-ttu-id="08e29-109">Описание</span><span class="sxs-lookup"><span data-stu-id="08e29-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08e29-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="08e29-110">encryptionMethod</span></span>|[<span data-ttu-id="08e29-111">Битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="08e29-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="08e29-112">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="08e29-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="08e29-113">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="08e29-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="08e29-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="08e29-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="08e29-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="08e29-115">Boolean</span></span>|<span data-ttu-id="08e29-116">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="08e29-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="08e29-117">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="08e29-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="08e29-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="08e29-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="08e29-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="08e29-119">Boolean</span></span>|<span data-ttu-id="08e29-120">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="08e29-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08e29-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="08e29-121">Relationships</span></span>
<span data-ttu-id="08e29-122">Нет</span><span class="sxs-lookup"><span data-stu-id="08e29-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08e29-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08e29-123">JSON Representation</span></span>
<span data-ttu-id="08e29-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08e29-124">Here is a JSON representation of the resource.</span></span>
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



