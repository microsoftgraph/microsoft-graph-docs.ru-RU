---
title: Тип ресурса Секуритибаселинестатесуммари
description: Сводка по состоянию соответствия нормативным требованиям безопасности для учетной записи базового уровня безопасности учетной записи.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8133fb325b0c2abdacf38e034aedc6523b13623c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562225"
---
# <a name="securitybaselinestatesummary-resource-type"></a>Тип ресурса Секуритибаселинестатесуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка по состоянию соответствия нормативным требованиям безопасности для учетной записи базового уровня безопасности учетной записи.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Секуритибаселинестатесуммари](../api/intune-deviceintent-securitybaselinestatesummary-get.md)|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|Чтение свойств и связей объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) .|
|[Обновление Секуритибаселинестатесуммари](../api/intune-deviceintent-securitybaselinestatesummary-update.md)|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|Обновление свойств объекта [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта.|
|Секурекаунт|Int32|Количество защищенных устройств|
|Нотсекурекаунт|Int32|Количество незащищенных устройств|
|unknownCount|Int32|Количество неизвестных устройств.|
|errorCount|Int32|Количество устройств с ошибками.|
|conflictCount|Int32|Количество конфликтующих устройств.|
|notApplicableCount|Int32|Количество неприменимых устройств.|

## <a name="relationships"></a>Отношения
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





