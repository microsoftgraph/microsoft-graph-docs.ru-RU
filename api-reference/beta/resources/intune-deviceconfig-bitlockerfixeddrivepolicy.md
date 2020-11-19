---
title: Тип ресурса свойства bitlockerfixeddrivepolicy
description: Политики фиксированного диска BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 323d45fb8109820a74f6b0394431a297ed2618e6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260616"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="eaba6-103">Тип ресурса свойства bitlockerfixeddrivepolicy</span><span class="sxs-lookup"><span data-stu-id="eaba6-103">bitLockerFixedDrivePolicy resource type</span></span>

<span data-ttu-id="eaba6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eaba6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eaba6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaba6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaba6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eaba6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaba6-107">Политики фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="eaba6-107">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="eaba6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eaba6-108">Properties</span></span>
|<span data-ttu-id="eaba6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eaba6-109">Property</span></span>|<span data-ttu-id="eaba6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eaba6-110">Type</span></span>|<span data-ttu-id="eaba6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eaba6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaba6-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="eaba6-112">encryptionMethod</span></span>|[<span data-ttu-id="eaba6-113">битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="eaba6-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="eaba6-114">Выберите метод шифрования для несъемных дисков.</span><span class="sxs-lookup"><span data-stu-id="eaba6-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="eaba6-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="eaba6-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="eaba6-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="eaba6-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="eaba6-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaba6-117">Boolean</span></span>|<span data-ttu-id="eaba6-118">Этот параметр политики определяет, требуется ли защита BitLocker для несъемных дисков с данными на компьютере.</span><span class="sxs-lookup"><span data-stu-id="eaba6-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="eaba6-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="eaba6-119">recoveryOptions</span></span>|<span data-ttu-id="eaba6-120">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="eaba6-120">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="eaba6-121">Этот параметр политики позволяет управлять восстановлением несъемных дисков с данными, защищенных с помощью BitLocker, в отсутствие необходимых учетных данных.</span><span class="sxs-lookup"><span data-stu-id="eaba6-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="eaba6-122">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="eaba6-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eaba6-123">Связи</span><span class="sxs-lookup"><span data-stu-id="eaba6-123">Relationships</span></span>
<span data-ttu-id="eaba6-124">Нет</span><span class="sxs-lookup"><span data-stu-id="eaba6-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eaba6-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eaba6-125">JSON Representation</span></span>
<span data-ttu-id="eaba6-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eaba6-126">Here is a JSON representation of the resource.</span></span>
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




