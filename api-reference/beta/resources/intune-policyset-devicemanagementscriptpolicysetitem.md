---
title: Тип ресурса Девицеманажементскриптполицисетитем
description: Класс, содержащий свойства, которые используются для Полицисетитем скриптов управления устройствами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4a11bc83a92049b3fce2e6b8b4e116ffce99438e
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201276"
---
# <a name="devicemanagementscriptpolicysetitem-resource-type"></a>Тип ресурса Девицеманажементскриптполицисетитем

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, которые используются для Полицисетитем скриптов управления устройствами.


Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементскриптполицисетитемс](../api/intune-policyset-devicemanagementscriptpolicysetitem-list.md)|Коллекция [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)|Список свойств и связей объектов [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) .|
|[Получение Девицеманажементскриптполицисетитем](../api/intune-policyset-devicemanagementscriptpolicysetitem-get.md)|[девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)|Чтение свойств и связей объекта [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) .|
|[Создание Девицеманажементскриптполицисетитем](../api/intune-policyset-devicemanagementscriptpolicysetitem-create.md)|[девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)|Создание нового объекта [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) .|
|[Удаление Девицеманажементскриптполицисетитем](../api/intune-policyset-devicemanagementscriptpolicysetitem-delete.md)|Нет|Удаляет объект [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md).|
|[Обновление Девицеманажементскриптполицисетитем](../api/intune-policyset-devicemanagementscriptpolicysetitem-update.md)|[девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md)|Обновление свойств объекта [девицеманажементскриптполицисетитем](../resources/intune-policyset-devicemanagementscriptpolicysetitem.md) .|

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



