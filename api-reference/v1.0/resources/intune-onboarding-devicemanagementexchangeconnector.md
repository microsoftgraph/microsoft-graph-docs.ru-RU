---
title: Тип ресурса deviceManagementExchangeConnector
description: Объект, представляющий подключение к среде Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 172a8ae7bbdbad77da9b7a67d57047441e5a039d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583986"
---
# <a name="devicemanagementexchangeconnector-resource-type"></a>Тип ресурса deviceManagementExchangeConnector

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий подключение к среде Exchange.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceManagementExchangeConnector](../api/intune-onboarding-devicemanagementexchangeconnector-list.md)|Коллекция [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Список свойств и связей объектов [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).|
|[Получение объекта deviceManagementExchangeConnector](../api/intune-onboarding-devicemanagementexchangeconnector-get.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md);|Чтение свойств и связей объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).|
|[Создание объекта deviceManagementExchangeConnector](../api/intune-onboarding-devicemanagementexchangeconnector-create.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md);|Создание объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).|
|[Удаление объекта deviceManagementExchangeConnector](../api/intune-onboarding-devicemanagementexchangeconnector-delete.md)|Нет|Удаляет объект [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).|
|[Обновление объекта deviceManagementExchangeConnector](../api/intune-onboarding-devicemanagementexchangeconnector-update.md)|[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md)|Обновление свойств объекта [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).|
|[Действие sync](../api/intune-onboarding-devicemanagementexchangeconnector-sync.md)|Нет|Пока не задокументировано|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Н/Д|
|lastSyncDateTime|DateTimeOffset|Время последней синхронизации соединителя Exchange|
|status|[Девицеманажементексчанжеконнекторстатус](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|Состояние соединителя Exchange. Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.|
|primarySmtpAddress|String|Электронный адрес, используемый для настройки соединителя Exchange между службами.|
|serverName|String|Имя сервера Exchange Server.|
|connectorServerName|String|Имя сервера, на котором размещается соединитель Exchange.|
|exchangeConnectorType|[Девицеманажементексчанжеконнектортипе](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|Тип настраиваемого соединителя Exchange. Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|version|Строка|Версия объекта ExchangeConnectorAgent|
|exchangeAlias|String|Псевдоним, назначенный серверу Exchange Server|
|exchangeOrganization|String|Организация Exchange, соответствующая серверу Exchange Server|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExchangeConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "status": "String",
  "primarySmtpAddress": "String",
  "serverName": "String",
  "connectorServerName": "String",
  "exchangeConnectorType": "String",
  "version": "String",
  "exchangeAlias": "String",
  "exchangeOrganization": "String"
}
```



