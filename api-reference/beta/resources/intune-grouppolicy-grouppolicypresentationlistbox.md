---
title: Тип ресурса Граупполиципресентатионлистбокс
description: Представляет элемент списка ADMX и элемент списка ADMX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c2318a827e4056fac2f6b984ddf4e43405a06c2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781654"
---
# <a name="grouppolicypresentationlistbox-resource-type"></a>Тип ресурса Граупполиципресентатионлистбокс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет элемент списка ADMX и элемент списка ADMX.


НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполиципресентатионлистбоксес](../api/intune-grouppolicy-grouppolicypresentationlistbox-list.md)|Коллекция [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Список свойств и связей объектов [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|
|[Получение Граупполиципресентатионлистбокс](../api/intune-grouppolicy-grouppolicypresentationlistbox-get.md)|[Граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Чтение свойств и связей объекта [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|
|[Создание Граупполиципресентатионлистбокс](../api/intune-grouppolicy-grouppolicypresentationlistbox-create.md)|[Граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Создание нового объекта [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|
|[Удаление Граупполиципресентатионлистбокс](../api/intune-grouppolicy-grouppolicypresentationlistbox-delete.md)|Нет|Удаляет объект [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).|
|[Обновление Граупполиципресентатионлистбокс](../api/intune-grouppolicy-grouppolicypresentationlistbox-update.md)|[Граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Обновление свойств объекта [граупполиципресентатионлистбокс](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|ЕксплиЦитвалуе|Boolean|Если этот параметр задан, пользователь должен указать значение подраздела реестра и имя подраздела реестра. В списке показаны два столбца: один для имени и один для данных. Значение по умолчанию  false.|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|RDLC|[Граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией. НаСледуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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
  "explicitValue": true
}
```





