---
title: Тип ресурса bitLockerFixedDrivePolicy
description: Предопределенные политики диска BitLocker.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f55c2b81f1649c1292c4a54209480583147c9c23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886942"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="c632b-103">Тип ресурса bitLockerFixedDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="c632b-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="c632b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c632b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c632b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c632b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c632b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c632b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c632b-107">Предопределенные политики диска BitLocker.</span><span class="sxs-lookup"><span data-stu-id="c632b-107">BitLocker Fixed Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="c632b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c632b-108">Properties</span></span>
|<span data-ttu-id="c632b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c632b-109">Property</span></span>|<span data-ttu-id="c632b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c632b-110">Type</span></span>|<span data-ttu-id="c632b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c632b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c632b-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="c632b-112">encryptionMethod</span></span>|[<span data-ttu-id="c632b-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="c632b-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="c632b-114">Выберите метод шифрования для фиксированных жестких дисков.</span><span class="sxs-lookup"><span data-stu-id="c632b-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="c632b-115">Возможные значения: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="c632b-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="c632b-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="c632b-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="c632b-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="c632b-117">Boolean</span></span>|<span data-ttu-id="c632b-118">Этот параметр определяет, необходим ли защита BitLocker для дисков основных данных для записи на компьютере.</span><span class="sxs-lookup"><span data-stu-id="c632b-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="c632b-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="c632b-119">recoveryOptions</span></span>|<span data-ttu-id="c632b-120">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md);</span><span class="sxs-lookup"><span data-stu-id="c632b-120">[bitLockerRecoveryOptions](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)</span></span>|<span data-ttu-id="c632b-121">Этот параметр политики позволяет управлять как BitLocker основных данных, защищенных дисков восстанавливаются при отсутствии требуемых учетных данных.</span><span class="sxs-lookup"><span data-stu-id="c632b-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="c632b-122">Этот параметр политики применяется при включении BitLocker.</span><span class="sxs-lookup"><span data-stu-id="c632b-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c632b-123">Связи</span><span class="sxs-lookup"><span data-stu-id="c632b-123">Relationships</span></span>
<span data-ttu-id="c632b-124">Нет</span><span class="sxs-lookup"><span data-stu-id="c632b-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c632b-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c632b-125">JSON Representation</span></span>
<span data-ttu-id="c632b-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c632b-126">Here is a JSON representation of the resource.</span></span>
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





