---
title: тип ресурса deviceConfigurationUserStateSummary
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: abd09c98022ceba37196766a434dbc043a11a155
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805438"
---
# <a name="deviceconfigurationuserstatesummary-resource-type"></a>тип ресурса deviceConfigurationUserStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get deviceConfigurationUserStateSummary](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-get.md)|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md);|Чтение свойств и связей [объекта deviceConfigurationUserStateSummary.](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|
|[Обновление устройстваConfigurationUserStateSummary](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-update.md)|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md);|Обновление свойств объекта [deviceConfigurationUserStateSummary.](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|unknownUserCount|Int32|Число неизвестных пользователей|
|notApplicableUserCount|Int32|Число не применимых пользователей|
|compliantUserCount|Int32|Количество совместимых пользователей|
|remediatedUserCount|Int32|Число исправленных пользователей|
|nonCompliantUserCount|Int32|Число некомплиентных пользователей|
|errorUserCount|Int32|Число пользователей ошибок|
|conflictUserCount|Int32|Число пользователей конфликтов|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "String (identifier)",
  "unknownUserCount": 1024,
  "notApplicableUserCount": 1024,
  "compliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "errorUserCount": 1024,
  "conflictUserCount": 1024
}
```



