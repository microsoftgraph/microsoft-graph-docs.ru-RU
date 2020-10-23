---
title: Тип ресурса networkIPv4ConfigurationManagementCondition
description: Можно определить условия управления IPv4 на основе конфигурации, которые будут срабатывать, когда устройство обнаружит определенные параметры IP-сети. Условия управления IP-конфигурацией будут считаться ИСТИНными, только если сетевое подключение активно.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9f30aeaa3027d7ed5e8b00b5ec5ec9be1b637ca
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722839"
---
# <a name="networkipv4configurationmanagementcondition-resource-type"></a>Тип ресурса networkIPv4ConfigurationManagementCondition

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Можно определить условия управления IPv4 на основе конфигурации, которые будут срабатывать, когда устройство обнаружит определенные параметры IP-сети. Условия управления IP-конфигурацией будут считаться ИСТИНными, только если сетевое подключение активно.


Наследуется от [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список networkIPv4ConfigurationManagementConditions](../api/intune-fencing-networkipv4configurationmanagementcondition-list.md)|Коллекция [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|Список свойств и связей объектов [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .|
|[Получение networkIPv4ConfigurationManagementCondition](../api/intune-fencing-networkipv4configurationmanagementcondition-get.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|Чтение свойств и связей объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .|
|[Создание networkIPv4ConfigurationManagementCondition](../api/intune-fencing-networkipv4configurationmanagementcondition-create.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|Создание нового объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .|
|[Удаление networkIPv4ConfigurationManagementCondition](../api/intune-fencing-networkipv4configurationmanagementcondition-delete.md)|Нет|Удаляет объект [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).|
|[Обновление networkIPv4ConfigurationManagementCondition](../api/intune-fencing-networkipv4configurationmanagementcondition-update.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|Обновление свойств объекта [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для условия управления. Созданное системой значение, назначаемое при создании. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|uniqueName|Строка|Уникальное имя условия управления. Используется в выражениях условия управления. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|displayName|Строка|Имя условия управления, определенное администратором. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|description|Строка|Описание условия управления, заданное администратором. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условия управления. Созданная сторона службы. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условия управления. Обновленная сторона службы. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|eTag|String|Тег ETag условия управления. Обновленная сторона службы. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|аппликаблеплатформс|Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|Соответствующие платформы для этого условия управления. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|ipV4Prefix|Строка|Подсеть IPv4, к которой необходимо подключиться. Например, 10.0.0.0/8|
|ipV4Gateway|Строка|IPv4-адрес шлюза. Например, 10.0.0.0|
|ipV4DHCPServer|Строка|IPv4-адрес DHCP-сервера для адаптера.|
|ipV4DNSServerList|Коллекция строк|DNS-серверы IPv4, настроенные для адаптера.|
|днссуффикслист|Коллекция строк|Допустимые DNS-суффиксы для текущей сети. Например, seattle.contoso.com|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|манажементкондитионстатементс|Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)|Операторы условия управления, связанные с условием управления. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkIPv4ConfigurationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
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
  "ipV4Prefix": "String",
  "ipV4Gateway": "String",
  "ipV4DHCPServer": "String",
  "ipV4DNSServerList": [
    "String"
  ],
  "dnsSuffixList": [
    "String"
  ]
}
```





