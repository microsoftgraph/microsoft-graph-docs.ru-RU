---
title: Тип ресурса свойства bitlockerfixeddrivepolicy
description: Политики фиксированного диска BitLocker.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4b44a56b02a6e8a15d4d2cfb0919cc852a9899fb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795866"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="3852f-103">Тип ресурса свойства bitlockerfixeddrivepolicy</span><span class="sxs-lookup"><span data-stu-id="3852f-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="3852f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3852f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3852f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3852f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3852f-106">Политики фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="3852f-106">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="3852f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3852f-107">Properties</span></span>
|<span data-ttu-id="3852f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3852f-108">Property</span></span>|<span data-ttu-id="3852f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3852f-109">Type</span></span>|<span data-ttu-id="3852f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3852f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3852f-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="3852f-111">encryptionMethod</span></span>|[<span data-ttu-id="3852f-112">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="3852f-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="3852f-113">Выберите метод шифрования для несъемных дисков.</span><span class="sxs-lookup"><span data-stu-id="3852f-113">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="3852f-114">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="3852f-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="3852f-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="3852f-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="3852f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="3852f-116">Boolean</span></span>|<span data-ttu-id="3852f-117">Этот параметр политики определяет, требуется ли защита BitLocker для несъемных дисков с данными на компьютере.</span><span class="sxs-lookup"><span data-stu-id="3852f-117">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="3852f-118">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="3852f-118">recoveryOptions</span></span>|<span data-ttu-id="3852f-119">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="3852f-119">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="3852f-120">Этот параметр политики позволяет управлять восстановлением несъемных дисков с данными, защищенных с помощью BitLocker, в отсутствие необходимых учетных данных.</span><span class="sxs-lookup"><span data-stu-id="3852f-120">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="3852f-121">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="3852f-121">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3852f-122">Связи</span><span class="sxs-lookup"><span data-stu-id="3852f-122">Relationships</span></span>
<span data-ttu-id="3852f-123">Нет</span><span class="sxs-lookup"><span data-stu-id="3852f-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3852f-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3852f-124">JSON Representation</span></span>
<span data-ttu-id="3852f-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3852f-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerFixedDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  }
}
```



