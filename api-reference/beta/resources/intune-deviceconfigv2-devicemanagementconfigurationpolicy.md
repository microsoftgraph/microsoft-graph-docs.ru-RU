---
title: Тип ресурса Девицеманажементконфигуратионполици
description: Политика конфигурации управления устройствами
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b00db0b46c03726561cff31a6a7f9a52b165a55b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242223"
---
# <a name="devicemanagementconfigurationpolicy-resource-type"></a>Тип ресурса Девицеманажементконфигуратионполици

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика конфигурации управления устройствами

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список ДевицеманажементконфигуратионполиЦиес](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-list.md)|Коллекция [девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Список свойств и связей объектов [девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) .|
|[Получение Девицеманажементконфигуратионполици](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-get.md)|[девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Чтение свойств и связей объекта [девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) .|
|[Создание Девицеманажементконфигуратионполици](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-create.md)|[девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Создание нового объекта [девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) .|
|[Удаление Девицеманажементконфигуратионполици](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-delete.md)|Нет|Удаляет объект [девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md).|
|[Обновление Девицеманажементконфигуратионполици](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-update.md)|[девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)|Обновление свойств объекта [девицеманажементконфигуратионполици](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) .|
|[Действие assign](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicy-assign.md)|Коллекция [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ документа политики. Создается автоматически.|
|name|String|Имя политики|
|description|String|Описание политики|
|Embedded|[девицеманажементконфигуратионплатформс](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|Платформы для этой политики. Возможные значения: `none`, `macOS`, `windows10X`, `windows10`.|
|технологически|[девицеманажементконфигуратионтечнологиес](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|Технологии для этой политики. Возможные значения: `none`, `mdm`, `windows10XManagement`, `configManager`.|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Это свойство доступно только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения политики. Это свойство доступно только для чтения.|
|settingCount|Int32|Количество параметров. Это свойство доступно только для чтения.|
|креатионсаурце|String|Источник создания политики|
|roleScopeTagIds|Коллекция строк|Список тегов областей для этого экземпляра сущности.|
|isAssigned|Boolean|Состояние назначения политики. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|параметры|Коллекция [девицеманажементконфигуратионсеттинг](../resources/intune-deviceconfigv2-devicemanagementconfigurationsetting.md)|Параметры политики|
|assignments|Коллекция [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Назначения политик|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "id": "String (identifier)",
  "name": "String",
  "description": "String",
  "platforms": "String",
  "technologies": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "settingCount": 1024,
  "creationSource": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "isAssigned": true
}
```




