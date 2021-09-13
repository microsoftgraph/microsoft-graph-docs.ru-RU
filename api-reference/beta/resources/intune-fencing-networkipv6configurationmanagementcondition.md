---
title: тип ресурса networkIPv6ConfigurationManagementCondition
description: Можно определить условия управления на основе конфигурации IPv6, которые срабатывает при обнаружении устройства определенных параметров IP-сети. Условие управления IP-конфигурами будет считаться TRUE только при активном подключении к сети. Адреса серверов DHCP IPv6 могут не совпадать. Это происходит потому, Windows (около Redstone) не предоставляет эту информацию службе естественной проверки подлинности.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bf74b6a655244e3ed7422ea1f9201f1dbe2f958e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063952"
---
# <a name="networkipv6configurationmanagementcondition-resource-type"></a>тип ресурса networkIPv6ConfigurationManagementCondition

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Можно определить условия управления на основе конфигурации IPv6, которые срабатывает при обнаружении устройства определенных параметров IP-сети. Условие управления IP-конфигурами будет считаться TRUE только при активном подключении к сети.
Адреса серверов DHCP IPv6 могут не совпадать. Это происходит потому, Windows (около Redstone) не предоставляет эту информацию службе естественной проверки подлинности.


Наследует [от networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список networkIPv6ConfigurationManagementConditions](../api/intune-fencing-networkipv6configurationmanagementcondition-list.md)|[networkIPv6ConfigurationManagementCondition collection](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Список свойств и связей объектов [networkIPv6ConfigurationManagementCondition.](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|
|[Get networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-get.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Чтение свойств и связей объекта [networkIPv6ConfigurationManagementCondition.](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|
|[Создание networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-create.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Создайте новый [объект networkIPv6ConfigurationManagementCondition.](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|
|[Удаление networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-delete.md)|Нет|Удаляет [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).|
|[Обновление networkIPv6ConfigurationManagementCondition](../api/intune-fencing-networkipv6configurationmanagementcondition-update.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|Обновление свойств объекта [networkIPv6ConfigurationManagementCondition.](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для состояния управления. Созданное в системе значение, назначенное при его создания. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|Строка|Уникальное имя для состояния управления. Используется в выражениях условий управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|String|Администратор определил имя условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|description|String|Администратор определил описание условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|Время создания условия управления. Сгенерированная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условия управления. Обновленная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag состояния управления. Обновленная сторона службы. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[коллекция devicePlatformType](../resources/intune-fencing-deviceplatformtype.md)|Применимые платформы для этого условия управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|
|ipV6Prefix|Строка|Подсеть IPv6, к которая должна быть подключена. например, 2001:db8::/32|
|ipV6Gateway|Строка|Адрес шлюза IPv6. например, 2001:db8::1|
|ipV6DNSServerList|Коллекция String|DNS-серверы IPv6, настроенные для адаптеров.|
|dnsSuffixList|Коллекция строк|Допустимые Суффиксы DNS для текущей сети. например, seattle.contoso.com|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|managementConditionStatements|[коллекция managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Утверждения условий управления, связанные с состоянием управления. Унаследованный от [managementCondition](../resources/intune-fencing-managementcondition.md)|

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



