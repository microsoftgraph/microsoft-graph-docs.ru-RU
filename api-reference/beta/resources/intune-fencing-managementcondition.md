---
title: Тип ресурса Манажементкондитион
description: Условия управления — это события, которые могут динамически запускаться, например, с географическими ограждениями, временными ограждениями и сетевыми ограждениями.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2e5cef389cd6349f11f5e5554146d220608a368a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528185"
---
# <a name="managementcondition-resource-type"></a>Тип ресурса Манажементкондитион

Пространство имен: Microsoft. Graph

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
|id|String|Уникальный идентификатор для условия управления. Созданное системой значение, назначаемое при создании.|
|uniqueName|String|Уникальное имя условия управления. Используется в выражениях условия управления.|
|displayName|Строка|Имя условия управления, определенное администратором.|
|description|String|Описание условия управления, заданное администратором.|
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



