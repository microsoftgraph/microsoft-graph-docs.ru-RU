---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
ms.openlocfilehash: 886ed1912c9c6626a06f1efaef83de5ed1f52a66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024386"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="319fd-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="319fd-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="319fd-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="319fd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="319fd-105">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="319fd-105">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="319fd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="319fd-106">Properties</span></span>
|<span data-ttu-id="319fd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="319fd-107">Property</span></span>|<span data-ttu-id="319fd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="319fd-108">Type</span></span>|<span data-ttu-id="319fd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="319fd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="319fd-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="319fd-110">encryptionMethod</span></span>|[<span data-ttu-id="319fd-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="319fd-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="319fd-112">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="319fd-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="319fd-113">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="319fd-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="319fd-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="319fd-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="319fd-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="319fd-115">Boolean</span></span>|<span data-ttu-id="319fd-116">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="319fd-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="319fd-117">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="319fd-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="319fd-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="319fd-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="319fd-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="319fd-119">Boolean</span></span>|<span data-ttu-id="319fd-120">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="319fd-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="319fd-121">Связи</span><span class="sxs-lookup"><span data-stu-id="319fd-121">Relationships</span></span>
<span data-ttu-id="319fd-122">Нет</span><span class="sxs-lookup"><span data-stu-id="319fd-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="319fd-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="319fd-123">JSON Representation</span></span>
<span data-ttu-id="319fd-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="319fd-124">Here is a JSON representation of the resource.</span></span>
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



