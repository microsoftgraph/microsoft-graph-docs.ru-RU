---
title: Тип ресурса sharedPCAccountManagerPolicy
description: Политика диспетчера учетных записей SharedPC. Применяется, только если включен диспетчер учетных записей.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f0e0a1b847c5c4f6481cd826ddac499cc5133dd
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60455304"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a>Тип ресурса sharedPCAccountManagerPolicy

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика диспетчера учетных записей SharedPC. Применяется, только если включен диспетчер учетных записей.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accountDeletionPolicy|[sharedPCAccountDeletionPolicyType](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|Настраивается при удалении учетных записей. Возможные значения: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.|
|cacheAccountsAboveDiskFreePercentage|Int32|Задает доступное место на диске в процентах, которое должно быть на компьютере, прежде чем будет прекращено удаление кэшированных учетных записей на общем компьютере. Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThreshold или DiskSpaceThresholdOrInactiveThreshold. Допустимые значения: от 0 до 100.|
|inactiveThresholdDays|Int32|Указывает, будут ли удаляться учетные записи, если в течение указанного периода (в днях) в них не входили пользователи. Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThreshold или DiskSpaceThresholdOrInactiveThreshold.|
|removeAccountsBelowDiskFreePercentage|Int32|Задает минимальное место на диске в процентах, оставшееся на компьютере, при сокращении которого кэшированные учетные записи будут удаляться для освобождения дискового пространства. Сначала будут удалены учетные записи, неактивные в течение самого длинного периода. Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThresholdOrInactiveThreshold. Допустимые значения: от 0 до 100.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```



