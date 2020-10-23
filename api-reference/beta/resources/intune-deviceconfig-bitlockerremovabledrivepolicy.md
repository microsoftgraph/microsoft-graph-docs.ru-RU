---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 424fcdff8d2c16bbba1cba295bf626eeae7eda50
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697982"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="04aa2-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="04aa2-103">bitLockerRemovableDrivePolicy resource type</span></span>

<span data-ttu-id="04aa2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04aa2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04aa2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04aa2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04aa2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="04aa2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04aa2-107">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="04aa2-107">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="04aa2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="04aa2-108">Properties</span></span>
|<span data-ttu-id="04aa2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="04aa2-109">Property</span></span>|<span data-ttu-id="04aa2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="04aa2-110">Type</span></span>|<span data-ttu-id="04aa2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="04aa2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04aa2-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="04aa2-112">encryptionMethod</span></span>|[<span data-ttu-id="04aa2-113">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="04aa2-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="04aa2-114">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="04aa2-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="04aa2-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="04aa2-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="04aa2-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="04aa2-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="04aa2-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="04aa2-117">Boolean</span></span>|<span data-ttu-id="04aa2-118">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="04aa2-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="04aa2-119">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="04aa2-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="04aa2-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="04aa2-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="04aa2-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="04aa2-121">Boolean</span></span>|<span data-ttu-id="04aa2-122">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="04aa2-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04aa2-123">Связи</span><span class="sxs-lookup"><span data-stu-id="04aa2-123">Relationships</span></span>
<span data-ttu-id="04aa2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="04aa2-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04aa2-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04aa2-125">JSON Representation</span></span>
<span data-ttu-id="04aa2-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04aa2-126">Here is a JSON representation of the resource.</span></span>
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





