---
title: Тип ресурса свойства bitlockerfixeddrivepolicy
description: Политики фиксированного диска BitLocker.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3269fb0865f8cf08a4dbade3d949701b027b84fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971090"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="de6bf-103">Тип ресурса свойства bitlockerfixeddrivepolicy</span><span class="sxs-lookup"><span data-stu-id="de6bf-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="de6bf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de6bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de6bf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de6bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de6bf-106">Политики фиксированного диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="de6bf-106">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="de6bf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="de6bf-107">Properties</span></span>
|<span data-ttu-id="de6bf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="de6bf-108">Property</span></span>|<span data-ttu-id="de6bf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="de6bf-109">Type</span></span>|<span data-ttu-id="de6bf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="de6bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de6bf-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="de6bf-111">encryptionMethod</span></span>|[<span data-ttu-id="de6bf-112">Битлоккеренкриптионмесод</span><span class="sxs-lookup"><span data-stu-id="de6bf-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="de6bf-113">Выберите метод шифрования для несъемных дисков.</span><span class="sxs-lookup"><span data-stu-id="de6bf-113">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="de6bf-114">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="de6bf-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="de6bf-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="de6bf-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="de6bf-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="de6bf-116">Boolean</span></span>|<span data-ttu-id="de6bf-117">Этот параметр политики определяет, требуется ли защита BitLocker для несъемных дисков с данными на компьютере.</span><span class="sxs-lookup"><span data-stu-id="de6bf-117">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="de6bf-118">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="de6bf-118">recoveryOptions</span></span>|<span data-ttu-id="de6bf-119">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="de6bf-119">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="de6bf-120">Этот параметр политики позволяет управлять восстановлением несъемных дисков с данными, защищенных с помощью BitLocker, в отсутствие необходимых учетных данных.</span><span class="sxs-lookup"><span data-stu-id="de6bf-120">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="de6bf-121">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="de6bf-121">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de6bf-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="de6bf-122">Relationships</span></span>
<span data-ttu-id="de6bf-123">Нет</span><span class="sxs-lookup"><span data-stu-id="de6bf-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de6bf-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de6bf-124">JSON Representation</span></span>
<span data-ttu-id="de6bf-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de6bf-125">Here is a JSON representation of the resource.</span></span>
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





