---
title: Тип ресурса Манажементкондитион
description: Условия управления — это события, которые могут динамически запускаться, например, с географическими ограждениями, временными ограждениями и сетевыми ограждениями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a9707268f648edc60ab7b37292b6e59f7721d983
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722874"
---
# <a name="managementcondition-resource-type"></a>Тип ресурса Манажементкондитион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Условия управления — это события, которые могут динамически запускаться, например, с географическими ограждениями, временными ограждениями и сетевыми ограждениями.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Манажементкондитионс](../api/intune-fencing-managementcondition-list.md)|Коллекция [манажементкондитион](../resources/intune-fencing-managementcondition.md)|Список свойств и связей объектов [манажементкондитион](../resources/intune-fencing-managementcondition.md) .|
|[Получение Манажементкондитион](../api/intune-fencing-managementcondition-get.md)|[манажементкондитион](../resources/intune-fencing-managementcondition.md)|Чтение свойств и связей объекта [манажементкондитион](../resources/intune-fencing-managementcondition.md) .|
|[Функция Жетманажементкондитионсфорплатформ](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|Коллекция [манажементкондитион](../resources/intune-fencing-managementcondition.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для условия управления. Созданное системой значение, назначаемое при создании.|
|uniqueName|Строка|Уникальное имя условия управления. Используется в выражениях условия управления.|
|displayName|Строка|Имя условия управления, определенное администратором.|
|description|Строка|Описание условия управления, заданное администратором.|
|createdDateTime|DateTimeOffset|Время создания условия управления. Созданная сторона службы.|
|modifiedDateTime|DateTimeOffset|Время последнего изменения условия управления. Обновленная сторона службы.|
|eTag|String|Тег ETag условия управления. Обновленная сторона службы.|
|аппликаблеплатформс|Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|Соответствующие платформы для этого условия управления.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|манажементкондитионстатементс|Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)|Операторы условия управления, связанные с условием управления.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





