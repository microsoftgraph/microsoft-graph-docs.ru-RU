---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57a3ad19e988327e126b6da757c2dc5b90c280de
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425619"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="4a624-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="4a624-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="4a624-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4a624-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4a624-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a624-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a624-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a624-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a624-107">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="4a624-107">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="4a624-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a624-108">Properties</span></span>
|<span data-ttu-id="4a624-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a624-109">Property</span></span>|<span data-ttu-id="4a624-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4a624-110">Type</span></span>|<span data-ttu-id="4a624-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4a624-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a624-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4a624-112">encryptionMethod</span></span>|[<span data-ttu-id="4a624-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4a624-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="4a624-114">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="4a624-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="4a624-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="4a624-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="4a624-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4a624-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="4a624-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a624-117">Boolean</span></span>|<span data-ttu-id="4a624-118">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="4a624-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="4a624-119">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="4a624-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="4a624-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4a624-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="4a624-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a624-121">Boolean</span></span>|<span data-ttu-id="4a624-122">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="4a624-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a624-123">Связи</span><span class="sxs-lookup"><span data-stu-id="4a624-123">Relationships</span></span>
<span data-ttu-id="4a624-124">Нет</span><span class="sxs-lookup"><span data-stu-id="4a624-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a624-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a624-125">JSON Representation</span></span>
<span data-ttu-id="4a624-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a624-126">Here is a JSON representation of the resource.</span></span>
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




