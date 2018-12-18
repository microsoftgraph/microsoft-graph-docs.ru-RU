---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: tfitzmac
ms.openlocfilehash: 77f4161f7cd7aef61ee257ba665ab19e03ff4dc8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340014"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="8ebde-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="8ebde-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="8ebde-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8ebde-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ebde-105">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="8ebde-105">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="8ebde-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ebde-106">Properties</span></span>
|<span data-ttu-id="8ebde-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ebde-107">Property</span></span>|<span data-ttu-id="8ebde-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8ebde-108">Type</span></span>|<span data-ttu-id="8ebde-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8ebde-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ebde-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="8ebde-110">encryptionMethod</span></span>|[<span data-ttu-id="8ebde-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="8ebde-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="8ebde-112">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="8ebde-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="8ebde-113">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="8ebde-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="8ebde-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="8ebde-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="8ebde-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ebde-115">Boolean</span></span>|<span data-ttu-id="8ebde-116">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="8ebde-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="8ebde-117">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="8ebde-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="8ebde-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="8ebde-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="8ebde-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ebde-119">Boolean</span></span>|<span data-ttu-id="8ebde-120">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="8ebde-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ebde-121">Связи</span><span class="sxs-lookup"><span data-stu-id="8ebde-121">Relationships</span></span>
<span data-ttu-id="8ebde-122">Нет</span><span class="sxs-lookup"><span data-stu-id="8ebde-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8ebde-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ebde-123">JSON Representation</span></span>
<span data-ttu-id="8ebde-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ebde-124">Here is a JSON representation of the resource.</span></span>
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



