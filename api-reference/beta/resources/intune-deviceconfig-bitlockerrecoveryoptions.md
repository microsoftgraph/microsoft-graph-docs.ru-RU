---
title: Тип ресурса Битлоккеррековерйоптионс
description: Параметры восстановления BitLocker.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c66de5025778a46f63712c61b888c0c2756e3e6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333802"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="d2572-103">Тип ресурса Битлоккеррековерйоптионс</span><span class="sxs-lookup"><span data-stu-id="d2572-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="d2572-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2572-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2572-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2572-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2572-106">Параметры восстановления BitLocker.</span><span class="sxs-lookup"><span data-stu-id="d2572-106">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="d2572-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2572-107">Properties</span></span>
|<span data-ttu-id="d2572-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2572-108">Property</span></span>|<span data-ttu-id="d2572-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d2572-109">Type</span></span>|<span data-ttu-id="d2572-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d2572-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2572-111">блоккдатарековеряжент</span><span class="sxs-lookup"><span data-stu-id="d2572-111">blockDataRecoveryAgent</span></span>|<span data-ttu-id="d2572-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2572-112">Boolean</span></span>|<span data-ttu-id="d2572-113">Указывает, следует ли заблокировать агент восстановления данных на основе сертификатов.</span><span class="sxs-lookup"><span data-stu-id="d2572-113">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="d2572-114">рековерипассвордусаже</span><span class="sxs-lookup"><span data-stu-id="d2572-114">recoveryPasswordUsage</span></span>|[<span data-ttu-id="d2572-115">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="d2572-115">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d2572-116">Указывает, разрешено ли пользователям создавать пароль восстановления для фиксированного или системного диска с 48 цифр.</span><span class="sxs-lookup"><span data-stu-id="d2572-116">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="d2572-117">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d2572-117">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d2572-118">рековерикэйусаже</span><span class="sxs-lookup"><span data-stu-id="d2572-118">recoveryKeyUsage</span></span>|[<span data-ttu-id="d2572-119">конфигуратионусаже</span><span class="sxs-lookup"><span data-stu-id="d2572-119">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="d2572-120">Указывает, могут ли пользователи создавать ключ восстановления 256 бит для фиксированного или системного диска.</span><span class="sxs-lookup"><span data-stu-id="d2572-120">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="d2572-121">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="d2572-121">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="d2572-122">хидерековерйоптионс</span><span class="sxs-lookup"><span data-stu-id="d2572-122">hideRecoveryOptions</span></span>|<span data-ttu-id="d2572-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2572-123">Boolean</span></span>|<span data-ttu-id="d2572-124">Указывает, можно ли отображать параметры восстановления в мастере установки BitLocker для фиксированного или системного диска.</span><span class="sxs-lookup"><span data-stu-id="d2572-124">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="d2572-125">енаблерековеринформатионсаветосторе</span><span class="sxs-lookup"><span data-stu-id="d2572-125">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="d2572-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2572-126">Boolean</span></span>|<span data-ttu-id="d2572-127">Указывает, следует ли запретить хранение данных восстановления BitLocker в доменных СЛУЖБах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d2572-127">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="d2572-128">рековеринформатионтосторе</span><span class="sxs-lookup"><span data-stu-id="d2572-128">recoveryInformationToStore</span></span>|[<span data-ttu-id="d2572-129">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="d2572-129">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="d2572-130">Настройте, какие части данных восстановления BitLocker хранятся в AD DS.</span><span class="sxs-lookup"><span data-stu-id="d2572-130">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="d2572-131">Возможные значения: `passwordAndKey`, `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="d2572-131">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="d2572-132">енаблебитлоккерафтеррековеринформатионтосторе</span><span class="sxs-lookup"><span data-stu-id="d2572-132">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="d2572-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2572-133">Boolean</span></span>|<span data-ttu-id="d2572-134">Указывает, следует ли включить BitLocker до тех пор, пока данные для восстановления не будут храниться в доменных СЛУЖБах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d2572-134">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2572-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="d2572-135">Relationships</span></span>
<span data-ttu-id="d2572-136">Нет</span><span class="sxs-lookup"><span data-stu-id="d2572-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2572-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2572-137">JSON Representation</span></span>
<span data-ttu-id="d2572-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2572-138">Here is a JSON representation of the resource.</span></span>
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



