---
title: тип ресурса groupPolicyPresentationValueMultiText
description: Объект представляет строковое значение многостройной презентации текстового окна в определении политики.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31977668f31e1928750d4d75274f20b4741689ed
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033498"
---
# <a name="grouppolicypresentationvaluemultitext-resource-type"></a>тип ресурса groupPolicyPresentationValueMultiText

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект представляет строковое значение многостройной презентации текстового окна в определении политики.


Наследует [от groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyPresentationValueMultiTexts](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-list.md)|[коллекция groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Список свойств и связей объектов [groupPolicyPresentationValueMultiText.](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|
|[Get groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-get.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Чтение свойств и связей объекта [groupPolicyPresentationValueMultiText.](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|
|[Создание groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-create.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Создайте новый [объект groupPolicyPresentationValueMultiText.](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|
|[Удаление groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-delete.md)|Нет|Удаляет [группуPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).|
|[Update groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-update.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Обновление свойств объекта [groupPolicyPresentationValueMultiText.](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|Ключ объекта. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|values|Коллекция String|Коллекция непустых строк для связанной презентации.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Значение определения групповой политики, связанное со значением представления. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|презентация|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|Презентация групповой политики, связанная со значением презентации. Унаследованный от [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueMultiText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "values": [
    "String"
  ]
}
```



