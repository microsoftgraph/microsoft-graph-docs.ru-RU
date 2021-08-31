---
title: тип ресурса securityBaselineStateSummary
description: Сводка состояния соответствия базовой безопасности для базового уровня безопасности учетной записи.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 732ea052ec544c88abdfb14f7f40085ff6fe8f2e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58782079"
---
# <a name="securitybaselinestatesummary-resource-type"></a>тип ресурса securityBaselineStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка состояния соответствия базовой безопасности для базового уровня безопасности учетной записи.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получить securityBaselineStateSummary](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|Чтение свойств и связей объекта [securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|[Обновление securityBaselineStateSummary](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|Обновление свойств объекта [securityBaselineStateSummary.](../resources/intune-deviceintent-securitybaselinestatesummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта.|
|secureCount|Int32|Количество защищенных устройств|
|notSecureCount|Int32|Число небезопасных устройств|
|unknownCount|Int32|Количество неизвестных устройств.|
|errorCount|Int32|Количество устройств с ошибками.|
|conflictCount|Int32|Количество конфликтующих устройств.|
|notApplicableCount|Int32|Количество неприменимых устройств.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024
}
```



