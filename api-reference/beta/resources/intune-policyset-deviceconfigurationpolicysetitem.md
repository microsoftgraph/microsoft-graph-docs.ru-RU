---
title: Тип ресурса Девицеконфигуратионполицисетитем
description: Класс, содержащий свойства, которые используются для настройки устройств Полицисетитем.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e9cf097667451d5e1440a54ddfba26b0d6e563a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201275"
---
# <a name="deviceconfigurationpolicysetitem-resource-type"></a>Тип ресурса Девицеконфигуратионполицисетитем

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, которые используются для настройки устройств Полицисетитем.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеконфигуратионполицисетитемс](../api/intune-policyset-deviceconfigurationpolicysetitem-list.md)|Коллекция [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|Список свойств и связей объектов [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) .|
|[Получение Девицеконфигуратионполицисетитем](../api/intune-policyset-deviceconfigurationpolicysetitem-get.md)|[девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|Чтение свойств и связей объекта [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) .|
|[Создание Девицеконфигуратионполицисетитем](../api/intune-policyset-deviceconfigurationpolicysetitem-create.md)|[девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|Создание нового объекта [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) .|
|[Удаление Девицеконфигуратионполицисетитем](../api/intune-policyset-deviceconfigurationpolicysetitem-delete.md)|Нет|Удаляет объект [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md).|
|[Обновление Девицеконфигуратионполицисетитем](../api/intune-policyset-deviceconfigurationpolicysetitem-update.md)|[девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|Обновление свойств объекта [девицеконфигуратионполицисетитем](../resources/intune-policyset-deviceconfigurationpolicysetitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Мобилеаппполицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Время создания Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|пайлоадид|String.|Пайлоадид Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|itemType|String.|Полицисеттипе Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|displayName|Строка|DisplayName объекта Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|status|[полицисетстатус](../resources/intune-policyset-policysetstatus.md)|Состояние Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[Коде](../resources/intune-policyset-errorcode.md)|Код ошибки (при возникновении ошибки). Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|гуидеддеплойменттагс|Коллекция строк|Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationPolicySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ]
}
```



