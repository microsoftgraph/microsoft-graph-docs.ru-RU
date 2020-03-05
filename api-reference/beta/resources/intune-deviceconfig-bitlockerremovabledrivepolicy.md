---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 90d1bcb5464b6fbd1d31d0ddbc3f2bbd525d80d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527023"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="4ecbb-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4ecbb-103">bitLockerRemovableDrivePolicy resource type</span></span>

<span data-ttu-id="4ecbb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4ecbb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ecbb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ecbb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ecbb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ecbb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ecbb-107">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="4ecbb-107">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="4ecbb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ecbb-108">Properties</span></span>
|<span data-ttu-id="4ecbb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ecbb-109">Property</span></span>|<span data-ttu-id="4ecbb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4ecbb-110">Type</span></span>|<span data-ttu-id="4ecbb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4ecbb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ecbb-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4ecbb-112">encryptionMethod</span></span>|[<span data-ttu-id="4ecbb-113">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="4ecbb-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="4ecbb-114">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="4ecbb-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="4ecbb-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="4ecbb-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="4ecbb-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4ecbb-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="4ecbb-117">Логический</span><span class="sxs-lookup"><span data-stu-id="4ecbb-117">Boolean</span></span>|<span data-ttu-id="4ecbb-118">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="4ecbb-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="4ecbb-119">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="4ecbb-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="4ecbb-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4ecbb-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="4ecbb-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ecbb-121">Boolean</span></span>|<span data-ttu-id="4ecbb-122">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="4ecbb-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ecbb-123">Связи</span><span class="sxs-lookup"><span data-stu-id="4ecbb-123">Relationships</span></span>
<span data-ttu-id="4ecbb-124">Нет</span><span class="sxs-lookup"><span data-stu-id="4ecbb-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ecbb-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ecbb-125">JSON Representation</span></span>
<span data-ttu-id="4ecbb-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ecbb-126">Here is a JSON representation of the resource.</span></span>
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



