---
title: Тип ресурса networkIPv4ConfigurationManagementCondition
description: Можно определить условия управления IPv4 на основе конфигурации, которые будут срабатывать, когда устройство обнаружит определенные параметры IP-сети. Условия управления IP-конфигурацией будут считаться ИСТИНными, только если сетевое подключение активно.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c670be3a74d3e612e7a6dd0236ddec16b663f774
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331618"
---
# <a name="networkipv4configurationmanagementcondition-resource-type"></a>Тип ресурса networkIPv4ConfigurationManagementCondition

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|String|Уникальный идентификатор для условия управления. Созданное системой значение, назначаемое при создании. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|uniqueName|String|Уникальное имя условия управления. Используется в выражениях условия управления. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|displayName|Строка|Имя условия управления, определенное администратором. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|description|String|Описание условия управления, заданное администратором. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условия управления. Созданная сторона службы. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условия управления. Обновленная сторона службы. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|eTag|String|Тег ETag условия управления. Обновленная сторона службы. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|аппликаблеплатформс|Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|Соответствующие платформы для этого условия управления. Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)|
|ipV4Prefix|String|Подсеть IPv4, к которой необходимо подключиться. Например, 10.0.0.0/8|
|ipV4Gateway|String|IPv4-адрес шлюза. Например, 10.0.0.0|
|ipV4DHCPServer|String|IPv4-адрес DHCP-сервера для адаптера.|
|ipV4DNSServerList|Коллекция строк|DNS-серверы IPv4, настроенные для адаптера.|
|днссуффикслист|Коллекция строк|Допустимые DNS-суффиксы для текущей сети. Например, seattle.contoso.com|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
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



