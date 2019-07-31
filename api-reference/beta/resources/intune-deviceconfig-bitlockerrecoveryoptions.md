---
title: Тип ресурса Битлоккеррековерйоптионс
description: Параметры восстановления BitLocker.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e9ac2b9fee5947de29cdf2d6cc4e56d521b9f131
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971076"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="86bda-103">Тип ресурса Битлоккеррековерйоптионс</span><span class="sxs-lookup"><span data-stu-id="86bda-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="86bda-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86bda-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86bda-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86bda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86bda-106">Параметры восстановления BitLocker.</span><span class="sxs-lookup"><span data-stu-id="86bda-106">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="86bda-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="86bda-107">Properties</span></span>
|<span data-ttu-id="86bda-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="86bda-108">Property</span></span>|<span data-ttu-id="86bda-109">Тип</span><span class="sxs-lookup"><span data-stu-id="86bda-109">Type</span></span>|<span data-ttu-id="86bda-110">Описание</span><span class="sxs-lookup"><span data-stu-id="86bda-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86bda-111">Блоккдатарековеряжент</span><span class="sxs-lookup"><span data-stu-id="86bda-111">blockDataRecoveryAgent</span></span>|<span data-ttu-id="86bda-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="86bda-112">Boolean</span></span>|<span data-ttu-id="86bda-113">Указывает, следует ли заблокировать агент восстановления данных на основе сертификатов.</span><span class="sxs-lookup"><span data-stu-id="86bda-113">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="86bda-114">Рековерипассвордусаже</span><span class="sxs-lookup"><span data-stu-id="86bda-114">recoveryPasswordUsage</span></span>|[<span data-ttu-id="86bda-115">Конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="86bda-115">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="86bda-116">Указывает, разрешено ли пользователям создавать пароль восстановления для фиксированного или системного диска с 48 цифр.</span><span class="sxs-lookup"><span data-stu-id="86bda-116">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="86bda-117">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="86bda-117">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="86bda-118">Рековерикэйусаже</span><span class="sxs-lookup"><span data-stu-id="86bda-118">recoveryKeyUsage</span></span>|[<span data-ttu-id="86bda-119">Конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="86bda-119">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="86bda-120">Указывает, могут ли пользователи создавать ключ восстановления 256 бит для фиксированного или системного диска.</span><span class="sxs-lookup"><span data-stu-id="86bda-120">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="86bda-121">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="86bda-121">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="86bda-122">Хидерековерйоптионс</span><span class="sxs-lookup"><span data-stu-id="86bda-122">hideRecoveryOptions</span></span>|<span data-ttu-id="86bda-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="86bda-123">Boolean</span></span>|<span data-ttu-id="86bda-124">Указывает, можно ли отображать параметры восстановления в мастере установки BitLocker для фиксированного или системного диска.</span><span class="sxs-lookup"><span data-stu-id="86bda-124">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="86bda-125">Енаблерековеринформатионсаветосторе</span><span class="sxs-lookup"><span data-stu-id="86bda-125">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="86bda-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="86bda-126">Boolean</span></span>|<span data-ttu-id="86bda-127">Указывает, следует ли запретить хранение данных восстановления BitLocker в доменных СЛУЖБах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="86bda-127">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="86bda-128">Рековеринформатионтосторе</span><span class="sxs-lookup"><span data-stu-id="86bda-128">recoveryInformationToStore</span></span>|[<span data-ttu-id="86bda-129">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="86bda-129">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="86bda-130">Настройте, какие части данных восстановления BitLocker хранятся в AD DS.</span><span class="sxs-lookup"><span data-stu-id="86bda-130">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="86bda-131">Возможные значения: `passwordAndKey`, `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="86bda-131">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="86bda-132">Енаблебитлоккерафтеррековеринформатионтосторе</span><span class="sxs-lookup"><span data-stu-id="86bda-132">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="86bda-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="86bda-133">Boolean</span></span>|<span data-ttu-id="86bda-134">Указывает, следует ли включить BitLocker до тех пор, пока данные для восстановления не будут храниться в доменных СЛУЖБах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="86bda-134">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86bda-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="86bda-135">Relationships</span></span>
<span data-ttu-id="86bda-136">Нет</span><span class="sxs-lookup"><span data-stu-id="86bda-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86bda-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86bda-137">JSON Representation</span></span>
<span data-ttu-id="86bda-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86bda-138">Here is a JSON representation of the resource.</span></span>
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





