---
title: Тип ресурса Микрософттуннелсервер
description: Сущность, представляющая один сервер туннеля (Майкрософт)
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed9968e5f1d0f4c530d09d0ff8950ad6864b90c2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302023"
---
# <a name="microsofttunnelserver-resource-type"></a>Тип ресурса Микрософттуннелсервер

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность, представляющая один сервер туннеля (Майкрософт)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Микрософттуннелсерверс](../api/intune-mstunnel-microsofttunnelserver-list.md)|Коллекция [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md)|Список свойств и связей объектов [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md) .|
|[Получение Микрософттуннелсервер](../api/intune-mstunnel-microsofttunnelserver-get.md)|[микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md)|Чтение свойств и связей объекта [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md) .|
|[Создание Микрософттуннелсервер](../api/intune-mstunnel-microsofttunnelserver-create.md)|[микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md)|Создание нового объекта [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md) .|
|[Удаление Микрософттуннелсервер](../api/intune-mstunnel-microsofttunnelserver-delete.md)|Нет|Удаляет объект [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md).|
|[Обновление Микрософттуннелсервер](../api/intune-mstunnel-microsofttunnelserver-update.md)|[микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md)|Обновление свойств объекта [микрософттуннелсервер](../resources/intune-mstunnel-microsofttunnelserver.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор Микрософттуннелсервер|
|displayName|String|Отображаемое имя Микрософттуннелсервер|
|туннелсерверхеалсстатус|[microsoftTunnelServerHealthStatus](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|Состояние работоспособности Микрософттуннелсервер. Возможные значения: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.|
|ластчеккиндатетиме|DateTimeOffset|При последнем возвращенном Микрософттуннелсервер|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftTunnelServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "id": "String (identifier)",
  "displayName": "String",
  "tunnelServerHealthStatus": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```




