---
title: тип ресурса deviceConfigurationUserStateSummary
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 202dd189e8e7cfdbf6e432c95421ad06296d41a9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127397"
---
# <a name="deviceconfigurationuserstatesummary-resource-type"></a>тип ресурса deviceConfigurationUserStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get deviceConfigurationUserStateSummary](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-get.md)|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|Чтение свойств и связей [объекта deviceConfigurationUserStateSummary.](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|
|[Обновление устройстваConfigurationUserStateSummary](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-update.md)|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|Обновление свойств объекта [deviceConfigurationUserStateSummary.](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
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



