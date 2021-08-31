---
title: тип ресурса groupPolicyPresentationValue
description: Объект базового значения презентации, который сохраняет значение для одной презентации групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ffd062e43e62c28c01cb0314233c8a97f6ab437
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803484"
---
# <a name="grouppolicypresentationvalue-resource-type"></a>тип ресурса groupPolicyPresentationValue

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект базового значения презентации, который сохраняет значение для одной презентации групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyPresentationValues](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|[коллекция groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Список свойств и связей объектов [groupPolicyPresentationValue.](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|[Get groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Чтение свойств и связей объекта [groupPolicyPresentationValue.](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|[Создание groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Создайте новый [объект GroupPolicyPresentationValue.](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|[Удаление groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|Нет|Удаляет [группуPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).|
|[Обновление groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Обновление свойств объекта [groupPolicyPresentationValue.](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|id|Строка|Ключ объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Значение определения групповой политики, связанное со значением представления.|
|презентация|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|Презентация групповой политики, связанная со значением презентации.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)"
}
```



