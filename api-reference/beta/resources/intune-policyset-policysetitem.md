---
title: Тип ресурса Полицисетитем
description: Класс, содержащий свойства, используемые для элемента "набор политик".
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 11ebd543bf14df00bddd408dcb26400e3e783b6f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37201253"
---
# <a name="policysetitem-resource-type"></a>Тип ресурса Полицисетитем

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для элемента "набор политик".

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Полицисетитемс](../api/intune-policyset-policysetitem-list.md)|Коллекция [полицисетитем](../resources/intune-policyset-policysetitem.md)|Список свойств и связей объектов [полицисетитем](../resources/intune-policyset-policysetitem.md) .|
|[Получение Полицисетитем](../api/intune-policyset-policysetitem-get.md)|[полицисетитем](../resources/intune-policyset-policysetitem.md)|Чтение свойств и связей объекта [полицисетитем](../resources/intune-policyset-policysetitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Мобилеаппполицисетитем.|
|createdDateTime|DateTimeOffset|Время создания Полицисетитем.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетитем.|
|пайлоадид|String.|Пайлоадид Полицисетитем.|
|itemType|String.|Полицисеттипе Полицисетитем.|
|displayName|Строка|DisplayName объекта Полицисетитем.|
|status|[полицисетстатус](../resources/intune-policyset-policysetstatus.md)|Состояние Полицисетитем. Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[Коде](../resources/intune-policyset-errorcode.md)|Код ошибки (при возникновении ошибки). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|гуидеддеплойменттагс|Коллекция строк|Теги в руководстве по развертыванию|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetItem",
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



