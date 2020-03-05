---
title: Тип ресурса Граупполиципресентатион
description: Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8a829f974a25412a88dcc44ef5e9b84a0c3f81a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528082"
---
# <a name="grouppolicypresentation-resource-type"></a>Тип ресурса Граупполиципресентатион

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовая сущность для отображения представления любого из дополнительных параметров в определении групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Граупполиципресентатион](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|Чтение свойств и связей объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .|
|[Обновление Граупполиципресентатион](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|Обновление свойств объекта [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|RDLC|[граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение групповой политики, связанное с презентацией.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



