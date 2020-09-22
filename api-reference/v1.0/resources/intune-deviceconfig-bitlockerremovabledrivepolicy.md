---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 645884953efb3814e3b74d96c2577ed37d202199
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062815"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="a6865-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="a6865-103">bitLockerRemovableDrivePolicy resource type</span></span>

<span data-ttu-id="a6865-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6865-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6865-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6865-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6865-106">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="a6865-106">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="a6865-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6865-107">Properties</span></span>
|<span data-ttu-id="a6865-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6865-108">Property</span></span>|<span data-ttu-id="a6865-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a6865-109">Type</span></span>|<span data-ttu-id="a6865-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a6865-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6865-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="a6865-111">encryptionMethod</span></span>|[<span data-ttu-id="a6865-112">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="a6865-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="a6865-113">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="a6865-113">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="a6865-114">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="a6865-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="a6865-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="a6865-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="a6865-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6865-116">Boolean</span></span>|<span data-ttu-id="a6865-117">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="a6865-117">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="a6865-118">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="a6865-118">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="a6865-119">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="a6865-119">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="a6865-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6865-120">Boolean</span></span>|<span data-ttu-id="a6865-121">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="a6865-121">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6865-122">Связи</span><span class="sxs-lookup"><span data-stu-id="a6865-122">Relationships</span></span>
<span data-ttu-id="a6865-123">Нет</span><span class="sxs-lookup"><span data-stu-id="a6865-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6865-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6865-124">JSON Representation</span></span>
<span data-ttu-id="a6865-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6865-125">Here is a JSON representation of the resource.</span></span>
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









