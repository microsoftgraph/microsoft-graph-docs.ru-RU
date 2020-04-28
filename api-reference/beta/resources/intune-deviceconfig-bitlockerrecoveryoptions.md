---
title: Тип ресурса Битлоккеррековерйоптионс
description: Параметры восстановления BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d8393843c92c106794d8b62ee0143c95f464ba2c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469689"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="93a3b-103">Тип ресурса Битлоккеррековерйоптионс</span><span class="sxs-lookup"><span data-stu-id="93a3b-103">bitLockerRecoveryOptions resource type</span></span>

<span data-ttu-id="93a3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93a3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93a3b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93a3b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93a3b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93a3b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93a3b-107">Параметры восстановления BitLocker.</span><span class="sxs-lookup"><span data-stu-id="93a3b-107">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="93a3b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="93a3b-108">Properties</span></span>
|<span data-ttu-id="93a3b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="93a3b-109">Property</span></span>|<span data-ttu-id="93a3b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="93a3b-110">Type</span></span>|<span data-ttu-id="93a3b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="93a3b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93a3b-112">блоккдатарековеряжент</span><span class="sxs-lookup"><span data-stu-id="93a3b-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="93a3b-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="93a3b-113">Boolean</span></span>|<span data-ttu-id="93a3b-114">Указывает, следует ли заблокировать агент восстановления данных на основе сертификатов.</span><span class="sxs-lookup"><span data-stu-id="93a3b-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="93a3b-115">рековерипассвордусаже</span><span class="sxs-lookup"><span data-stu-id="93a3b-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="93a3b-116">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="93a3b-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="93a3b-117">Указывает, разрешено ли пользователям создавать пароль восстановления для фиксированного или системного диска с 48 цифр.</span><span class="sxs-lookup"><span data-stu-id="93a3b-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="93a3b-118">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="93a3b-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="93a3b-119">рековерикэйусаже</span><span class="sxs-lookup"><span data-stu-id="93a3b-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="93a3b-120">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="93a3b-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="93a3b-121">Указывает, могут ли пользователи создавать ключ восстановления 256 бит для фиксированного или системного диска.</span><span class="sxs-lookup"><span data-stu-id="93a3b-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="93a3b-122">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="93a3b-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="93a3b-123">хидерековерйоптионс</span><span class="sxs-lookup"><span data-stu-id="93a3b-123">hideRecoveryOptions</span></span>|<span data-ttu-id="93a3b-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="93a3b-124">Boolean</span></span>|<span data-ttu-id="93a3b-125">Указывает, можно ли отображать параметры восстановления в мастере установки BitLocker для фиксированного или системного диска.</span><span class="sxs-lookup"><span data-stu-id="93a3b-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="93a3b-126">енаблерековеринформатионсаветосторе</span><span class="sxs-lookup"><span data-stu-id="93a3b-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="93a3b-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="93a3b-127">Boolean</span></span>|<span data-ttu-id="93a3b-128">Указывает, следует ли запретить хранение данных восстановления BitLocker в доменных СЛУЖБах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="93a3b-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="93a3b-129">рековеринформатионтосторе</span><span class="sxs-lookup"><span data-stu-id="93a3b-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="93a3b-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="93a3b-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="93a3b-131">Настройте, какие части данных восстановления BitLocker хранятся в AD DS.</span><span class="sxs-lookup"><span data-stu-id="93a3b-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="93a3b-132">Возможные значения: `passwordAndKey`, `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="93a3b-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="93a3b-133">енаблебитлоккерафтеррековеринформатионтосторе</span><span class="sxs-lookup"><span data-stu-id="93a3b-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="93a3b-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="93a3b-134">Boolean</span></span>|<span data-ttu-id="93a3b-135">Указывает, следует ли включить BitLocker до тех пор, пока данные для восстановления не будут храниться в доменных СЛУЖБах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="93a3b-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93a3b-136">Связи</span><span class="sxs-lookup"><span data-stu-id="93a3b-136">Relationships</span></span>
<span data-ttu-id="93a3b-137">Нет</span><span class="sxs-lookup"><span data-stu-id="93a3b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93a3b-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93a3b-138">JSON Representation</span></span>
<span data-ttu-id="93a3b-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93a3b-139">Here is a JSON representation of the resource.</span></span>
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



