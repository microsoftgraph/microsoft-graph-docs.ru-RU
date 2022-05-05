---
title: Тип ресурса zebraFotaConnector
description: Сущность соединителя Zebra FOTA, представляющая состояние авторизации клиента для Intune вызова служб Zebra Update Services.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae01c91dc398f2780b4f0288233664c36ad7a8b4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213539"
---
# <a name="zebrafotaconnector-resource-type"></a>Тип ресурса zebraFotaConnector

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность соединителя Zebra FOTA, представляющая состояние авторизации клиента для Intune вызова служб Zebra Update Services.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение zebraFotaConnector](../api/intune-androidfotaservice-zebrafotaconnector-get.md)|[zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md)|Чтение свойств и связей объекта [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) .|
|[Обновление zebraFotaConnector](../api/intune-androidfotaservice-zebrafotaconnector-update.md)|[zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md)|Обновление свойств объекта [zebraFotaConnector](../resources/intune-androidfotaservice-zebrafotaconnector.md) .|
|[Действие hasActiveDeployments](../api/intune-androidfotaservice-zebrafotaconnector-hasactivedeployments.md)|Boolean|Н/Д|
|[Действие approveFotaApps](../api/intune-androidfotaservice-zebrafotaconnector-approvefotaapps.md)|Boolean|Н/Д|
|[Действие подключения](../api/intune-androidfotaservice-zebrafotaconnector-connect.md)|Boolean|Н/Д|
|[Действие disconnect](../api/intune-androidfotaservice-zebrafotaconnector-disconnect.md)|Boolean|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор ZebraFotaConnector.|
|state|[zebraFotaConnectorState](../resources/intune-androidfotaservice-zebrafotaconnectorstate.md)|Состояние соединителя Zebra. Возможные значения: `none`, `connected`, `disconnected`, `unknownFutureValue`.|
|enrollmentToken|Строка|Маркер регистрации клиента от Zebra. Маркер используется для регистрации устройств Zebra в службе FOTA с помощью конфигурации приложения.|
|enrollmentAuthorizationUrl|Строка|Полный URL-адрес авторизации регистрации учетной записи. Это соответствует verification_uri_complete документации по API Zebra.|
|lastSyncDateTime|DateTimeOffset|Дата и время последней синхронизации учетной записи с Zebra|
|fotaAppsApproved|Логическое|Флаг, указывающий, утверждены ли необходимые приложения встроенного ПО по беспроводной сети (FOTA).|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.zebraFotaConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaConnector",
  "id": "String (identifier)",
  "state": "String",
  "enrollmentToken": "String",
  "enrollmentAuthorizationUrl": "String",
  "lastSyncDateTime": "String (timestamp)",
  "fotaAppsApproved": true
}
```




