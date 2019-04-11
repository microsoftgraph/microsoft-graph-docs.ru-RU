---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aef69dc1ac05b838d1bb6a17e17f8ebde27edc1a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805588"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="95532-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="95532-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="95532-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95532-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95532-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95532-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95532-106">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="95532-106">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="95532-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="95532-107">Properties</span></span>
|<span data-ttu-id="95532-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="95532-108">Property</span></span>|<span data-ttu-id="95532-109">Тип</span><span class="sxs-lookup"><span data-stu-id="95532-109">Type</span></span>|<span data-ttu-id="95532-110">Описание</span><span class="sxs-lookup"><span data-stu-id="95532-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95532-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="95532-111">encryptionMethod</span></span>|[<span data-ttu-id="95532-112">Битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="95532-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="95532-113">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="95532-113">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="95532-114">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="95532-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="95532-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="95532-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="95532-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="95532-116">Boolean</span></span>|<span data-ttu-id="95532-117">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="95532-117">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="95532-118">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="95532-118">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="95532-119">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="95532-119">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="95532-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="95532-120">Boolean</span></span>|<span data-ttu-id="95532-121">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="95532-121">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95532-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="95532-122">Relationships</span></span>
<span data-ttu-id="95532-123">Нет</span><span class="sxs-lookup"><span data-stu-id="95532-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95532-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95532-124">JSON Representation</span></span>
<span data-ttu-id="95532-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95532-125">Here is a JSON representation of the resource.</span></span>
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





