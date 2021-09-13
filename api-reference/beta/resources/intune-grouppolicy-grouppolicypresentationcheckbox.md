---
title: тип ресурса groupPolicyPresentationCheckBox
description: Представляет элемент checkBox ADMX и элемент boolean ADMX.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9afa92ae390e26f3198c48df9b60e09facbbf10
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086094"
---
# <a name="grouppolicypresentationcheckbox-resource-type"></a>тип ресурса groupPolicyPresentationCheckBox

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент checkBox ADMX и элемент boolean ADMX.


Наследует [от groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyPresentationCheckBoxes](../api/intune-grouppolicy-grouppolicypresentationcheckbox-list.md)|[коллекция groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Список свойств и связей объектов [groupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|
|[Get groupPolicyPresentationCheckBox](../api/intune-grouppolicy-grouppolicypresentationcheckbox-get.md)|[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Чтение свойств и связей объекта [groupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|
|[Создание groupPolicyPresentationCheckBox](../api/intune-grouppolicy-grouppolicypresentationcheckbox-create.md)|[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Создайте новый [объект GroupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|
|[Удаление groupPolicyPresentationCheckBox](../api/intune-grouppolicy-grouppolicypresentationcheckbox-delete.md)|Нет|Удаляет [группуPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).|
|[Обновление groupPolicyPresentationCheckBox](../api/intune-grouppolicy-grouppolicypresentationcheckbox-update.md)|[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Обновление свойств объекта [groupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|подпись|String|Локализованная текстовая метка для любого объекта презентации. По умолчанию это значение пусто. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultChecked|Логическое|Значение по умолчанию для контрольного окна. Значение по умолчанию  false.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|определение|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Унаследованный от [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationCheckBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultChecked": true
}
```



