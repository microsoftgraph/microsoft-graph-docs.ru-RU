---
title: тип ресурса cloudPCConnectivityIssue
description: Пользователь испытывает аналитичность объекта проблемы подключения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5b232a2848a66dfc242f83da39667e9b891f852f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58784480"
---
# <a name="cloudpcconnectivityissue-resource-type"></a>тип ресурса cloudPCConnectivityIssue

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пользователь испытывает аналитичность объекта проблемы подключения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список cloudPCConnectivityIssues](../api/intune-devices-cloudpcconnectivityissue-list.md)|[коллекция cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md)|Список свойств и связей объектов [cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)|
|[Get cloudPCConnectivityIssue](../api/intune-devices-cloudpcconnectivityissue-get.md)|[cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md)|Чтение свойств и связей объекта [cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)|
|[Создание cloudPCConnectivityIssue](../api/intune-devices-cloudpcconnectivityissue-create.md)|[cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md)|Создание нового [объекта cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)|
|[Удаление cloudPCConnectivityIssue](../api/intune-devices-cloudpcconnectivityissue-delete.md)|Нет|Удаляет [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md).|
|[Обновление cloudPCConnectivityIssue](../api/intune-devices-cloudpcconnectivityissue-update.md)|[cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md)|Обновление свойств объекта [cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта событий событий для аналитики пользовательского интерфейса.|
|deviceId|String|Устройство Intune устройства, с которое связано подключение.|
|errorCode|String|Код ошибки проблемы подключения.|
|errorDateTime|DateTimeOffset|Время начала подключения. Время отображается в формате ISO 8601 и времени скоординированного универсального времени (UTC).|
|userId|String|Уникальный id пользователя, который инициализирует подключение.|
|errorDescription|String|Подробное описание того, что пошло не так.|
|recommendedAction|String|Рекомендуемое действие для устранения соответствующей ошибки.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPCConnectivityIssue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "id": "String (identifier)",
  "deviceId": "String",
  "errorCode": "String",
  "errorDateTime": "String (timestamp)",
  "userId": "String",
  "errorDescription": "String",
  "recommendedAction": "String"
}
```



