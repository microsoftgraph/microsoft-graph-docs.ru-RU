---
title: Тип ресурса networkIPv6ConfigurationManagementCondition
description: Параметры сети IPv6 условия управления на основе конфигурации может быть определен, который будет запускать при обнаружении определенных IP-адрес устройства. Условие управления конфигурации IP-адресов только рассматривается как TRUE при активной сетевого подключения. Не может быть сопоставлен адресов IPv6 DHCP-сервера. Это, так как Windows (приблизительно Redstone) не предоставляет эти сведения в службу природные проверки подлинности.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 497e5ec8d2fbde5a4687b6f30afef9383f2a890b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421195"
---
# <a name="networkipv6configurationmanagementcondition-resource-type"></a>Тип ресурса networkIPv6ConfigurationManagementCondition

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры сети IPv6 условия управления на основе конфигурации может быть определен, который будет запускать при обнаружении определенных IP-адрес устройства. Условие управления конфигурации IP-адресов только рассматривается как TRUE при активной сетевого подключения.
Не может быть сопоставлен адресов IPv6 DHCP-сервера. Это, так как Windows (приблизительно Redstone) не предоставляет эти сведения в службу природные проверки подлинности.


Наследуется от [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список networkIPv6ConfigurationManagementConditions](../api/intune-fencing-networkipv6configurationmanagementcondition-list.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) коллекции|Свойства списка и связей объектов [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .|
|[Получение networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-get.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Чтение свойства и связи объекта [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .|
|[Создание networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-create.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Создание нового объекта [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .|
|[Удаление networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-delete.md)|Нет|Удаляет [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).|
|[Обновление networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-update.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Обновление свойства объекта [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для управления условия. Значение, назначенное при создании создаваемый системой. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|уникального имени|String|Уникальное имя для управления условия. Используется в выражениях условие управления. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|Имя условия управления определенные администратором. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|String|Описание управления условия, определенные администратором. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условие управления. Создан со стороны службы. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условие управления. Обновление со стороны службы. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag условие управления. Обновление со стороны службы. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции|Применимые платформ для этого условия управления. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|ipV6Prefix|String|Подсеть IP версии 6, подключенных к. например 2001:db8:: / 32|
|ipV6Gateway|String|Адрес шлюза IP версии 6 для. например 2001:db8::1|
|ipV6DNSServerList|Коллекция String|Серверы IPv6 DNS, настроенные для адаптера.|
|dnsSuffixList|Коллекция String|Допустимое DNS-суффиксы для текущей сети. Например seattle.contoso.com|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции|Операторы условие управления, связанные с условием управления. Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkIPv6ConfigurationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "ipV6Prefix": "String",
  "ipV6Gateway": "String",
  "ipV6DNSServerList": [
    "String"
  ],
  "dnsSuffixList": [
    "String"
  ]
}
```




