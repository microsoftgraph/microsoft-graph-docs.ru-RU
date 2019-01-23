---
title: Тип ресурса bitLockerRecoveryOptions
description: Варианты восстановления BitLocker.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df1a2d0a9be3f4ec52b5fa289d0315bda36e4a59
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398515"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="4435c-103">Тип ресурса bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="4435c-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="4435c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4435c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4435c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4435c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4435c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4435c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4435c-107">Варианты восстановления BitLocker.</span><span class="sxs-lookup"><span data-stu-id="4435c-107">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="4435c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4435c-108">Properties</span></span>
|<span data-ttu-id="4435c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4435c-109">Property</span></span>|<span data-ttu-id="4435c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4435c-110">Type</span></span>|<span data-ttu-id="4435c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4435c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4435c-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="4435c-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="4435c-113">Логический</span><span class="sxs-lookup"><span data-stu-id="4435c-113">Boolean</span></span>|<span data-ttu-id="4435c-114">Указывает, следует ли блокировать агентом восстановления данных на основе сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4435c-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="4435c-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="4435c-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="4435c-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="4435c-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="4435c-117">Указывает ли пользователи могут или должны создавать пароль восстановления из 48 цифр основных или системный диск.</span><span class="sxs-lookup"><span data-stu-id="4435c-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="4435c-118">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="4435c-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="4435c-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="4435c-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="4435c-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="4435c-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="4435c-121">Указывает ли пользователям разрешено или необходимо создание ключа восстановления 256-разрядный основных или системный диск.</span><span class="sxs-lookup"><span data-stu-id="4435c-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="4435c-122">Возможные значения: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="4435c-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="4435c-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="4435c-123">hideRecoveryOptions</span></span>|<span data-ttu-id="4435c-124">Логический</span><span class="sxs-lookup"><span data-stu-id="4435c-124">Boolean</span></span>|<span data-ttu-id="4435c-125">Указывает ли разрешать отображение параметры восстановления в мастер установки BitLocker основных или системный диск.</span><span class="sxs-lookup"><span data-stu-id="4435c-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="4435c-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="4435c-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="4435c-127">Логический</span><span class="sxs-lookup"><span data-stu-id="4435c-127">Boolean</span></span>|<span data-ttu-id="4435c-128">Указывает, следует ли разрешить сведения о восстановлении BitLocker для хранения в Доменных службах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4435c-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="4435c-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="4435c-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="4435c-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="4435c-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="4435c-131">Настройте, какие части сведения о восстановлении BitLocker хранятся в Доменных службах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4435c-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="4435c-132">Возможные значения: `passwordAndKey`, `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="4435c-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="4435c-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="4435c-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="4435c-134">Логический</span><span class="sxs-lookup"><span data-stu-id="4435c-134">Boolean</span></span>|<span data-ttu-id="4435c-135">Указывает, следует ли включить BitLocker до восстановления данные хранятся в Доменных службах Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4435c-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4435c-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="4435c-136">Relationships</span></span>
<span data-ttu-id="4435c-137">Нет</span><span class="sxs-lookup"><span data-stu-id="4435c-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4435c-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4435c-138">JSON Representation</span></span>
<span data-ttu-id="4435c-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4435c-139">Here is a JSON representation of the resource.</span></span>
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




