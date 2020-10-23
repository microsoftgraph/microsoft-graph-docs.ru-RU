---
title: Тип ресурса Девицеманажементдомаинжоинконнектор
description: Соединитель присоединения к домену это соединитель, отвечающий за выделение и удаление больших двоичных объектов учетной записи компьютера.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e078626edb5b4d8a4d66813ddc358a24624cedb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691171"
---
# <a name="devicemanagementdomainjoinconnector-resource-type"></a>Тип ресурса Девицеманажементдомаинжоинконнектор

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Соединитель присоединения к домену это соединитель, отвечающий за выделение и удаление больших двоичных объектов учетной записи компьютера.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементдомаинжоинконнекторс](../api/intune-odj-devicemanagementdomainjoinconnector-list.md)|Коллекция [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Список свойств и связей объектов [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .|
|[Получение Девицеманажементдомаинжоинконнектор](../api/intune-odj-devicemanagementdomainjoinconnector-get.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Чтение свойств и связей объекта [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .|
|[Создание Девицеманажементдомаинжоинконнектор](../api/intune-odj-devicemanagementdomainjoinconnector-create.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Создание нового объекта [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .|
|[Удаление Девицеманажементдомаинжоинконнектор](../api/intune-odj-devicemanagementdomainjoinconnector-delete.md)|Нет|Удаляет объект [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md).|
|[Обновление Девицеманажементдомаинжоинконнектор](../api/intune-odj-devicemanagementdomainjoinconnector-update.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Обновление свойств объекта [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор, представляющий соединитель.|
|displayName|Строка|Отображаемое имя соединителя.|
|lastConnectionDateTime|DateTimeOffset|Последний соединитель времени с обращением к Intune.|
|state|[deviceManagementDomainJoinConnectorState](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|Состояние соединителя. Возможные значения: `active`, `error`, `inactive`.|
|version|String|Версия соединителя.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDomainJoinConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
}
```





