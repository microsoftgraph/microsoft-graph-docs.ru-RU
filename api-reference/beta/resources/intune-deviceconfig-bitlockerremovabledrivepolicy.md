---
title: Тип ресурса bitLockerRemovableDrivePolicy
description: Политика BitLocker в отношении съемных дисков.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e05b8a1762e4eca1c693c4ea2ba6dcb6e3be1806
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260546"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="de2fb-103">Тип ресурса bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="de2fb-103">bitLockerRemovableDrivePolicy resource type</span></span>

<span data-ttu-id="de2fb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de2fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="de2fb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de2fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de2fb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de2fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de2fb-107">Политика BitLocker в отношении съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="de2fb-107">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="de2fb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="de2fb-108">Properties</span></span>
|<span data-ttu-id="de2fb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="de2fb-109">Property</span></span>|<span data-ttu-id="de2fb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="de2fb-110">Type</span></span>|<span data-ttu-id="de2fb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="de2fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de2fb-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="de2fb-112">encryptionMethod</span></span>|[<span data-ttu-id="de2fb-113">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="de2fb-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="de2fb-114">Выберите метод шифрования для съемных дисков.</span><span class="sxs-lookup"><span data-stu-id="de2fb-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="de2fb-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="de2fb-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="de2fb-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="de2fb-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="de2fb-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="de2fb-117">Boolean</span></span>|<span data-ttu-id="de2fb-118">Определяет, нужно ли блокировать доступ на запись к устройствам, настроенным в другой организации.</span><span class="sxs-lookup"><span data-stu-id="de2fb-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="de2fb-119">Если для свойства requireEncryptionForWriteAccess задано значение false, это значение не учитывается.</span><span class="sxs-lookup"><span data-stu-id="de2fb-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="de2fb-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="de2fb-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="de2fb-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="de2fb-121">Boolean</span></span>|<span data-ttu-id="de2fb-122">Этот параметр политики определяет, требуется ли защита BitLocker для съемных дисков, доступных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="de2fb-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de2fb-123">Связи</span><span class="sxs-lookup"><span data-stu-id="de2fb-123">Relationships</span></span>
<span data-ttu-id="de2fb-124">Нет</span><span class="sxs-lookup"><span data-stu-id="de2fb-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de2fb-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de2fb-125">JSON Representation</span></span>
<span data-ttu-id="de2fb-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de2fb-126">Here is a JSON representation of the resource.</span></span>
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




