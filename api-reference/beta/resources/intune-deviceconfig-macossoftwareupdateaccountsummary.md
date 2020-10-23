---
title: Тип ресурса Макоссофтвареупдатеаккаунтсуммари
description: Сводный отчет по учетной записи обновления программного обеспечения MacOS для устройства и пользователя
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 46a7cf012954189a3c14bdcdb6364ed9557d7f84
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727472"
---
# <a name="macossoftwareupdateaccountsummary-resource-type"></a>Тип ресурса Макоссофтвареупдатеаккаунтсуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сводный отчет по учетной записи обновления программного обеспечения MacOS для устройства и пользователя

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Макоссофтвареупдатеаккаунтсуммариес](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-list.md)|Коллекция [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|Список свойств и связей объектов [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) .|
|[Получение Макоссофтвареупдатеаккаунтсуммари](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-get.md)|[макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|Чтение свойств и связей объекта [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) .|
|[Создание Макоссофтвареупдатеаккаунтсуммари](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-create.md)|[макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|Создание нового объекта [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) .|
|[Удаление Макоссофтвареупдатеаккаунтсуммари](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-delete.md)|Нет|Удаляет объект [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md).|
|[Обновление Макоссофтвареупдатеаккаунтсуммари](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-update.md)|[макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|Обновление свойств объекта [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|displayName|Строка|Имя отчета|
|deviceId|String|ИДЕНТИФИКАТОР устройства.|
|userId|String|Идентификатор пользователя.|
|deviceName|String|Имя устройства.|
|userPrincipalName|String|Имя участника пользователя|
|osVersion|String|Версия ОС.|
|сукцессфулупдатекаунт|Int32|Количество успешных обновлений на устройстве.|
|фаиледупдатекаунт|Int32|Количество неудачных обновлений на устройстве.|
|тоталупдатекаунт|Int32|Общее количество обновлений на устройстве.|
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления отчета для этого устройства.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|категорисуммариес|Коллекция [макоссофтвареупдатекатегорисуммари](../resources/intune-deviceconfig-macossoftwareupdatecategorysummary.md)|Сводка обновлений по категории.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSSoftwareUpdateAccountSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "deviceId": "String",
  "userId": "String",
  "deviceName": "String",
  "userPrincipalName": "String",
  "osVersion": "String",
  "successfulUpdateCount": 1024,
  "failedUpdateCount": 1024,
  "totalUpdateCount": 1024,
  "lastUpdatedDateTime": "String (timestamp)"
}
```





