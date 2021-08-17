---
title: тип ресурса deviceManagementScriptPolicySetItem
description: Класс, содержащий свойства, используемые для скрипта управления устройствами PolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e9ab5b0faf3c522f28659bf0d304f7d64790e61b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265370"
---
# <a name="devicemanagementscriptpolicysetitem-resource-type"></a>тип ресурса deviceManagementScriptPolicySetItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для скрипта управления устройствами PolicySetItem.


Наследует от [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementScriptPolicySetItems](../api/intune-policyset-devicemanagementscriptpolicysetitem-list.md)|[коллекция deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)|Список свойств и связей объектов [deviceManagementScriptPolicySetItem.](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)|
|[Get deviceManagementScriptPolicySetItem](../api/intune-policyset-devicemanagementscriptpolicysetitem-get.md)|[deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)|Чтение свойств и связей [объекта deviceManagementScriptPolicySetItem.](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)|
|[Создание deviceManagementScriptPolicySetItem](../api/intune-policyset-devicemanagementscriptpolicysetitem-create.md)|[deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)|Создание нового [объекта deviceManagementScriptPolicySetItem.](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)|
|[Удаление deviceManagementScriptPolicySetItem](../api/intune-policyset-devicemanagementscriptpolicysetitem-delete.md)|Нет|Удаляет [устройствоManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md).|
|[Обновление deviceManagementScriptPolicySetItem](../api/intune-policyset-devicemanagementscriptpolicysetitem-update.md)|[deviceManagementScriptPolicySetItem](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)|Обновление свойств объекта [deviceManagementScriptPolicySetItem.](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)|

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
  "@odata.type": "microsoft.graph.deviceManagementScriptPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptPolicySetItem",
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




