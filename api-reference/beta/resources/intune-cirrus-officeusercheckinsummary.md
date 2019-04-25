---
title: Тип ресурса Оффицеусерчеккинсуммари
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b74d7508c9ef3b1d7183c806783e567cb75859ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526386"
---
# <a name="officeusercheckinsummary-resource-type"></a>Тип ресурса Оффицеусерчеккинсуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, описывающая статистику по возврату клиента.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|Сукцеедедусеркаунт|Int32|Общее количество успешных проверок пользователей за последние 3 месяца.|
|failedUserCount|Int32|Общее число неудачных проверок пользователей за последние 3 месяца.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```



