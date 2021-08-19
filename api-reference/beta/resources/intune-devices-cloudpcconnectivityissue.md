---
title: тип ресурса cloudPCConnectivityIssue
description: Пользователь испытывает аналитичность объекта проблемы подключения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 70e0e31ea7451952800830aa7ef259a19592cd0a12d5919a8df85340904ee53a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54172976"
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
|id|String|Уникальный идентификатор объекта событий событий для аналитики пользовательского интерфейса.|
|deviceId|String|Устройство Intune устройства, с которое связано подключение.|
|errorCode|String|Код ошибки проблемы подключения.|
|errorDateTime|DateTimeOffset|Время начала подключения. Время отображается в формате ISO 8601 и времени скоординированного универсального времени (UTC).|
|userId|String|Уникальный id пользователя, который инициализирует подключение.|
|errorDescription|String|Подробное описание того, что пошло не так.|
|recommendedAction|Строка|Рекомендуемое действие для устранения соответствующей ошибки.|

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




