---
title: Тип ресурса Битлоккеррековерйоптионс
description: Параметры восстановления BitLocker.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f5ffc5c3246dbe8eeafd39df6669079e060f0da
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947508"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="d0d4f-103">Тип ресурса Битлоккеррековерйоптионс</span><span class="sxs-lookup"><span data-stu-id="d0d4f-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="d0d4f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0d4f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0d4f-106">Параметры восстановления BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-106">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="d0d4f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0d4f-107">Properties</span></span>
|<span data-ttu-id="d0d4f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0d4f-108">Property</span></span>|<span data-ttu-id="d0d4f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d0d4f-109">Type</span></span>|<span data-ttu-id="d0d4f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d0d4f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0d4f-111">Блоккдатарековеряжент</span><span class="sxs-lookup"><span data-stu-id="d0d4f-111">blockDataRecoveryAgent</span></span>|<span data-ttu-id="d0d4f-112">Логический</span><span class="sxs-lookup"><span data-stu-id="d0d4f-112">Boolean</span></span>|<span data-ttu-id="d0d4f-113">Указывает, следует ли заблокировать агент восстановления данных на основе сертификатов.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-113">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="d0d4f-114">Рековерипассвордусаже</span><span class="sxs-lookup"><span data-stu-id="d0d4f-114">recoveryPasswordUsage</span></span>|[<span data-ttu-id="d0d4f-115">Конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="d0d4f-115">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d0d4f-116">Указывает, разрешено ли пользователям создавать пароль восстановления для фиксированного или системного диска с 48 цифр.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-116">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="d0d4f-117">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-117">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d0d4f-118">Рековерикэйусаже</span><span class="sxs-lookup"><span data-stu-id="d0d4f-118">recoveryKeyUsage</span></span>|[<span data-ttu-id="d0d4f-119">Конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="d0d4f-119">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d0d4f-120">Указывает, могут ли пользователи создавать ключ восстановления 256 бит для фиксированного или системного диска.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-120">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="d0d4f-121">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-121">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d0d4f-122">Хидерековерйоптионс</span><span class="sxs-lookup"><span data-stu-id="d0d4f-122">hideRecoveryOptions</span></span>|<span data-ttu-id="d0d4f-123">Логический</span><span class="sxs-lookup"><span data-stu-id="d0d4f-123">Boolean</span></span>|<span data-ttu-id="d0d4f-124">Указывает, можно ли отображать параметры восстановления в мастере установки BitLocker для фиксированного или системного диска.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-124">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="d0d4f-125">Енаблерековеринформатионсаветосторе</span><span class="sxs-lookup"><span data-stu-id="d0d4f-125">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="d0d4f-126">Логический</span><span class="sxs-lookup"><span data-stu-id="d0d4f-126">Boolean</span></span>|<span data-ttu-id="d0d4f-127">Указывает, следует ли запретить хранение данных восстановления BitLocker в доменных СЛУЖБах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-127">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="d0d4f-128">Рековеринформатионтосторе</span><span class="sxs-lookup"><span data-stu-id="d0d4f-128">recoveryInformationToStore</span></span>|[<span data-ttu-id="d0d4f-129">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="d0d4f-129">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="d0d4f-130">Настройте, какие части данных восстановления BitLocker хранятся в AD DS.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-130">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="d0d4f-131">Возможные значения: `passwordAndKey`, `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-131">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="d0d4f-132">Енаблебитлоккерафтеррековеринформатионтосторе</span><span class="sxs-lookup"><span data-stu-id="d0d4f-132">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="d0d4f-133">Логический</span><span class="sxs-lookup"><span data-stu-id="d0d4f-133">Boolean</span></span>|<span data-ttu-id="d0d4f-134">Указывает, следует ли включить BitLocker до тех пор, пока данные для восстановления не будут храниться в доменных СЛУЖБах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-134">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0d4f-135">Связи</span><span class="sxs-lookup"><span data-stu-id="d0d4f-135">Relationships</span></span>
<span data-ttu-id="d0d4f-136">Нет</span><span class="sxs-lookup"><span data-stu-id="d0d4f-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0d4f-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0d4f-137">JSON Representation</span></span>
<span data-ttu-id="d0d4f-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0d4f-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```




