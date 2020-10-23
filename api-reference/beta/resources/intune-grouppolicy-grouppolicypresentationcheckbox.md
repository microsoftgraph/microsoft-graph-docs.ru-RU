---
title: Тип ресурса Граупполиципресентатиончеккбокс
description: Представляет элемент checkBox ADMX и логический элемент ADMX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e24eb26d5bdf1e87cf3147fdd2d81ad2d4b36f6e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684745"
---
# <a name="grouppolicypresentationcheckbox-resource-type"></a>Тип ресурса Граупполиципресентатиончеккбокс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент checkBox ADMX и логический элемент ADMX.


Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатиончеккбоксес](../api/intune-grouppolicy-grouppolicypresentationcheckbox-list.md)|Коллекция [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Список свойств и связей объектов [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .|
|[Получение Граупполиципресентатиончеккбокс](../api/intune-grouppolicy-grouppolicypresentationcheckbox-get.md)|[граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Чтение свойств и связей объекта [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .|
|[Создание Граупполиципресентатиончеккбокс](../api/intune-grouppolicy-grouppolicypresentationcheckbox-create.md)|[граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Создание нового объекта [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .|
|[Удаление Граупполиципресентатиончеккбокс](../api/intune-grouppolicy-grouppolicypresentationcheckbox-delete.md)|Нет|Удаляет объект [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).|
|[Обновление Граупполиципресентатиончеккбокс](../api/intune-grouppolicy-grouppolicypresentationcheckbox-update.md)|[граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Обновление свойств объекта [граупполиципресентатиончеккбокс](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|Строка|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Строка|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|дефаултчеккед|Логический|Значение по умолчанию для этого флажка. Значение по умолчанию  false.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|RDLC|[граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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





