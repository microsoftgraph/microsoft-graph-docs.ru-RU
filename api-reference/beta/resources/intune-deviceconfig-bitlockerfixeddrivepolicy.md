---
title: Тип ресурса bitLockerFixedDrivePolicy
description: Предопределенные политики диска BitLocker.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8f233e4c1779a860cc40dc97007aa0216795928f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424667"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="47bbe-103">Тип ресурса bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="47bbe-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="47bbe-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47bbe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="47bbe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47bbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47bbe-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47bbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47bbe-107">Предопределенные политики диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="47bbe-107">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="47bbe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="47bbe-108">Properties</span></span>
|<span data-ttu-id="47bbe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="47bbe-109">Property</span></span>|<span data-ttu-id="47bbe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="47bbe-110">Type</span></span>|<span data-ttu-id="47bbe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="47bbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47bbe-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="47bbe-112">encryptionMethod</span></span>|[<span data-ttu-id="47bbe-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="47bbe-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="47bbe-114">Выберите метод шифрования для фиксированных жестких дисков.</span><span class="sxs-lookup"><span data-stu-id="47bbe-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="47bbe-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="47bbe-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="47bbe-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="47bbe-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="47bbe-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="47bbe-117">Boolean</span></span>|<span data-ttu-id="47bbe-118">Этот параметр определяет, необходим ли защита BitLocker для дисков основных данных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="47bbe-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="47bbe-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="47bbe-119">recoveryOptions</span></span>|<span data-ttu-id="47bbe-120">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="47bbe-120">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="47bbe-121">Этот параметр политики позволяет управлять как BitLocker основных данных, защищенных дисков восстанавливаются при отсутствии требуемых учетных данных.</span><span class="sxs-lookup"><span data-stu-id="47bbe-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="47bbe-122">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="47bbe-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47bbe-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="47bbe-123">Relationships</span></span>
<span data-ttu-id="47bbe-124">Нет</span><span class="sxs-lookup"><span data-stu-id="47bbe-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47bbe-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47bbe-125">JSON Representation</span></span>
<span data-ttu-id="47bbe-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47bbe-126">Here is a JSON representation of the resource.</span></span>
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




