---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8437ab4c6b816efe9b2af83f2c5593cce43132bc
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795738"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="1887d-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1887d-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="1887d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1887d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1887d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1887d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1887d-106">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="1887d-106">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="1887d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1887d-107">Properties</span></span>
|<span data-ttu-id="1887d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1887d-108">Property</span></span>|<span data-ttu-id="1887d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1887d-109">Type</span></span>|<span data-ttu-id="1887d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1887d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1887d-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="1887d-111">encryptionMethod</span></span>|[<span data-ttu-id="1887d-112">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="1887d-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="1887d-113">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="1887d-113">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="1887d-114">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="1887d-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="1887d-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="1887d-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="1887d-116">Логический</span><span class="sxs-lookup"><span data-stu-id="1887d-116">Boolean</span></span>|<span data-ttu-id="1887d-117">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="1887d-117">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="1887d-118">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="1887d-118">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="1887d-119">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="1887d-119">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="1887d-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="1887d-120">Boolean</span></span>|<span data-ttu-id="1887d-121">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="1887d-121">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1887d-122">Связи</span><span class="sxs-lookup"><span data-stu-id="1887d-122">Relationships</span></span>
<span data-ttu-id="1887d-123">Нет</span><span class="sxs-lookup"><span data-stu-id="1887d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1887d-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1887d-124">JSON Representation</span></span>
<span data-ttu-id="1887d-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1887d-125">Here is a JSON representation of the resource.</span></span>
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



