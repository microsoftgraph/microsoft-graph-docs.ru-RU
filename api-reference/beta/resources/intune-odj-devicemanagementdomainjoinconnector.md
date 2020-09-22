---
title: Тип ресурса Девицеманажементдомаинжоинконнектор
description: Соединитель присоединения к домену это соединитель, отвечающий за выделение и удаление больших двоичных объектов учетной записи компьютера.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c5f5cfd272e8f2adc5d2916f3783192be9a5a5ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029850"
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
|id|String|Уникальный идентификатор, представляющий соединитель.|
|displayName|String|Отображаемое имя соединителя.|
|lastConnectionDateTime|DateTimeOffset|Последний соединитель времени с обращением к Intune.|
|state|[deviceManagementDomainJoinConnectorState](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|Состояние соединителя. Возможные значения: `active`, `error`, `inactive`.|
|version|String|Версия соединителя.|

## <a name="relationships"></a>Отношения
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






