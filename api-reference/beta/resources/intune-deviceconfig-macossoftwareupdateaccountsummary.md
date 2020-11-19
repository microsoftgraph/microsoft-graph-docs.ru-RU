---
title: Тип ресурса Макоссофтвареупдатеаккаунтсуммари
description: Сводный отчет по учетной записи обновления программного обеспечения MacOS для устройства и пользователя
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac1b4a458325671252655986cb3089940be10bd4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294132"
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
|[Получение Макоссофтвареупдатеаккаунтсуммари](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-get.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|Чтение свойств и связей объекта [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) .|
|[Создание Макоссофтвареупдатеаккаунтсуммари](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-create.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|Создание нового объекта [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) .|
|[Удаление Макоссофтвареупдатеаккаунтсуммари](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-delete.md)|Нет|Удаляет объект [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md).|
|[Обновление Макоссофтвареупдатеаккаунтсуммари](../api/intune-deviceconfig-macossoftwareupdateaccountsummary-update.md)|[macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)|Обновление свойств объекта [макоссофтвареупдатеаккаунтсуммари](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|String|Имя отчета|
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




