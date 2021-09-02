---
title: тип ресурса deviceManagementDomainJoinConnector
description: Соединителя подключения к домену является соединитетелем, который отвечает за выделение (и удаление) blobs учетной записи компьютера
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f99f8dc17e292ca01a614cf1201cab8d0f918cd4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783864"
---
# <a name="devicemanagementdomainjoinconnector-resource-type"></a>тип ресурса deviceManagementDomainJoinConnector

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Соединителя подключения к домену является соединитетелем, который отвечает за выделение (и удаление) blobs учетной записи компьютера

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List deviceManagementDomainJoinConnectors](../api/intune-odj-devicemanagementdomainjoinconnector-list.md)|[коллекция deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Список свойств и связей объектов [deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|
|[Get deviceManagementDomainJoinConnector](../api/intune-odj-devicemanagementdomainjoinconnector-get.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Чтение свойств и связей [объекта deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|
|[Создание deviceManagementDomainJoinConnector](../api/intune-odj-devicemanagementdomainjoinconnector-create.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Создайте новый [объект deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|
|[Удаление deviceManagementDomainJoinConnector](../api/intune-odj-devicemanagementdomainjoinconnector-delete.md)|Нет|Удаляет [устройствоManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).|
|[Обновление deviceManagementDomainJoinConnector](../api/intune-odj-devicemanagementdomainjoinconnector-update.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Обновление свойств объекта [deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для представления соединитетеля.|
|displayName|Строка|Имя отображения соединитетеля.|
|lastConnectionDateTime|DateTimeOffset|Последний раз соединитель связывался с Intune.|
|state|[deviceManagementDomainJoinConnectorState](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|Состояние соединитетеля. Возможные значения: `active`, `error`, `inactive`.|
|version|String|Версия соединитетеля.|

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



