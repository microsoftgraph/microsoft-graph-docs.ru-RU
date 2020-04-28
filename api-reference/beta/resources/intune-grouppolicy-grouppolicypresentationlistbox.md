---
title: Тип ресурса Граупполиципресентатионлистбокс
description: Представляет элемент списка ADMX и элемент списка ADMX.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1fb7a2e7cad8785b23eaf14e165d3d7b28b9beb2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462447"
---
# <a name="grouppolicypresentationlistbox-resource-type"></a>Тип ресурса Граупполиципресентатионлистбокс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент списка ADMX и элемент списка ADMX.


Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионлистбоксес](../api/intune-grouppolicy-grouppolicypresentationlistbox-list.md)|Коллекция [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Список свойств и связей объектов [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|
|[Получение Граупполиципресентатионлистбокс](../api/intune-grouppolicy-grouppolicypresentationlistbox-get.md)|[граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Чтение свойств и связей объекта [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|
|[Создание Граупполиципресентатионлистбокс](../api/intune-grouppolicy-grouppolicypresentationlistbox-create.md)|[граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Создание нового объекта [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|
|[Удаление Граупполиципресентатионлистбокс](../api/intune-grouppolicy-grouppolicypresentationlistbox-delete.md)|Нет|Удаляет объект [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).|
|[Обновление Граупполиципресентатионлистбокс](../api/intune-grouppolicy-grouppolicypresentationlistbox-update.md)|[граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Обновление свойств объекта [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|експлиЦитвалуе|Boolean|Если этот параметр задан, пользователь должен указать значение подраздела реестра и имя подраздела реестра. В списке показаны два столбца: один для имени и один для данных. Значение по умолчанию  false.|
|валуепрефикс|String|Н/Д|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|RDLC|[граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationListBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "explicitValue": true,
  "valuePrefix": "String"
}
```



