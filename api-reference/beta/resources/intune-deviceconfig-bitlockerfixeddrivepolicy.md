---
title: Тип ресурса свойства bitlockerfixeddrivepolicy
description: Политики фиксированного диска BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4d53028e901d65403e282abecb91ca70d68cec96
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690709"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="ed795-103">Тип ресурса свойства bitlockerfixeddrivepolicy</span><span class="sxs-lookup"><span data-stu-id="ed795-103">bitLockerFixedDrivePolicy resource type</span></span>

<span data-ttu-id="ed795-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed795-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed795-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ed795-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed795-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ed795-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed795-107">Политики фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="ed795-107">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="ed795-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed795-108">Properties</span></span>
|<span data-ttu-id="ed795-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed795-109">Property</span></span>|<span data-ttu-id="ed795-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ed795-110">Type</span></span>|<span data-ttu-id="ed795-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ed795-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed795-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="ed795-112">encryptionMethod</span></span>|[<span data-ttu-id="ed795-113">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="ed795-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="ed795-114">Выберите метод шифрования для несъемных дисков.</span><span class="sxs-lookup"><span data-stu-id="ed795-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="ed795-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="ed795-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="ed795-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="ed795-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="ed795-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed795-117">Boolean</span></span>|<span data-ttu-id="ed795-118">Этот параметр политики определяет, требуется ли защита BitLocker для несъемных дисков с данными на компьютере.</span><span class="sxs-lookup"><span data-stu-id="ed795-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="ed795-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="ed795-119">recoveryOptions</span></span>|<span data-ttu-id="ed795-120">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="ed795-120">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="ed795-121">Этот параметр политики позволяет управлять восстановлением несъемных дисков с данными, защищенных с помощью BitLocker, в отсутствие необходимых учетных данных.</span><span class="sxs-lookup"><span data-stu-id="ed795-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="ed795-122">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="ed795-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed795-123">Связи</span><span class="sxs-lookup"><span data-stu-id="ed795-123">Relationships</span></span>
<span data-ttu-id="ed795-124">Нет</span><span class="sxs-lookup"><span data-stu-id="ed795-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed795-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed795-125">JSON Representation</span></span>
<span data-ttu-id="ed795-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed795-126">Here is a JSON representation of the resource.</span></span>
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





