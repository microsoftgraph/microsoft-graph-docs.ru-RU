---
title: Тип ресурса Девицеманажементдомаинжоинконнектор
description: Соединитель присоединения к домену это соединитель, отвечающий за выделение и удаление больших двоичных объектов учетной записи компьютера.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0537d38d87a2cb574ca8984f895ed3796c33703a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001925"
---
# <a name="devicemanagementdomainjoinconnector-resource-type"></a>Тип ресурса Девицеманажементдомаинжоинконнектор

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Соединитель присоединения к домену это соединитель, отвечающий за выделение и удаление больших двоичных объектов учетной записи компьютера.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементдомаинжоинконнекторс](../api/intune-odj-devicemanagementdomainjoinconnector-list.md)|Коллекция [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Список свойств и связей объектов [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .|
|[Получение Девицеманажементдомаинжоинконнектор](../api/intune-odj-devicemanagementdomainjoinconnector-get.md)|[Девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Чтение свойств и связей объекта [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .|
|[Создание Девицеманажементдомаинжоинконнектор](../api/intune-odj-devicemanagementdomainjoinconnector-create.md)|[Девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Создание нового объекта [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .|
|[Удаление Девицеманажементдомаинжоинконнектор](../api/intune-odj-devicemanagementdomainjoinconnector-delete.md)|Нет|Удаляет объект [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md).|
|[Обновление Девицеманажементдомаинжоинконнектор](../api/intune-odj-devicemanagementdomainjoinconnector-update.md)|[Девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Обновление свойств объекта [девицеманажементдомаинжоинконнектор](../resources/intune-odj-devicemanagementdomainjoinconnector.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор, представляющий соединитель.|
|displayName|Строка|Отображаемое имя соединителя.|
|lastConnectionDateTime|DateTimeOffset|Последний соединитель времени с обращением к Intune.|
|состояние|[Девицеманажементдомаинжоинконнекторстате](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|Состояние соединителя. Возможные значения: `active`, `error`, `inactive`.|
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





