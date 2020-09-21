---
title: Тип ресурса Полицисетитем
description: Класс, содержащий свойства, используемые для элемента "набор политик".
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 530dd10960eacd0ded5c5c8d9340469c66020e8c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993415"
---
# <a name="policysetitem-resource-type"></a>Тип ресурса Полицисетитем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для элемента "набор политик".

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Полицисетитемс](../api/intune-policyset-policysetitem-list.md)|Коллекция [полицисетитем](../resources/intune-policyset-policysetitem.md)|Список свойств и связей объектов [полицисетитем](../resources/intune-policyset-policysetitem.md) .|
|[Получение Полицисетитем](../api/intune-policyset-policysetitem-get.md)|[policySetItem](../resources/intune-policyset-policysetitem.md)|Чтение свойств и связей объекта [полицисетитем](../resources/intune-policyset-policysetitem.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Мобилеаппполицисетитем.|
|createdDateTime|DateTimeOffset|Время создания Полицисетитем.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетитем.|
|пайлоадид|String|Пайлоадид Полицисетитем.|
|itemType|String|Полицисеттипе Полицисетитем.|
|displayName|String|DisplayName объекта Полицисетитем.|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Состояние Полицисетитем. Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Код ошибки (при возникновении ошибки). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|гуидеддеплойменттагс|Коллекция String|Теги в руководстве по развертыванию|

## <a name="relationships"></a>Связи
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






