---
title: тип ресурса deviceConfigurationPolicySetItem
description: Класс, содержащий свойства, используемые для конфигурации устройств PolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aea465f27a43acf42197305728fd8f558ace355d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266823"
---
# <a name="deviceconfigurationpolicysetitem-resource-type"></a>тип ресурса deviceConfigurationPolicySetItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для конфигурации устройств PolicySetItem.


Наследует от [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список устройствConfigurationPolicySetItems](../api/intune-policyset-deviceconfigurationpolicysetitem-list.md)|[коллекция deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|Список свойств и связей объектов [deviceConfigurationPolicySetItem.](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|
|[Get deviceConfigurationPolicySetItem](../api/intune-policyset-deviceconfigurationpolicysetitem-get.md)|[deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|Чтение свойств и связей [объекта deviceConfigurationPolicySetItem.](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|
|[Создание устройстваConfigurationPolicySetItem](../api/intune-policyset-deviceconfigurationpolicysetitem-create.md)|[deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|Создание нового [объекта deviceConfigurationPolicySetItem.](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|
|[Удаление устройстваConfigurationPolicySetItem](../api/intune-policyset-deviceconfigurationpolicysetitem-delete.md)|Нет|Удаляет [устройствоConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md).|
|[Обновление устройстваConfigurationPolicySetItem](../api/intune-policyset-deviceconfigurationpolicysetitem-update.md)|[deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|Обновление свойств объекта [deviceConfigurationPolicySetItem.](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Клавиша PolicySetItem. Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Время создания PolicySetItem. Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время политикиSetItem. Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|Строка|PayloadId of the PolicySetItem. Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|String|policySetType policySetItem. Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|Строка|DisplayName of the PolicySetItem. Унаследованный от [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Состояние PolicySetItem. Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md). Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Код ошибки, если таковое произошло. Унаследовано от [policySetItem](../resources/intune-policyset-policysetitem.md). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|Коллекция String|Теги управляемого развертывания, унаследованной [от policySetItem](../resources/intune-policyset-policysetitem.md)|

## <a name="relationships"></a>Связи
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




