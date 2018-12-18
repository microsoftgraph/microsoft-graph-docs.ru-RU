---
title: Тип ресурса bitLockerFixedDrivePolicy
description: Предопределенные политики диска BitLocker.
author: tfitzmac
ms.openlocfilehash: 71fc28fc88689165cdcd187542460432948f78c2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342618"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="1bdd6-103">Тип ресурса bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="1bdd6-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="1bdd6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1bdd6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1bdd6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bdd6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1bdd6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1bdd6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1bdd6-107">Предопределенные политики диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="1bdd6-107">BitLocker Fixed Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="1bdd6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1bdd6-108">Properties</span></span>
|<span data-ttu-id="1bdd6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bdd6-109">Property</span></span>|<span data-ttu-id="1bdd6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1bdd6-110">Type</span></span>|<span data-ttu-id="1bdd6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1bdd6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bdd6-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="1bdd6-112">encryptionMethod</span></span>|[<span data-ttu-id="1bdd6-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="1bdd6-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="1bdd6-114">Выберите метод шифрования для фиксированных жестких дисков.</span><span class="sxs-lookup"><span data-stu-id="1bdd6-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="1bdd6-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="1bdd6-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="1bdd6-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="1bdd6-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="1bdd6-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bdd6-117">Boolean</span></span>|<span data-ttu-id="1bdd6-118">Этот параметр определяет, необходим ли защита BitLocker для дисков основных данных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="1bdd6-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="1bdd6-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="1bdd6-119">recoveryOptions</span></span>|<span data-ttu-id="1bdd6-120">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="1bdd6-120">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="1bdd6-121">Этот параметр политики позволяет управлять как BitLocker основных данных, защищенных дисков восстанавливаются при отсутствии требуемых учетных данных.</span><span class="sxs-lookup"><span data-stu-id="1bdd6-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="1bdd6-122">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="1bdd6-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1bdd6-123">Связи</span><span class="sxs-lookup"><span data-stu-id="1bdd6-123">Relationships</span></span>
<span data-ttu-id="1bdd6-124">Нет</span><span class="sxs-lookup"><span data-stu-id="1bdd6-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1bdd6-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1bdd6-125">JSON Representation</span></span>
<span data-ttu-id="1bdd6-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bdd6-126">Here is a JSON representation of the resource.</span></span>
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





