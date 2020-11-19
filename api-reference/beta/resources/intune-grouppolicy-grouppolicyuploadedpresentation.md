---
title: Тип ресурса Граупполициуплоадедпресентатион
description: Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 09f4ff988377ad4e409f33cb78d9b7c6c2f69cac
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298101"
---
# <a name="grouppolicyuploadedpresentation-resource-type"></a>Тип ресурса Граупполициуплоадедпресентатион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.


Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполициуплоадедпресентатионс](../api/intune-grouppolicy-grouppolicyuploadedpresentation-list.md)|Коллекция [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)|Список свойств и связей объектов [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .|
|[Получение Граупполициуплоадедпресентатион](../api/intune-grouppolicy-grouppolicyuploadedpresentation-get.md)|[граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)|Чтение свойств и связей объекта [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .|
|[Создание Граупполициуплоадедпресентатион](../api/intune-grouppolicy-grouppolicyuploadedpresentation-create.md)|[граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)|Создание нового объекта [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .|
|[Удаление Граупполициуплоадедпресентатион](../api/intune-grouppolicy-grouppolicyuploadedpresentation-delete.md)|Нет|Удаляет объект [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).|
|[Обновление Граупполициуплоадедпресентатион](../api/intune-grouppolicy-grouppolicyuploadedpresentation-update.md)|[граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)|Обновление свойств объекта [граупполициуплоадедпресентатион](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|RDLC|[граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyUploadedPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




