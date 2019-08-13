---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 41397aa9d2c10481a9eaab54d70f65a84b4d26c9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333788"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="49d80-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="49d80-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="49d80-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49d80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49d80-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49d80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49d80-106">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="49d80-106">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="49d80-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="49d80-107">Properties</span></span>
|<span data-ttu-id="49d80-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="49d80-108">Property</span></span>|<span data-ttu-id="49d80-109">Тип</span><span class="sxs-lookup"><span data-stu-id="49d80-109">Type</span></span>|<span data-ttu-id="49d80-110">Описание</span><span class="sxs-lookup"><span data-stu-id="49d80-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49d80-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="49d80-111">encryptionMethod</span></span>|[<span data-ttu-id="49d80-112">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="49d80-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="49d80-113">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="49d80-113">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="49d80-114">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="49d80-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="49d80-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="49d80-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="49d80-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="49d80-116">Boolean</span></span>|<span data-ttu-id="49d80-117">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="49d80-117">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="49d80-118">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="49d80-118">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="49d80-119">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="49d80-119">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="49d80-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="49d80-120">Boolean</span></span>|<span data-ttu-id="49d80-121">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="49d80-121">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49d80-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="49d80-122">Relationships</span></span>
<span data-ttu-id="49d80-123">Нет</span><span class="sxs-lookup"><span data-stu-id="49d80-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49d80-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49d80-124">JSON Representation</span></span>
<span data-ttu-id="49d80-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49d80-125">Here is a JSON representation of the resource.</span></span>
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



