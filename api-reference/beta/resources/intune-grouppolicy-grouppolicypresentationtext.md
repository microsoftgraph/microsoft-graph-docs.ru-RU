---
title: тип ресурса groupPolicyPresentationText
description: Представляет текстовый элемент ADMX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bf3eb2d1d99a62699950421ce2bde69a85c8e834
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788663"
---
# <a name="grouppolicypresentationtext-resource-type"></a>тип ресурса groupPolicyPresentationText

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет текстовый элемент ADMX.


Наследует [от groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyPresentationTexts](../api/intune-grouppolicy-grouppolicypresentationtext-list.md)|[коллекция groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Список свойств и связей объектов [groupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|
|[Get groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-get.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Чтение свойств и связей объекта [groupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|
|[Создание groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-create.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Создайте новый [объект GroupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|
|[Удаление groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-delete.md)|Нет|Удаляет [группуPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).|
|[Update groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-update.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Обновление свойств объекта [groupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|подпись|Строка|Локализованная текстовая метка для любого объекта презентации. По умолчанию это значение пусто. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|определение|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



