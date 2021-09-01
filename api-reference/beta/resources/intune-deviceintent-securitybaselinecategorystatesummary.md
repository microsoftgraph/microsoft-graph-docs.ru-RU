---
title: тип ресурса securityBaselineCategoryStateSummary
description: Сводка состояния соответствия требованиям безопасности для базового уровня безопасности учетной записи.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bc0bb04e7545ade025b3659a921ccb34237a0290
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801474"
---
# <a name="securitybaselinecategorystatesummary-resource-type"></a>тип ресурса securityBaselineCategoryStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводка состояния соответствия требованиям безопасности для базового уровня безопасности учетной записи.


Наследует [от securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список securityBaselineCategoryStateSummaries](../api/intune-deviceintent-securitybaselinecategorystatesummary-list.md)|[коллекция securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Список свойств и связей объектов [securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|
|[Получить securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-get.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Чтение свойств и связей объекта [securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|
|[Создание securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-create.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Создайте новый [объект securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|
|[Удаление securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-delete.md)|Нет|Удаляет [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).|
|[Обновление securityBaselineCategoryStateSummary](../api/intune-deviceintent-securitybaselinecategorystatesummary-update.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Обновление свойств объекта [securityBaselineCategoryStateSummary.](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта. Унаследованный от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|secureCount|Int32|Количество защищенных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|notSecureCount|Int32|Количество не защищенных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|unknownCount|Int32|Количество неизвестных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|errorCount|Int32|Количество устройств с ошибками, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|conflictCount|Int32|Количество конфликтных устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|notApplicableCount|Int32|Количество не применимых устройств, унаследованных от [securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|displayName|Строка|Имя категории|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineCategoryStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024,
  "displayName": "String"
}
```



